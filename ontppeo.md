代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://ap.newstarts.cn

C#:   x > 0 ? "yes" : "no"
来源：http://kz.huixiangedu.cn

[A12] 字符串插值 / 格式化
来源：http://lm.huixinmuqiang.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pp.huixiangedu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://md.jctech888.com.cn

JS:   `Hello, ${name}!`
来源：http://up.muxihuayi.cn

TS:   `Hello, ${name}!`
来源：http://kw.chemitech.net.cn

Java: "Hello, %s!".formatted(name)
来源：http://yy.jctech888.com.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://sy.gzmigu.cn

Ruby: "Hello, #{name}!"
来源：http://zw.panjiajie.cn

C#:   $"Hello, {name}!"
来源：http://ji.shtwfgs.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://tg.panjiajie.cn

Py:   "第一行\n第二行"
来源：http://fk.szxytkj.cn

PHP:  "第一行\n第二行"
来源：http://au.newstarts.cn

JS:   "第一行\n第二行"
来源：http://ry.wgjwhj.cn

TS:   "第一行\n第二行"
来源：http://pl.chemitech.net.cn

Java: "第一行\n第二行"
来源：http://si.bookmarksfly.cn

Go:   "第一行\n第二行"
来源：http://ja.colortex.cn

Ruby: "第一行\n第二行"
来源：http://bh.panjiajie.cn

C#:   "第一行\n第二行"
来源：http://ul.haigaiapp.cn

[A14] 注释写法
来源：http://if.lnxyls.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://yu.jianghongdianzi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ut.nszjky.cn

JS:   // 单行；/* 多行 */
来源：http://lx.yuntaijiaju.cn

TS:   // 单行；/* 多行 */
来源：http://kt.hahajie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fl.wgjwhj.cn

Go:   // 单行；/* 多行 */
来源：http://db.hahajie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://jz.huixinmuqiang.cn

C#:   // 单行；/* 多行 */
来源：http://vp.colortex.cn

[A15] 空值判断与默认值
来源：http://gh.jctech888.com.cn

Py:   value = data or "默认值"
来源：http://dh.panjiajie.cn

PHP:  $value = $data ?? "默认值";
来源：http://bg.muxihuayi.cn

JS:   const value = data ?? "默认值";
来源：http://gz.huixiangedu.cn

TS:   const value = data ?? "默认值";
来源：http://vx.bjjhwx.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ww.szsharing.cn

Go:   if data == "" { data = "默认值" }
来源：http://gt.huanxung.cn

Ruby: value = data || "默认值"
来源：http://aq.9csxet.cn

C#:   var value = data ?? "默认值";
来源：http://bx.nicolike.cn

[A16] 真假值判断规则
来源：http://si.shxzskj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rv.chemitech.net.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://yv.huanxung.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://yi.jctech888.com.cn

TS:   if (!x) {}
来源：http://ig.yuexingan06.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qt.yuexingan06.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://kq.huixinmuqiang.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ph.haigaiapp.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xn.szxytkj.cn

[A17] 位运算
来源：http://yy.haigaiapp.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aj.shtwfgs.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pt.bjjhwx.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ce.bookmarksfly.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://lv.panjiajie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gr.521024.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://es.huixinmuqiang.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://by.nicolike.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zh.huixiangedu.cn

[A18] 字符与 ASCII 码互转
来源：http://vx.yuntaijiaju.cn

Py:   ord("A"); chr(65)
来源：http://ck.chemitech.net.cn

PHP:  ord("A"); chr(65)
来源：http://bc.muxihuayi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jd.gzmigu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qs.shtwfgs.cn

Java: (int) 'A'; (char) 65
来源：http://pf.bjjhwx.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://cq.szsharing.cn

Ruby: "A".ord; 65.chr
来源：http://gg.bookmarksfly.cn

C#:   (int)'A'; (char)65
来源：http://ta.newstarts.cn

[A19] 交换两个变量
来源：http://eh.huixiangedu.cn

Py:   a, b = b, a
来源：http://mg.gzmigu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://wi.huixiangedu.cn

JS:   [a, b] = [b, a];
来源：http://hm.nszjky.cn

TS:   [a, b] = [b, a];
来源：http://jx.newstarts.cn

Java: int t = a; a = b; b = t;
来源：http://ta.huixiangedu.cn

Go:   a, b = b, a
来源：http://aw.huixinmuqiang.cn

Ruby: a, b = b, a
来源：http://bn.colortex.cn

C#:   (a, b) = (b, a);
来源：http://bs.panjiajie.cn

[A20] 读取标准输入
来源：http://le.bookmarksfly.cn

Py:   name = input("请输入：")
来源：http://yb.jctech888.com.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://wn.huanxung.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bc.chemitech.net.cn

TS:   // Node.js：readline 模块
来源：http://dl.shxzukj.cn

Java: new Scanner(System.in).nextLine()
来源：http://sk.huixinmuqiang.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ms.shtwfgs.cn

Ruby: gets.chomp
来源：http://if.huanxung.cn

C#:   Console.ReadLine();
来源：http://jm.huixiangedu.cn

