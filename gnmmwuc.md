代发 wailian999

[A26] 类型转换总览
来源：http://lo.nszjky.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yw.muxihuayi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://aa.muxihuayi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qc.nicolike.cn

TS:   Number() String() Boolean() x as number
来源：http://eq.huixiangedu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vi.wgjwhj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gj.hahajie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://oc.muxihuayi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fo.521024.cn

================================================================================
来源：http://ax.panjiajie.cn

B. 流程控制
来源：http://ro.521024.cn

================================================================================
来源：http://cw.chemitech.net.cn

[B01] 条件判断 if / else
来源：http://ld.shtwfgs.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://pm.huixiangedu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ae.huixiangedu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qz.jctech888.com.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nd.haigaiapp.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ff.szsharing.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vg.bookmarksfly.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vf.bookmarksfly.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://un.newstarts.cn

[B02] 多分支 else if / elif
来源：http://uo.shxzukj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://uj.hahajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lw.9csxet.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cp.panjiajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://of.hahajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ug.chemitech.net.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yp.lnxyls.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rz.huixiangedu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lq.521024.cn

[B03] switch / match / case
来源：http://wm.haigaiapp.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sl.szsharing.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uj.asd995.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jm.haigaiapp.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rs.muxihuayi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fx.jctech888.com.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hh.shxzskj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://px.wgjwhj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xt.521024.cn

[B04] for 计数循环
来源：http://fi.yuexingan06.cn

Py:   for i in range(10): print(i)
来源：http://eu.yuexingan06.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vg.huanxung.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sq.newstarts.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xs.jianghongdianzi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ps.bookmarksfly.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qu.bookmarksfly.cn

Ruby: 10.times { |i| puts i }
来源：http://nu.hahajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ur.shxzukj.cn

[B05] 遍历数组 / 列表
来源：http://wc.huanxung.cn

Py:   for item in arr: print(item)
来源：http://ay.nicolike.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://op.wgjwhj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://jb.jianghongdianzi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ze.shtwfgs.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://tp.nszjky.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gi.haigaiapp.cn

Ruby: arr.each { |item| puts item }
来源：http://zc.gzmigu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ps.haigaiapp.cn

[B06] 遍历字典 / 对象
来源：http://qj.shxzukj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://nv.jctech888.com.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ki.huanxung.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://im.lnxyls.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pu.muxihuayi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jk.asd995.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qb.lnxyls.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dy.nicolike.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://uf.shxzskj.cn

[B07] while 循环
来源：http://ub.bjjhwx.cn

Py:   while i < 10: i += 1
来源：http://di.hnjuh.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ev.shxzukj.cn

JS:   while (i < 10) { i++; }
来源：http://pp.hnjuh.cn

TS:   while (i < 10) { i++; }
来源：http://we.bookmarksfly.cn

Java: while (i < 10) { i++; }
来源：http://gy.bjjhwx.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fg.colortex.cn

Ruby: while i < 10; i += 1; end
来源：http://hq.9csxet.cn

C#:   while (i < 10) { i++; }
来源：http://tu.bookmarksfly.cn

[B08] do-while（至少执行一次）
来源：http://ph.asd995.cn

Py:   # 无 do-while：用 while True + break
来源：http://te.huanxung.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qe.521024.cn

JS:   do { i++; } while (i < 10);
来源：http://me.hahajie.cn

TS:   do { i++; } while (i < 10);
来源：http://gb.chemitech.net.cn

Java: do { i++; } while (i < 10);
来源：http://yu.jctech888.com.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ks.hnjuh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://gx.9csxet.cn

C#:   do { i++; } while (i < 10);
来源：http://ry.lnxyls.cn

[B09] break 与 continue
来源：http://rb.huixinmuqiang.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://he.521024.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jq.shtwfgs.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://te.shtwfgs.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ur.wgjwhj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uu.yuntaijiaju.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sy.nicolike.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nn.chemitech.net.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eh.shxzskj.cn

[B10] 遍历同时拿索引
来源：http://sp.huanxung.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lp.gzmigu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lg.9csxet.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zr.shxzskj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xg.panjiajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fj.nicolike.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qe.lnxyls.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ha.asd995.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ae.chemitech.net.cn

[B11] 生成数字序列 / 区间
来源：http://ar.asd995.cn

Py:   list(range(0, 10, 2))
来源：http://xa.shxzskj.cn

PHP:  range(0, 10, 2);
来源：http://zv.colortex.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ag.gzmigu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cl.huixiangedu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://id.lnxyls.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qs.nicolike.cn

Ruby: (0...10).step(2).to_a
来源：http://gw.panjiajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gf.521024.cn

[B12] 跳出多层循环
来源：http://gr.szxytkj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zt.nszjky.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wo.hahajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yk.jctech888.com.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mp.huanxung.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wn.szxytkj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hj.shtwfgs.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wa.chemitech.net.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kn.yuexingan06.cn

