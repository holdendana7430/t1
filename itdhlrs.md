代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yq.panjiajie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://vv.hnjuh.cn

[A24] 去除首尾空白
来源：http://ew.jianghongdianzi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rq.nicolike.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ko.huixinmuqiang.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://aw.haigaiapp.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zz.asd995.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mf.asd995.cn

Go:   strings.TrimSpace(s)
来源：http://jp.shxzukj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wp.yuntaijiaju.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zm.szxytkj.cn

[A25] 字符串比较
来源：http://mq.bookmarksfly.cn

Py:   s1 == s2; s1 != s2
来源：http://tb.shxzskj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dp.hahajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://oa.jctech888.com.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jh.colortex.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qc.lnxyls.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wv.bookmarksfly.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://um.gzmigu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ws.bjjhwx.cn

[A26] 类型转换总览
来源：http://xv.muxihuayi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://du.wgjwhj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://if.hahajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qi.yuntaijiaju.cn

TS:   Number() String() Boolean() x as number
来源：http://wb.newstarts.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tf.huixiangedu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zt.shtwfgs.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://hu.haigaiapp.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lm.haigaiapp.cn

================================================================================
来源：http://kt.nszjky.cn

B. 流程控制
来源：http://us.yuexingan06.cn

================================================================================
来源：http://lo.shxzukj.cn

[B01] 条件判断 if / else
来源：http://xn.colortex.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://qv.nszjky.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://aj.hnjuh.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yx.newstarts.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ug.muxihuayi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://mp.hahajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gl.wgjwhj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cp.521024.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tr.shtwfgs.cn

[B02] 多分支 else if / elif
来源：http://uv.panjiajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lp.huanxung.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ai.jianghongdianzi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qr.asd995.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ob.hnjuh.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ka.lnxyls.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hs.huixiangedu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jw.jctech888.com.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xr.9csxet.cn

[B03] switch / match / case
来源：http://fv.521024.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hc.jianghongdianzi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wl.huixinmuqiang.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://iy.szxytkj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nr.shxzskj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zj.szxytkj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nt.asd995.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gz.hahajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sp.szxytkj.cn

[B04] for 计数循环
来源：http://ud.gzmigu.cn

Py:   for i in range(10): print(i)
来源：http://lj.newstarts.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gx.huixinmuqiang.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rn.chemitech.net.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ia.hnjuh.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hi.szsharing.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ql.newstarts.cn

Ruby: 10.times { |i| puts i }
来源：http://wr.chemitech.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zf.huanxung.cn

[B05] 遍历数组 / 列表
来源：http://tt.colortex.cn

Py:   for item in arr: print(item)
来源：http://pw.szxytkj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tl.yuexingan06.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://as.jianghongdianzi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ex.jianghongdianzi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ex.huanxung.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rg.muxihuayi.cn

Ruby: arr.each { |item| puts item }
来源：http://kw.muxihuayi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ah.nszjky.cn

[B06] 遍历字典 / 对象
来源：http://qr.bjjhwx.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://yk.haigaiapp.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://of.shxzskj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://al.yuntaijiaju.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ol.nicolike.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mw.chemitech.net.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sy.shxzukj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mf.jianghongdianzi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://he.521024.cn

[B07] while 循环
来源：http://vt.szxytkj.cn

Py:   while i < 10: i += 1
来源：http://or.haigaiapp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lp.lnxyls.cn

JS:   while (i < 10) { i++; }
来源：http://hm.521024.cn

TS:   while (i < 10) { i++; }
来源：http://yj.huanxung.cn

Java: while (i < 10) { i++; }
来源：http://sl.lnxyls.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yb.521024.cn

Ruby: while i < 10; i += 1; end
来源：http://be.nicolike.cn

C#:   while (i < 10) { i++; }
来源：http://pf.jianghongdianzi.cn

[B08] do-while（至少执行一次）
来源：http://qt.shxzskj.cn

Py:   # 无 do-while：用 while True + break
来源：http://wp.nicolike.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ac.nicolike.cn

JS:   do { i++; } while (i < 10);
来源：http://pg.colortex.cn

TS:   do { i++; } while (i < 10);
来源：http://gs.shxzukj.cn

Java: do { i++; } while (i < 10);
来源：http://lg.wgjwhj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://cn.jianghongdianzi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://oy.colortex.cn

C#:   do { i++; } while (i < 10);
来源：http://ij.shxzskj.cn

[B09] break 与 continue
来源：http://rg.huixiangedu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sf.wgjwhj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fz.newstarts.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ka.9csxet.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wd.haigaiapp.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vy.521024.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ps.521024.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qt.lnxyls.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yf.yuexingan06.cn

