代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://bm.bookmarksfly.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ll.lnxyls.cn

Java: x > 0 ? "yes" : "no"
来源：http://mx.shtwfgs.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ci.yuexingan06.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://xv.panjiajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ag.huixiangedu.cn

[A12] 字符串插值 / 格式化
来源：http://jl.szxytkj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hu.521024.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://kr.yuntaijiaju.cn

JS:   `Hello, ${name}!`
来源：http://lu.wgjwhj.cn

TS:   `Hello, ${name}!`
来源：http://fb.yuexingan06.cn

Java: "Hello, %s!".formatted(name)
来源：http://cd.jianghongdianzi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://cj.huixiangedu.cn

Ruby: "Hello, #{name}!"
来源：http://vy.huixiangedu.cn

C#:   $"Hello, {name}!"
来源：http://is.huixinmuqiang.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://hh.yuexingan06.cn

Py:   "第一行\n第二行"
来源：http://hl.nicolike.cn

PHP:  "第一行\n第二行"
来源：http://lx.hnjuh.cn

JS:   "第一行\n第二行"
来源：http://oi.jianghongdianzi.cn

TS:   "第一行\n第二行"
来源：http://fz.lnxyls.cn

Java: "第一行\n第二行"
来源：http://wr.hahajie.cn

Go:   "第一行\n第二行"
来源：http://mg.yuntaijiaju.cn

Ruby: "第一行\n第二行"
来源：http://bv.521024.cn

C#:   "第一行\n第二行"
来源：http://wx.huanxung.cn

[A14] 注释写法
来源：http://vv.nicolike.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://yw.panjiajie.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://tl.shxzskj.cn

JS:   // 单行；/* 多行 */
来源：http://up.panjiajie.cn

TS:   // 单行；/* 多行 */
来源：http://je.shxzukj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wo.jctech888.com.cn

Go:   // 单行；/* 多行 */
来源：http://sz.hahajie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://hh.shtwfgs.cn

C#:   // 单行；/* 多行 */
来源：http://gb.haigaiapp.cn

[A15] 空值判断与默认值
来源：http://wx.huanxung.cn

Py:   value = data or "默认值"
来源：http://wz.bjjhwx.cn

PHP:  $value = $data ?? "默认值";
来源：http://tm.bjjhwx.cn

JS:   const value = data ?? "默认值";
来源：http://pp.szsharing.cn

TS:   const value = data ?? "默认值";
来源：http://mb.szxytkj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gt.hnjuh.cn

Go:   if data == "" { data = "默认值" }
来源：http://vu.nszjky.cn

Ruby: value = data || "默认值"
来源：http://va.bookmarksfly.cn

C#:   var value = data ?? "默认值";
来源：http://ku.yuntaijiaju.cn

[A16] 真假值判断规则
来源：http://zq.panjiajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://am.yuntaijiaju.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://uw.haigaiapp.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mt.nicolike.cn

TS:   if (!x) {}
来源：http://fg.jctech888.com.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yc.szxytkj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ti.colortex.cn

Ruby: unless x            # nil 与 false 为假
来源：http://hg.hahajie.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rb.panjiajie.cn

[A17] 位运算
来源：http://ih.521024.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hw.muxihuayi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://nn.hnjuh.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cx.gzmigu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fz.asd995.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yx.shtwfgs.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://yu.9csxet.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jz.gzmigu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kk.szsharing.cn

[A18] 字符与 ASCII 码互转
来源：http://fd.huixiangedu.cn

Py:   ord("A"); chr(65)
来源：http://yj.lnxyls.cn

PHP:  ord("A"); chr(65)
来源：http://tc.nszjky.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vh.muxihuayi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rm.haigaiapp.cn

Java: (int) 'A'; (char) 65
来源：http://sb.asd995.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ad.colortex.cn

Ruby: "A".ord; 65.chr
来源：http://ne.huixiangedu.cn

C#:   (int)'A'; (char)65
来源：http://wt.colortex.cn

[A19] 交换两个变量
来源：http://ug.panjiajie.cn

Py:   a, b = b, a
来源：http://sm.shxzskj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ba.szxytkj.cn

JS:   [a, b] = [b, a];
来源：http://zy.shxzskj.cn

TS:   [a, b] = [b, a];
来源：http://rs.521024.cn

Java: int t = a; a = b; b = t;
来源：http://qa.huixinmuqiang.cn

Go:   a, b = b, a
来源：http://ha.bookmarksfly.cn

Ruby: a, b = b, a
来源：http://gf.nszjky.cn

C#:   (a, b) = (b, a);
来源：http://dy.jianghongdianzi.cn

[A20] 读取标准输入
来源：http://gq.chemitech.net.cn

Py:   name = input("请输入：")
来源：http://ry.muxihuayi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://vs.huixinmuqiang.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jg.nszjky.cn

TS:   // Node.js：readline 模块
来源：http://cr.9csxet.cn

Java: new Scanner(System.in).nextLine()
来源：http://ns.bjjhwx.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kx.shxzukj.cn

