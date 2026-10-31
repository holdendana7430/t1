代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mg.bjjhwx.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wh.jctech888.com.cn

TS:   if (!x) {}
来源：http://ra.colortex.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gu.colortex.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://jt.shxzskj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://sz.shxzukj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fh.hahajie.cn

[A17] 位运算
来源：http://pb.muxihuayi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tx.bookmarksfly.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zd.lnxyls.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ry.bjjhwx.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://py.muxihuayi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gk.gzmigu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://av.nicolike.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ql.hnjuh.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jc.9csxet.cn

[A18] 字符与 ASCII 码互转
来源：http://io.colortex.cn

Py:   ord("A"); chr(65)
来源：http://un.szxytkj.cn

PHP:  ord("A"); chr(65)
来源：http://qm.shxzukj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yq.yuntaijiaju.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oc.hahajie.cn

Java: (int) 'A'; (char) 65
来源：http://eg.muxihuayi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ks.gzmigu.cn

Ruby: "A".ord; 65.chr
来源：http://xo.hnjuh.cn

C#:   (int)'A'; (char)65
来源：http://sl.muxihuayi.cn

[A19] 交换两个变量
来源：http://fq.asd995.cn

Py:   a, b = b, a
来源：http://ag.shxzskj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://zt.shxzukj.cn

JS:   [a, b] = [b, a];
来源：http://vt.huixiangedu.cn

TS:   [a, b] = [b, a];
来源：http://bl.gzmigu.cn

Java: int t = a; a = b; b = t;
来源：http://sn.hahajie.cn

Go:   a, b = b, a
来源：http://qw.wgjwhj.cn

Ruby: a, b = b, a
来源：http://ai.jianghongdianzi.cn

C#:   (a, b) = (b, a);
来源：http://tg.newstarts.cn

[A20] 读取标准输入
来源：http://wp.huixiangedu.cn

Py:   name = input("请输入：")
来源：http://xc.nszjky.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://xj.szsharing.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bo.haigaiapp.cn

TS:   // Node.js：readline 模块
来源：http://we.nicolike.cn

Java: new Scanner(System.in).nextLine()
来源：http://vx.shxzskj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ra.muxihuayi.cn

Ruby: gets.chomp
来源：http://hv.jianghongdianzi.cn

C#:   Console.ReadLine();
来源：http://uc.nszjky.cn

[A21] 保留指定小数位输出
来源：http://lg.9csxet.cn

Py:   f"{3.14159:.2f}"
来源：http://bu.jctech888.com.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rn.colortex.cn

JS:   (3.14159).toFixed(2)
来源：http://ae.lnxyls.cn

TS:   (3.14159).toFixed(2)
来源：http://ip.yuexingan06.cn

Java: String.format("%.2f", 3.14159)
来源：http://ap.hnjuh.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zc.lnxyls.cn

Ruby: format("%.2f", 3.14159)
来源：http://xu.haigaiapp.cn

C#:   3.14159.ToString("F2")
来源：http://kr.shxzukj.cn

[A22] 获取字符串长度
来源：http://up.newstarts.cn

Py:   len(s)
来源：http://gh.gzmigu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pc.nszjky.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qs.bookmarksfly.cn

TS:   s.length
来源：http://fc.huixiangedu.cn

Java: s.length()
来源：http://gj.shxzskj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qi.yuexingan06.cn

Ruby: s.length
来源：http://yc.szxytkj.cn

C#:   s.Length
来源：http://nn.521024.cn

[A23] 大小写转换
来源：http://hd.bookmarksfly.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://if.lnxyls.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zw.colortex.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ap.gzmigu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ui.hnjuh.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ja.wgjwhj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mi.wgjwhj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gl.huanxung.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://gu.gzmigu.cn

[A24] 去除首尾空白
来源：http://kc.shxzskj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mp.jianghongdianzi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://yu.huanxung.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tb.jianghongdianzi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bf.colortex.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qh.bjjhwx.cn

Go:   strings.TrimSpace(s)
来源：http://hw.yuntaijiaju.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vu.jctech888.com.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qn.lnxyls.cn

[A25] 字符串比较
来源：http://nc.jianghongdianzi.cn

Py:   s1 == s2; s1 != s2
来源：http://iw.shtwfgs.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ds.asd995.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bb.bjjhwx.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vm.hnjuh.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zo.huixiangedu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ap.hahajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rh.bjjhwx.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vb.huixinmuqiang.cn

[A26] 类型转换总览
来源：http://az.jianghongdianzi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wn.lnxyls.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jw.huanxung.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://br.bjjhwx.cn

TS:   Number() String() Boolean() x as number
来源：http://ja.bjjhwx.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lk.haigaiapp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vw.szxytkj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://tk.jianghongdianzi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rr.huixinmuqiang.cn

================================================================================
来源：http://ps.szsharing.cn

B. 流程控制
来源：http://hu.huixiangedu.cn

