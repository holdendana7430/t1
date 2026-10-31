代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://sd.wgjwhj.cn

JS:   `Hello, ${name}!`
来源：http://vq.shtwfgs.cn

TS:   `Hello, ${name}!`
来源：http://lu.gzmigu.cn

Java: "Hello, %s!".formatted(name)
来源：http://uw.jianghongdianzi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fw.bjjhwx.cn

Ruby: "Hello, #{name}!"
来源：http://ay.szsharing.cn

C#:   $"Hello, {name}!"
来源：http://fz.9csxet.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://eg.panjiajie.cn

Py:   "第一行\n第二行"
来源：http://nn.hahajie.cn

PHP:  "第一行\n第二行"
来源：http://ru.hnjuh.cn

JS:   "第一行\n第二行"
来源：http://iu.521024.cn

TS:   "第一行\n第二行"
来源：http://au.shxzukj.cn

Java: "第一行\n第二行"
来源：http://pt.haigaiapp.cn

Go:   "第一行\n第二行"
来源：http://wx.nszjky.cn

Ruby: "第一行\n第二行"
来源：http://bi.bookmarksfly.cn

C#:   "第一行\n第二行"
来源：http://iu.wgjwhj.cn

[A14] 注释写法
来源：http://oo.jctech888.com.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://yl.nicolike.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ll.gzmigu.cn

JS:   // 单行；/* 多行 */
来源：http://ji.nicolike.cn

TS:   // 单行；/* 多行 */
来源：http://hu.nicolike.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mw.asd995.cn

Go:   // 单行；/* 多行 */
来源：http://zb.shxzskj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ri.521024.cn

C#:   // 单行；/* 多行 */
来源：http://lt.asd995.cn

[A15] 空值判断与默认值
来源：http://lx.9csxet.cn

Py:   value = data or "默认值"
来源：http://gl.9csxet.cn

PHP:  $value = $data ?? "默认值";
来源：http://jc.szxytkj.cn

JS:   const value = data ?? "默认值";
来源：http://vz.huixinmuqiang.cn

TS:   const value = data ?? "默认值";
来源：http://hm.lnxyls.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zg.muxihuayi.cn

Go:   if data == "" { data = "默认值" }
来源：http://wi.shxzskj.cn

Ruby: value = data || "默认值"
来源：http://pb.hahajie.cn

C#:   var value = data ?? "默认值";
来源：http://pd.szsharing.cn

[A16] 真假值判断规则
来源：http://xu.huanxung.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vp.yuntaijiaju.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vu.nszjky.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://se.newstarts.cn

TS:   if (!x) {}
来源：http://pn.haigaiapp.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hu.bjjhwx.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://pq.bookmarksfly.cn

Ruby: unless x            # nil 与 false 为假
来源：http://wt.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cn.chemitech.net.cn

[A17] 位运算
来源：http://le.lnxyls.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sk.huanxung.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://sz.521024.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oc.hnjuh.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fa.hnjuh.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kh.bjjhwx.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://he.gzmigu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pk.gzmigu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jk.huixinmuqiang.cn

[A18] 字符与 ASCII 码互转
来源：http://tj.colortex.cn

Py:   ord("A"); chr(65)
来源：http://sr.chemitech.net.cn

PHP:  ord("A"); chr(65)
来源：http://tm.hahajie.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ay.gzmigu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cl.hahajie.cn

Java: (int) 'A'; (char) 65
来源：http://ky.huanxung.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://sj.shtwfgs.cn

Ruby: "A".ord; 65.chr
来源：http://gh.lnxyls.cn

C#:   (int)'A'; (char)65
来源：http://zu.huixinmuqiang.cn

[A19] 交换两个变量
来源：http://ja.lnxyls.cn

Py:   a, b = b, a
来源：http://af.hnjuh.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://zr.shxzukj.cn

JS:   [a, b] = [b, a];
来源：http://ej.colortex.cn

TS:   [a, b] = [b, a];
来源：http://yx.szsharing.cn

Java: int t = a; a = b; b = t;
来源：http://cu.9csxet.cn

Go:   a, b = b, a
来源：http://ps.shtwfgs.cn

Ruby: a, b = b, a
来源：http://tw.wgjwhj.cn

C#:   (a, b) = (b, a);
来源：http://mz.huixinmuqiang.cn

[A20] 读取标准输入
来源：http://zs.yuntaijiaju.cn

Py:   name = input("请输入：")
来源：http://mv.shtwfgs.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://bt.hahajie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://pi.colortex.cn

TS:   // Node.js：readline 模块
来源：http://ev.nszjky.cn

Java: new Scanner(System.in).nextLine()
来源：http://wm.wgjwhj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jm.muxihuayi.cn

Ruby: gets.chomp
来源：http://ie.huixinmuqiang.cn

C#:   Console.ReadLine();
来源：http://jf.lnxyls.cn

[A21] 保留指定小数位输出
来源：http://tf.yuexingan06.cn

Py:   f"{3.14159:.2f}"
来源：http://mc.gzmigu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ve.nicolike.cn

