代发 wailian999

[B01] 条件判断 if / else
来源：http://ii.panjiajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ur.huixinmuqiang.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bk.yuntaijiaju.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dq.panjiajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kv.yuexingan06.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://mb.bookmarksfly.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nv.chemitech.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qe.521024.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xt.9csxet.cn

[B02] 多分支 else if / elif
来源：http://md.panjiajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://no.haigaiapp.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tn.szsharing.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pe.shtwfgs.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lb.gzmigu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://th.huanxung.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ao.haigaiapp.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pe.shtwfgs.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vy.gzmigu.cn

[B03] switch / match / case
来源：http://cu.wgjwhj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nn.huixiangedu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cp.panjiajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uz.521024.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yw.yuntaijiaju.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dz.yuexingan06.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yu.lnxyls.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qp.jianghongdianzi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://oc.hnjuh.cn

[B04] for 计数循环
来源：http://hb.hahajie.cn

Py:   for i in range(10): print(i)
来源：http://ou.huixiangedu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xq.nicolike.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gp.huanxung.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zg.shxzskj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://as.panjiajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hy.panjiajie.cn

Ruby: 10.times { |i| puts i }
来源：http://ba.shxzskj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://it.chemitech.net.cn

[B05] 遍历数组 / 列表
来源：http://el.newstarts.cn

Py:   for item in arr: print(item)
来源：http://kz.asd995.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://oq.muxihuayi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yq.nszjky.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://wj.nicolike.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://nz.jctech888.com.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://df.newstarts.cn

Ruby: arr.each { |item| puts item }
来源：http://bm.hnjuh.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vy.panjiajie.cn

[B06] 遍历字典 / 对象
来源：http://hd.shxzukj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xn.chemitech.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ad.nszjky.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lp.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ve.9csxet.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://am.colortex.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vh.yuexingan06.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xj.newstarts.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://du.szsharing.cn

[B07] while 循环
来源：http://be.shxzskj.cn

Py:   while i < 10: i += 1
来源：http://zk.lnxyls.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ew.yuexingan06.cn

JS:   while (i < 10) { i++; }
来源：http://hl.shxzskj.cn

TS:   while (i < 10) { i++; }
来源：http://oq.hnjuh.cn

Java: while (i < 10) { i++; }
来源：http://wl.panjiajie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gg.nicolike.cn

Ruby: while i < 10; i += 1; end
来源：http://yt.jianghongdianzi.cn

C#:   while (i < 10) { i++; }
来源：http://dv.bjjhwx.cn

[B08] do-while（至少执行一次）
来源：http://nj.chemitech.net.cn

Py:   # 无 do-while：用 while True + break
来源：http://ua.521024.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ok.bookmarksfly.cn

JS:   do { i++; } while (i < 10);
来源：http://wz.bjjhwx.cn

TS:   do { i++; } while (i < 10);
来源：http://ed.asd995.cn

Java: do { i++; } while (i < 10);
来源：http://vs.szxytkj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jw.huixinmuqiang.cn

Ruby: begin; i += 1; end while i < 10
来源：http://oe.nicolike.cn

C#:   do { i++; } while (i < 10);
来源：http://xx.shxzskj.cn

[B09] break 与 continue
来源：http://zj.yuexingan06.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lp.nszjky.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xc.9csxet.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ku.bookmarksfly.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tt.hnjuh.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://en.haigaiapp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://iq.hahajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nc.shxzskj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ge.bjjhwx.cn

[B10] 遍历同时拿索引
来源：http://rg.huanxung.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yj.bjjhwx.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vk.bjjhwx.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kj.gzmigu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://re.huixinmuqiang.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jm.wgjwhj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sc.asd995.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gj.wgjwhj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cv.bookmarksfly.cn

[B11] 生成数字序列 / 区间
来源：http://gh.wgjwhj.cn

Py:   list(range(0, 10, 2))
来源：http://xm.yuntaijiaju.cn

PHP:  range(0, 10, 2);
来源：http://rb.gzmigu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ij.nszjky.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://te.szxytkj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bv.nicolike.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://md.521024.cn

Ruby: (0...10).step(2).to_a
来源：http://bk.jctech888.com.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bq.haigaiapp.cn

[B12] 跳出多层循环
来源：http://rk.gzmigu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://uq.colortex.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://pc.hahajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ie.lnxyls.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mf.shtwfgs.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://oe.huixinmuqiang.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cm.gzmigu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xm.newstarts.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://et.521024.cn

[B13] 判断是否为数字
来源：http://zn.yuexingan06.cn

Py:   isinstance(x, (int, float))
来源：http://pw.521024.cn

PHP:  is_numeric($x)
来源：http://zq.lnxyls.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ws.gzmigu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://af.nszjky.cn

Java: x instanceof Number
来源：http://pt.521024.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kq.521024.cn