================================================================================
来源：http://td.huixinmuqiang.cn

[B01] 条件判断 if / else
来源：http://rj.shxzukj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://rz.chemitech.net.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xe.newstarts.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mj.hahajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bb.shxzskj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://eb.shxzskj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ex.hnjuh.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://al.hahajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sb.huanxung.cn

[B02] 多分支 else if / elif
来源：http://by.szsharing.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nm.gzmigu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zy.haigaiapp.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://la.lnxyls.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xd.newstarts.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mi.szsharing.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ta.wgjwhj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bu.szxytkj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nj.huanxung.cn

[B03] switch / match / case
来源：http://vm.colortex.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ra.521024.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://un.huixinmuqiang.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gj.asd995.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vz.nszjky.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://py.huanxung.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gq.lnxyls.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hu.shxzskj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yz.nszjky.cn

[B04] for 计数循环
来源：http://zv.haigaiapp.cn

Py:   for i in range(10): print(i)
来源：http://uc.jianghongdianzi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wa.huanxung.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tp.shxzukj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://us.panjiajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ex.panjiajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://sx.shxzskj.cn

Ruby: 10.times { |i| puts i }
来源：http://le.gzmigu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://we.haigaiapp.cn

[B05] 遍历数组 / 列表
来源：http://hg.chemitech.net.cn

Py:   for item in arr: print(item)
来源：http://ja.hnjuh.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://uo.huanxung.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://sp.newstarts.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tu.nicolike.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yr.muxihuayi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ny.nszjky.cn

Ruby: arr.each { |item| puts item }
来源：http://nj.yuntaijiaju.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ts.huixiangedu.cn

[B06] 遍历字典 / 对象
来源：http://hf.bookmarksfly.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zg.hahajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pg.lnxyls.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pd.jctech888.com.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mu.asd995.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ke.521024.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://la.haigaiapp.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://iy.huanxung.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qb.hnjuh.cn

[B07] while 循环
来源：http://ml.yuntaijiaju.cn

Py:   while i < 10: i += 1
来源：http://mm.colortex.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bw.hahajie.cn

JS:   while (i < 10) { i++; }
来源：http://sd.szsharing.cn

TS:   while (i < 10) { i++; }
来源：http://bh.shxzukj.cn

Java: while (i < 10) { i++; }
来源：http://vk.lnxyls.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gd.yuexingan06.cn

Ruby: while i < 10; i += 1; end
来源：http://ur.hahajie.cn

C#:   while (i < 10) { i++; }
来源：http://gi.shxzskj.cn

[B08] do-while（至少执行一次）
来源：http://sz.gzmigu.cn

Py:   # 无 do-while：用 while True + break
来源：http://st.huixinmuqiang.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://az.huixinmuqiang.cn

JS:   do { i++; } while (i < 10);
来源：http://sm.haigaiapp.cn

TS:   do { i++; } while (i < 10);
来源：http://yo.gzmigu.cn

Java: do { i++; } while (i < 10);
来源：http://nl.9csxet.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://nn.huixiangedu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://yv.shxzskj.cn

C#:   do { i++; } while (i < 10);
来源：http://ua.lnxyls.cn

[B09] break 与 continue
来源：http://ad.haigaiapp.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ku.szsharing.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rp.muxihuayi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wv.huixiangedu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oq.nicolike.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tl.nszjky.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fy.9csxet.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bm.jctech888.com.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yu.shxzskj.cn

[B10] 遍历同时拿索引
来源：http://nn.jctech888.com.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pl.hnjuh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ct.lnxyls.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ik.9csxet.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wc.521024.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://au.bookmarksfly.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qa.nszjky.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://my.wgjwhj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lb.shxzskj.cn

[B11] 生成数字序列 / 区间
来源：http://fv.hnjuh.cn

Py:   list(range(0, 10, 2))
来源：http://wl.wgjwhj.cn

PHP:  range(0, 10, 2);
来源：http://qp.shxzukj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jb.huixiangedu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ix.newstarts.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pq.shxzskj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yj.chemitech.net.cn

Ruby: (0...10).step(2).to_a
来源：http://bq.wgjwhj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hx.521024.cn

[B12] 跳出多层循环
来源：http://et.521024.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://we.shtwfgs.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://eh.szsharing.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bd.huixiangedu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kw.hahajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://un.huixiangedu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tk.huixiangedu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xz.gzmigu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yi.nicolike.cn

[B13] 判断是否为数字
来源：http://th.newstarts.cn

Py:   isinstance(x, (int, float))
来源：http://lj.asd995.cn

PHP:  is_numeric($x)
来源：http://oz.shxzskj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://is.yuntaijiaju.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ou.wgjwhj.cn

Java: x instanceof Number
来源：http://bi.szsharing.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hq.shtwfgs.cn

Ruby: x.is_a?(Numeric)
来源：http://ex.haigaiapp.cn

