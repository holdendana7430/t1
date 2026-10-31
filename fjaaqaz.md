代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qr.huanxung.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://yn.shxzskj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oz.newstarts.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://kd.bookmarksfly.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://so.lnxyls.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vt.szsharing.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://as.shxzskj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ov.yuexingan06.cn

[A18] 字符与 ASCII 码互转
来源：http://ps.shxzskj.cn

Py:   ord("A"); chr(65)
来源：http://cw.hnjuh.cn

PHP:  ord("A"); chr(65)
来源：http://fo.shtwfgs.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zd.nszjky.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yo.hnjuh.cn

Java: (int) 'A'; (char) 65
来源：http://bu.huixiangedu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://yx.521024.cn

Ruby: "A".ord; 65.chr
来源：http://jr.nicolike.cn

C#:   (int)'A'; (char)65
来源：http://bc.shtwfgs.cn

[A19] 交换两个变量
来源：http://if.haigaiapp.cn

Py:   a, b = b, a
来源：http://uc.haigaiapp.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ap.muxihuayi.cn

JS:   [a, b] = [b, a];
来源：http://mk.asd995.cn

TS:   [a, b] = [b, a];
来源：http://ks.bookmarksfly.cn

Java: int t = a; a = b; b = t;
来源：http://nb.jctech888.com.cn

Go:   a, b = b, a
来源：http://kj.huixinmuqiang.cn

Ruby: a, b = b, a
来源：http://jz.huixinmuqiang.cn

C#:   (a, b) = (b, a);
来源：http://mi.panjiajie.cn

[A20] 读取标准输入
来源：http://ui.jianghongdianzi.cn

Py:   name = input("请输入：")
来源：http://js.gzmigu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://xl.hnjuh.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ql.nszjky.cn

TS:   // Node.js：readline 模块
来源：http://pu.shtwfgs.cn

Java: new Scanner(System.in).nextLine()
来源：http://cv.shtwfgs.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xm.szsharing.cn

Ruby: gets.chomp
来源：http://nj.lnxyls.cn

C#:   Console.ReadLine();
来源：http://rq.huixinmuqiang.cn

[A21] 保留指定小数位输出
来源：http://kt.hnjuh.cn

Py:   f"{3.14159:.2f}"
来源：http://fc.bjjhwx.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cj.jianghongdianzi.cn

JS:   (3.14159).toFixed(2)
来源：http://ps.nszjky.cn

TS:   (3.14159).toFixed(2)
来源：http://iv.szxytkj.cn

Java: String.format("%.2f", 3.14159)
来源：http://pr.bjjhwx.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://iu.bjjhwx.cn

Ruby: format("%.2f", 3.14159)
来源：http://px.jctech888.com.cn

C#:   3.14159.ToString("F2")
来源：http://rq.lnxyls.cn

[A22] 获取字符串长度
来源：http://kn.wgjwhj.cn

Py:   len(s)
来源：http://rk.shxzskj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bq.bjjhwx.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ee.bjjhwx.cn

TS:   s.length
来源：http://wk.huixiangedu.cn

Java: s.length()
来源：http://lk.huixinmuqiang.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ch.bookmarksfly.cn

Ruby: s.length
来源：http://gd.hnjuh.cn

C#:   s.Length
来源：http://cz.shxzskj.cn

[A23] 大小写转换
来源：http://bn.nszjky.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ny.nicolike.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zw.bjjhwx.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bs.hnjuh.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ak.hnjuh.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pi.nicolike.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bc.huixiangedu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ry.yuexingan06.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://nj.gzmigu.cn

[A24] 去除首尾空白
来源：http://dm.asd995.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://kp.bjjhwx.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fs.yuntaijiaju.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gz.yuntaijiaju.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ah.haigaiapp.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jl.nicolike.cn

Go:   strings.TrimSpace(s)
来源：http://mp.yuntaijiaju.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fm.yuexingan06.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://en.muxihuayi.cn

[A25] 字符串比较
来源：http://oj.nszjky.cn

Py:   s1 == s2; s1 != s2
来源：http://im.chemitech.net.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gh.jianghongdianzi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jk.szsharing.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mc.muxihuayi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fg.521024.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ej.shxzukj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://qj.shtwfgs.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sx.521024.cn

[A26] 类型转换总览
来源：http://pz.yuntaijiaju.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://at.szsharing.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qh.jctech888.com.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ar.wgjwhj.cn

TS:   Number() String() Boolean() x as number
来源：http://wu.jctech888.com.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ty.9csxet.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://su.panjiajie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mw.521024.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jl.shxzskj.cn

================================================================================
来源：http://fg.panjiajie.cn

B. 流程控制
来源：http://ry.szxytkj.cn

================================================================================
来源：http://ri.szxytkj.cn

[B01] 条件判断 if / else
来源：http://gz.bjjhwx.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bb.szxytkj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yy.colortex.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vi.shtwfgs.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mp.nicolike.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ce.chemitech.net.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jq.jianghongdianzi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jj.shtwfgs.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ca.bookmarksfly.cn

