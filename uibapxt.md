代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://cu.huixinmuqiang.cn

Ruby: "Hello, #{name}!"
来源：http://di.lnxyls.cn

C#:   $"Hello, {name}!"
来源：http://pe.panjiajie.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://av.jctech888.com.cn

Py:   "第一行\n第二行"
来源：http://ij.yuexingan06.cn

PHP:  "第一行\n第二行"
来源：http://nw.jctech888.com.cn

JS:   "第一行\n第二行"
来源：http://zh.shxzukj.cn

TS:   "第一行\n第二行"
来源：http://ff.yuntaijiaju.cn

Java: "第一行\n第二行"
来源：http://nv.huixinmuqiang.cn

Go:   "第一行\n第二行"
来源：http://yy.9csxet.cn

Ruby: "第一行\n第二行"
来源：http://gm.hahajie.cn

C#:   "第一行\n第二行"
来源：http://sf.9csxet.cn

[A14] 注释写法
来源：http://ry.huixiangedu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ve.szxytkj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://cj.huanxung.cn

JS:   // 单行；/* 多行 */
来源：http://zn.jctech888.com.cn

TS:   // 单行；/* 多行 */
来源：http://sl.yuexingan06.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://nv.muxihuayi.cn

Go:   // 单行；/* 多行 */
来源：http://sh.szxytkj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://vk.szsharing.cn

C#:   // 单行；/* 多行 */
来源：http://vh.hahajie.cn

[A15] 空值判断与默认值
来源：http://ls.chemitech.net.cn

Py:   value = data or "默认值"
来源：http://ar.jianghongdianzi.cn

PHP:  $value = $data ?? "默认值";
来源：http://zx.jctech888.com.cn

JS:   const value = data ?? "默认值";
来源：http://ct.bjjhwx.cn

TS:   const value = data ?? "默认值";
来源：http://vo.asd995.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gt.bookmarksfly.cn

Go:   if data == "" { data = "默认值" }
来源：http://xq.szxytkj.cn

Ruby: value = data || "默认值"
来源：http://fx.newstarts.cn

C#:   var value = data ?? "默认值";
来源：http://tj.hnjuh.cn

[A16] 真假值判断规则
来源：http://lr.shxzukj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jf.gzmigu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://cg.jctech888.com.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hu.muxihuayi.cn

TS:   if (!x) {}
来源：http://mu.muxihuayi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://su.gzmigu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yf.521024.cn

Ruby: unless x            # nil 与 false 为假
来源：http://mz.nszjky.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://eh.shxzukj.cn

[A17] 位运算
来源：http://av.nszjky.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qx.nszjky.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gb.jianghongdianzi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ix.asd995.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ww.asd995.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xd.szxytkj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ih.jianghongdianzi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gs.shtwfgs.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vw.521024.cn

[A18] 字符与 ASCII 码互转
来源：http://fz.huixiangedu.cn

Py:   ord("A"); chr(65)
来源：http://jp.huixiangedu.cn

PHP:  ord("A"); chr(65)
来源：http://qn.shxzukj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ji.hahajie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ap.szsharing.cn

Java: (int) 'A'; (char) 65
来源：http://ej.yuntaijiaju.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hs.huixinmuqiang.cn

Ruby: "A".ord; 65.chr
来源：http://ab.wgjwhj.cn

C#:   (int)'A'; (char)65
来源：http://nb.panjiajie.cn

[A19] 交换两个变量
来源：http://zj.panjiajie.cn

Py:   a, b = b, a
来源：http://ug.bookmarksfly.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://fz.jianghongdianzi.cn

JS:   [a, b] = [b, a];
来源：http://nd.muxihuayi.cn

TS:   [a, b] = [b, a];
来源：http://sy.9csxet.cn

Java: int t = a; a = b; b = t;
来源：http://ma.panjiajie.cn

Go:   a, b = b, a
来源：http://as.bjjhwx.cn

Ruby: a, b = b, a
来源：http://ev.shtwfgs.cn

C#:   (a, b) = (b, a);
来源：http://rd.shtwfgs.cn

[A20] 读取标准输入
来源：http://hr.wgjwhj.cn

Py:   name = input("请输入：")
来源：http://ln.muxihuayi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://qn.shxzukj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jd.gzmigu.cn

TS:   // Node.js：readline 模块
来源：http://sd.asd995.cn

Java: new Scanner(System.in).nextLine()
来源：http://ae.shxzukj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://uw.huanxung.cn

Ruby: gets.chomp
来源：http://ge.jianghongdianzi.cn

C#:   Console.ReadLine();
来源：http://md.gzmigu.cn

[A21] 保留指定小数位输出
来源：http://dw.gzmigu.cn

Py:   f"{3.14159:.2f}"
来源：http://gz.shxzukj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dl.colortex.cn

JS:   (3.14159).toFixed(2)
来源：http://jj.szxytkj.cn

TS:   (3.14159).toFixed(2)
来源：http://vd.9csxet.cn

Java: String.format("%.2f", 3.14159)
来源：http://pu.hahajie.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yn.lnxyls.cn

