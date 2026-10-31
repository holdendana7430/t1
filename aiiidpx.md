代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gx.huixinmuqiang.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gt.bookmarksfly.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://fa.shxzukj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zb.9csxet.cn

[A26] 类型转换总览
来源：http://te.shxzukj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qu.haigaiapp.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://il.shxzskj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xm.colortex.cn

TS:   Number() String() Boolean() x as number
来源：http://vf.yuexingan06.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ax.jianghongdianzi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ne.lnxyls.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://te.huixinmuqiang.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://br.lnxyls.cn

================================================================================
来源：http://aa.hahajie.cn

B. 流程控制
来源：http://as.shxzukj.cn

================================================================================
来源：http://nd.chemitech.net.cn

[B01] 条件判断 if / else
来源：http://hk.newstarts.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://nm.jctech888.com.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ks.asd995.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lj.nszjky.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nj.muxihuayi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qs.9csxet.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vo.yuexingan06.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zu.bjjhwx.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ce.muxihuayi.cn

[B02] 多分支 else if / elif
来源：http://cx.chemitech.net.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lw.newstarts.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tb.gzmigu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ey.huixiangedu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ee.wgjwhj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vz.muxihuayi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tj.huixinmuqiang.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pj.bookmarksfly.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ha.521024.cn

[B03] switch / match / case
来源：http://po.szxytkj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lm.jctech888.com.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tf.shxzukj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ps.huanxung.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://du.panjiajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gu.nicolike.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ce.yuexingan06.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tk.lnxyls.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ok.chemitech.net.cn

[B04] for 计数循环
来源：http://mq.chemitech.net.cn

Py:   for i in range(10): print(i)
来源：http://qz.newstarts.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qh.haigaiapp.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tp.yuexingan06.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ci.hahajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bj.shxzskj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kv.gzmigu.cn

Ruby: 10.times { |i| puts i }
来源：http://qv.shxzukj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gg.9csxet.cn

[B05] 遍历数组 / 列表
来源：http://ph.jctech888.com.cn

Py:   for item in arr: print(item)
来源：http://ey.panjiajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pj.9csxet.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fc.hahajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://oz.lnxyls.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ay.jctech888.com.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mw.bookmarksfly.cn

Ruby: arr.each { |item| puts item }
来源：http://sq.nicolike.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zr.bjjhwx.cn

[B06] 遍历字典 / 对象
来源：http://vg.lnxyls.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://oh.shxzukj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dw.521024.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gu.nicolike.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oy.hnjuh.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ob.lnxyls.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qw.huixiangedu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://uw.yuntaijiaju.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sv.yuntaijiaju.cn

[B07] while 循环
来源：http://up.jianghongdianzi.cn

Py:   while i < 10: i += 1
来源：http://js.lnxyls.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bh.lnxyls.cn

JS:   while (i < 10) { i++; }
来源：http://fv.wgjwhj.cn

TS:   while (i < 10) { i++; }
来源：http://hd.lnxyls.cn

Java: while (i < 10) { i++; }
来源：http://er.nszjky.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hc.wgjwhj.cn

Ruby: while i < 10; i += 1; end
来源：http://aw.nicolike.cn

C#:   while (i < 10) { i++; }
来源：http://do.wgjwhj.cn

[B08] do-while（至少执行一次）
来源：http://kx.bookmarksfly.cn

Py:   # 无 do-while：用 while True + break
来源：http://wt.wgjwhj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://tl.hahajie.cn

JS:   do { i++; } while (i < 10);
来源：http://uv.shxzukj.cn

TS:   do { i++; } while (i < 10);
来源：http://ck.panjiajie.cn

Java: do { i++; } while (i < 10);
来源：http://jl.yuntaijiaju.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ms.newstarts.cn

Ruby: begin; i += 1; end while i < 10
来源：http://us.jctech888.com.cn

C#:   do { i++; } while (i < 10);
来源：http://bt.9csxet.cn

[B09] break 与 continue
来源：http://ub.yuexingan06.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jr.nszjky.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bz.hnjuh.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fm.521024.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://br.521024.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tm.huixinmuqiang.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sk.shxzukj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gx.nicolike.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wj.panjiajie.cn

[B10] 遍历同时拿索引
来源：http://cm.szxytkj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gr.huanxung.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yh.hnjuh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://no.jctech888.com.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ye.nszjky.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sl.newstarts.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sr.chemitech.net.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yi.521024.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ta.yuexingan06.cn

[B11] 生成数字序列 / 区间
来源：http://pv.chemitech.net.cn

Py:   list(range(0, 10, 2))
来源：http://zb.newstarts.cn

PHP:  range(0, 10, 2);
来源：http://ma.shxzukj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tc.asd995.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qj.nicolike.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qj.bookmarksfly.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mw.wgjwhj.cn