Ruby: x.is_a?(Numeric)
来源：http://bh.szsharing.cn

C#:   x is int or double or decimal
来源：http://is.9csxet.cn

[B14] 判断值是否在集合内
来源：http://np.asd995.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ch.shxzukj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ca.panjiajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://se.newstarts.cn

TS:   [1, 2, 3].includes(x)
来源：http://aa.panjiajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qu.jianghongdianzi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pe.panjiajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ot.newstarts.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://np.shtwfgs.cn

[B15] 布尔运算与取反
来源：http://ys.szsharing.cn

Py:   a and b or not c
来源：http://jl.hnjuh.cn

PHP:  $a && $b || !$c
来源：http://vw.bjjhwx.cn

JS:   a && b || !c
来源：http://uq.muxihuayi.cn

TS:   a && b || !c
来源：http://ft.bookmarksfly.cn

Java: a && b || !c
来源：http://lv.jianghongdianzi.cn

Go:   a && b || !c
来源：http://ho.huixiangedu.cn

Ruby: a && b || !c
来源：http://az.shtwfgs.cn

C#:   a && b || !c
来源：http://wy.muxihuayi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ix.lnxyls.cn

Py:   if not data: return
来源：http://bd.yuntaijiaju.cn

PHP:  if (!$data) { return; }
来源：http://mh.huixiangedu.cn

JS:   if (!data) return;
来源：http://zf.shtwfgs.cn

TS:   if (!data) return;
来源：http://ft.newstarts.cn

Java: if (data == null) return;
来源：http://hq.jianghongdianzi.cn

Go:   if data == nil { return }
来源：http://ml.huanxung.cn

Ruby: return if data.nil?
来源：http://gm.huixiangedu.cn

C#:   if (data == null) return;
来源：http://em.hahajie.cn

================================================================================
来源：http://ot.haigaiapp.cn

C. 函数与作用域
来源：http://ar.wgjwhj.cn

================================================================================
来源：http://yo.lnxyls.cn

[C01] 定义函数
来源：http://cz.nicolike.cn

Py:   def add(a, b): return a + b
来源：http://xl.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://re.nicolike.cn

JS:   function add(a, b) { return a + b; }
来源：http://oo.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yx.szsharing.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://tj.huixiangedu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://bi.shtwfgs.cn

Ruby: def add(a, b); a + b; end
来源：http://nq.wgjwhj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://il.shtwfgs.cn

[C02] 默认参数
来源：http://pf.bookmarksfly.cn

Py:   def greet(name="World"): return name
来源：http://dz.haigaiapp.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://pu.shtwfgs.cn

JS:   function greet(name = "World") { return name; }
来源：http://jx.shxzskj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://nb.huixinmuqiang.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qp.nicolike.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xx.muxihuayi.cn

Ruby: def greet(name = "World") = name
来源：http://ve.szxytkj.cn

C#:   string Greet(string name = "World") => name;
来源：http://oy.gzmigu.cn

[C03] 可变参数
来源：http://xm.wgjwhj.cn

Py:   def total(*args): return sum(args)
来源：http://ak.jianghongdianzi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cc.asd995.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://br.nszjky.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bz.szxytkj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://iv.jctech888.com.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lm.jianghongdianzi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://dq.nszjky.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ys.szsharing.cn

[C04] 命名参数 / 关键字参数
来源：http://bg.asd995.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://co.jctech888.com.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://an.521024.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://iu.nicolike.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hg.szsharing.cn

Java: // 无：用 Builder 模式或 record
来源：http://qs.wgjwhj.cn

Go:   // 无：用配置结构体参数
来源：http://ym.lnxyls.cn

Ruby: f(a: 1, b: 2)
来源：http://mv.nszjky.cn

C#:   f(a: 1, b: 2)
来源：http://kk.nszjky.cn

[C05] 返回多个值
来源：http://hp.yuntaijiaju.cn

Py:   return a, b
来源：http://xg.asd995.cn

PHP:  return [$a, $b];
来源：http://ye.huixinmuqiang.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://uw.newstarts.cn

TS:   return { a, b };
来源：http://sb.panjiajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ho.yuexingan06.cn

Go:   return a, b
来源：http://qu.huanxung.cn

Ruby: return a, b
来源：http://wa.bookmarksfly.cn

C#:   return (a, b);              // ValueTuple
来源：http://kx.newstarts.cn

[C06] 匿名函数 / lambda
来源：http://mh.nicolike.cn

Py:   square = lambda x: x * x
来源：http://up.haigaiapp.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ri.shxzukj.cn

JS:   const square = x => x * x;
来源：http://wo.hahajie.cn

TS:   const square = (x: number): number => x * x;
来源：http://kh.haigaiapp.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zo.jctech888.com.cn

Go:   sq := func(x int) int { return x * x }
来源：http://eo.wgjwhj.cn