Ruby: format("%.2f", 3.14159)
来源：http://fh.shtwfgs.cn

C#:   3.14159.ToString("F2")
来源：http://yn.newstarts.cn

[A22] 获取字符串长度
来源：http://jl.haigaiapp.cn

Py:   len(s)
来源：http://oc.shxzukj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://oi.nicolike.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vw.muxihuayi.cn

TS:   s.length
来源：http://ri.nicolike.cn

Java: s.length()
来源：http://mx.newstarts.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://li.muxihuayi.cn

Ruby: s.length
来源：http://qo.jianghongdianzi.cn

C#:   s.Length
来源：http://yo.lnxyls.cn

[A23] 大小写转换
来源：http://bz.panjiajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ag.huanxung.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://es.jctech888.com.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vj.yuexingan06.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cs.jctech888.com.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rv.muxihuayi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mb.yuntaijiaju.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wn.yuexingan06.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://fu.shtwfgs.cn

[A24] 去除首尾空白
来源：http://tj.huixinmuqiang.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tv.nszjky.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ve.yuexingan06.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://to.muxihuayi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hm.bookmarksfly.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://sy.muxihuayi.cn

Go:   strings.TrimSpace(s)
来源：http://oo.gzmigu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mk.9csxet.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sp.wgjwhj.cn

[A25] 字符串比较
来源：http://sm.bjjhwx.cn

Py:   s1 == s2; s1 != s2
来源：http://ng.nszjky.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cr.newstarts.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wl.jianghongdianzi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://im.shxzukj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://im.szxytkj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bj.szxytkj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rn.muxihuayi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xe.yuntaijiaju.cn

[A26] 类型转换总览
来源：http://lt.9csxet.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lb.huixiangedu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://my.huanxung.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://io.chemitech.net.cn

TS:   Number() String() Boolean() x as number
来源：http://lm.huanxung.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://js.szxytkj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yc.nicolike.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://if.newstarts.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ji.panjiajie.cn

================================================================================
来源：http://pq.yuntaijiaju.cn

B. 流程控制
来源：http://xv.9csxet.cn

================================================================================
来源：http://vx.nszjky.cn

[B01] 条件判断 if / else
来源：http://gi.szxytkj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ol.lnxyls.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://el.shxzskj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bp.yuexingan06.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://uy.lnxyls.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://dd.bookmarksfly.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tl.lnxyls.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zn.newstarts.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xx.shxzukj.cn

[B02] 多分支 else if / elif
来源：http://cn.panjiajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rg.521024.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ho.bjjhwx.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gr.chemitech.net.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yi.nicolike.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ni.szxytkj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://px.lnxyls.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ur.nszjky.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hg.bookmarksfly.cn

[B03] switch / match / case
来源：http://vd.hnjuh.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bx.jctech888.com.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ad.szxytkj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jz.bookmarksfly.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ix.szxytkj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://oe.szsharing.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ve.muxihuayi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bm.nszjky.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zt.szxytkj.cn

[B04] for 计数循环
来源：http://ho.jctech888.com.cn

Py:   for i in range(10): print(i)
来源：http://ti.shtwfgs.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bc.nszjky.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qh.colortex.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dx.colortex.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tf.szxytkj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://uu.bjjhwx.cn

Ruby: 10.times { |i| puts i }
来源：http://ry.chemitech.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://au.asd995.cn

[B05] 遍历数组 / 列表
来源：http://pv.huanxung.cn

Py:   for item in arr: print(item)
来源：http://zl.panjiajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jc.jctech888.com.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://rt.haigaiapp.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ii.szsharing.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ho.yuntaijiaju.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mw.gzmigu.cn

Ruby: arr.each { |item| puts item }
来源：http://kz.shxzskj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sx.shtwfgs.cn

[B06] 遍历字典 / 对象
来源：http://dv.9csxet.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ky.colortex.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://so.shtwfgs.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qw.yuexingan06.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mb.newstarts.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://oj.huixiangedu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ew.panjiajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://of.panjiajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vu.shxzukj.cn

[B07] while 循环
来源：http://my.shxzukj.cn

Py:   while i < 10: i += 1
来源：http://gv.gzmigu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wq.521024.cn

JS:   while (i < 10) { i++; }
来源：http://da.haigaiapp.cn

TS:   while (i < 10) { i++; }
来源：http://ko.haigaiapp.cn

Java: while (i < 10) { i++; }
来源：http://lm.szxytkj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pp.shxzukj.cn

Ruby: while i < 10; i += 1; end
来源：http://cp.panjiajie.cn

C#:   while (i < 10) { i++; }
来源：http://wm.szxytkj.cn

[B08] do-while（至少执行一次）
来源：http://li.szsharing.cn

Py:   # 无 do-while：用 while True + break
来源：http://fa.bookmarksfly.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cj.wgjwhj.cn

JS:   do { i++; } while (i < 10);
来源：http://ni.shxzskj.cn

TS:   do { i++; } while (i < 10);
来源：http://yh.yuexingan06.cn