C#:   x is int or double or decimal
来源：http://aw.gzmigu.cn

[B14] 判断值是否在集合内
来源：http://xj.haigaiapp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://es.gzmigu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lw.hahajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://oj.yuntaijiaju.cn

TS:   [1, 2, 3].includes(x)
来源：http://rj.jianghongdianzi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ow.szxytkj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ud.newstarts.cn

Ruby: [1, 2, 3].include?(x)
来源：http://au.panjiajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ow.newstarts.cn

[B15] 布尔运算与取反
来源：http://vn.colortex.cn

Py:   a and b or not c
来源：http://yd.nicolike.cn

PHP:  $a && $b || !$c
来源：http://cm.9csxet.cn

JS:   a && b || !c
来源：http://qi.lnxyls.cn

TS:   a && b || !c
来源：http://yt.chemitech.net.cn

Java: a && b || !c
来源：http://vu.szxytkj.cn

Go:   a && b || !c
来源：http://yf.hahajie.cn

Ruby: a && b || !c
来源：http://op.panjiajie.cn

C#:   a && b || !c
来源：http://fa.haigaiapp.cn

[B16] 卫语句：不满足条件提前返回
来源：http://em.bjjhwx.cn

Py:   if not data: return
来源：http://tx.yuexingan06.cn

PHP:  if (!$data) { return; }
来源：http://dd.9csxet.cn

JS:   if (!data) return;
来源：http://bt.szxytkj.cn

TS:   if (!data) return;
来源：http://jf.panjiajie.cn

Java: if (data == null) return;
来源：http://mv.szxytkj.cn

Go:   if data == nil { return }
来源：http://uz.lnxyls.cn

Ruby: return if data.nil?
来源：http://mc.newstarts.cn

C#:   if (data == null) return;
来源：http://ap.hnjuh.cn

================================================================================
来源：http://ia.hnjuh.cn

C. 函数与作用域
来源：http://pv.haigaiapp.cn

================================================================================
来源：http://ae.huixiangedu.cn

[C01] 定义函数
来源：http://oa.huixiangedu.cn

Py:   def add(a, b): return a + b
来源：http://qx.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://le.szxytkj.cn

JS:   function add(a, b) { return a + b; }
来源：http://cq.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hk.jianghongdianzi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://tr.shtwfgs.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zo.lnxyls.cn

Ruby: def add(a, b); a + b; end
来源：http://ff.521024.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://be.shxzukj.cn

[C02] 默认参数
来源：http://su.gzmigu.cn

Py:   def greet(name="World"): return name
来源：http://xn.szsharing.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://jp.bookmarksfly.cn

JS:   function greet(name = "World") { return name; }
来源：http://yf.szxytkj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://si.shtwfgs.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ym.hnjuh.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gd.521024.cn

Ruby: def greet(name = "World") = name
来源：http://vx.asd995.cn

C#:   string Greet(string name = "World") => name;
来源：http://sn.huanxung.cn

[C03] 可变参数
来源：http://je.yuexingan06.cn

Py:   def total(*args): return sum(args)
来源：http://sy.shxzukj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ry.bookmarksfly.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mw.nszjky.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vi.jctech888.com.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gn.hahajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ci.shtwfgs.cn

Ruby: def total(*nums); nums.sum; end
来源：http://lj.asd995.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jm.jianghongdianzi.cn

[C04] 命名参数 / 关键字参数
来源：http://id.newstarts.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wt.9csxet.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ey.haigaiapp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://si.colortex.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://iq.shtwfgs.cn

Java: // 无：用 Builder 模式或 record
来源：http://ls.9csxet.cn

Go:   // 无：用配置结构体参数
来源：http://wn.9csxet.cn

Ruby: f(a: 1, b: 2)
来源：http://xv.haigaiapp.cn

C#:   f(a: 1, b: 2)
来源：http://pn.asd995.cn

[C05] 返回多个值
来源：http://ge.shxzskj.cn

Py:   return a, b
来源：http://ud.lnxyls.cn

PHP:  return [$a, $b];
来源：http://cy.nszjky.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vd.chemitech.net.cn

TS:   return { a, b };
来源：http://sw.huanxung.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nc.521024.cn

Go:   return a, b
来源：http://lh.bookmarksfly.cn

Ruby: return a, b
来源：http://jd.hnjuh.cn

C#:   return (a, b);              // ValueTuple
来源：http://os.muxihuayi.cn

[C06] 匿名函数 / lambda
来源：http://do.521024.cn

Py:   square = lambda x: x * x
来源：http://mc.chemitech.net.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://hv.shxzskj.cn

JS:   const square = x => x * x;
来源：http://cq.jianghongdianzi.cn

TS:   const square = (x: number): number => x * x;
来源：http://zq.nicolike.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xf.huixinmuqiang.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wa.muxihuayi.cn

Ruby: square = ->(x) { x * x }
来源：http://lc.szsharing.cn


<!-- 参考信息 -->