Ruby: gets.chomp
来源：http://xz.chemitech.net.cn

C#:   Console.ReadLine();
来源：http://gq.bjjhwx.cn

[A21] 保留指定小数位输出
来源：http://lg.yuexingan06.cn

Py:   f"{3.14159:.2f}"
来源：http://zm.nicolike.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ff.yuntaijiaju.cn

JS:   (3.14159).toFixed(2)
来源：http://cy.colortex.cn

TS:   (3.14159).toFixed(2)
来源：http://tk.shxzskj.cn

Java: String.format("%.2f", 3.14159)
来源：http://mp.shtwfgs.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ph.haigaiapp.cn

Ruby: format("%.2f", 3.14159)
来源：http://kl.muxihuayi.cn

C#:   3.14159.ToString("F2")
来源：http://rm.jianghongdianzi.cn

[A22] 获取字符串长度
来源：http://yj.yuexingan06.cn

Py:   len(s)
来源：http://gg.bookmarksfly.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jo.521024.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hq.lnxyls.cn

TS:   s.length
来源：http://gw.huixinmuqiang.cn

Java: s.length()
来源：http://xw.nszjky.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://yw.wgjwhj.cn

Ruby: s.length
来源：http://og.shxzukj.cn

C#:   s.Length
来源：http://eg.asd995.cn

[A23] 大小写转换
来源：http://br.jctech888.com.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://no.lnxyls.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wd.hahajie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fa.bjjhwx.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dc.shxzskj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dp.huixinmuqiang.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zs.colortex.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fl.newstarts.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qe.yuntaijiaju.cn

[A24] 去除首尾空白
来源：http://lh.chemitech.net.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mr.shxzukj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cv.521024.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mn.panjiajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gh.521024.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://du.jctech888.com.cn

Go:   strings.TrimSpace(s)
来源：http://sb.colortex.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jf.lnxyls.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ld.wgjwhj.cn

[A25] 字符串比较
来源：http://qs.yuexingan06.cn

Py:   s1 == s2; s1 != s2
来源：http://ud.gzmigu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nc.asd995.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hh.nszjky.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vn.jctech888.com.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kj.hnjuh.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lx.hnjuh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://oe.szxytkj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wj.bjjhwx.cn

[A26] 类型转换总览
来源：http://ye.huanxung.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ac.jianghongdianzi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hu.jianghongdianzi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wo.huixiangedu.cn

TS:   Number() String() Boolean() x as number
来源：http://ir.haigaiapp.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zh.bookmarksfly.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dw.asd995.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://du.hahajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ll.yuexingan06.cn

================================================================================
来源：http://sv.wgjwhj.cn

B. 流程控制
来源：http://pe.hahajie.cn

================================================================================
来源：http://ha.jctech888.com.cn

[B01] 条件判断 if / else
来源：http://qx.yuntaijiaju.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://zq.panjiajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vf.shtwfgs.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lw.haigaiapp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://md.chemitech.net.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ox.shxzukj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://uc.gzmigu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nh.shxzukj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qg.panjiajie.cn

[B02] 多分支 else if / elif
来源：http://lu.colortex.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ll.bjjhwx.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ub.yuexingan06.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xp.chemitech.net.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://al.shtwfgs.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://km.huixinmuqiang.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mn.panjiajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yd.yuntaijiaju.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gg.huanxung.cn

[B03] switch / match / case
来源：http://cw.gzmigu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://je.panjiajie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://av.huanxung.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://io.newstarts.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mo.9csxet.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nr.gzmigu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ia.huixinmuqiang.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ck.asd995.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mw.wgjwhj.cn

[B04] for 计数循环
来源：http://mi.shxzukj.cn

Py:   for i in range(10): print(i)
来源：http://lr.szxytkj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sh.shxzukj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zs.jianghongdianzi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://el.9csxet.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bv.lnxyls.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://oa.newstarts.cn

Ruby: 10.times { |i| puts i }
来源：http://dh.muxihuayi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wy.bjjhwx.cn

[B05] 遍历数组 / 列表
来源：http://dd.huixinmuqiang.cn

Py:   for item in arr: print(item)
来源：http://na.haigaiapp.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vm.jctech888.com.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://en.shxzskj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://cy.shxzukj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xw.chemitech.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pt.panjiajie.cn

Ruby: arr.each { |item| puts item }
来源：http://xo.wgjwhj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kj.szsharing.cn

[B06] 遍历字典 / 对象
来源：http://py.lnxyls.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fx.szxytkj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ur.nszjky.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tk.nicolike.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wn.521024.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tb.bjjhwx.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pt.yuexingan06.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vm.wgjwhj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://st.haigaiapp.cn

[B07] while 循环
来源：http://oq.szsharing.cn

Py:   while i < 10: i += 1
来源：http://lm.szxytkj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://oy.wgjwhj.cn

JS:   while (i < 10) { i++; }
来源：http://bi.huanxung.cn

TS:   while (i < 10) { i++; }
来源：http://ye.521024.cn

