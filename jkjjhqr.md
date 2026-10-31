代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jo.wgjwhj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://wy.huixinmuqiang.cn

[A24] 去除首尾空白
来源：http://qi.huanxung.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sr.hnjuh.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ub.nszjky.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nw.9csxet.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fz.lnxyls.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kf.shxzskj.cn

Go:   strings.TrimSpace(s)
来源：http://ut.shxzskj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mq.hnjuh.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hg.nicolike.cn

[A25] 字符串比较
来源：http://zb.lnxyls.cn

Py:   s1 == s2; s1 != s2
来源：http://ug.newstarts.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://df.szxytkj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vf.shxzskj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://op.huanxung.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fo.shtwfgs.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wm.9csxet.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://im.hnjuh.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dv.yuexingan06.cn

[A26] 类型转换总览
来源：http://hc.szsharing.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wx.bookmarksfly.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sv.bjjhwx.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ss.hnjuh.cn

TS:   Number() String() Boolean() x as number
来源：http://ox.szsharing.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kh.huixiangedu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bp.lnxyls.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rw.szsharing.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gh.nicolike.cn

================================================================================
来源：http://yx.shxzskj.cn

B. 流程控制
来源：http://oy.shxzskj.cn

================================================================================
来源：http://pc.muxihuayi.cn

[B01] 条件判断 if / else
来源：http://ev.yuntaijiaju.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://jj.lnxyls.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gd.yuntaijiaju.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://to.wgjwhj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rl.bjjhwx.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://de.shxzukj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yp.lnxyls.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fa.chemitech.net.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kl.szxytkj.cn

[B02] 多分支 else if / elif
来源：http://me.shtwfgs.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://be.yuntaijiaju.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qe.newstarts.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hc.muxihuayi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xo.shxzskj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xq.szsharing.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tb.521024.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ks.huixinmuqiang.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ge.bookmarksfly.cn

[B03] switch / match / case
来源：http://cb.colortex.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ug.521024.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hg.asd995.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qq.shxzukj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hu.hnjuh.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://iz.asd995.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qb.nszjky.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://eo.huixinmuqiang.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gc.chemitech.net.cn

[B04] for 计数循环
来源：http://pr.colortex.cn

Py:   for i in range(10): print(i)
来源：http://mj.jianghongdianzi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ab.jianghongdianzi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kz.panjiajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rt.yuntaijiaju.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ir.yuntaijiaju.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ax.nicolike.cn

Ruby: 10.times { |i| puts i }
来源：http://hm.shxzskj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gn.huixiangedu.cn

[B05] 遍历数组 / 列表
来源：http://ih.chemitech.net.cn

Py:   for item in arr: print(item)
来源：http://qs.huixinmuqiang.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xz.jianghongdianzi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qg.gzmigu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://oy.asd995.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://aq.bjjhwx.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zs.nszjky.cn

Ruby: arr.each { |item| puts item }
来源：http://ju.bookmarksfly.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sk.bookmarksfly.cn

[B06] 遍历字典 / 对象
来源：http://sd.yuntaijiaju.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://me.yuexingan06.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kr.panjiajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zq.bookmarksfly.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ol.shxzukj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gs.wgjwhj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hv.9csxet.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gy.yuexingan06.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ao.jianghongdianzi.cn

[B07] while 循环
来源：http://np.9csxet.cn

Py:   while i < 10: i += 1
来源：http://dy.lnxyls.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xm.bookmarksfly.cn

JS:   while (i < 10) { i++; }
来源：http://ky.lnxyls.cn

TS:   while (i < 10) { i++; }
来源：http://bm.huixinmuqiang.cn

Java: while (i < 10) { i++; }
来源：http://dy.haigaiapp.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xl.shxzskj.cn

Ruby: while i < 10; i += 1; end
来源：http://gd.asd995.cn

C#:   while (i < 10) { i++; }
来源：http://dc.yuexingan06.cn

[B08] do-while（至少执行一次）
来源：http://ma.yuntaijiaju.cn

Py:   # 无 do-while：用 while True + break
来源：http://mp.hahajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zv.wgjwhj.cn

JS:   do { i++; } while (i < 10);
来源：http://dg.muxihuayi.cn

TS:   do { i++; } while (i < 10);
来源：http://ai.newstarts.cn

Java: do { i++; } while (i < 10);
来源：http://dx.huixinmuqiang.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sg.wgjwhj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mg.szxytkj.cn

C#:   do { i++; } while (i < 10);
来源：http://or.shxzskj.cn

[B09] break 与 continue
来源：http://sp.szsharing.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sn.newstarts.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kv.yuntaijiaju.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://of.nicolike.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kl.panjiajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mf.9csxet.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xr.panjiajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pl.haigaiapp.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yk.nicolike.cn

