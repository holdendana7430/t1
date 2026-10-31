代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://co.jianghongdianzi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gd.yuexingan06.cn

Ruby: format("%.2f", 3.14159)
来源：http://wb.9csxet.cn

C#:   3.14159.ToString("F2")
来源：http://mn.huanxung.cn

[A22] 获取字符串长度
来源：http://lt.newstarts.cn

Py:   len(s)
来源：http://fe.nicolike.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wv.521024.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mx.yuntaijiaju.cn

TS:   s.length
来源：http://ky.521024.cn

Java: s.length()
来源：http://fh.jianghongdianzi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jb.huixiangedu.cn

Ruby: s.length
来源：http://vk.huanxung.cn

C#:   s.Length
来源：http://xc.jianghongdianzi.cn

[A23] 大小写转换
来源：http://rn.521024.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://hh.chemitech.net.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://aj.huanxung.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://sv.chemitech.net.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fn.hnjuh.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://oj.chemitech.net.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yf.nicolike.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mj.shxzukj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://iw.szsharing.cn

[A24] 去除首尾空白
来源：http://tg.wgjwhj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mb.lnxyls.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tx.huixinmuqiang.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hk.shxzskj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nx.chemitech.net.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ub.gzmigu.cn

Go:   strings.TrimSpace(s)
来源：http://ve.yuexingan06.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mp.521024.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dt.521024.cn

[A25] 字符串比较
来源：http://tz.huixiangedu.cn

Py:   s1 == s2; s1 != s2
来源：http://dd.hnjuh.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ga.shxzukj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://eg.huanxung.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pl.hnjuh.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yq.szxytkj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://if.yuntaijiaju.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://yj.lnxyls.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sd.shtwfgs.cn

[A26] 类型转换总览
来源：http://tb.chemitech.net.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vk.hnjuh.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hh.huixiangedu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ts.hnjuh.cn

TS:   Number() String() Boolean() x as number
来源：http://uq.nszjky.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rz.nicolike.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xo.panjiajie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://yt.lnxyls.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gp.muxihuayi.cn

================================================================================
来源：http://ho.yuexingan06.cn

B. 流程控制
来源：http://fa.szsharing.cn

================================================================================
来源：http://wt.muxihuayi.cn

[B01] 条件判断 if / else
来源：http://sv.szsharing.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://zr.huanxung.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ec.haigaiapp.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ro.jianghongdianzi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ug.wgjwhj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://lr.521024.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qn.chemitech.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ar.colortex.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wg.521024.cn

[B02] 多分支 else if / elif
来源：http://kx.huixiangedu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fs.nicolike.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vq.shxzskj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eb.szxytkj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://el.bjjhwx.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rb.chemitech.net.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kp.huanxung.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nl.huixiangedu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wy.newstarts.cn

[B03] switch / match / case
来源：http://qc.hnjuh.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hh.shxzukj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fl.szsharing.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://at.chemitech.net.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://iu.huixiangedu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fb.jctech888.com.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ri.yuntaijiaju.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ty.9csxet.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://iq.hnjuh.cn

[B04] for 计数循环
来源：http://ij.shxzskj.cn

Py:   for i in range(10): print(i)
来源：http://yn.yuexingan06.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vb.asd995.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wd.hnjuh.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://av.shxzukj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nn.yuexingan06.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bj.bookmarksfly.cn

Ruby: 10.times { |i| puts i }
来源：http://vn.colortex.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ze.shxzskj.cn

[B05] 遍历数组 / 列表
来源：http://yg.hnjuh.cn

Py:   for item in arr: print(item)
来源：http://qn.panjiajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lc.szsharing.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://iq.shxzukj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yi.yuexingan06.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://iz.gzmigu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nt.jianghongdianzi.cn

Ruby: arr.each { |item| puts item }
来源：http://dm.nszjky.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://oc.hnjuh.cn

[B06] 遍历字典 / 对象
来源：http://kf.shxzukj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tv.haigaiapp.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ks.szsharing.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rs.9csxet.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zd.bjjhwx.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gh.bookmarksfly.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gy.bookmarksfly.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rj.haigaiapp.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hx.panjiajie.cn

[B07] while 循环
来源：http://pb.asd995.cn

Py:   while i < 10: i += 1
来源：http://jk.newstarts.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ad.521024.cn

JS:   while (i < 10) { i++; }
来源：http://yv.huixinmuqiang.cn

TS:   while (i < 10) { i++; }
来源：http://lo.bjjhwx.cn

Java: while (i < 10) { i++; }
来源：http://ep.nszjky.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://es.shxzskj.cn

Ruby: while i < 10; i += 1; end
来源：http://do.shxzskj.cn

C#:   while (i < 10) { i++; }
来源：http://ui.shtwfgs.cn

