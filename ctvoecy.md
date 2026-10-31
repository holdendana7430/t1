代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://io.lnxyls.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ra.nicolike.cn

TS:   if (!x) {}
来源：http://yy.haigaiapp.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yd.gzmigu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://bw.bjjhwx.cn

Ruby: unless x            # nil 与 false 为假
来源：http://py.newstarts.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cq.jctech888.com.cn

[A17] 位运算
来源：http://nd.shxzukj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://un.nszjky.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://km.9csxet.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://by.nicolike.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ae.muxihuayi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qr.jianghongdianzi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ao.hahajie.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pd.lnxyls.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fc.wgjwhj.cn

[A18] 字符与 ASCII 码互转
来源：http://pl.yuntaijiaju.cn

Py:   ord("A"); chr(65)
来源：http://ag.yuntaijiaju.cn

PHP:  ord("A"); chr(65)
来源：http://pv.shtwfgs.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lh.gzmigu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://er.wgjwhj.cn

Java: (int) 'A'; (char) 65
来源：http://yo.szxytkj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pj.szsharing.cn

Ruby: "A".ord; 65.chr
来源：http://fk.521024.cn

C#:   (int)'A'; (char)65
来源：http://zo.huanxung.cn

[A19] 交换两个变量
来源：http://kv.szxytkj.cn

Py:   a, b = b, a
来源：http://mc.hahajie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://bw.jctech888.com.cn

JS:   [a, b] = [b, a];
来源：http://ht.521024.cn

TS:   [a, b] = [b, a];
来源：http://xf.jctech888.com.cn

Java: int t = a; a = b; b = t;
来源：http://tp.chemitech.net.cn

Go:   a, b = b, a
来源：http://bw.jctech888.com.cn

Ruby: a, b = b, a
来源：http://ua.gzmigu.cn

C#:   (a, b) = (b, a);
来源：http://gy.hahajie.cn

[A20] 读取标准输入
来源：http://xy.9csxet.cn

Py:   name = input("请输入：")
来源：http://ug.nicolike.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ie.lnxyls.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ry.muxihuayi.cn

TS:   // Node.js：readline 模块
来源：http://vu.huixiangedu.cn

Java: new Scanner(System.in).nextLine()
来源：http://kb.hahajie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kz.colortex.cn

Ruby: gets.chomp
来源：http://jf.chemitech.net.cn

C#:   Console.ReadLine();
来源：http://fc.yuexingan06.cn

[A21] 保留指定小数位输出
来源：http://aw.newstarts.cn

Py:   f"{3.14159:.2f}"
来源：http://nd.newstarts.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pn.521024.cn

JS:   (3.14159).toFixed(2)
来源：http://oz.jctech888.com.cn

TS:   (3.14159).toFixed(2)
来源：http://dz.asd995.cn

Java: String.format("%.2f", 3.14159)
来源：http://hc.muxihuayi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tb.muxihuayi.cn

Ruby: format("%.2f", 3.14159)
来源：http://wt.huanxung.cn

C#:   3.14159.ToString("F2")
来源：http://xq.huixinmuqiang.cn

[A22] 获取字符串长度
来源：http://om.jianghongdianzi.cn

Py:   len(s)
来源：http://vl.muxihuayi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tw.szsharing.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://yw.szsharing.cn

TS:   s.length
来源：http://ar.wgjwhj.cn

Java: s.length()
来源：http://ew.hnjuh.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ms.lnxyls.cn

Ruby: s.length
来源：http://hx.chemitech.net.cn

C#:   s.Length
来源：http://nr.wgjwhj.cn

[A23] 大小写转换
来源：http://qk.huixiangedu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wz.shxzskj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ck.jctech888.com.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wi.shtwfgs.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cj.szsharing.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ut.nszjky.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mb.nszjky.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hy.521024.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://pi.huixinmuqiang.cn

[A24] 去除首尾空白
来源：http://ux.shxzukj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://kt.chemitech.net.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fh.muxihuayi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bj.colortex.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cv.colortex.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ck.bookmarksfly.cn

Go:   strings.TrimSpace(s)
来源：http://xf.nicolike.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qb.nszjky.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://za.yuexingan06.cn

[A25] 字符串比较
来源：http://tn.gzmigu.cn

Py:   s1 == s2; s1 != s2
来源：http://lq.haigaiapp.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://el.newstarts.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pz.gzmigu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xy.huanxung.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tt.huanxung.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pz.hahajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://yy.haigaiapp.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://in.9csxet.cn

[A26] 类型转换总览
来源：http://ih.panjiajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ks.nicolike.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://we.lnxyls.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xd.nicolike.cn

TS:   Number() String() Boolean() x as number
来源：http://kd.muxihuayi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ff.shxzskj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dp.huixiangedu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ke.521024.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fa.jctech888.com.cn

================================================================================
来源：http://sc.nicolike.cn

