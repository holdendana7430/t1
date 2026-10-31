代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uf.newstarts.cn

================================================================================
来源：http://th.szxytkj.cn

B. 流程控制
来源：http://xv.colortex.cn

================================================================================
来源：http://jm.gzmigu.cn

[B01] 条件判断 if / else
来源：http://jc.jctech888.com.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://oj.jianghongdianzi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jx.haigaiapp.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pt.9csxet.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fh.huixinmuqiang.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xb.bookmarksfly.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hp.szxytkj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lj.jianghongdianzi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nu.shxzskj.cn

[B02] 多分支 else if / elif
来源：http://po.huanxung.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xk.521024.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://md.yuexingan06.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qp.wgjwhj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vd.huixinmuqiang.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xd.szxytkj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dh.shxzskj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fk.bookmarksfly.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ie.huanxung.cn

[B03] switch / match / case
来源：http://fp.colortex.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://so.szxytkj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hf.asd995.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lm.hahajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kl.hnjuh.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ad.yuntaijiaju.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vf.huanxung.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rd.chemitech.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yg.hnjuh.cn

[B04] for 计数循环
来源：http://jq.521024.cn

Py:   for i in range(10): print(i)
来源：http://nq.yuexingan06.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kh.szxytkj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lq.nicolike.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vw.jctech888.com.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pd.yuexingan06.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ah.nicolike.cn

Ruby: 10.times { |i| puts i }
来源：http://mu.szxytkj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cb.lnxyls.cn

[B05] 遍历数组 / 列表
来源：http://hu.yuexingan06.cn

Py:   for item in arr: print(item)
来源：http://ld.shxzukj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pd.muxihuayi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://eo.nicolike.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ij.9csxet.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xn.521024.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ws.521024.cn

Ruby: arr.each { |item| puts item }
来源：http://pm.yuntaijiaju.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zu.hnjuh.cn

[B06] 遍历字典 / 对象
来源：http://sg.newstarts.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://rz.shtwfgs.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jx.szxytkj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ri.shtwfgs.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kr.nicolike.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rs.huixiangedu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://te.jctech888.com.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ig.bookmarksfly.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://na.colortex.cn

[B07] while 循环
来源：http://qn.nszjky.cn

Py:   while i < 10: i += 1
来源：http://qa.panjiajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bi.haigaiapp.cn

JS:   while (i < 10) { i++; }
来源：http://fn.gzmigu.cn

TS:   while (i < 10) { i++; }
来源：http://ur.shtwfgs.cn

Java: while (i < 10) { i++; }
来源：http://oj.bjjhwx.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yi.jianghongdianzi.cn

Ruby: while i < 10; i += 1; end
来源：http://zx.szxytkj.cn

C#:   while (i < 10) { i++; }
来源：http://rj.521024.cn

[B08] do-while（至少执行一次）
来源：http://rj.huanxung.cn

Py:   # 无 do-while：用 while True + break
来源：http://qw.shxzskj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mz.haigaiapp.cn

JS:   do { i++; } while (i < 10);
来源：http://kl.haigaiapp.cn

TS:   do { i++; } while (i < 10);
来源：http://kn.nicolike.cn

Java: do { i++; } while (i < 10);
来源：http://kh.jianghongdianzi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://cq.szsharing.cn

Ruby: begin; i += 1; end while i < 10
来源：http://lk.asd995.cn

C#:   do { i++; } while (i < 10);
来源：http://by.huixiangedu.cn

[B09] break 与 continue
来源：http://mu.9csxet.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zl.panjiajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vf.hahajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bh.muxihuayi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://he.hahajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vh.huixiangedu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tu.nszjky.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nr.asd995.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aq.shxzskj.cn

[B10] 遍历同时拿索引
来源：http://op.szxytkj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wo.gzmigu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gp.hahajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xr.hahajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pl.chemitech.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qy.huixinmuqiang.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ng.nicolike.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lr.newstarts.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bb.9csxet.cn

[B11] 生成数字序列 / 区间
来源：http://yw.bookmarksfly.cn

Py:   list(range(0, 10, 2))
来源：http://pb.hnjuh.cn

PHP:  range(0, 10, 2);
来源：http://hi.jctech888.com.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hf.yuexingan06.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wv.colortex.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://oi.shxzskj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ox.szxytkj.cn

Ruby: (0...10).step(2).to_a
来源：http://ca.hnjuh.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://th.shtwfgs.cn

[B12] 跳出多层循环
来源：http://ty.panjiajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://rf.nszjky.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hn.shxzskj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://eu.wgjwhj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fu.nicolike.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pg.521024.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mc.shxzukj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hw.yuexingan06.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ph.9csxet.cn

[B13] 判断是否为数字
来源：http://eo.wgjwhj.cn

Py:   isinstance(x, (int, float))
来源：http://zr.huixinmuqiang.cn

