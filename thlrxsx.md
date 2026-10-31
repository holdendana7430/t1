代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rl.shtwfgs.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pm.shtwfgs.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ks.nicolike.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bl.yuexingan06.cn

[A26] 类型转换总览
来源：http://kb.huanxung.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lv.haigaiapp.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qw.yuexingan06.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://by.muxihuayi.cn

TS:   Number() String() Boolean() x as number
来源：http://nw.huanxung.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tu.jctech888.com.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ft.bookmarksfly.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://tm.yuntaijiaju.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ci.shxzukj.cn

================================================================================
来源：http://au.yuntaijiaju.cn

B. 流程控制
来源：http://uf.lnxyls.cn

================================================================================
来源：http://nu.521024.cn

[B01] 条件判断 if / else
来源：http://ut.521024.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://eq.hnjuh.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gj.muxihuayi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://da.wgjwhj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ch.chemitech.net.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://rk.muxihuayi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rq.9csxet.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pd.shxzskj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://no.521024.cn

[B02] 多分支 else if / elif
来源：http://je.yuntaijiaju.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qf.gzmigu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://df.lnxyls.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ht.newstarts.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://la.wgjwhj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hq.yuntaijiaju.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vt.panjiajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cd.colortex.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ir.szsharing.cn

[B03] switch / match / case
来源：http://uz.szxytkj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wl.hnjuh.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ha.hnjuh.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://za.panjiajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fo.nicolike.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ph.yuntaijiaju.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://am.lnxyls.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rb.muxihuayi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://in.szsharing.cn

[B04] for 计数循环
来源：http://sl.huanxung.cn

Py:   for i in range(10): print(i)
来源：http://fn.newstarts.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://em.muxihuayi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ae.shtwfgs.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vr.huanxung.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jz.bookmarksfly.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ks.haigaiapp.cn

Ruby: 10.times { |i| puts i }
来源：http://pn.nszjky.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://im.9csxet.cn

[B05] 遍历数组 / 列表
来源：http://if.shxzukj.cn

Py:   for item in arr: print(item)
来源：http://lv.szxytkj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yu.huixinmuqiang.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://iz.newstarts.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bd.gzmigu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ov.nszjky.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://to.yuntaijiaju.cn

Ruby: arr.each { |item| puts item }
来源：http://ic.hnjuh.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ol.huixinmuqiang.cn

[B06] 遍历字典 / 对象
来源：http://zu.yuntaijiaju.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ub.hnjuh.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yv.chemitech.net.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xn.panjiajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pd.gzmigu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ur.521024.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://js.yuntaijiaju.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fi.colortex.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ni.shtwfgs.cn

[B07] while 循环
来源：http://ku.newstarts.cn

Py:   while i < 10: i += 1
来源：http://lc.szsharing.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ot.nicolike.cn

JS:   while (i < 10) { i++; }
来源：http://sy.gzmigu.cn

TS:   while (i < 10) { i++; }
来源：http://vg.huanxung.cn

Java: while (i < 10) { i++; }
来源：http://dm.jctech888.com.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ar.wgjwhj.cn

Ruby: while i < 10; i += 1; end
来源：http://oq.jctech888.com.cn

C#:   while (i < 10) { i++; }
来源：http://oy.jianghongdianzi.cn

[B08] do-while（至少执行一次）
来源：http://aw.haigaiapp.cn

Py:   # 无 do-while：用 while True + break
来源：http://pt.yuexingan06.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://bf.9csxet.cn

JS:   do { i++; } while (i < 10);
来源：http://an.colortex.cn

TS:   do { i++; } while (i < 10);
来源：http://lx.colortex.cn

Java: do { i++; } while (i < 10);
来源：http://gb.wgjwhj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mi.yuexingan06.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hd.haigaiapp.cn

C#:   do { i++; } while (i < 10);
来源：http://er.huanxung.cn

[B09] break 与 continue
来源：http://cn.521024.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fk.yuexingan06.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wr.panjiajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jc.huanxung.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yf.huixiangedu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wt.yuexingan06.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vs.bookmarksfly.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wx.hahajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eo.asd995.cn

[B10] 遍历同时拿索引
来源：http://bp.shxzukj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hj.muxihuayi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://my.nicolike.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cs.yuexingan06.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ej.nszjky.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cw.hahajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cg.yuntaijiaju.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nj.nszjky.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dz.yuexingan06.cn

[B11] 生成数字序列 / 区间
来源：http://kc.huanxung.cn

Py:   list(range(0, 10, 2))
来源：http://nr.huanxung.cn

PHP:  range(0, 10, 2);
来源：http://nw.szxytkj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://az.wgjwhj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gt.szsharing.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gp.jctech888.com.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tg.newstarts.cn