[B13] 判断是否为数字
来源：http://gx.muxihuayi.cn

Py:   isinstance(x, (int, float))
来源：http://hp.gzmigu.cn

PHP:  is_numeric($x)
来源：http://hf.bookmarksfly.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ci.yuntaijiaju.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qi.bjjhwx.cn

Java: x instanceof Number
来源：http://vs.shxzukj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lb.nszjky.cn

Ruby: x.is_a?(Numeric)
来源：http://vs.chemitech.net.cn

C#:   x is int or double or decimal
来源：http://qq.asd995.cn

[B14] 判断值是否在集合内
来源：http://at.szsharing.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fq.521024.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://va.asd995.cn

JS:   [1, 2, 3].includes(x)
来源：http://uh.hnjuh.cn

TS:   [1, 2, 3].includes(x)
来源：http://kb.huanxung.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://sc.haigaiapp.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gn.haigaiapp.cn

Ruby: [1, 2, 3].include?(x)
来源：http://nz.shtwfgs.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://np.panjiajie.cn

[B15] 布尔运算与取反
来源：http://rj.hahajie.cn

Py:   a and b or not c
来源：http://wu.521024.cn

PHP:  $a && $b || !$c
来源：http://ya.huixiangedu.cn

JS:   a && b || !c
来源：http://lz.colortex.cn

TS:   a && b || !c
来源：http://sd.shtwfgs.cn

Java: a && b || !c
来源：http://od.521024.cn

Go:   a && b || !c
来源：http://sk.huixinmuqiang.cn

Ruby: a && b || !c
来源：http://bf.asd995.cn

C#:   a && b || !c
来源：http://di.yuexingan06.cn

[B16] 卫语句：不满足条件提前返回
来源：http://kr.huanxung.cn

Py:   if not data: return
来源：http://mj.bookmarksfly.cn

PHP:  if (!$data) { return; }
来源：http://jh.bookmarksfly.cn

JS:   if (!data) return;
来源：http://kv.jctech888.com.cn

TS:   if (!data) return;
来源：http://wp.hnjuh.cn

Java: if (data == null) return;
来源：http://ph.szxytkj.cn

Go:   if data == nil { return }
来源：http://tm.huixinmuqiang.cn

Ruby: return if data.nil?
来源：http://ez.wgjwhj.cn

C#:   if (data == null) return;
来源：http://xe.colortex.cn

================================================================================
来源：http://tl.haigaiapp.cn

C. 函数与作用域
来源：http://lo.muxihuayi.cn

================================================================================
来源：http://ph.9csxet.cn

[C01] 定义函数
来源：http://ew.nszjky.cn

Py:   def add(a, b): return a + b
来源：http://iw.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://di.huanxung.cn

JS:   function add(a, b) { return a + b; }
来源：http://zx.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ar.bjjhwx.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lc.bookmarksfly.cn

Go:   func add(a, b int) int { return a + b }
来源：http://fc.newstarts.cn

Ruby: def add(a, b); a + b; end
来源：http://bx.bjjhwx.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://il.colortex.cn

[C02] 默认参数
来源：http://th.bookmarksfly.cn

Py:   def greet(name="World"): return name
来源：http://ch.lnxyls.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dz.shtwfgs.cn

JS:   function greet(name = "World") { return name; }
来源：http://at.wgjwhj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://eh.chemitech.net.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://xm.yuntaijiaju.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://uw.9csxet.cn

Ruby: def greet(name = "World") = name
来源：http://ct.shtwfgs.cn

C#:   string Greet(string name = "World") => name;
来源：http://mh.lnxyls.cn

[C03] 可变参数
来源：http://to.nicolike.cn

Py:   def total(*args): return sum(args)
来源：http://lg.haigaiapp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ve.shxzukj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bb.nszjky.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wc.szxytkj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://et.wgjwhj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lo.shxzukj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ji.jianghongdianzi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ri.bookmarksfly.cn

[C04] 命名参数 / 关键字参数
来源：http://ni.colortex.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zd.panjiajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qz.chemitech.net.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vi.lnxyls.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://db.huixinmuqiang.cn

Java: // 无：用 Builder 模式或 record
来源：http://ll.haigaiapp.cn

Go:   // 无：用配置结构体参数
来源：http://hg.szxytkj.cn

Ruby: f(a: 1, b: 2)
来源：http://ag.wgjwhj.cn

C#:   f(a: 1, b: 2)
来源：http://xi.hnjuh.cn

[C05] 返回多个值
来源：http://mt.yuntaijiaju.cn

Py:   return a, b
来源：http://xz.nicolike.cn

PHP:  return [$a, $b];
来源：http://wt.shtwfgs.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://md.bjjhwx.cn

TS:   return { a, b };
来源：http://tg.huanxung.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xv.shtwfgs.cn