PHP:  is_numeric($x)
来源：http://rt.bjjhwx.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oi.huixinmuqiang.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lm.yuntaijiaju.cn

Java: x instanceof Number
来源：http://zr.hahajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sy.colortex.cn

Ruby: x.is_a?(Numeric)
来源：http://iz.huanxung.cn

C#:   x is int or double or decimal
来源：http://qb.muxihuayi.cn

[B14] 判断值是否在集合内
来源：http://kz.muxihuayi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tj.szsharing.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nm.hahajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://gb.nszjky.cn

TS:   [1, 2, 3].includes(x)
来源：http://hu.yuntaijiaju.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://or.panjiajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://uv.colortex.cn

Ruby: [1, 2, 3].include?(x)
来源：http://wb.szxytkj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ar.hahajie.cn

[B15] 布尔运算与取反
来源：http://jq.hahajie.cn

Py:   a and b or not c
来源：http://zt.panjiajie.cn

PHP:  $a && $b || !$c
来源：http://pg.bookmarksfly.cn

JS:   a && b || !c
来源：http://az.jianghongdianzi.cn

TS:   a && b || !c
来源：http://ra.haigaiapp.cn

Java: a && b || !c
来源：http://ao.hahajie.cn

Go:   a && b || !c
来源：http://gr.hnjuh.cn

Ruby: a && b || !c
来源：http://ux.hahajie.cn

C#:   a && b || !c
来源：http://nk.yuntaijiaju.cn

[B16] 卫语句：不满足条件提前返回
来源：http://rx.szsharing.cn

Py:   if not data: return
来源：http://ll.shxzskj.cn

PHP:  if (!$data) { return; }
来源：http://rh.bookmarksfly.cn

JS:   if (!data) return;
来源：http://ry.bjjhwx.cn

TS:   if (!data) return;
来源：http://kj.huixiangedu.cn

Java: if (data == null) return;
来源：http://po.asd995.cn

Go:   if data == nil { return }
来源：http://jt.asd995.cn

Ruby: return if data.nil?
来源：http://ay.gzmigu.cn

C#:   if (data == null) return;
来源：http://fi.shxzukj.cn

================================================================================
来源：http://bk.lnxyls.cn

C. 函数与作用域
来源：http://fg.521024.cn

================================================================================
来源：http://oz.haigaiapp.cn

[C01] 定义函数
来源：http://yj.yuexingan06.cn

Py:   def add(a, b): return a + b
来源：http://pl.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cq.bjjhwx.cn

JS:   function add(a, b) { return a + b; }
来源：http://qc.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fr.jianghongdianzi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mp.chemitech.net.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vk.wgjwhj.cn

Ruby: def add(a, b); a + b; end
来源：http://yx.szsharing.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fk.jctech888.com.cn

[C02] 默认参数
来源：http://bo.nszjky.cn

Py:   def greet(name="World"): return name
来源：http://yp.bjjhwx.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qd.szxytkj.cn

JS:   function greet(name = "World") { return name; }
来源：http://tc.521024.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rk.hahajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vw.shxzukj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://og.bookmarksfly.cn

Ruby: def greet(name = "World") = name
来源：http://rs.chemitech.net.cn

C#:   string Greet(string name = "World") => name;
来源：http://te.wgjwhj.cn

[C03] 可变参数
来源：http://ad.huanxung.cn

Py:   def total(*args): return sum(args)
来源：http://fd.shxzukj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://km.colortex.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xm.asd995.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://on.9csxet.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://eh.huixiangedu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zk.gzmigu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://np.asd995.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ye.9csxet.cn

[C04] 命名参数 / 关键字参数
来源：http://pc.bjjhwx.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nq.jianghongdianzi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wt.colortex.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sl.szxytkj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ab.huixinmuqiang.cn

Java: // 无：用 Builder 模式或 record
来源：http://od.lnxyls.cn

Go:   // 无：用配置结构体参数
来源：http://mw.szxytkj.cn

Ruby: f(a: 1, b: 2)
来源：http://gb.nszjky.cn

C#:   f(a: 1, b: 2)
来源：http://vg.szxytkj.cn

[C05] 返回多个值
来源：http://gj.yuntaijiaju.cn

Py:   return a, b
来源：http://an.hahajie.cn

PHP:  return [$a, $b];
来源：http://wb.hahajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zt.muxihuayi.cn

TS:   return { a, b };
来源：http://fd.gzmigu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nc.huixinmuqiang.cn

Go:   return a, b
来源：http://ko.chemitech.net.cn

Ruby: return a, b
来源：http://sv.asd995.cn

C#:   return (a, b);              // ValueTuple
来源：http://ik.newstarts.cn

[C06] 匿名函数 / lambda
来源：http://bk.gzmigu.cn

Py:   square = lambda x: x * x
来源：http://hr.wgjwhj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://uo.newstarts.cn

JS:   const square = x => x * x;
来源：http://id.newstarts.cn