Ruby: (0...10).step(2).to_a
来源：http://jl.huixinmuqiang.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vw.yuexingan06.cn

[B12] 跳出多层循环
来源：http://sp.hnjuh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://th.haigaiapp.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://nf.colortex.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mr.asd995.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xr.yuntaijiaju.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ab.asd995.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://aa.bjjhwx.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ym.panjiajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ko.shxzukj.cn

[B13] 判断是否为数字
来源：http://mj.newstarts.cn

Py:   isinstance(x, (int, float))
来源：http://mn.yuntaijiaju.cn

PHP:  is_numeric($x)
来源：http://gd.huixinmuqiang.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wl.hnjuh.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gw.huanxung.cn

Java: x instanceof Number
来源：http://po.shxzukj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rd.wgjwhj.cn

Ruby: x.is_a?(Numeric)
来源：http://kw.bookmarksfly.cn

C#:   x is int or double or decimal
来源：http://fa.panjiajie.cn

[B14] 判断值是否在集合内
来源：http://tj.shtwfgs.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ri.szsharing.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pv.muxihuayi.cn

JS:   [1, 2, 3].includes(x)
来源：http://wm.chemitech.net.cn

TS:   [1, 2, 3].includes(x)
来源：http://xy.huixinmuqiang.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vu.panjiajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tt.hnjuh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://wa.panjiajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tg.huanxung.cn

[B15] 布尔运算与取反
来源：http://jj.huanxung.cn

Py:   a and b or not c
来源：http://qb.haigaiapp.cn

PHP:  $a && $b || !$c
来源：http://tc.521024.cn

JS:   a && b || !c
来源：http://om.newstarts.cn

TS:   a && b || !c
来源：http://el.9csxet.cn

Java: a && b || !c
来源：http://ko.haigaiapp.cn

Go:   a && b || !c
来源：http://rg.szxytkj.cn

Ruby: a && b || !c
来源：http://jx.nszjky.cn

C#:   a && b || !c
来源：http://ak.huixiangedu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jy.lnxyls.cn

Py:   if not data: return
来源：http://fl.muxihuayi.cn

PHP:  if (!$data) { return; }
来源：http://ex.panjiajie.cn

JS:   if (!data) return;
来源：http://wn.lnxyls.cn

TS:   if (!data) return;
来源：http://lv.huixiangedu.cn

Java: if (data == null) return;
来源：http://pa.nszjky.cn

Go:   if data == nil { return }
来源：http://md.shxzskj.cn

Ruby: return if data.nil?
来源：http://oe.szsharing.cn

C#:   if (data == null) return;
来源：http://ga.shtwfgs.cn

================================================================================
来源：http://wj.yuntaijiaju.cn

C. 函数与作用域
来源：http://xx.521024.cn

================================================================================
来源：http://hx.huanxung.cn

[C01] 定义函数
来源：http://iy.lnxyls.cn

Py:   def add(a, b): return a + b
来源：http://em.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qy.shxzukj.cn

JS:   function add(a, b) { return a + b; }
来源：http://fg.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kt.jctech888.com.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fp.panjiajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://sh.wgjwhj.cn

Ruby: def add(a, b); a + b; end
来源：http://wg.shxzskj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xl.9csxet.cn

[C02] 默认参数
来源：http://wh.muxihuayi.cn

Py:   def greet(name="World"): return name
来源：http://gg.huixiangedu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://jn.haigaiapp.cn

JS:   function greet(name = "World") { return name; }
来源：http://ma.panjiajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://kx.521024.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://af.521024.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gt.jianghongdianzi.cn

Ruby: def greet(name = "World") = name
来源：http://er.newstarts.cn

C#:   string Greet(string name = "World") => name;
来源：http://cw.nszjky.cn

[C03] 可变参数
来源：http://oo.huixiangedu.cn

Py:   def total(*args): return sum(args)
来源：http://xn.wgjwhj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wm.bookmarksfly.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qi.lnxyls.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bi.lnxyls.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fp.hahajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gp.huanxung.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ev.bookmarksfly.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nr.huixinmuqiang.cn

[C04] 命名参数 / 关键字参数
来源：http://fe.muxihuayi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sx.huixinmuqiang.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dx.nicolike.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xd.jctech888.com.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ze.muxihuayi.cn

Java: // 无：用 Builder 模式或 record
来源：http://ng.hahajie.cn

Go:   // 无：用配置结构体参数
来源：http://qm.yuntaijiaju.cn

Ruby: f(a: 1, b: 2)
来源：http://he.shtwfgs.cn

C#:   f(a: 1, b: 2)
来源：http://qg.yuntaijiaju.cn

[C05] 返回多个值
来源：http://of.9csxet.cn

Py:   return a, b
来源：http://os.521024.cn

PHP:  return [$a, $b];
来源：http://do.huixiangedu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pl.hnjuh.cn