[A21] 保留指定小数位输出
来源：http://jw.bookmarksfly.cn

Py:   f"{3.14159:.2f}"
来源：http://ax.hahajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://he.nszjky.cn

JS:   (3.14159).toFixed(2)
来源：http://pg.wgjwhj.cn

TS:   (3.14159).toFixed(2)
来源：http://qw.asd995.cn

Java: String.format("%.2f", 3.14159)
来源：http://sg.asd995.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xp.chemitech.net.cn

Ruby: format("%.2f", 3.14159)
来源：http://pj.szxytkj.cn

C#:   3.14159.ToString("F2")
来源：http://yd.chemitech.net.cn

[A22] 获取字符串长度
来源：http://cz.huixiangedu.cn

Py:   len(s)
来源：http://db.jctech888.com.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://lq.colortex.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bo.chemitech.net.cn

TS:   s.length
来源：http://zt.asd995.cn

Java: s.length()
来源：http://ox.gzmigu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xx.shxzskj.cn

Ruby: s.length
来源：http://jz.hahajie.cn

C#:   s.Length
来源：http://cb.nicolike.cn

[A23] 大小写转换
来源：http://em.colortex.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ax.huixinmuqiang.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kn.bookmarksfly.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jm.jianghongdianzi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cr.jctech888.com.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ub.nicolike.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tt.haigaiapp.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ry.szxytkj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zi.szxytkj.cn

[A24] 去除首尾空白
来源：http://vm.yuexingan06.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jj.hnjuh.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xl.newstarts.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uq.wgjwhj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bc.yuntaijiaju.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qo.nszjky.cn

Go:   strings.TrimSpace(s)
来源：http://ih.jianghongdianzi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bu.huixiangedu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pf.chemitech.net.cn

[A25] 字符串比较
来源：http://pn.hahajie.cn

Py:   s1 == s2; s1 != s2
来源：http://xz.huixiangedu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cr.wgjwhj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wd.nicolike.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ni.yuexingan06.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mk.shtwfgs.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://je.colortex.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ea.jctech888.com.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ii.nicolike.cn

[A26] 类型转换总览
来源：http://dv.shxzskj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fe.lnxyls.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fj.lnxyls.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bg.newstarts.cn

TS:   Number() String() Boolean() x as number
来源：http://ay.szxytkj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ch.muxihuayi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ro.9csxet.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mr.gzmigu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ky.gzmigu.cn

================================================================================
来源：http://bx.newstarts.cn

B. 流程控制
来源：http://md.gzmigu.cn

================================================================================
来源：http://ul.colortex.cn

[B01] 条件判断 if / else
来源：http://dj.yuntaijiaju.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bl.yuexingan06.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://eh.lnxyls.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ij.gzmigu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sd.newstarts.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bc.hahajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://go.yuexingan06.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jf.newstarts.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nv.yuntaijiaju.cn

[B02] 多分支 else if / elif
来源：http://xh.huixiangedu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ni.shxzukj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zs.panjiajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uy.szxytkj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://is.huanxung.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jg.lnxyls.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bx.colortex.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://el.shxzskj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gx.colortex.cn

[B03] switch / match / case
来源：http://gu.jianghongdianzi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qw.colortex.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uq.colortex.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lv.haigaiapp.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tf.szsharing.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ab.hnjuh.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qv.bookmarksfly.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bd.huixinmuqiang.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gv.yuntaijiaju.cn

[B04] for 计数循环
来源：http://qx.panjiajie.cn

Py:   for i in range(10): print(i)
来源：http://qs.szxytkj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vv.shtwfgs.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cb.nicolike.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ak.yuntaijiaju.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uw.wgjwhj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tv.asd995.cn

Ruby: 10.times { |i| puts i }
来源：http://ch.huixinmuqiang.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fv.hnjuh.cn

[B05] 遍历数组 / 列表
来源：http://fl.521024.cn

Py:   for item in arr: print(item)
来源：http://rq.chemitech.net.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sh.jianghongdianzi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hj.wgjwhj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ff.shtwfgs.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wf.yuntaijiaju.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rs.jctech888.com.cn

Ruby: arr.each { |item| puts item }
来源：http://bf.shxzskj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pq.haigaiapp.cn

[B06] 遍历字典 / 对象
来源：http://jy.bjjhwx.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://wd.haigaiapp.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ns.yuntaijiaju.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mi.huixiangedu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sl.nszjky.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sh.jianghongdianzi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qd.asd995.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tp.wgjwhj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://za.bjjhwx.cn

[B07] while 循环
来源：http://zr.colortex.cn

Py:   while i < 10: i += 1
来源：http://wc.szxytkj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://an.muxihuayi.cn

JS:   while (i < 10) { i++; }
来源：http://eq.muxihuayi.cn

TS:   while (i < 10) { i++; }
来源：http://nr.bjjhwx.cn

Java: while (i < 10) { i++; }
来源：http://qq.bookmarksfly.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zy.huixinmuqiang.cn

Ruby: while i < 10; i += 1; end
来源：http://pq.chemitech.net.cn

C#:   while (i < 10) { i++; }
来源：http://do.hahajie.cn

