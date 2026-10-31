代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ow.hnjuh.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lf.asd995.cn

TS:   if (!x) {}
来源：http://lg.yuntaijiaju.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://pl.gzmigu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ri.colortex.cn

Ruby: unless x            # nil 与 false 为假
来源：http://gp.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://tm.nszjky.cn

[A17] 位运算
来源：http://ta.shtwfgs.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nt.bjjhwx.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jv.shtwfgs.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rs.haigaiapp.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hc.9csxet.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://km.jctech888.com.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://yx.yuexingan06.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wh.szxytkj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ng.wgjwhj.cn

[A18] 字符与 ASCII 码互转
来源：http://ff.shxzukj.cn

Py:   ord("A"); chr(65)
来源：http://cs.haigaiapp.cn

PHP:  ord("A"); chr(65)
来源：http://ko.bookmarksfly.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vk.yuntaijiaju.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nl.asd995.cn

Java: (int) 'A'; (char) 65
来源：http://qg.bookmarksfly.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ko.gzmigu.cn

Ruby: "A".ord; 65.chr
来源：http://wt.haigaiapp.cn

C#:   (int)'A'; (char)65
来源：http://uj.shxzukj.cn

[A19] 交换两个变量
来源：http://kc.bjjhwx.cn

Py:   a, b = b, a
来源：http://nn.nszjky.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ne.yuexingan06.cn

JS:   [a, b] = [b, a];
来源：http://dh.lnxyls.cn

TS:   [a, b] = [b, a];
来源：http://kk.huixiangedu.cn

Java: int t = a; a = b; b = t;
来源：http://ws.hahajie.cn

Go:   a, b = b, a
来源：http://nj.chemitech.net.cn

Ruby: a, b = b, a
来源：http://ll.lnxyls.cn

C#:   (a, b) = (b, a);
来源：http://nj.shxzukj.cn

[A20] 读取标准输入
来源：http://ky.hahajie.cn

Py:   name = input("请输入：")
来源：http://ur.nicolike.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://fi.muxihuayi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ab.chemitech.net.cn

TS:   // Node.js：readline 模块
来源：http://py.lnxyls.cn

Java: new Scanner(System.in).nextLine()
来源：http://me.panjiajie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://sw.huixiangedu.cn

Ruby: gets.chomp
来源：http://te.bjjhwx.cn

C#:   Console.ReadLine();
来源：http://rc.szsharing.cn

[A21] 保留指定小数位输出
来源：http://xi.hnjuh.cn

Py:   f"{3.14159:.2f}"
来源：http://jv.asd995.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://af.yuntaijiaju.cn

JS:   (3.14159).toFixed(2)
来源：http://fi.jctech888.com.cn

TS:   (3.14159).toFixed(2)
来源：http://gc.bjjhwx.cn

Java: String.format("%.2f", 3.14159)
来源：http://dq.9csxet.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://cc.wgjwhj.cn

Ruby: format("%.2f", 3.14159)
来源：http://cj.colortex.cn

C#:   3.14159.ToString("F2")
来源：http://il.newstarts.cn

[A22] 获取字符串长度
来源：http://ye.jianghongdianzi.cn

Py:   len(s)
来源：http://jj.szxytkj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rz.hnjuh.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jq.hahajie.cn

TS:   s.length
来源：http://vd.szsharing.cn

Java: s.length()
来源：http://pv.bjjhwx.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mt.bjjhwx.cn

Ruby: s.length
来源：http://gm.shxzukj.cn

C#:   s.Length
来源：http://vh.hahajie.cn

[A23] 大小写转换
来源：http://gn.shxzukj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ms.asd995.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://br.521024.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vq.huixinmuqiang.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ph.9csxet.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nn.bookmarksfly.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ob.nicolike.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ah.9csxet.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://fx.hahajie.cn

[A24] 去除首尾空白
来源：http://og.huanxung.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mz.colortex.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vr.huixiangedu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fj.panjiajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fa.szxytkj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zo.shxzskj.cn

Go:   strings.TrimSpace(s)
来源：http://pn.haigaiapp.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://iu.haigaiapp.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ol.szxytkj.cn

[A25] 字符串比较
来源：http://gx.shxzskj.cn

Py:   s1 == s2; s1 != s2
来源：http://rt.panjiajie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ox.muxihuayi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://em.bjjhwx.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fg.newstarts.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ze.wgjwhj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://le.newstarts.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://xo.gzmigu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wp.jianghongdianzi.cn

[A26] 类型转换总览
来源：http://af.9csxet.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ia.asd995.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://py.shxzskj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://in.colortex.cn

TS:   Number() String() Boolean() x as number
来源：http://ye.huixiangedu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cy.bookmarksfly.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bc.bookmarksfly.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://hu.huixinmuqiang.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://es.panjiajie.cn

================================================================================
来源：http://hj.bookmarksfly.cn

B. 流程控制
来源：http://hq.colortex.cn

================================================================================
来源：http://bq.asd995.cn