[B02] 多分支 else if / elif
来源：http://uc.huixiangedu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tx.bjjhwx.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hm.shxzskj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://of.hahajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://va.wgjwhj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://np.9csxet.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://af.hnjuh.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://sh.yuntaijiaju.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ww.szsharing.cn

[B03] switch / match / case
来源：http://fu.bjjhwx.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mi.jianghongdianzi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wu.521024.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wg.lnxyls.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://iz.huixinmuqiang.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://yd.bookmarksfly.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wg.wgjwhj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ho.chemitech.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bi.muxihuayi.cn

[B04] for 计数循环
来源：http://tg.yuntaijiaju.cn

Py:   for i in range(10): print(i)
来源：http://jr.hahajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://po.jctech888.com.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fv.shxzskj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://md.huixinmuqiang.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rc.gzmigu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ew.muxihuayi.cn

Ruby: 10.times { |i| puts i }
来源：http://rr.lnxyls.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ss.bjjhwx.cn

[B05] 遍历数组 / 列表
来源：http://wp.szxytkj.cn

Py:   for item in arr: print(item)
来源：http://uy.szxytkj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://eh.muxihuayi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ag.shxzskj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://pn.jctech888.com.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sr.huixiangedu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kq.jctech888.com.cn

Ruby: arr.each { |item| puts item }
来源：http://bw.szsharing.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ny.yuntaijiaju.cn

[B06] 遍历字典 / 对象
来源：http://ke.shxzukj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ok.chemitech.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bd.521024.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tc.panjiajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kj.yuntaijiaju.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yi.muxihuayi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://as.panjiajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ly.yuexingan06.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://oc.9csxet.cn

[B07] while 循环
来源：http://im.colortex.cn

Py:   while i < 10: i += 1
来源：http://fq.jianghongdianzi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://uo.gzmigu.cn

JS:   while (i < 10) { i++; }
来源：http://jj.colortex.cn

TS:   while (i < 10) { i++; }
来源：http://dy.shxzukj.cn

Java: while (i < 10) { i++; }
来源：http://wl.521024.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tr.yuntaijiaju.cn

Ruby: while i < 10; i += 1; end
来源：http://ah.nicolike.cn

C#:   while (i < 10) { i++; }
来源：http://kd.colortex.cn

[B08] do-while（至少执行一次）
来源：http://ad.colortex.cn

Py:   # 无 do-while：用 while True + break
来源：http://zj.jctech888.com.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pg.huanxung.cn

JS:   do { i++; } while (i < 10);
来源：http://me.colortex.cn

TS:   do { i++; } while (i < 10);
来源：http://hj.nszjky.cn

Java: do { i++; } while (i < 10);
来源：http://xu.yuexingan06.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mx.szsharing.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wc.shxzskj.cn

C#:   do { i++; } while (i < 10);
来源：http://do.shtwfgs.cn

[B09] break 与 continue
来源：http://pc.shxzukj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ds.hahajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qg.huixinmuqiang.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uu.shtwfgs.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rh.yuntaijiaju.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pi.haigaiapp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jm.yuexingan06.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mz.shxzskj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sg.bookmarksfly.cn

[B10] 遍历同时拿索引
来源：http://bj.wgjwhj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fs.huanxung.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zr.yuexingan06.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qy.jianghongdianzi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lx.bjjhwx.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fi.asd995.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vu.bookmarksfly.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xq.muxihuayi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cr.haigaiapp.cn

[B11] 生成数字序列 / 区间
来源：http://lc.bookmarksfly.cn

Py:   list(range(0, 10, 2))
来源：http://dw.shxzskj.cn

PHP:  range(0, 10, 2);
来源：http://hw.nszjky.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tn.lnxyls.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gb.shxzskj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nr.nszjky.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://uh.huixiangedu.cn

Ruby: (0...10).step(2).to_a
来源：http://fm.chemitech.net.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bh.huixinmuqiang.cn

[B12] 跳出多层循环
来源：http://wg.jctech888.com.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ug.jianghongdianzi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://rz.chemitech.net.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bj.panjiajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://el.asd995.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jb.yuntaijiaju.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fh.shxzukj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://za.colortex.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zn.huixinmuqiang.cn

[B13] 判断是否为数字
来源：http://th.shxzukj.cn

Py:   isinstance(x, (int, float))
来源：http://wv.wgjwhj.cn

PHP:  is_numeric($x)
来源：http://fy.yuexingan06.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ry.yuntaijiaju.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xp.shxzukj.cn

Java: x instanceof Number
来源：http://hs.newstarts.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rc.shtwfgs.cn

Ruby: x.is_a?(Numeric)
来源：http://am.wgjwhj.cn

C#:   x is int or double or decimal
来源：http://me.colortex.cn

[B14] 判断值是否在集合内
来源：http://tp.521024.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fg.jctech888.com.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ot.chemitech.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://dh.szxytkj.cn