Ruby: (0...10).step(2).to_a
来源：http://vd.gzmigu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wv.huixiangedu.cn

[B12] 跳出多层循环
来源：http://lt.nszjky.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://uj.wgjwhj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://yj.shtwfgs.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hv.bookmarksfly.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pm.521024.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tx.jctech888.com.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gi.shtwfgs.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yx.muxihuayi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kb.asd995.cn

[B13] 判断是否为数字
来源：http://uf.9csxet.cn

Py:   isinstance(x, (int, float))
来源：http://en.asd995.cn

PHP:  is_numeric($x)
来源：http://kq.huixiangedu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pz.huixiangedu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dx.hahajie.cn

Java: x instanceof Number
来源：http://pr.szsharing.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://he.hnjuh.cn

Ruby: x.is_a?(Numeric)
来源：http://ir.newstarts.cn

C#:   x is int or double or decimal
来源：http://np.haigaiapp.cn

[B14] 判断值是否在集合内
来源：http://ws.huixinmuqiang.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gu.521024.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vg.asd995.cn

JS:   [1, 2, 3].includes(x)
来源：http://tv.jctech888.com.cn

TS:   [1, 2, 3].includes(x)
来源：http://ej.shxzukj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://tb.newstarts.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yz.haigaiapp.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ml.szsharing.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ap.jctech888.com.cn

[B15] 布尔运算与取反
来源：http://zp.muxihuayi.cn

Py:   a and b or not c
来源：http://km.yuexingan06.cn

PHP:  $a && $b || !$c
来源：http://gd.huixinmuqiang.cn

JS:   a && b || !c
来源：http://xa.shxzskj.cn

TS:   a && b || !c
来源：http://xz.haigaiapp.cn

Java: a && b || !c
来源：http://nu.jctech888.com.cn

Go:   a && b || !c
来源：http://sx.shtwfgs.cn

Ruby: a && b || !c
来源：http://ji.asd995.cn

C#:   a && b || !c
来源：http://vq.yuntaijiaju.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zj.gzmigu.cn

Py:   if not data: return
来源：http://lj.bookmarksfly.cn

PHP:  if (!$data) { return; }
来源：http://zv.wgjwhj.cn

JS:   if (!data) return;
来源：http://fo.newstarts.cn

TS:   if (!data) return;
来源：http://al.jctech888.com.cn

Java: if (data == null) return;
来源：http://xh.panjiajie.cn

Go:   if data == nil { return }
来源：http://lv.haigaiapp.cn

Ruby: return if data.nil?
来源：http://op.huixiangedu.cn

C#:   if (data == null) return;
来源：http://dt.shtwfgs.cn

================================================================================
来源：http://te.panjiajie.cn

C. 函数与作用域
来源：http://nt.muxihuayi.cn

================================================================================
来源：http://vb.colortex.cn

[C01] 定义函数
来源：http://oj.panjiajie.cn

Py:   def add(a, b): return a + b
来源：http://sq.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nf.521024.cn

JS:   function add(a, b) { return a + b; }
来源：http://ij.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://am.lnxyls.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://co.jianghongdianzi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qd.521024.cn

Ruby: def add(a, b); a + b; end
来源：http://ev.shtwfgs.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kn.szsharing.cn

[C02] 默认参数
来源：http://ur.bookmarksfly.cn

Py:   def greet(name="World"): return name
来源：http://rw.hnjuh.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hu.shtwfgs.cn

JS:   function greet(name = "World") { return name; }
来源：http://mi.gzmigu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gq.szsharing.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wo.shxzukj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sr.panjiajie.cn

Ruby: def greet(name = "World") = name
来源：http://ct.haigaiapp.cn

C#:   string Greet(string name = "World") => name;
来源：http://vc.jianghongdianzi.cn

[C03] 可变参数
来源：http://cu.huixinmuqiang.cn

Py:   def total(*args): return sum(args)
来源：http://uo.jianghongdianzi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zo.shxzskj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hs.szxytkj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cg.haigaiapp.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yl.yuexingan06.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nr.wgjwhj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://nf.haigaiapp.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wo.gzmigu.cn

[C04] 命名参数 / 关键字参数
来源：http://xz.huanxung.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pn.lnxyls.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ua.asd995.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fn.yuexingan06.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ne.szxytkj.cn

Java: // 无：用 Builder 模式或 record
来源：http://nw.asd995.cn

Go:   // 无：用配置结构体参数
来源：http://pd.shtwfgs.cn

Ruby: f(a: 1, b: 2)
来源：http://kt.yuntaijiaju.cn

C#:   f(a: 1, b: 2)
来源：http://tm.gzmigu.cn

[C05] 返回多个值
来源：http://bm.jianghongdianzi.cn

Py:   return a, b
来源：http://xa.9csxet.cn