Java: do { i++; } while (i < 10);
来源：http://qt.gzmigu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vy.gzmigu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ga.asd995.cn

C#:   do { i++; } while (i < 10);
来源：http://ww.huanxung.cn

[B09] break 与 continue
来源：http://py.bjjhwx.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wb.asd995.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ap.shxzukj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qz.yuntaijiaju.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cb.muxihuayi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://le.szxytkj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sg.nicolike.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kt.huixinmuqiang.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gn.yuexingan06.cn

[B10] 遍历同时拿索引
来源：http://pl.gzmigu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sc.colortex.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cc.hahajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://iq.colortex.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nx.lnxyls.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fq.nicolike.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kz.nicolike.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://do.hahajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://id.huixiangedu.cn

[B11] 生成数字序列 / 区间
来源：http://gu.newstarts.cn

Py:   list(range(0, 10, 2))
来源：http://vb.bjjhwx.cn

PHP:  range(0, 10, 2);
来源：http://uo.gzmigu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ah.muxihuayi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ez.muxihuayi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ro.muxihuayi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ji.hnjuh.cn

Ruby: (0...10).step(2).to_a
来源：http://qq.shxzskj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kp.muxihuayi.cn

[B12] 跳出多层循环
来源：http://az.asd995.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ix.hahajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://et.gzmigu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ea.szsharing.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bw.shxzukj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hi.hnjuh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mt.521024.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bx.panjiajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ne.521024.cn

[B13] 判断是否为数字
来源：http://ax.bjjhwx.cn

Py:   isinstance(x, (int, float))
来源：http://qp.huixiangedu.cn

PHP:  is_numeric($x)
来源：http://us.asd995.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lo.521024.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yv.wgjwhj.cn

Java: x instanceof Number
来源：http://nl.shtwfgs.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://eq.bookmarksfly.cn

Ruby: x.is_a?(Numeric)
来源：http://xh.szxytkj.cn

C#:   x is int or double or decimal
来源：http://ai.asd995.cn

[B14] 判断值是否在集合内
来源：http://pa.shxzskj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wx.521024.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dl.nszjky.cn

JS:   [1, 2, 3].includes(x)
来源：http://ra.muxihuayi.cn

TS:   [1, 2, 3].includes(x)
来源：http://kw.bjjhwx.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://bt.asd995.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hw.9csxet.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xe.huixinmuqiang.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://by.nicolike.cn

[B15] 布尔运算与取反
来源：http://fu.bookmarksfly.cn

Py:   a and b or not c
来源：http://yp.jianghongdianzi.cn

PHP:  $a && $b || !$c
来源：http://zq.hnjuh.cn

JS:   a && b || !c
来源：http://qu.shxzukj.cn

TS:   a && b || !c
来源：http://vv.muxihuayi.cn

Java: a && b || !c
来源：http://dl.huixiangedu.cn

Go:   a && b || !c
来源：http://tm.panjiajie.cn

Ruby: a && b || !c
来源：http://bk.gzmigu.cn

C#:   a && b || !c
来源：http://ch.lnxyls.cn

[B16] 卫语句：不满足条件提前返回
来源：http://tg.521024.cn

Py:   if not data: return
来源：http://rz.asd995.cn

PHP:  if (!$data) { return; }
来源：http://ni.colortex.cn

JS:   if (!data) return;
来源：http://mf.gzmigu.cn

TS:   if (!data) return;
来源：http://xh.shtwfgs.cn

Java: if (data == null) return;
来源：http://uk.gzmigu.cn

Go:   if data == nil { return }
来源：http://tl.colortex.cn

Ruby: return if data.nil?
来源：http://qo.521024.cn

C#:   if (data == null) return;
来源：http://zk.colortex.cn

================================================================================
来源：http://ua.521024.cn

C. 函数与作用域
来源：http://uy.colortex.cn

================================================================================
来源：http://jm.yuexingan06.cn

[C01] 定义函数
来源：http://oc.9csxet.cn

Py:   def add(a, b): return a + b
来源：http://dj.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pn.shxzskj.cn

JS:   function add(a, b) { return a + b; }
来源：http://tc.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://us.szxytkj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ue.panjiajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hj.huanxung.cn

Ruby: def add(a, b); a + b; end
来源：http://pi.hnjuh.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ur.hnjuh.cn

[C02] 默认参数
来源：http://yf.szxytkj.cn

Py:   def greet(name="World"): return name
来源：http://ef.shtwfgs.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vi.9csxet.cn

JS:   function greet(name = "World") { return name; }
来源：http://ke.muxihuayi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yo.hnjuh.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jb.gzmigu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qr.nicolike.cn

Ruby: def greet(name = "World") = name
来源：http://lu.yuexingan06.cn

C#:   string Greet(string name = "World") => name;
来源：http://vy.nicolike.cn

[C03] 可变参数
来源：http://kl.bookmarksfly.cn

Py:   def total(*args): return sum(args)
来源：http://dw.bjjhwx.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qr.chemitech.net.cn


<!-- 参考信息 -->