B. 流程控制
来源：http://su.9csxet.cn

================================================================================
来源：http://wr.nicolike.cn

[B01] 条件判断 if / else
来源：http://ft.bjjhwx.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://jd.chemitech.net.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sm.9csxet.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sn.panjiajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ki.huixiangedu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bi.jctech888.com.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mq.huixiangedu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tb.szsharing.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tl.colortex.cn

[B02] 多分支 else if / elif
来源：http://lu.asd995.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hs.huixiangedu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wm.hnjuh.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ig.nszjky.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pa.muxihuayi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qg.521024.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qy.huixinmuqiang.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mc.asd995.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jf.jianghongdianzi.cn

[B03] switch / match / case
来源：http://wr.lnxyls.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zw.521024.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kk.hnjuh.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ag.shtwfgs.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pd.yuexingan06.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://da.shtwfgs.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zg.wgjwhj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://av.9csxet.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sr.huixinmuqiang.cn

[B04] for 计数循环
来源：http://bm.shxzukj.cn

Py:   for i in range(10): print(i)
来源：http://sb.hahajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vd.nicolike.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fq.colortex.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pn.jctech888.com.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://sw.lnxyls.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rr.haigaiapp.cn

Ruby: 10.times { |i| puts i }
来源：http://on.shxzskj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://py.yuntaijiaju.cn

[B05] 遍历数组 / 列表
来源：http://hr.shxzukj.cn

Py:   for item in arr: print(item)
来源：http://uv.szxytkj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hv.asd995.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ft.wgjwhj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ep.asd995.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://oj.nicolike.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jl.gzmigu.cn

Ruby: arr.each { |item| puts item }
来源：http://qz.hahajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qn.muxihuayi.cn

[B06] 遍历字典 / 对象
来源：http://fu.newstarts.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sc.jctech888.com.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pw.hahajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://li.gzmigu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bk.chemitech.net.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vv.jctech888.com.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mb.colortex.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://uu.shtwfgs.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xe.huixiangedu.cn

[B07] while 循环
来源：http://ht.yuexingan06.cn

Py:   while i < 10: i += 1
来源：http://me.szxytkj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ij.chemitech.net.cn

JS:   while (i < 10) { i++; }
来源：http://po.shtwfgs.cn

TS:   while (i < 10) { i++; }
来源：http://uc.jctech888.com.cn

Java: while (i < 10) { i++; }
来源：http://of.shxzukj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jq.panjiajie.cn

Ruby: while i < 10; i += 1; end
来源：http://oy.yuexingan06.cn

C#:   while (i < 10) { i++; }
来源：http://bo.bookmarksfly.cn

[B08] do-while（至少执行一次）
来源：http://tp.wgjwhj.cn

Py:   # 无 do-while：用 while True + break
来源：http://fp.huixiangedu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vg.muxihuayi.cn

JS:   do { i++; } while (i < 10);
来源：http://nh.panjiajie.cn

TS:   do { i++; } while (i < 10);
来源：http://jh.9csxet.cn

Java: do { i++; } while (i < 10);
来源：http://ey.shtwfgs.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ds.wgjwhj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ct.panjiajie.cn

C#:   do { i++; } while (i < 10);
来源：http://eg.nicolike.cn

[B09] break 与 continue
来源：http://yq.hahajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pf.hahajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://us.szsharing.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ub.bookmarksfly.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vl.hahajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ui.nicolike.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ec.szxytkj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hg.shtwfgs.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xj.muxihuayi.cn

[B10] 遍历同时拿索引
来源：http://ad.colortex.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dn.nicolike.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://io.hahajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gq.jianghongdianzi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dm.nicolike.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yv.szxytkj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fa.colortex.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gs.9csxet.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kc.nicolike.cn

[B11] 生成数字序列 / 区间
来源：http://bh.colortex.cn

Py:   list(range(0, 10, 2))
来源：http://ms.szxytkj.cn

PHP:  range(0, 10, 2);
来源：http://ck.muxihuayi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mu.huixiangedu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zn.panjiajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bn.hahajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xq.szxytkj.cn

Ruby: (0...10).step(2).to_a
来源：http://ol.huixinmuqiang.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wj.521024.cn

[B12] 跳出多层循环
来源：http://qe.yuntaijiaju.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://jd.muxihuayi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gr.hahajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ml.hahajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vq.shxzukj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://we.jctech888.com.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://it.lnxyls.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bp.yuexingan06.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hc.521024.cn

[B13] 判断是否为数字
来源：http://jo.bjjhwx.cn

Py:   isinstance(x, (int, float))
来源：http://qk.hahajie.cn

PHP:  is_numeric($x)
来源：http://mx.chemitech.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bu.huanxung.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xz.colortex.cn

Java: x instanceof Number
来源：http://qo.bjjhwx.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://um.jianghongdianzi.cn

Ruby: x.is_a?(Numeric)
来源：http://eo.jctech888.com.cn