[B10] 遍历同时拿索引
来源：http://mq.shtwfgs.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://eu.lnxyls.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gg.yuntaijiaju.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yy.lnxyls.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xn.bjjhwx.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rz.nicolike.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://db.shtwfgs.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ki.szxytkj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nq.shxzskj.cn

[B11] 生成数字序列 / 区间
来源：http://lv.szsharing.cn

Py:   list(range(0, 10, 2))
来源：http://em.jctech888.com.cn

PHP:  range(0, 10, 2);
来源：http://su.lnxyls.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wn.asd995.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sl.yuntaijiaju.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xj.huixinmuqiang.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ft.jctech888.com.cn

Ruby: (0...10).step(2).to_a
来源：http://ot.asd995.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.bjjhwx.cn

[B12] 跳出多层循环
来源：http://vo.hahajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://sd.bookmarksfly.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mz.asd995.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ho.colortex.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kj.chemitech.net.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lg.chemitech.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://us.shxzskj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qy.szxytkj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yl.wgjwhj.cn

[B13] 判断是否为数字
来源：http://xf.bookmarksfly.cn

Py:   isinstance(x, (int, float))
来源：http://de.panjiajie.cn

PHP:  is_numeric($x)
来源：http://fn.yuntaijiaju.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kv.nszjky.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bc.9csxet.cn

Java: x instanceof Number
来源：http://gw.huanxung.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://em.jianghongdianzi.cn

Ruby: x.is_a?(Numeric)
来源：http://xo.szsharing.cn

C#:   x is int or double or decimal
来源：http://db.newstarts.cn

[B14] 判断值是否在集合内
来源：http://pp.huixinmuqiang.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ph.jctech888.com.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vf.huixinmuqiang.cn

JS:   [1, 2, 3].includes(x)
来源：http://tt.colortex.cn

TS:   [1, 2, 3].includes(x)
来源：http://he.hahajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://yr.bookmarksfly.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hu.jctech888.com.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jm.nicolike.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ab.colortex.cn

[B15] 布尔运算与取反
来源：http://hz.gzmigu.cn

Py:   a and b or not c
来源：http://ue.szxytkj.cn

PHP:  $a && $b || !$c
来源：http://vb.lnxyls.cn

JS:   a && b || !c
来源：http://av.jianghongdianzi.cn

TS:   a && b || !c
来源：http://oq.huanxung.cn

Java: a && b || !c
来源：http://vy.shxzskj.cn

Go:   a && b || !c
来源：http://qt.jctech888.com.cn

Ruby: a && b || !c
来源：http://wk.haigaiapp.cn

C#:   a && b || !c
来源：http://rl.haigaiapp.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xw.chemitech.net.cn

Py:   if not data: return
来源：http://kv.panjiajie.cn

PHP:  if (!$data) { return; }
来源：http://xp.shtwfgs.cn

JS:   if (!data) return;
来源：http://vp.9csxet.cn

TS:   if (!data) return;
来源：http://uu.hnjuh.cn

Java: if (data == null) return;
来源：http://fy.szsharing.cn

Go:   if data == nil { return }
来源：http://ny.shxzskj.cn

Ruby: return if data.nil?
来源：http://de.shxzukj.cn

C#:   if (data == null) return;
来源：http://rs.bjjhwx.cn

================================================================================
来源：http://wk.521024.cn

C. 函数与作用域
来源：http://ct.nszjky.cn

================================================================================
来源：http://kd.wgjwhj.cn

[C01] 定义函数
来源：http://nd.chemitech.net.cn

Py:   def add(a, b): return a + b
来源：http://pp.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ky.521024.cn

JS:   function add(a, b) { return a + b; }
来源：http://zl.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://to.hahajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://pg.lnxyls.cn

Go:   func add(a, b int) int { return a + b }
来源：http://pd.asd995.cn

Ruby: def add(a, b); a + b; end
来源：http://eh.hnjuh.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://km.wgjwhj.cn

[C02] 默认参数
来源：http://el.521024.cn

Py:   def greet(name="World"): return name
来源：http://kc.shxzukj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ii.colortex.cn

JS:   function greet(name = "World") { return name; }
来源：http://mp.hnjuh.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://pi.yuntaijiaju.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vd.hahajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yd.haigaiapp.cn

Ruby: def greet(name = "World") = name
来源：http://rj.chemitech.net.cn

C#:   string Greet(string name = "World") => name;
来源：http://jr.panjiajie.cn

[C03] 可变参数
来源：http://sh.jctech888.com.cn

Py:   def total(*args): return sum(args)
来源：http://zv.muxihuayi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://od.colortex.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dr.hnjuh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uu.521024.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://so.gzmigu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://il.yuexingan06.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rq.hahajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dw.chemitech.net.cn

[C04] 命名参数 / 关键字参数
来源：http://bz.nszjky.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ce.szxytkj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wt.haigaiapp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fn.nicolike.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bm.nszjky.cn