[B01] 条件判断 if / else
来源：http://co.nszjky.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://jn.shtwfgs.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vg.521024.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tn.521024.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://or.yuexingan06.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ru.521024.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qr.nicolike.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yh.hahajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gd.huixiangedu.cn

[B02] 多分支 else if / elif
来源：http://we.haigaiapp.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qg.asd995.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wt.huanxung.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nu.newstarts.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sa.9csxet.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tt.gzmigu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uj.521024.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bg.colortex.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xf.haigaiapp.cn

[B03] switch / match / case
来源：http://em.wgjwhj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dr.nicolike.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hh.hnjuh.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://au.shtwfgs.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://re.yuntaijiaju.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fw.nicolike.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ws.hahajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rt.nicolike.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yg.huixinmuqiang.cn

[B04] for 计数循环
来源：http://ky.bookmarksfly.cn

Py:   for i in range(10): print(i)
来源：http://vu.asd995.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xd.bookmarksfly.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mn.asd995.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vv.wgjwhj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ke.colortex.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hc.szsharing.cn

Ruby: 10.times { |i| puts i }
来源：http://bu.panjiajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ds.asd995.cn

[B05] 遍历数组 / 列表
来源：http://cs.haigaiapp.cn

Py:   for item in arr: print(item)
来源：http://vo.jctech888.com.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sw.huanxung.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ot.wgjwhj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://kf.bookmarksfly.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://mg.nicolike.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nj.shtwfgs.cn

Ruby: arr.each { |item| puts item }
来源：http://hz.bjjhwx.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hk.huixiangedu.cn

[B06] 遍历字典 / 对象
来源：http://qd.huixiangedu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sv.bookmarksfly.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hx.nszjky.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rm.chemitech.net.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lg.shtwfgs.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uw.wgjwhj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dp.hahajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qv.szsharing.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pu.huixinmuqiang.cn

[B07] while 循环
来源：http://gf.newstarts.cn

Py:   while i < 10: i += 1
来源：http://vg.shxzukj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://al.hahajie.cn

JS:   while (i < 10) { i++; }
来源：http://ki.gzmigu.cn

TS:   while (i < 10) { i++; }
来源：http://ib.gzmigu.cn

Java: while (i < 10) { i++; }
来源：http://sp.huixinmuqiang.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sa.huanxung.cn

Ruby: while i < 10; i += 1; end
来源：http://ul.bookmarksfly.cn

C#:   while (i < 10) { i++; }
来源：http://ak.bjjhwx.cn

[B08] do-while（至少执行一次）
来源：http://vf.huixiangedu.cn

Py:   # 无 do-while：用 while True + break
来源：http://qj.newstarts.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://nf.nszjky.cn

JS:   do { i++; } while (i < 10);
来源：http://he.jctech888.com.cn

TS:   do { i++; } while (i < 10);
来源：http://og.muxihuayi.cn

Java: do { i++; } while (i < 10);
来源：http://za.hnjuh.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vj.huanxung.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wp.nszjky.cn

C#:   do { i++; } while (i < 10);
来源：http://eg.nszjky.cn

[B09] break 与 continue
来源：http://ds.newstarts.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ye.huixiangedu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qw.lnxyls.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jy.shxzskj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.szsharing.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ct.hnjuh.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ib.yuexingan06.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xj.lnxyls.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vk.szsharing.cn

[B10] 遍历同时拿索引
来源：http://as.shtwfgs.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xk.huixiangedu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qf.shtwfgs.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yg.huixinmuqiang.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uy.9csxet.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ac.haigaiapp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tu.shxzskj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ac.nszjky.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dp.panjiajie.cn

[B11] 生成数字序列 / 区间
来源：http://zi.huixinmuqiang.cn

Py:   list(range(0, 10, 2))
来源：http://un.muxihuayi.cn

PHP:  range(0, 10, 2);
来源：http://ks.521024.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pq.jctech888.com.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ey.shxzukj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lr.yuexingan06.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hp.gzmigu.cn

Ruby: (0...10).step(2).to_a
来源：http://lo.huanxung.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rk.huixinmuqiang.cn

[B12] 跳出多层循环
来源：http://bn.newstarts.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ze.haigaiapp.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zs.huanxung.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lk.szsharing.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ya.yuntaijiaju.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://py.wgjwhj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gy.jianghongdianzi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ck.huixiangedu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://oc.yuexingan06.cn

[B13] 判断是否为数字
来源：http://ca.panjiajie.cn

Py:   isinstance(x, (int, float))
来源：http://qq.yuexingan06.cn

PHP:  is_numeric($x)
来源：http://sa.nszjky.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ns.huanxung.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qa.szsharing.cn

Java: x instanceof Number
来源：http://xw.colortex.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ad.bookmarksfly.cn

Ruby: x.is_a?(Numeric)
来源：http://qc.asd995.cn

C#:   x is int or double or decimal
来源：http://gz.jctech888.com.cn