PHP:  return [$a, $b];
来源：http://lh.szxytkj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://hy.bjjhwx.cn

TS:   return { a, b };
来源：http://up.szsharing.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dr.nszjky.cn

Go:   return a, b
来源：http://fe.haigaiapp.cn

Ruby: return a, b
来源：http://dl.nicolike.cn

C#:   return (a, b);              // ValueTuple
来源：http://yq.asd995.cn

[C06] 匿名函数 / lambda
来源：http://tm.jianghongdianzi.cn

Py:   square = lambda x: x * x
来源：http://ph.gzmigu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wy.bookmarksfly.cn

JS:   const square = x => x * x;
来源：http://zf.521024.cn

TS:   const square = (x: number): number => x * x;
来源：http://kg.shxzukj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gx.huixinmuqiang.cn

Go:   sq := func(x int) int { return x * x }
来源：http://lz.chemitech.net.cn

Ruby: square = ->(x) { x * x }
来源：http://mc.wgjwhj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ij.newstarts.cn

[C07] 把函数作为参数传入
来源：http://ps.wgjwhj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dk.szsharing.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bo.muxihuayi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jr.colortex.cn

TS:   arr.map(String)
来源：http://db.colortex.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://en.9csxet.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nv.huixinmuqiang.cn

Ruby: arr.map(&:upcase)
来源：http://um.huixinmuqiang.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ec.huanxung.cn

[C08] 闭包
来源：http://ka.newstarts.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wl.shxzukj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pp.shxzukj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vz.asd995.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pb.lnxyls.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://th.jctech888.com.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ad.huanxung.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://es.wgjwhj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nr.521024.cn

[C09] 递归
来源：http://oz.hnjuh.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fj.hnjuh.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mi.yuexingan06.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cc.shtwfgs.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mv.muxihuayi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tx.521024.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gz.asd995.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qm.yuexingan06.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://er.panjiajie.cn

[C10] 变量作用域
来源：http://ge.9csxet.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ej.szxytkj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xe.shtwfgs.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cy.yuexingan06.cn

TS:   同 JS
来源：http://es.shxzukj.cn

Java: 方法内为块级作用域
来源：http://tb.huixiangedu.cn

Go:   花括号块级作用域
来源：http://il.szsharing.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bp.jctech888.com.cn

C#:   块级作用域
来源：http://mr.jianghongdianzi.cn

[C11] 模块导入与导出
来源：http://eh.nicolike.cn

Py:   from module import func
来源：http://oh.shxzskj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zh.521024.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://dh.lnxyls.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jp.colortex.cn

Java: import java.util.List;
来源：http://or.newstarts.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ot.szxytkj.cn

Ruby: require "json"; require_relative "./util"
来源：http://xh.gzmigu.cn

C#:   using System.Text;
来源：http://lx.gzmigu.cn

[C12] 立即执行函数 IIFE
来源：http://fx.muxihuayi.cn

Py:   (lambda: print("run"))()
来源：http://xt.wgjwhj.cn

PHP:  (function () { echo "run"; })();
来源：http://oj.bookmarksfly.cn

JS:   (() => { console.log("run"); })();
来源：http://vm.szxytkj.cn

TS:   (() => { console.log("run"); })();
来源：http://yr.huixinmuqiang.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ud.hahajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://iu.haigaiapp.cn

Ruby: -> { puts "run" }.call
来源：http://ds.hnjuh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mo.huixiangedu.cn

[C13] 类型声明 / 类型注解
来源：http://cv.shxzskj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zc.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mg.huixiangedu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kp.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://aw.yuexingan06.cn

Java: int add(int a, int b) { return a + b; }
来源：http://oz.huanxung.cn

Go:   func add(a, b int) int
来源：http://zt.huixiangedu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://me.shtwfgs.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cj.asd995.cn

[C14] 泛型函数
来源：http://ag.jianghongdianzi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://oc.haigaiapp.cn

PHP:  // 无泛型
来源：http://rb.yuexingan06.cn

JS:   // 无泛型
来源：http://tl.9csxet.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ty.szxytkj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rk.wgjwhj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ug.asd995.cn

Ruby: # 无泛型
来源：http://uw.muxihuayi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ly.szxytkj.cn

[C15] 解构 / 展开参数
来源：http://vq.colortex.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ss.szsharing.cn

PHP:  [$a, $b] = $pair;
来源：http://ye.yuntaijiaju.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pf.jctech888.com.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://za.lnxyls.cn

Java: // 无解构
来源：http://pn.colortex.cn

Go:   // 无解构
来源：http://iq.muxihuayi.cn

Ruby: a, b = pair
来源：http://uh.hahajie.cn

C#:   var (a, b) = pair;
来源：http://vr.521024.cn

[C16] 函数 / 方法重载
来源：http://go.asd995.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hm.chemitech.net.cn


<!-- 参考信息 -->