[B08] do-while（至少执行一次）
来源：http://id.colortex.cn

Py:   # 无 do-while：用 while True + break
来源：http://iy.jianghongdianzi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qm.panjiajie.cn

JS:   do { i++; } while (i < 10);
来源：http://mx.colortex.cn

TS:   do { i++; } while (i < 10);
来源：http://wk.asd995.cn

Java: do { i++; } while (i < 10);
来源：http://si.panjiajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ie.shxzukj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://of.huixinmuqiang.cn

C#:   do { i++; } while (i < 10);
来源：http://fa.panjiajie.cn

[B09] break 与 continue
来源：http://gm.huixinmuqiang.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nd.lnxyls.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nf.szsharing.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://li.chemitech.net.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vb.shtwfgs.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nz.huixiangedu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ut.chemitech.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jc.colortex.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://og.huixiangedu.cn

[B10] 遍历同时拿索引
来源：http://uq.hnjuh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zy.huanxung.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rj.szsharing.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pa.shxzukj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kk.bookmarksfly.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kx.haigaiapp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qz.muxihuayi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vg.huixiangedu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gc.shxzukj.cn

[B11] 生成数字序列 / 区间
来源：http://hv.yuntaijiaju.cn

Py:   list(range(0, 10, 2))
来源：http://fv.asd995.cn

PHP:  range(0, 10, 2);
来源：http://lm.jianghongdianzi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nt.bookmarksfly.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bz.newstarts.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rt.huanxung.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dk.hahajie.cn

Ruby: (0...10).step(2).to_a
来源：http://uc.szsharing.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pq.hahajie.cn

[B12] 跳出多层循环
来源：http://bk.jctech888.com.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pk.huixiangedu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vf.huixiangedu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://us.colortex.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cw.nszjky.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zj.haigaiapp.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sw.hahajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://er.huixinmuqiang.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vd.szxytkj.cn

[B13] 判断是否为数字
来源：http://lr.lnxyls.cn

Py:   isinstance(x, (int, float))
来源：http://wu.colortex.cn

PHP:  is_numeric($x)
来源：http://jg.huixiangedu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dv.shtwfgs.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yn.szxytkj.cn

Java: x instanceof Number
来源：http://ut.bookmarksfly.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vg.bookmarksfly.cn

Ruby: x.is_a?(Numeric)
来源：http://dh.nszjky.cn

C#:   x is int or double or decimal
来源：http://cp.bookmarksfly.cn

[B14] 判断值是否在集合内
来源：http://zs.521024.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ba.shxzskj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ve.chemitech.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://en.nszjky.cn

TS:   [1, 2, 3].includes(x)
来源：http://xe.jianghongdianzi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://uk.jctech888.com.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ub.hahajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://dn.jianghongdianzi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tb.colortex.cn

[B15] 布尔运算与取反
来源：http://gq.hnjuh.cn

Py:   a and b or not c
来源：http://wr.muxihuayi.cn

PHP:  $a && $b || !$c
来源：http://kc.chemitech.net.cn

JS:   a && b || !c
来源：http://rt.9csxet.cn

TS:   a && b || !c
来源：http://gq.newstarts.cn

Java: a && b || !c
来源：http://rr.9csxet.cn

Go:   a && b || !c
来源：http://it.gzmigu.cn

Ruby: a && b || !c
来源：http://oj.newstarts.cn

C#:   a && b || !c
来源：http://db.nicolike.cn

[B16] 卫语句：不满足条件提前返回
来源：http://de.newstarts.cn

Py:   if not data: return
来源：http://dq.szxytkj.cn

PHP:  if (!$data) { return; }
来源：http://wx.yuntaijiaju.cn

JS:   if (!data) return;
来源：http://ta.yuntaijiaju.cn

TS:   if (!data) return;
来源：http://hb.szsharing.cn

Java: if (data == null) return;
来源：http://qi.9csxet.cn

Go:   if data == nil { return }
来源：http://oh.yuexingan06.cn

Ruby: return if data.nil?
来源：http://vq.huixiangedu.cn

C#:   if (data == null) return;
来源：http://qs.shxzukj.cn

================================================================================
来源：http://vi.yuntaijiaju.cn

C. 函数与作用域
来源：http://in.shtwfgs.cn

================================================================================
来源：http://qx.bjjhwx.cn

[C01] 定义函数
来源：http://tx.hahajie.cn

Py:   def add(a, b): return a + b
来源：http://bu.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sz.shxzskj.cn

JS:   function add(a, b) { return a + b; }
来源：http://dk.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pj.bookmarksfly.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gv.hnjuh.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qg.bookmarksfly.cn

Ruby: def add(a, b); a + b; end
来源：http://il.bjjhwx.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pk.asd995.cn