TS:   return { a, b };
来源：http://pj.hahajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vv.9csxet.cn

Go:   return a, b
来源：http://pj.jctech888.com.cn

Ruby: return a, b
来源：http://zu.huanxung.cn

C#:   return (a, b);              // ValueTuple
来源：http://lv.jctech888.com.cn

[C06] 匿名函数 / lambda
来源：http://yx.szsharing.cn

Py:   square = lambda x: x * x
来源：http://ev.wgjwhj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xf.bjjhwx.cn

JS:   const square = x => x * x;
来源：http://wr.panjiajie.cn

TS:   const square = (x: number): number => x * x;
来源：http://gx.nicolike.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sk.shxzukj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rg.9csxet.cn

Ruby: square = ->(x) { x * x }
来源：http://vk.nicolike.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bp.shxzukj.cn

[C07] 把函数作为参数传入
来源：http://zx.nicolike.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qe.newstarts.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bd.shtwfgs.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hp.bjjhwx.cn

TS:   arr.map(String)
来源：http://hf.jianghongdianzi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mc.yuntaijiaju.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ah.nicolike.cn

Ruby: arr.map(&:upcase)
来源：http://jy.huixiangedu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://yr.szxytkj.cn

[C08] 闭包
来源：http://cr.haigaiapp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ap.asd995.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mh.huanxung.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jw.jianghongdianzi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://us.521024.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uk.jianghongdianzi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sw.hahajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yj.wgjwhj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uu.nicolike.cn

[C09] 递归
来源：http://az.huixinmuqiang.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zu.wgjwhj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://go.chemitech.net.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ko.asd995.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vw.bookmarksfly.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lb.bjjhwx.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wh.huixinmuqiang.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hn.hahajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://oa.colortex.cn

[C10] 变量作用域
来源：http://hc.haigaiapp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lk.szsharing.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bu.chemitech.net.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yuexingan06.cn

TS:   同 JS
来源：http://se.nicolike.cn

Java: 方法内为块级作用域
来源：http://uy.huanxung.cn

Go:   花括号块级作用域
来源：http://nf.hahajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vo.huanxung.cn

C#:   块级作用域
来源：http://nq.gzmigu.cn

[C11] 模块导入与导出
来源：http://bx.panjiajie.cn

Py:   from module import func
来源：http://ht.shxzukj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tb.9csxet.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ai.huanxung.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fc.huixiangedu.cn

Java: import java.util.List;
来源：http://en.huixinmuqiang.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tv.yuexingan06.cn

Ruby: require "json"; require_relative "./util"
来源：http://mc.szxytkj.cn

C#:   using System.Text;
来源：http://gd.chemitech.net.cn

[C12] 立即执行函数 IIFE
来源：http://nd.asd995.cn

Py:   (lambda: print("run"))()
来源：http://rp.shtwfgs.cn

PHP:  (function () { echo "run"; })();
来源：http://wp.asd995.cn

JS:   (() => { console.log("run"); })();
来源：http://wz.szxytkj.cn

TS:   (() => { console.log("run"); })();
来源：http://jm.shtwfgs.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ee.huanxung.cn

Go:   func() { fmt.Println("run") }()
来源：http://vd.newstarts.cn

Ruby: -> { puts "run" }.call
来源：http://zi.wgjwhj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jl.gzmigu.cn

[C13] 类型声明 / 类型注解
来源：http://sk.huixinmuqiang.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mr.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ft.nszjky.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://be.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xg.jctech888.com.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qx.yuntaijiaju.cn

Go:   func add(a, b int) int
来源：http://xx.nicolike.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wg.yuexingan06.cn

C#:   int Add(int a, int b) => a + b;
来源：http://oy.shxzskj.cn

[C14] 泛型函数
来源：http://pe.panjiajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gb.haigaiapp.cn

PHP:  // 无泛型
来源：http://xw.shxzskj.cn

JS:   // 无泛型
来源：http://za.hnjuh.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ig.wgjwhj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ai.panjiajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xn.yuexingan06.cn

Ruby: # 无泛型
来源：http://wn.gzmigu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cz.chemitech.net.cn

[C15] 解构 / 展开参数
来源：http://qb.newstarts.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sf.asd995.cn

PHP:  [$a, $b] = $pair;
来源：http://fx.jianghongdianzi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zs.chemitech.net.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xv.huixiangedu.cn

Java: // 无解构
来源：http://gi.huanxung.cn

Go:   // 无解构
来源：http://zq.chemitech.net.cn

Ruby: a, b = pair
来源：http://is.lnxyls.cn

C#:   var (a, b) = pair;
来源：http://qd.szsharing.cn

[C16] 函数 / 方法重载
来源：http://ql.wgjwhj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fp.shtwfgs.cn


<!-- 参考信息 -->