TS:   const square = (x: number): number => x * x;
来源：http://nz.panjiajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ng.shxzskj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jc.wgjwhj.cn

Ruby: square = ->(x) { x * x }
来源：http://bb.wgjwhj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qd.lnxyls.cn

[C07] 把函数作为参数传入
来源：http://kt.szsharing.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pi.huixiangedu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hh.yuexingan06.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vu.bookmarksfly.cn

TS:   arr.map(String)
来源：http://du.gzmigu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qj.jianghongdianzi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zs.yuexingan06.cn

Ruby: arr.map(&:upcase)
来源：http://tt.9csxet.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qz.szxytkj.cn

[C08] 闭包
来源：http://ud.chemitech.net.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nl.wgjwhj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hg.hahajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rk.hahajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yz.lnxyls.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://oa.shtwfgs.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cw.huanxung.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fa.szxytkj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dc.gzmigu.cn

[C09] 递归
来源：http://nf.521024.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cv.shxzskj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wi.9csxet.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zx.panjiajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cl.wgjwhj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gc.nszjky.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ec.newstarts.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pm.bookmarksfly.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ui.chemitech.net.cn

[C10] 变量作用域
来源：http://hk.bookmarksfly.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gf.jianghongdianzi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lr.huixiangedu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ja.9csxet.cn

TS:   同 JS
来源：http://lc.nszjky.cn

Java: 方法内为块级作用域
来源：http://qv.jianghongdianzi.cn

Go:   花括号块级作用域
来源：http://rp.jianghongdianzi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jh.asd995.cn

C#:   块级作用域
来源：http://aa.9csxet.cn

[C11] 模块导入与导出
来源：http://hl.nszjky.cn

Py:   from module import func
来源：http://dj.bookmarksfly.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://jx.shtwfgs.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://cx.wgjwhj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vs.jctech888.com.cn

Java: import java.util.List;
来源：http://hc.bjjhwx.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zz.9csxet.cn

Ruby: require "json"; require_relative "./util"
来源：http://fo.hnjuh.cn

C#:   using System.Text;
来源：http://ne.hnjuh.cn

[C12] 立即执行函数 IIFE
来源：http://ex.chemitech.net.cn

Py:   (lambda: print("run"))()
来源：http://gz.nicolike.cn

PHP:  (function () { echo "run"; })();
来源：http://al.nicolike.cn

JS:   (() => { console.log("run"); })();
来源：http://lr.yuntaijiaju.cn

TS:   (() => { console.log("run"); })();
来源：http://gk.haigaiapp.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kz.bjjhwx.cn

Go:   func() { fmt.Println("run") }()
来源：http://tq.lnxyls.cn

Ruby: -> { puts "run" }.call
来源：http://hw.bjjhwx.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://op.hnjuh.cn

[C13] 类型声明 / 类型注解
来源：http://ca.asd995.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ao.muxihuayi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hk.jianghongdianzi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mj.yuexingan06.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://aw.muxihuayi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ai.huixinmuqiang.cn

Go:   func add(a, b int) int
来源：http://ik.newstarts.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ib.521024.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nh.shxzskj.cn

[C14] 泛型函数
来源：http://zv.panjiajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fq.huixinmuqiang.cn

PHP:  // 无泛型
来源：http://ad.panjiajie.cn

JS:   // 无泛型
来源：http://ol.colortex.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ph.muxihuayi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xv.yuexingan06.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://iv.9csxet.cn

Ruby: # 无泛型
来源：http://lb.jianghongdianzi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fo.jianghongdianzi.cn

[C15] 解构 / 展开参数
来源：http://wz.panjiajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bj.asd995.cn

PHP:  [$a, $b] = $pair;
来源：http://ni.colortex.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nf.asd995.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cj.panjiajie.cn

Java: // 无解构
来源：http://lq.huanxung.cn

Go:   // 无解构
来源：http://iz.nszjky.cn

Ruby: a, b = pair
来源：http://br.wgjwhj.cn

C#:   var (a, b) = pair;
来源：http://mj.lnxyls.cn

[C16] 函数 / 方法重载
来源：http://ij.wgjwhj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ba.9csxet.cn

PHP:  // 无重载
来源：http://in.nszjky.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://dn.huanxung.cn

TS:   // 用联合类型或重载签名声明
来源：http://ls.huanxung.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qa.shxzskj.cn

Go:   // 无重载：用不同函数名
来源：http://ep.newstarts.cn

Ruby: # 无重载：靠动态参数
来源：http://vm.wgjwhj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gr.newstarts.cn

================================================================================
来源：http://pj.asd995.cn

D. 数组 / 列表 / 集合
来源：http://ex.nicolike.cn

================================================================================
来源：http://ol.wgjwhj.cn

[D01] 创建数组 / 列表
来源：http://vi.wgjwhj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://uw.gzmigu.cn


<!-- 参考信息 -->