[B10] 遍历同时拿索引
来源：http://za.haigaiapp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zw.colortex.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gj.bookmarksfly.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fn.nicolike.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vy.jctech888.com.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cl.jianghongdianzi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ld.jianghongdianzi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qe.huanxung.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tf.jctech888.com.cn

[B11] 生成数字序列 / 区间
来源：http://lz.huixinmuqiang.cn

Py:   list(range(0, 10, 2))
来源：http://ce.muxihuayi.cn

PHP:  range(0, 10, 2);
来源：http://fk.chemitech.net.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rj.panjiajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rj.bjjhwx.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://np.szxytkj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ug.muxihuayi.cn

Ruby: (0...10).step(2).to_a
来源：http://nv.haigaiapp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xp.yuntaijiaju.cn

[B12] 跳出多层循环
来源：http://gb.panjiajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ae.wgjwhj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://uq.muxihuayi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gq.huanxung.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://eh.shtwfgs.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ou.wgjwhj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jo.muxihuayi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sk.panjiajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gk.lnxyls.cn

[B13] 判断是否为数字
来源：http://oa.nszjky.cn

Py:   isinstance(x, (int, float))
来源：http://mn.9csxet.cn

PHP:  is_numeric($x)
来源：http://an.shxzukj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tv.bookmarksfly.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://py.yuntaijiaju.cn

Java: x instanceof Number
来源：http://wp.shxzskj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ax.yuntaijiaju.cn

Ruby: x.is_a?(Numeric)
来源：http://ul.9csxet.cn

C#:   x is int or double or decimal
来源：http://ys.jctech888.com.cn

[B14] 判断值是否在集合内
来源：http://jk.bookmarksfly.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pl.yuexingan06.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bg.huanxung.cn

JS:   [1, 2, 3].includes(x)
来源：http://eu.shtwfgs.cn

TS:   [1, 2, 3].includes(x)
来源：http://dj.shtwfgs.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://on.bjjhwx.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://iy.bookmarksfly.cn

Ruby: [1, 2, 3].include?(x)
来源：http://uv.shxzskj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sk.asd995.cn

[B15] 布尔运算与取反
来源：http://mj.colortex.cn

Py:   a and b or not c
来源：http://te.shtwfgs.cn

PHP:  $a && $b || !$c
来源：http://xa.nicolike.cn

JS:   a && b || !c
来源：http://th.hahajie.cn

TS:   a && b || !c
来源：http://lp.hnjuh.cn

Java: a && b || !c
来源：http://qs.panjiajie.cn

Go:   a && b || !c
来源：http://cr.hnjuh.cn

Ruby: a && b || !c
来源：http://ec.jianghongdianzi.cn

C#:   a && b || !c
来源：http://ct.hahajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://us.wgjwhj.cn

Py:   if not data: return
来源：http://ys.lnxyls.cn

PHP:  if (!$data) { return; }
来源：http://dw.nicolike.cn

JS:   if (!data) return;
来源：http://lo.newstarts.cn

TS:   if (!data) return;
来源：http://pv.huanxung.cn

Java: if (data == null) return;
来源：http://xi.jctech888.com.cn

Go:   if data == nil { return }
来源：http://at.yuexingan06.cn

Ruby: return if data.nil?
来源：http://ew.lnxyls.cn

C#:   if (data == null) return;
来源：http://cx.hnjuh.cn

================================================================================
来源：http://kl.hnjuh.cn

C. 函数与作用域
来源：http://pl.haigaiapp.cn

================================================================================
来源：http://pc.bookmarksfly.cn

[C01] 定义函数
来源：http://lf.chemitech.net.cn

Py:   def add(a, b): return a + b
来源：http://vz.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qm.jctech888.com.cn

JS:   function add(a, b) { return a + b; }
来源：http://zr.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sd.lnxyls.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://yb.yuntaijiaju.cn

Go:   func add(a, b int) int { return a + b }
来源：http://fq.shxzukj.cn

Ruby: def add(a, b); a + b; end
来源：http://wr.shxzskj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rh.asd995.cn

[C02] 默认参数
来源：http://tc.hnjuh.cn

Py:   def greet(name="World"): return name
来源：http://ho.muxihuayi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zz.huanxung.cn

JS:   function greet(name = "World") { return name; }
来源：http://yc.jianghongdianzi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lh.hahajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://pf.bookmarksfly.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xb.bookmarksfly.cn

Ruby: def greet(name = "World") = name
来源：http://ua.shtwfgs.cn

C#:   string Greet(string name = "World") => name;
来源：http://zm.szsharing.cn

[C03] 可变参数
来源：http://fn.yuntaijiaju.cn

Py:   def total(*args): return sum(args)
来源：http://yn.huixiangedu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pu.bjjhwx.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ip.chemitech.net.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vq.newstarts.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gc.chemitech.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zz.panjiajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://dc.shtwfgs.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sq.gzmigu.cn