TS:   [1, 2, 3].includes(x)
来源：http://zs.yuexingan06.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://br.9csxet.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sk.bookmarksfly.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xz.9csxet.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mx.shxzukj.cn

[B15] 布尔运算与取反
来源：http://sk.shtwfgs.cn

Py:   a and b or not c
来源：http://wa.yuntaijiaju.cn

PHP:  $a && $b || !$c
来源：http://ee.colortex.cn

JS:   a && b || !c
来源：http://lu.chemitech.net.cn

TS:   a && b || !c
来源：http://po.wgjwhj.cn

Java: a && b || !c
来源：http://ua.newstarts.cn

Go:   a && b || !c
来源：http://dv.nszjky.cn

Ruby: a && b || !c
来源：http://vw.yuexingan06.cn

C#:   a && b || !c
来源：http://lx.huixiangedu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lu.bjjhwx.cn

Py:   if not data: return
来源：http://mo.huixinmuqiang.cn

PHP:  if (!$data) { return; }
来源：http://sw.haigaiapp.cn

JS:   if (!data) return;
来源：http://ft.szxytkj.cn

TS:   if (!data) return;
来源：http://ct.huixinmuqiang.cn

Java: if (data == null) return;
来源：http://ld.chemitech.net.cn

Go:   if data == nil { return }
来源：http://dl.9csxet.cn

Ruby: return if data.nil?
来源：http://ur.bjjhwx.cn

C#:   if (data == null) return;
来源：http://sh.shxzskj.cn

================================================================================
来源：http://bo.szsharing.cn

C. 函数与作用域
来源：http://qe.szsharing.cn

================================================================================
来源：http://qf.jianghongdianzi.cn

[C01] 定义函数
来源：http://vl.panjiajie.cn

Py:   def add(a, b): return a + b
来源：http://gj.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ia.newstarts.cn

JS:   function add(a, b) { return a + b; }
来源：http://es.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qq.bookmarksfly.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ib.huixinmuqiang.cn

Go:   func add(a, b int) int { return a + b }
来源：http://bw.haigaiapp.cn

Ruby: def add(a, b); a + b; end
来源：http://xw.yuntaijiaju.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://py.hnjuh.cn

[C02] 默认参数
来源：http://dj.nszjky.cn

Py:   def greet(name="World"): return name
来源：http://cr.szsharing.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xx.nszjky.cn

JS:   function greet(name = "World") { return name; }
来源：http://ta.bookmarksfly.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wz.huixiangedu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ag.wgjwhj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ts.chemitech.net.cn

Ruby: def greet(name = "World") = name
来源：http://dk.huanxung.cn

C#:   string Greet(string name = "World") => name;
来源：http://fp.newstarts.cn

[C03] 可变参数
来源：http://ct.haigaiapp.cn

Py:   def total(*args): return sum(args)
来源：http://wh.jctech888.com.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ny.bjjhwx.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nh.jctech888.com.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xb.szxytkj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ab.lnxyls.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xo.nszjky.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yq.muxihuayi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rr.hnjuh.cn

[C04] 命名参数 / 关键字参数
来源：http://zy.yuexingan06.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://oq.panjiajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xt.521024.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jm.szxytkj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yn.chemitech.net.cn

Java: // 无：用 Builder 模式或 record
来源：http://ai.newstarts.cn

Go:   // 无：用配置结构体参数
来源：http://nd.lnxyls.cn

Ruby: f(a: 1, b: 2)
来源：http://zj.panjiajie.cn

C#:   f(a: 1, b: 2)
来源：http://fs.yuntaijiaju.cn

[C05] 返回多个值
来源：http://ir.jianghongdianzi.cn

Py:   return a, b
来源：http://fy.nszjky.cn

PHP:  return [$a, $b];
来源：http://ml.bookmarksfly.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://za.yuexingan06.cn

TS:   return { a, b };
来源：http://av.nszjky.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mu.szxytkj.cn

Go:   return a, b
来源：http://wn.9csxet.cn

Ruby: return a, b
来源：http://jb.colortex.cn

C#:   return (a, b);              // ValueTuple
来源：http://pl.shxzskj.cn

[C06] 匿名函数 / lambda
来源：http://qr.panjiajie.cn

Py:   square = lambda x: x * x
来源：http://pk.9csxet.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://vh.yuntaijiaju.cn

JS:   const square = x => x * x;
来源：http://rz.jianghongdianzi.cn

TS:   const square = (x: number): number => x * x;
来源：http://gy.chemitech.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mq.yuntaijiaju.cn

Go:   sq := func(x int) int { return x * x }
来源：http://yg.szsharing.cn

Ruby: square = ->(x) { x * x }
来源：http://hf.yuexingan06.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zf.chemitech.net.cn

[C07] 把函数作为参数传入
来源：http://le.szxytkj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rw.jianghongdianzi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ic.nicolike.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zr.muxihuayi.cn

TS:   arr.map(String)
来源：http://zx.bookmarksfly.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ww.szxytkj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wg.huanxung.cn


<!-- 参考信息 -->