Java: // 无：用 Builder 模式或 record
来源：http://kg.jctech888.com.cn

Go:   // 无：用配置结构体参数
来源：http://hq.haigaiapp.cn

Ruby: f(a: 1, b: 2)
来源：http://vx.asd995.cn

C#:   f(a: 1, b: 2)
来源：http://ay.yuexingan06.cn

[C05] 返回多个值
来源：http://cc.huixinmuqiang.cn

Py:   return a, b
来源：http://pr.521024.cn

PHP:  return [$a, $b];
来源：http://by.hnjuh.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://nw.szsharing.cn

TS:   return { a, b };
来源：http://bm.hnjuh.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gn.jianghongdianzi.cn

Go:   return a, b
来源：http://qc.jctech888.com.cn

Ruby: return a, b
来源：http://mt.bookmarksfly.cn

C#:   return (a, b);              // ValueTuple
来源：http://pg.yuntaijiaju.cn

[C06] 匿名函数 / lambda
来源：http://wn.shxzukj.cn

Py:   square = lambda x: x * x
来源：http://fp.nszjky.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://tq.newstarts.cn

JS:   const square = x => x * x;
来源：http://fl.jianghongdianzi.cn

TS:   const square = (x: number): number => x * x;
来源：http://xn.bjjhwx.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kn.shxzskj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://uz.szxytkj.cn

Ruby: square = ->(x) { x * x }
来源：http://hc.asd995.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ap.bookmarksfly.cn

[C07] 把函数作为参数传入
来源：http://ri.yuntaijiaju.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hb.huanxung.cn

PHP:  array_map("strtoupper", $arr);
来源：http://dq.bookmarksfly.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ih.521024.cn

TS:   arr.map(String)
来源：http://bb.newstarts.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rx.nszjky.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vp.jctech888.com.cn

Ruby: arr.map(&:upcase)
来源：http://ln.hnjuh.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hp.panjiajie.cn

[C08] 闭包
来源：http://mz.colortex.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rr.newstarts.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jf.521024.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jf.hahajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ay.haigaiapp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tg.gzmigu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ro.huanxung.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://iu.panjiajie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ii.hnjuh.cn

[C09] 递归
来源：http://wl.newstarts.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kc.bjjhwx.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://oy.huixinmuqiang.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dd.huixinmuqiang.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xa.haigaiapp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jj.shxzukj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fa.colortex.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://aw.hnjuh.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wr.szsharing.cn

[C10] 变量作用域
来源：http://ab.bookmarksfly.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hj.yuntaijiaju.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hc.shtwfgs.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xn.yuntaijiaju.cn

TS:   同 JS
来源：http://ej.yuntaijiaju.cn

Java: 方法内为块级作用域
来源：http://gc.nicolike.cn

Go:   花括号块级作用域
来源：http://bt.yuntaijiaju.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zy.haigaiapp.cn

C#:   块级作用域
来源：http://nf.wgjwhj.cn

[C11] 模块导入与导出
来源：http://ta.hahajie.cn

Py:   from module import func
来源：http://en.yuntaijiaju.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://iv.wgjwhj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://mi.jctech888.com.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vg.chemitech.net.cn

Java: import java.util.List;
来源：http://qt.gzmigu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jc.asd995.cn

Ruby: require "json"; require_relative "./util"
来源：http://jm.shxzukj.cn

C#:   using System.Text;
来源：http://hm.szxytkj.cn

[C12] 立即执行函数 IIFE
来源：http://ha.shtwfgs.cn

Py:   (lambda: print("run"))()
来源：http://fd.haigaiapp.cn

PHP:  (function () { echo "run"; })();
来源：http://tx.bjjhwx.cn

JS:   (() => { console.log("run"); })();
来源：http://vg.haigaiapp.cn

TS:   (() => { console.log("run"); })();
来源：http://sh.colortex.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nb.shtwfgs.cn

Go:   func() { fmt.Println("run") }()
来源：http://wf.newstarts.cn

Ruby: -> { puts "run" }.call
来源：http://kf.bjjhwx.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jl.jctech888.com.cn

[C13] 类型声明 / 类型注解
来源：http://xy.nszjky.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ck.muxihuayi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vy.huixinmuqiang.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ht.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ek.shxzukj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ia.jianghongdianzi.cn

Go:   func add(a, b int) int
来源：http://xn.hnjuh.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gp.asd995.cn

C#:   int Add(int a, int b) => a + b;
来源：http://zz.bjjhwx.cn

[C14] 泛型函数
来源：http://rd.jctech888.com.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ie.haigaiapp.cn

PHP:  // 无泛型
来源：http://vc.yuexingan06.cn

JS:   // 无泛型
来源：http://hy.szsharing.cn


<!-- 参考信息 -->