[C04] 命名参数 / 关键字参数
来源：http://yy.gzmigu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ne.gzmigu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ne.bjjhwx.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mw.szsharing.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jt.shxzukj.cn

Java: // 无：用 Builder 模式或 record
来源：http://im.szxytkj.cn

Go:   // 无：用配置结构体参数
来源：http://sx.shxzukj.cn

Ruby: f(a: 1, b: 2)
来源：http://op.haigaiapp.cn

C#:   f(a: 1, b: 2)
来源：http://if.asd995.cn

[C05] 返回多个值
来源：http://na.panjiajie.cn

Py:   return a, b
来源：http://wi.asd995.cn

PHP:  return [$a, $b];
来源：http://fx.521024.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zc.lnxyls.cn

TS:   return { a, b };
来源：http://sm.yuexingan06.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fg.shxzukj.cn

Go:   return a, b
来源：http://ik.yuexingan06.cn

Ruby: return a, b
来源：http://qx.yuexingan06.cn

C#:   return (a, b);              // ValueTuple
来源：http://jw.yuexingan06.cn

[C06] 匿名函数 / lambda
来源：http://zg.colortex.cn

Py:   square = lambda x: x * x
来源：http://bz.haigaiapp.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bc.521024.cn

JS:   const square = x => x * x;
来源：http://sg.nszjky.cn

TS:   const square = (x: number): number => x * x;
来源：http://co.jianghongdianzi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rp.521024.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ji.muxihuayi.cn

Ruby: square = ->(x) { x * x }
来源：http://pb.hahajie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://nq.jianghongdianzi.cn

[C07] 把函数作为参数传入
来源：http://ph.shxzskj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xa.wgjwhj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ry.gzmigu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bz.521024.cn

TS:   arr.map(String)
来源：http://gy.521024.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hc.shxzskj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ns.panjiajie.cn

Ruby: arr.map(&:upcase)
来源：http://yj.521024.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ty.jianghongdianzi.cn

[C08] 闭包
来源：http://nk.huixiangedu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lt.yuntaijiaju.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bx.nszjky.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ef.wgjwhj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ze.panjiajie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pk.jianghongdianzi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kr.bookmarksfly.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://np.shxzukj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zy.szxytkj.cn

[C09] 递归
来源：http://gi.lnxyls.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fe.nicolike.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fp.asd995.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vn.wgjwhj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wt.bookmarksfly.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ob.shxzukj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wf.jctech888.com.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ph.asd995.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fd.colortex.cn

[C10] 变量作用域
来源：http://jo.chemitech.net.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nt.szsharing.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dx.nicolike.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jg.bookmarksfly.cn

TS:   同 JS
来源：http://wr.bookmarksfly.cn

Java: 方法内为块级作用域
来源：http://ak.yuexingan06.cn

Go:   花括号块级作用域
来源：http://qa.asd995.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cc.bjjhwx.cn

C#:   块级作用域
来源：http://pk.9csxet.cn

[C11] 模块导入与导出
来源：http://vx.nszjky.cn

Py:   from module import func
来源：http://zl.nicolike.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://dy.asd995.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://tu.szxytkj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://el.shxzskj.cn

Java: import java.util.List;
来源：http://cg.haigaiapp.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ty.huixinmuqiang.cn

Ruby: require "json"; require_relative "./util"
来源：http://te.hahajie.cn

C#:   using System.Text;
来源：http://gq.lnxyls.cn

[C12] 立即执行函数 IIFE
来源：http://fq.hnjuh.cn

Py:   (lambda: print("run"))()
来源：http://cu.hahajie.cn

PHP:  (function () { echo "run"; })();
来源：http://qz.hahajie.cn

JS:   (() => { console.log("run"); })();
来源：http://to.bjjhwx.cn

TS:   (() => { console.log("run"); })();
来源：http://fs.asd995.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ao.jctech888.com.cn

Go:   func() { fmt.Println("run") }()
来源：http://ea.nszjky.cn

Ruby: -> { puts "run" }.call
来源：http://qj.wgjwhj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ni.9csxet.cn

[C13] 类型声明 / 类型注解
来源：http://sq.jianghongdianzi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zq.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ye.nszjky.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wj.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oe.9csxet.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tn.panjiajie.cn

Go:   func add(a, b int) int
来源：http://bw.wgjwhj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://se.nszjky.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ud.wgjwhj.cn

[C14] 泛型函数
来源：http://nd.chemitech.net.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hx.hnjuh.cn

PHP:  // 无泛型
来源：http://nl.szxytkj.cn

JS:   // 无泛型
来源：http://wm.bookmarksfly.cn


<!-- 参考信息 -->