Java: while (i < 10) { i++; }
来源：http://kd.lnxyls.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://im.haigaiapp.cn

Ruby: while i < 10; i += 1; end
来源：http://pr.szsharing.cn

C#:   while (i < 10) { i++; }
来源：http://kq.jianghongdianzi.cn

[B08] do-while（至少执行一次）
来源：http://bl.huanxung.cn

Py:   # 无 do-while：用 while True + break
来源：http://qv.muxihuayi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ju.shtwfgs.cn

JS:   do { i++; } while (i < 10);
来源：http://qb.huanxung.cn

TS:   do { i++; } while (i < 10);
来源：http://wu.bjjhwx.cn

Java: do { i++; } while (i < 10);
来源：http://rg.asd995.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gv.wgjwhj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://tx.nicolike.cn

C#:   do { i++; } while (i < 10);
来源：http://ou.yuexingan06.cn

[B09] break 与 continue
来源：http://ea.huanxung.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vj.huanxung.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gy.jctech888.com.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mk.haigaiapp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tz.bookmarksfly.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ve.colortex.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://px.panjiajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yc.bookmarksfly.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mj.hnjuh.cn

[B10] 遍历同时拿索引
来源：http://qe.yuntaijiaju.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ya.colortex.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jk.huanxung.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lt.shxzukj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ai.bjjhwx.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uy.jctech888.com.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sd.newstarts.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wo.muxihuayi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ba.lnxyls.cn

[B11] 生成数字序列 / 区间
来源：http://ew.wgjwhj.cn

Py:   list(range(0, 10, 2))
来源：http://ud.chemitech.net.cn

PHP:  range(0, 10, 2);
来源：http://hh.lnxyls.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://se.huanxung.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://we.jianghongdianzi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lc.panjiajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cc.yuexingan06.cn

Ruby: (0...10).step(2).to_a
来源：http://ky.huixinmuqiang.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ct.szxytkj.cn

[B12] 跳出多层循环
来源：http://uz.yuexingan06.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://sk.nicolike.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://te.haigaiapp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dt.chemitech.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://oc.shxzskj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ze.nszjky.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ep.bjjhwx.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jj.huixiangedu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bo.521024.cn

[B13] 判断是否为数字
来源：http://cy.haigaiapp.cn

Py:   isinstance(x, (int, float))
来源：http://jt.szxytkj.cn

PHP:  is_numeric($x)
来源：http://vz.szxytkj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fo.shxzukj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://um.nszjky.cn

Java: x instanceof Number
来源：http://ms.jianghongdianzi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hk.wgjwhj.cn

Ruby: x.is_a?(Numeric)
来源：http://cr.newstarts.cn

C#:   x is int or double or decimal
来源：http://lb.huanxung.cn

[B14] 判断值是否在集合内
来源：http://bg.shtwfgs.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gj.hnjuh.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://po.shtwfgs.cn

JS:   [1, 2, 3].includes(x)
来源：http://wp.gzmigu.cn

TS:   [1, 2, 3].includes(x)
来源：http://wu.huixiangedu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://bn.bookmarksfly.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zd.wgjwhj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qk.bjjhwx.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wl.haigaiapp.cn

[B15] 布尔运算与取反
来源：http://sy.huixiangedu.cn

Py:   a and b or not c
来源：http://vz.muxihuayi.cn

PHP:  $a && $b || !$c
来源：http://se.newstarts.cn

JS:   a && b || !c
来源：http://hh.shxzukj.cn

TS:   a && b || !c
来源：http://wh.9csxet.cn

Java: a && b || !c
来源：http://am.bjjhwx.cn

Go:   a && b || !c
来源：http://dh.huixinmuqiang.cn

Ruby: a && b || !c
来源：http://bk.newstarts.cn

C#:   a && b || !c
来源：http://zz.lnxyls.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jh.yuntaijiaju.cn

Py:   if not data: return
来源：http://hh.9csxet.cn

PHP:  if (!$data) { return; }
来源：http://dp.nszjky.cn

JS:   if (!data) return;
来源：http://ai.huixiangedu.cn

TS:   if (!data) return;
来源：http://se.9csxet.cn

Java: if (data == null) return;
来源：http://nf.9csxet.cn

Go:   if data == nil { return }
来源：http://bi.haigaiapp.cn

Ruby: return if data.nil?
来源：http://pb.hnjuh.cn

C#:   if (data == null) return;
来源：http://gp.yuntaijiaju.cn

================================================================================
来源：http://th.nicolike.cn

C. 函数与作用域
来源：http://lj.panjiajie.cn

================================================================================
来源：http://hs.shtwfgs.cn

[C01] 定义函数
来源：http://rm.wgjwhj.cn

Py:   def add(a, b): return a + b
来源：http://nb.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ho.colortex.cn

JS:   function add(a, b) { return a + b; }
来源：http://jh.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gh.jctech888.com.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qe.shxzskj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ct.nszjky.cn

Ruby: def add(a, b); a + b; end
来源：http://kv.hnjuh.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sg.muxihuayi.cn


<!-- 参考信息 -->