C#:   x is int or double or decimal
来源：http://ty.lnxyls.cn

[B14] 判断值是否在集合内
来源：http://dx.muxihuayi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qs.jctech888.com.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://uk.bookmarksfly.cn

JS:   [1, 2, 3].includes(x)
来源：http://xz.wgjwhj.cn

TS:   [1, 2, 3].includes(x)
来源：http://pf.bookmarksfly.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://mz.521024.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://eo.bookmarksfly.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zh.yuntaijiaju.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sg.nszjky.cn

[B15] 布尔运算与取反
来源：http://bx.muxihuayi.cn

Py:   a and b or not c
来源：http://er.panjiajie.cn

PHP:  $a && $b || !$c
来源：http://zy.yuntaijiaju.cn

JS:   a && b || !c
来源：http://xn.bookmarksfly.cn

TS:   a && b || !c
来源：http://xw.yuntaijiaju.cn

Java: a && b || !c
来源：http://ca.nicolike.cn

Go:   a && b || !c
来源：http://zt.yuexingan06.cn

Ruby: a && b || !c
来源：http://km.colortex.cn

C#:   a && b || !c
来源：http://dm.yuntaijiaju.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lg.newstarts.cn

Py:   if not data: return
来源：http://ma.9csxet.cn

PHP:  if (!$data) { return; }
来源：http://yx.szsharing.cn

JS:   if (!data) return;
来源：http://nw.newstarts.cn

TS:   if (!data) return;
来源：http://zw.shxzskj.cn

Java: if (data == null) return;
来源：http://bo.colortex.cn

Go:   if data == nil { return }
来源：http://jo.jianghongdianzi.cn

Ruby: return if data.nil?
来源：http://bz.shtwfgs.cn

C#:   if (data == null) return;
来源：http://xt.yuexingan06.cn

================================================================================
来源：http://uv.hahajie.cn

C. 函数与作用域
来源：http://nw.asd995.cn

================================================================================
来源：http://ql.hnjuh.cn

[C01] 定义函数
来源：http://zj.nszjky.cn

Py:   def add(a, b): return a + b
来源：http://li.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ye.yuntaijiaju.cn

JS:   function add(a, b) { return a + b; }
来源：http://oh.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jc.szsharing.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://nf.yuntaijiaju.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ve.jianghongdianzi.cn

Ruby: def add(a, b); a + b; end
来源：http://xq.yuntaijiaju.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qk.hahajie.cn

[C02] 默认参数
来源：http://yi.panjiajie.cn

Py:   def greet(name="World"): return name
来源：http://if.panjiajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wt.panjiajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://ko.521024.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://mc.9csxet.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hr.huixinmuqiang.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rr.shtwfgs.cn

Ruby: def greet(name = "World") = name
来源：http://kq.muxihuayi.cn

C#:   string Greet(string name = "World") => name;
来源：http://nr.asd995.cn

[C03] 可变参数
来源：http://yk.colortex.cn

Py:   def total(*args): return sum(args)
来源：http://zm.shxzskj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://og.szxytkj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cv.9csxet.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bu.shtwfgs.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yk.nszjky.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rm.panjiajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vp.haigaiapp.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tp.huixiangedu.cn

[C04] 命名参数 / 关键字参数
来源：http://yl.muxihuayi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mv.huanxung.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://af.nicolike.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xn.shtwfgs.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yz.gzmigu.cn

Java: // 无：用 Builder 模式或 record
来源：http://pm.hnjuh.cn

Go:   // 无：用配置结构体参数
来源：http://ek.hnjuh.cn

Ruby: f(a: 1, b: 2)
来源：http://ag.panjiajie.cn

C#:   f(a: 1, b: 2)
来源：http://bw.panjiajie.cn

[C05] 返回多个值
来源：http://bg.bookmarksfly.cn

Py:   return a, b
来源：http://ov.szxytkj.cn

PHP:  return [$a, $b];
来源：http://ca.lnxyls.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://lk.chemitech.net.cn

TS:   return { a, b };
来源：http://za.shtwfgs.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://de.nszjky.cn

Go:   return a, b
来源：http://la.huixinmuqiang.cn

Ruby: return a, b
来源：http://co.chemitech.net.cn

C#:   return (a, b);              // ValueTuple
来源：http://ur.9csxet.cn

[C06] 匿名函数 / lambda
来源：http://gw.nicolike.cn

Py:   square = lambda x: x * x
来源：http://rq.nicolike.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ch.colortex.cn

JS:   const square = x => x * x;
来源：http://ih.huanxung.cn

TS:   const square = (x: number): number => x * x;
来源：http://fw.chemitech.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fn.lnxyls.cn

Go:   sq := func(x int) int { return x * x }
来源：http://pp.521024.cn

Ruby: square = ->(x) { x * x }
来源：http://hg.9csxet.cn


<!-- 参考信息 -->