Ruby: square = ->(x) { x * x }
来源：http://al.wgjwhj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xg.yuntaijiaju.cn

[C07] 把函数作为参数传入
来源：http://fh.bjjhwx.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://st.nicolike.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xh.huixiangedu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ty.wgjwhj.cn

TS:   arr.map(String)
来源：http://eg.yuexingan06.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xs.hnjuh.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ub.huixiangedu.cn

Ruby: arr.map(&:upcase)
来源：http://it.jianghongdianzi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cn.shtwfgs.cn

[C08] 闭包
来源：http://sm.shtwfgs.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qb.shtwfgs.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yr.hahajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qd.yuntaijiaju.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://aw.jctech888.com.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vd.521024.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nr.shxzukj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tr.nicolike.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://sz.jctech888.com.cn

[C09] 递归
来源：http://jl.bjjhwx.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ds.muxihuayi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dy.newstarts.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mm.nicolike.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yq.bjjhwx.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://up.chemitech.net.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xg.chemitech.net.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fm.shxzskj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dl.jctech888.com.cn

[C10] 变量作用域
来源：http://lb.huixinmuqiang.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dc.shxzukj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ko.lnxyls.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fx.hahajie.cn

TS:   同 JS
来源：http://sx.chemitech.net.cn

Java: 方法内为块级作用域
来源：http://ch.huixinmuqiang.cn

Go:   花括号块级作用域
来源：http://oj.muxihuayi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rv.yuntaijiaju.cn

C#:   块级作用域
来源：http://im.jianghongdianzi.cn

[C11] 模块导入与导出
来源：http://qq.colortex.cn

Py:   from module import func
来源：http://wz.asd995.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://gu.521024.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://az.bookmarksfly.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jq.gzmigu.cn

Java: import java.util.List;
来源：http://hf.shxzskj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xg.haigaiapp.cn

Ruby: require "json"; require_relative "./util"
来源：http://nj.newstarts.cn

C#:   using System.Text;
来源：http://dh.bookmarksfly.cn

[C12] 立即执行函数 IIFE
来源：http://yf.wgjwhj.cn

Py:   (lambda: print("run"))()
来源：http://mh.shxzskj.cn

PHP:  (function () { echo "run"; })();
来源：http://id.szsharing.cn

JS:   (() => { console.log("run"); })();
来源：http://rx.chemitech.net.cn

TS:   (() => { console.log("run"); })();
来源：http://dj.asd995.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ef.lnxyls.cn

Go:   func() { fmt.Println("run") }()
来源：http://od.yuexingan06.cn

Ruby: -> { puts "run" }.call
来源：http://ps.bjjhwx.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gs.yuexingan06.cn

[C13] 类型声明 / 类型注解
来源：http://fi.hahajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ej.shxzskj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ol.bookmarksfly.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://va.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kk.panjiajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ej.gzmigu.cn

Go:   func add(a, b int) int
来源：http://rs.lnxyls.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jx.hahajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tf.colortex.cn

[C14] 泛型函数
来源：http://gf.shxzukj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://no.bjjhwx.cn

PHP:  // 无泛型
来源：http://lj.nicolike.cn

JS:   // 无泛型
来源：http://dh.lnxyls.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qm.nszjky.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ra.nszjky.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qs.hnjuh.cn

Ruby: # 无泛型
来源：http://qb.nicolike.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ac.jianghongdianzi.cn

[C15] 解构 / 展开参数
来源：http://mi.chemitech.net.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qe.wgjwhj.cn

PHP:  [$a, $b] = $pair;
来源：http://gr.shxzskj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qq.panjiajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ll.newstarts.cn

Java: // 无解构
来源：http://ee.bookmarksfly.cn

Go:   // 无解构
来源：http://eh.521024.cn

Ruby: a, b = pair
来源：http://le.newstarts.cn

C#:   var (a, b) = pair;
来源：http://ho.bjjhwx.cn

[C16] 函数 / 方法重载
来源：http://ei.hnjuh.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gl.szxytkj.cn

PHP:  // 无重载
来源：http://et.jianghongdianzi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://pp.asd995.cn

TS:   // 用联合类型或重载签名声明
来源：http://lc.9csxet.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ee.bookmarksfly.cn

Go:   // 无重载：用不同函数名
来源：http://sl.szxytkj.cn

Ruby: # 无重载：靠动态参数
来源：http://fe.szxytkj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://pu.asd995.cn

================================================================================
来源：http://jr.szxytkj.cn

D. 数组 / 列表 / 集合
来源：http://ut.szxytkj.cn

================================================================================
来源：http://yu.shxzskj.cn

[D01] 创建数组 / 列表
来源：http://qj.yuntaijiaju.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rg.jianghongdianzi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zu.521024.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://st.asd995.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dm.hnjuh.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fo.jctech888.com.cn


<!-- 参考信息 -->