[B14] 判断值是否在集合内
来源：http://jd.shtwfgs.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://re.huixinmuqiang.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gw.shtwfgs.cn

JS:   [1, 2, 3].includes(x)
来源：http://gi.szxytkj.cn

TS:   [1, 2, 3].includes(x)
来源：http://su.hahajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://fl.yuexingan06.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bl.nicolike.cn

Ruby: [1, 2, 3].include?(x)
来源：http://bk.huixiangedu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ny.jianghongdianzi.cn

[B15] 布尔运算与取反
来源：http://oq.newstarts.cn

Py:   a and b or not c
来源：http://ye.lnxyls.cn

PHP:  $a && $b || !$c
来源：http://po.jianghongdianzi.cn

JS:   a && b || !c
来源：http://rs.chemitech.net.cn

TS:   a && b || !c
来源：http://zm.shtwfgs.cn

Java: a && b || !c
来源：http://da.haigaiapp.cn

Go:   a && b || !c
来源：http://nj.shxzukj.cn

Ruby: a && b || !c
来源：http://up.shtwfgs.cn

C#:   a && b || !c
来源：http://gi.lnxyls.cn

[B16] 卫语句：不满足条件提前返回
来源：http://go.gzmigu.cn

Py:   if not data: return
来源：http://gf.nszjky.cn

PHP:  if (!$data) { return; }
来源：http://sk.jianghongdianzi.cn

JS:   if (!data) return;
来源：http://dr.521024.cn

TS:   if (!data) return;
来源：http://ec.wgjwhj.cn

Java: if (data == null) return;
来源：http://uz.szxytkj.cn

Go:   if data == nil { return }
来源：http://vo.hnjuh.cn

Ruby: return if data.nil?
来源：http://vb.hahajie.cn

C#:   if (data == null) return;
来源：http://ol.hnjuh.cn

================================================================================
来源：http://rk.lnxyls.cn

C. 函数与作用域
来源：http://gd.shxzskj.cn

================================================================================
来源：http://qi.jianghongdianzi.cn

[C01] 定义函数
来源：http://ph.521024.cn

Py:   def add(a, b): return a + b
来源：http://ax.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ws.shxzukj.cn

JS:   function add(a, b) { return a + b; }
来源：http://vd.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dx.szsharing.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://nx.newstarts.cn

Go:   func add(a, b int) int { return a + b }
来源：http://pn.huanxung.cn

Ruby: def add(a, b); a + b; end
来源：http://tj.lnxyls.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dv.huixiangedu.cn

[C02] 默认参数
来源：http://jk.asd995.cn

Py:   def greet(name="World"): return name
来源：http://gk.bookmarksfly.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qt.szsharing.cn

JS:   function greet(name = "World") { return name; }
来源：http://xe.huixinmuqiang.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hy.haigaiapp.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cn.szsharing.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xv.hnjuh.cn

Ruby: def greet(name = "World") = name
来源：http://fr.lnxyls.cn

C#:   string Greet(string name = "World") => name;
来源：http://rp.colortex.cn

[C03] 可变参数
来源：http://gn.szxytkj.cn

Py:   def total(*args): return sum(args)
来源：http://lh.nicolike.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ml.panjiajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ql.jianghongdianzi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ws.hnjuh.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vh.colortex.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gi.nszjky.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ib.huixiangedu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qs.szxytkj.cn

[C04] 命名参数 / 关键字参数
来源：http://tz.yuntaijiaju.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ne.shxzskj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ig.asd995.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bi.nicolike.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vq.gzmigu.cn

Java: // 无：用 Builder 模式或 record
来源：http://cc.521024.cn

Go:   // 无：用配置结构体参数
来源：http://xx.panjiajie.cn

Ruby: f(a: 1, b: 2)
来源：http://xo.newstarts.cn

C#:   f(a: 1, b: 2)
来源：http://eu.huixinmuqiang.cn

[C05] 返回多个值
来源：http://xm.yuexingan06.cn

Py:   return a, b
来源：http://ze.nszjky.cn

PHP:  return [$a, $b];
来源：http://fr.bookmarksfly.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://id.nicolike.cn

TS:   return { a, b };
来源：http://di.gzmigu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ub.521024.cn

Go:   return a, b
来源：http://bb.asd995.cn

Ruby: return a, b
来源：http://eg.lnxyls.cn

C#:   return (a, b);              // ValueTuple
来源：http://ma.newstarts.cn

[C06] 匿名函数 / lambda
来源：http://un.9csxet.cn

Py:   square = lambda x: x * x
来源：http://do.newstarts.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bk.gzmigu.cn

JS:   const square = x => x * x;
来源：http://sd.muxihuayi.cn

TS:   const square = (x: number): number => x * x;
来源：http://zs.yuntaijiaju.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xd.jianghongdianzi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qe.haigaiapp.cn

Ruby: square = ->(x) { x * x }
来源：http://fj.huanxung.cn


<!-- 参考信息 -->