[C02] 默认参数
来源：http://cr.shxzskj.cn

Py:   def greet(name="World"): return name
来源：http://zc.hahajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://il.newstarts.cn

JS:   function greet(name = "World") { return name; }
来源：http://xo.hahajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://iq.yuexingan06.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://yw.szsharing.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lm.hnjuh.cn

Ruby: def greet(name = "World") = name
来源：http://kv.bjjhwx.cn

C#:   string Greet(string name = "World") => name;
来源：http://cl.newstarts.cn

[C03] 可变参数
来源：http://ie.haigaiapp.cn

Py:   def total(*args): return sum(args)
来源：http://gl.muxihuayi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pl.lnxyls.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ot.hnjuh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hr.huixiangedu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rx.huanxung.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yd.huanxung.cn

Ruby: def total(*nums); nums.sum; end
来源：http://dn.muxihuayi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ag.hnjuh.cn

[C04] 命名参数 / 关键字参数
来源：http://fk.yuexingan06.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mn.hahajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hy.521024.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://iu.szxytkj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ol.yuexingan06.cn

Java: // 无：用 Builder 模式或 record
来源：http://az.huixiangedu.cn

Go:   // 无：用配置结构体参数
来源：http://ud.haigaiapp.cn

Ruby: f(a: 1, b: 2)
来源：http://mn.hnjuh.cn

C#:   f(a: 1, b: 2)
来源：http://wh.newstarts.cn

[C05] 返回多个值
来源：http://ke.nicolike.cn

Py:   return a, b
来源：http://ob.nszjky.cn

PHP:  return [$a, $b];
来源：http://yn.newstarts.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://si.bjjhwx.cn

TS:   return { a, b };
来源：http://hw.521024.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mc.jctech888.com.cn

Go:   return a, b
来源：http://bu.wgjwhj.cn

Ruby: return a, b
来源：http://dt.szxytkj.cn

C#:   return (a, b);              // ValueTuple
来源：http://vc.wgjwhj.cn

[C06] 匿名函数 / lambda
来源：http://fy.bjjhwx.cn

Py:   square = lambda x: x * x
来源：http://vy.asd995.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://iz.jctech888.com.cn

JS:   const square = x => x * x;
来源：http://ba.newstarts.cn

TS:   const square = (x: number): number => x * x;
来源：http://pc.shtwfgs.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://eu.hnjuh.cn

Go:   sq := func(x int) int { return x * x }
来源：http://iq.szxytkj.cn

Ruby: square = ->(x) { x * x }
来源：http://gm.9csxet.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ft.haigaiapp.cn

[C07] 把函数作为参数传入
来源：http://jo.szsharing.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ri.szsharing.cn

PHP:  array_map("strtoupper", $arr);
来源：http://og.shtwfgs.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://is.9csxet.cn

TS:   arr.map(String)
来源：http://pq.huixinmuqiang.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sa.hnjuh.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ih.chemitech.net.cn

Ruby: arr.map(&:upcase)
来源：http://qn.9csxet.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://lj.nszjky.cn

[C08] 闭包
来源：http://nc.jianghongdianzi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gj.muxihuayi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://eb.colortex.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zy.jianghongdianzi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lu.9csxet.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tm.yuntaijiaju.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://eg.521024.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ln.colortex.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://go.bjjhwx.cn

[C09] 递归
来源：http://ic.yuntaijiaju.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mm.hnjuh.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pq.shtwfgs.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nw.nicolike.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bw.521024.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dv.hnjuh.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ln.bjjhwx.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://un.bookmarksfly.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://eo.nszjky.cn

[C10] 变量作用域
来源：http://bt.nicolike.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ll.shtwfgs.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fh.hnjuh.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://az.bookmarksfly.cn

TS:   同 JS
来源：http://sb.colortex.cn

Java: 方法内为块级作用域
来源：http://vl.wgjwhj.cn

Go:   花括号块级作用域
来源：http://qu.nszjky.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ti.shxzskj.cn

C#:   块级作用域
来源：http://sm.wgjwhj.cn

[C11] 模块导入与导出
来源：http://ri.521024.cn

Py:   from module import func
来源：http://wz.hahajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qy.gzmigu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ka.wgjwhj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ix.jianghongdianzi.cn

Java: import java.util.List;
来源：http://wp.shtwfgs.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uh.hnjuh.cn

Ruby: require "json"; require_relative "./util"
来源：http://jl.bjjhwx.cn

C#:   using System.Text;
来源：http://uj.huixinmuqiang.cn

[C12] 立即执行函数 IIFE
来源：http://vn.hnjuh.cn

Py:   (lambda: print("run"))()
来源：http://nz.wgjwhj.cn


<!-- 参考信息 -->