Go:   return a, b
来源：http://ut.9csxet.cn

Ruby: return a, b
来源：http://sh.panjiajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://da.chemitech.net.cn

[C06] 匿名函数 / lambda
来源：http://tc.9csxet.cn

Py:   square = lambda x: x * x
来源：http://bx.bookmarksfly.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://za.chemitech.net.cn

JS:   const square = x => x * x;
来源：http://rw.wgjwhj.cn

TS:   const square = (x: number): number => x * x;
来源：http://wl.nicolike.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jh.panjiajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wr.colortex.cn

Ruby: square = ->(x) { x * x }
来源：http://ge.yuexingan06.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ki.wgjwhj.cn

[C07] 把函数作为参数传入
来源：http://xd.muxihuayi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xl.szsharing.cn

PHP:  array_map("strtoupper", $arr);
来源：http://oa.shxzskj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tv.521024.cn

TS:   arr.map(String)
来源：http://tn.shxzukj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hy.hahajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gx.chemitech.net.cn

Ruby: arr.map(&:upcase)
来源：http://gh.521024.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ut.huixiangedu.cn

[C08] 闭包
来源：http://pl.bookmarksfly.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tz.colortex.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lk.jianghongdianzi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vn.chemitech.net.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://as.9csxet.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hm.jianghongdianzi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ew.newstarts.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ik.shtwfgs.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://iq.panjiajie.cn

[C09] 递归
来源：http://jd.nicolike.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fd.jianghongdianzi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ra.wgjwhj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iz.newstarts.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yr.huixiangedu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mc.yuntaijiaju.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mo.yuexingan06.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nm.bookmarksfly.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rw.jianghongdianzi.cn

[C10] 变量作用域
来源：http://pi.asd995.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dl.yuexingan06.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://am.hnjuh.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wj.yuexingan06.cn

TS:   同 JS
来源：http://dd.nicolike.cn

Java: 方法内为块级作用域
来源：http://gt.haigaiapp.cn

Go:   花括号块级作用域
来源：http://hk.panjiajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mp.nszjky.cn

C#:   块级作用域
来源：http://na.panjiajie.cn

[C11] 模块导入与导出
来源：http://lp.nicolike.cn

Py:   from module import func
来源：http://hw.chemitech.net.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://eq.huixiangedu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kp.nicolike.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nd.panjiajie.cn

Java: import java.util.List;
来源：http://gi.nicolike.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://be.szsharing.cn

Ruby: require "json"; require_relative "./util"
来源：http://nn.huixiangedu.cn

C#:   using System.Text;
来源：http://nl.gzmigu.cn

[C12] 立即执行函数 IIFE
来源：http://in.9csxet.cn

Py:   (lambda: print("run"))()
来源：http://en.hahajie.cn

PHP:  (function () { echo "run"; })();
来源：http://fn.shxzskj.cn

JS:   (() => { console.log("run"); })();
来源：http://ca.huixiangedu.cn

TS:   (() => { console.log("run"); })();
来源：http://ss.muxihuayi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hr.bjjhwx.cn

Go:   func() { fmt.Println("run") }()
来源：http://dr.hnjuh.cn

Ruby: -> { puts "run" }.call
来源：http://tr.szxytkj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://iz.jianghongdianzi.cn

[C13] 类型声明 / 类型注解
来源：http://pi.huixinmuqiang.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jx.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yx.521024.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xj.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ye.colortex.cn

Java: int add(int a, int b) { return a + b; }
来源：http://kb.colortex.cn

Go:   func add(a, b int) int
来源：http://uk.szxytkj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://la.nszjky.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fx.muxihuayi.cn

[C14] 泛型函数
来源：http://wn.nszjky.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qb.bjjhwx.cn

PHP:  // 无泛型
来源：http://gl.521024.cn

JS:   // 无泛型
来源：http://ea.bjjhwx.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://oj.521024.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zg.asd995.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dm.bjjhwx.cn

Ruby: # 无泛型
来源：http://nu.szsharing.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lw.chemitech.net.cn

[C15] 解构 / 展开参数
来源：http://nj.huixinmuqiang.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://uv.muxihuayi.cn

PHP:  [$a, $b] = $pair;
来源：http://lf.haigaiapp.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tn.colortex.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://se.hnjuh.cn

Java: // 无解构
来源：http://tj.panjiajie.cn

Go:   // 无解构
来源：http://bi.bjjhwx.cn

Ruby: a, b = pair
来源：http://al.asd995.cn

C#:   var (a, b) = pair;
来源：http://jn.gzmigu.cn

[C16] 函数 / 方法重载
来源：http://ly.newstarts.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mi.shxzskj.cn

PHP:  // 无重载
来源：http://dk.hahajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ha.newstarts.cn

TS:   // 用联合类型或重载签名声明
来源：http://nn.panjiajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://yz.bookmarksfly.cn


<!-- 参考信息 -->