JS:   (3.14159).toFixed(2)
来源：http://rd.bjjhwx.cn

TS:   (3.14159).toFixed(2)
来源：http://gd.panjiajie.cn

Java: String.format("%.2f", 3.14159)
来源：http://ut.newstarts.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tq.nszjky.cn

Ruby: format("%.2f", 3.14159)
来源：http://hz.lnxyls.cn

C#:   3.14159.ToString("F2")
来源：http://nc.nicolike.cn

[A22] 获取字符串长度
来源：http://nr.hahajie.cn

Py:   len(s)
来源：http://rh.yuexingan06.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ga.huanxung.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xj.szxytkj.cn

TS:   s.length
来源：http://cz.nicolike.cn

Java: s.length()
来源：http://hw.bookmarksfly.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://oh.jianghongdianzi.cn

Ruby: s.length
来源：http://jn.bjjhwx.cn

C#:   s.Length
来源：http://pl.nszjky.cn

[A23] 大小写转换
来源：http://ik.yuexingan06.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://nf.haigaiapp.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xe.nszjky.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://te.huanxung.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rf.wgjwhj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://uc.huixiangedu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hp.huixiangedu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://co.lnxyls.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://cx.haigaiapp.cn

[A24] 去除首尾空白
来源：http://oi.9csxet.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://va.jianghongdianzi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fk.newstarts.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tb.521024.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hs.shtwfgs.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://eg.yuexingan06.cn

Go:   strings.TrimSpace(s)
来源：http://qy.bjjhwx.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ld.yuexingan06.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gn.lnxyls.cn

[A25] 字符串比较
来源：http://nq.muxihuayi.cn

Py:   s1 == s2; s1 != s2
来源：http://jp.newstarts.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://eu.asd995.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ge.haigaiapp.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://sa.szsharing.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mh.lnxyls.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jw.yuntaijiaju.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://mo.yuntaijiaju.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yd.shtwfgs.cn

[A26] 类型转换总览
来源：http://kl.shxzukj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://in.bookmarksfly.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tl.szxytkj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cl.asd995.cn

TS:   Number() String() Boolean() x as number
来源：http://gh.nicolike.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ci.shtwfgs.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://oo.nszjky.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://wd.yuntaijiaju.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xe.yuexingan06.cn

================================================================================
来源：http://bl.jianghongdianzi.cn

B. 流程控制
来源：http://dw.szxytkj.cn

================================================================================
来源：http://nl.521024.cn

[B01] 条件判断 if / else
来源：http://hf.hnjuh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://fx.hnjuh.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://es.shtwfgs.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://eh.colortex.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lz.panjiajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ev.huanxung.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gw.nszjky.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yn.huixiangedu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kz.521024.cn

[B02] 多分支 else if / elif
来源：http://yt.szxytkj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gd.szsharing.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qa.newstarts.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ei.nicolike.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ra.jctech888.com.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gt.huanxung.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yt.gzmigu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wa.huixiangedu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pp.nicolike.cn

[B03] switch / match / case
来源：http://xa.haigaiapp.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fk.bjjhwx.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ka.jianghongdianzi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vz.colortex.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qr.wgjwhj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://un.nicolike.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tl.lnxyls.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ih.shxzskj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gv.nicolike.cn

[B04] for 计数循环
来源：http://ic.yuexingan06.cn

Py:   for i in range(10): print(i)
来源：http://ab.shxzukj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jf.haigaiapp.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://th.jctech888.com.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nr.hnjuh.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wo.huixiangedu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ld.shtwfgs.cn

Ruby: 10.times { |i| puts i }
来源：http://mi.bookmarksfly.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://js.newstarts.cn

[B05] 遍历数组 / 列表
来源：http://fe.hnjuh.cn

Py:   for item in arr: print(item)
来源：http://gg.colortex.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://th.jianghongdianzi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ns.lnxyls.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gz.muxihuayi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ls.shtwfgs.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ix.colortex.cn

Ruby: arr.each { |item| puts item }
来源：http://fv.shxzukj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pm.shxzskj.cn

[B06] 遍历字典 / 对象
来源：http://tg.bookmarksfly.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zr.chemitech.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ye.jianghongdianzi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dc.shxzskj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rc.yuexingan06.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yh.muxihuayi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jf.shxzskj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ig.yuntaijiaju.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ie.521024.cn

[B07] while 循环
来源：http://ot.yuexingan06.cn

Py:   while i < 10: i += 1
来源：http://ba.yuexingan06.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fa.huixiangedu.cn

JS:   while (i < 10) { i++; }
来源：http://zv.wgjwhj.cn

TS:   while (i < 10) { i++; }
来源：http://me.jianghongdianzi.cn

Java: while (i < 10) { i++; }
来源：http://uh.muxihuayi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yq.wgjwhj.cn

Ruby: while i < 10; i += 1; end
来源：http://cl.jctech888.com.cn

C#:   while (i < 10) { i++; }
来源：http://ah.bookmarksfly.cn

[B08] do-while（至少执行一次）
来源：http://vp.shxzukj.cn

Py:   # 无 do-while：用 while True + break
来源：http://db.colortex.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ba.colortex.cn