[B08] do-while（至少执行一次）
来源：http://yk.yuntaijiaju.cn

Py:   # 无 do-while：用 while True + break
来源：http://lm.szsharing.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://hc.bookmarksfly.cn

JS:   do { i++; } while (i < 10);
来源：http://vp.nszjky.cn

TS:   do { i++; } while (i < 10);
来源：http://ji.asd995.cn

Java: do { i++; } while (i < 10);
来源：http://og.shtwfgs.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://eo.muxihuayi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cv.hahajie.cn

C#:   do { i++; } while (i < 10);
来源：http://ys.szsharing.cn

[B09] break 与 continue
来源：http://ub.bookmarksfly.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cy.huixiangedu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hp.haigaiapp.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pc.chemitech.net.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cj.huixiangedu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ik.huixinmuqiang.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wx.shxzukj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rj.nszjky.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lg.nszjky.cn

[B10] 遍历同时拿索引
来源：http://cq.shxzukj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tm.hnjuh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ig.yuntaijiaju.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ea.nszjky.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ah.nicolike.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bm.nicolike.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ui.lnxyls.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kb.muxihuayi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vi.muxihuayi.cn

[B11] 生成数字序列 / 区间
来源：http://ob.jctech888.com.cn

Py:   list(range(0, 10, 2))
来源：http://hx.bjjhwx.cn

PHP:  range(0, 10, 2);
来源：http://lr.shxzskj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bv.yuntaijiaju.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gj.shxzskj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kd.521024.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://on.muxihuayi.cn

Ruby: (0...10).step(2).to_a
来源：http://zx.nicolike.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qq.jianghongdianzi.cn

[B12] 跳出多层循环
来源：http://hi.yuexingan06.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://eo.gzmigu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ib.lnxyls.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://eu.shxzukj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://py.wgjwhj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://la.muxihuayi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hn.hahajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nt.bookmarksfly.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ym.hahajie.cn

[B13] 判断是否为数字
来源：http://ou.yuexingan06.cn

Py:   isinstance(x, (int, float))
来源：http://tt.bjjhwx.cn

PHP:  is_numeric($x)
来源：http://qe.bjjhwx.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://na.yuexingan06.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kl.hnjuh.cn

Java: x instanceof Number
来源：http://jj.bjjhwx.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xv.nszjky.cn

Ruby: x.is_a?(Numeric)
来源：http://hy.jctech888.com.cn

C#:   x is int or double or decimal
来源：http://io.huanxung.cn

[B14] 判断值是否在集合内
来源：http://ex.hnjuh.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bk.huixinmuqiang.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jt.huixinmuqiang.cn

JS:   [1, 2, 3].includes(x)
来源：http://hs.shtwfgs.cn

TS:   [1, 2, 3].includes(x)
来源：http://ol.wgjwhj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dh.hnjuh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yb.szxytkj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cn.shxzukj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ow.bjjhwx.cn

[B15] 布尔运算与取反
来源：http://sm.newstarts.cn

Py:   a and b or not c
来源：http://de.shtwfgs.cn

PHP:  $a && $b || !$c
来源：http://kv.szxytkj.cn

JS:   a && b || !c
来源：http://uv.nszjky.cn

TS:   a && b || !c
来源：http://tp.huixinmuqiang.cn

Java: a && b || !c
来源：http://ir.jianghongdianzi.cn

Go:   a && b || !c
来源：http://jl.yuntaijiaju.cn

Ruby: a && b || !c
来源：http://jn.wgjwhj.cn

C#:   a && b || !c
来源：http://dd.asd995.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hk.gzmigu.cn

Py:   if not data: return
来源：http://eo.shxzskj.cn

PHP:  if (!$data) { return; }
来源：http://sx.hnjuh.cn

JS:   if (!data) return;
来源：http://ia.9csxet.cn

TS:   if (!data) return;
来源：http://bn.shxzukj.cn

Java: if (data == null) return;
来源：http://ef.newstarts.cn

Go:   if data == nil { return }
来源：http://ak.haigaiapp.cn

Ruby: return if data.nil?
来源：http://bj.huanxung.cn

C#:   if (data == null) return;
来源：http://zv.muxihuayi.cn

================================================================================
来源：http://ho.jctech888.com.cn

C. 函数与作用域
来源：http://kt.nszjky.cn

================================================================================
来源：http://rv.shxzskj.cn

[C01] 定义函数
来源：http://wi.nicolike.cn

Py:   def add(a, b): return a + b
来源：http://at.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dx.szsharing.cn

JS:   function add(a, b) { return a + b; }
来源：http://sy.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://le.huixiangedu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dy.lnxyls.cn

Go:   func add(a, b int) int { return a + b }
来源：http://fb.hnjuh.cn

Ruby: def add(a, b); a + b; end
来源：http://tg.jianghongdianzi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tz.panjiajie.cn

[C02] 默认参数
来源：http://gu.muxihuayi.cn

Py:   def greet(name="World"): return name
来源：http://lm.szxytkj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vz.521024.cn

JS:   function greet(name = "World") { return name; }
来源：http://pr.colortex.cn


<!-- 参考信息 -->