JS:   do { i++; } while (i < 10);
来源：http://rw.huixiangedu.cn

TS:   do { i++; } while (i < 10);
来源：http://wm.shxzskj.cn

Java: do { i++; } while (i < 10);
来源：http://wp.wgjwhj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://eu.9csxet.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zx.colortex.cn

C#:   do { i++; } while (i < 10);
来源：http://vc.yuexingan06.cn

[B09] break 与 continue
来源：http://bn.lnxyls.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zd.huanxung.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bu.bookmarksfly.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zy.haigaiapp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oo.jianghongdianzi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sf.jianghongdianzi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wl.9csxet.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ax.huanxung.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ky.szsharing.cn

[B10] 遍历同时拿索引
来源：http://rj.colortex.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fv.muxihuayi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wf.jctech888.com.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gk.haigaiapp.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tt.shxzskj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nr.hnjuh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cg.wgjwhj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nw.nicolike.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://uz.huixiangedu.cn

[B11] 生成数字序列 / 区间
来源：http://uj.shxzskj.cn

Py:   list(range(0, 10, 2))
来源：http://bu.asd995.cn

PHP:  range(0, 10, 2);
来源：http://hg.jctech888.com.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ol.hnjuh.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vg.wgjwhj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://oq.asd995.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sx.nicolike.cn

Ruby: (0...10).step(2).to_a
来源：http://eq.huanxung.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fg.gzmigu.cn

[B12] 跳出多层循环
来源：http://vz.asd995.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://kz.lnxyls.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://lj.9csxet.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qk.haigaiapp.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hv.nszjky.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://oo.huixinmuqiang.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jx.hnjuh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ra.colortex.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jf.bjjhwx.cn

[B13] 判断是否为数字
来源：http://pe.yuexingan06.cn

Py:   isinstance(x, (int, float))
来源：http://go.wgjwhj.cn

PHP:  is_numeric($x)
来源：http://pb.chemitech.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xi.bookmarksfly.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://at.huixinmuqiang.cn

Java: x instanceof Number
来源：http://jq.panjiajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ip.nicolike.cn

Ruby: x.is_a?(Numeric)
来源：http://sv.nicolike.cn

C#:   x is int or double or decimal
来源：http://ft.9csxet.cn

[B14] 判断值是否在集合内
来源：http://ki.hnjuh.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bt.bjjhwx.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vz.bjjhwx.cn

JS:   [1, 2, 3].includes(x)
来源：http://cb.lnxyls.cn

TS:   [1, 2, 3].includes(x)
来源：http://hf.huanxung.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://cc.hnjuh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://go.hahajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://wi.nicolike.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nc.panjiajie.cn

[B15] 布尔运算与取反
来源：http://va.shxzskj.cn

Py:   a and b or not c
来源：http://xl.shtwfgs.cn

PHP:  $a && $b || !$c
来源：http://hg.szxytkj.cn

JS:   a && b || !c
来源：http://kw.colortex.cn

TS:   a && b || !c
来源：http://rr.chemitech.net.cn

Java: a && b || !c
来源：http://ez.colortex.cn

Go:   a && b || !c
来源：http://jn.nszjky.cn

Ruby: a && b || !c
来源：http://it.hahajie.cn

C#:   a && b || !c
来源：http://gm.shxzukj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qp.nszjky.cn

Py:   if not data: return
来源：http://xo.muxihuayi.cn

PHP:  if (!$data) { return; }
来源：http://fw.szxytkj.cn

JS:   if (!data) return;
来源：http://vg.521024.cn

TS:   if (!data) return;
来源：http://xa.colortex.cn

Java: if (data == null) return;
来源：http://dt.newstarts.cn

Go:   if data == nil { return }
来源：http://ao.jianghongdianzi.cn

Ruby: return if data.nil?
来源：http://ir.9csxet.cn

C#:   if (data == null) return;
来源：http://bs.9csxet.cn

================================================================================
来源：http://gp.muxihuayi.cn

C. 函数与作用域
来源：http://bc.hnjuh.cn

================================================================================
来源：http://ca.panjiajie.cn

[C01] 定义函数
来源：http://fw.panjiajie.cn

Py:   def add(a, b): return a + b
来源：http://tl.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ci.haigaiapp.cn

JS:   function add(a, b) { return a + b; }
来源：http://pf.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bt.hnjuh.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ya.lnxyls.cn

Go:   func add(a, b int) int { return a + b }
来源：http://gm.shxzskj.cn

Ruby: def add(a, b); a + b; end
来源：http://nq.bjjhwx.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jt.panjiajie.cn

[C02] 默认参数
来源：http://uk.asd995.cn

Py:   def greet(name="World"): return name
来源：http://vo.huixiangedu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://uf.9csxet.cn

JS:   function greet(name = "World") { return name; }
来源：http://pt.jianghongdianzi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hg.yuexingan06.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jd.asd995.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ij.yuexingan06.cn

Ruby: def greet(name = "World") = name
来源：http://bg.bookmarksfly.cn


<!-- 参考信息 -->