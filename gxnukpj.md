代发 wailian999

[B01] 条件判断 if / else
来源：http://lu.newstarts.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://se.shtwfgs.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://es.jctech888.com.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fv.szsharing.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://iz.panjiajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://oz.521024.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ve.jctech888.com.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://eb.newstarts.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pa.shtwfgs.cn

[B02] 多分支 else if / elif
来源：http://rf.bjjhwx.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://aj.panjiajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fk.huanxung.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://or.huixiangedu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qv.hnjuh.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qc.bjjhwx.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ek.chemitech.net.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nt.haigaiapp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mg.hahajie.cn

[B03] switch / match / case
来源：http://ht.shxzukj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yz.lnxyls.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bu.hahajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dj.huixinmuqiang.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lb.yuexingan06.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ln.yuntaijiaju.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xg.wgjwhj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lc.shxzskj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qh.szxytkj.cn

[B04] for 计数循环
来源：http://wa.muxihuayi.cn

Py:   for i in range(10): print(i)
来源：http://pc.bookmarksfly.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://uw.shxzukj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yf.hahajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zl.hahajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rw.asd995.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xc.huixiangedu.cn

Ruby: 10.times { |i| puts i }
来源：http://ph.521024.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dv.colortex.cn

[B05] 遍历数组 / 列表
来源：http://ey.szxytkj.cn

Py:   for item in arr: print(item)
来源：http://sp.9csxet.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mo.huixinmuqiang.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://nz.newstarts.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://jm.yuntaijiaju.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://rh.szxytkj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://oe.colortex.cn

Ruby: arr.each { |item| puts item }
来源：http://ev.9csxet.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xe.haigaiapp.cn

[B06] 遍历字典 / 对象
来源：http://rp.hahajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://og.yuexingan06.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bl.shxzukj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ox.muxihuayi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://co.gzmigu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xs.hnjuh.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sn.huixiangedu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rs.huixinmuqiang.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tv.jianghongdianzi.cn

[B07] while 循环
来源：http://ao.huixiangedu.cn

Py:   while i < 10: i += 1
来源：http://sb.bookmarksfly.cn

PHP:  while ($i < 10) { $i++; }
来源：http://cb.nszjky.cn

JS:   while (i < 10) { i++; }
来源：http://vm.bjjhwx.cn

TS:   while (i < 10) { i++; }
来源：http://kq.colortex.cn

Java: while (i < 10) { i++; }
来源：http://gb.521024.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rh.gzmigu.cn

Ruby: while i < 10; i += 1; end
来源：http://sz.bjjhwx.cn

C#:   while (i < 10) { i++; }
来源：http://pv.wgjwhj.cn

[B08] do-while（至少执行一次）
来源：http://gd.yuexingan06.cn

Py:   # 无 do-while：用 while True + break
来源：http://uq.bookmarksfly.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://wb.bookmarksfly.cn

JS:   do { i++; } while (i < 10);
来源：http://xb.521024.cn

TS:   do { i++; } while (i < 10);
来源：http://tw.huixinmuqiang.cn

Java: do { i++; } while (i < 10);
来源：http://yw.nszjky.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://nk.521024.cn

Ruby: begin; i += 1; end while i < 10
来源：http://yo.hahajie.cn

C#:   do { i++; } while (i < 10);
来源：http://le.hahajie.cn

[B09] break 与 continue
来源：http://rz.haigaiapp.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yu.panjiajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://if.szsharing.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ki.wgjwhj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://he.huixinmuqiang.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rq.huixinmuqiang.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jx.chemitech.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ij.shxzukj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ps.newstarts.cn

[B10] 遍历同时拿索引
来源：http://zd.wgjwhj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://av.yuexingan06.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://de.huanxung.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wn.yuntaijiaju.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ik.szsharing.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://iz.lnxyls.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sw.jianghongdianzi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fu.asd995.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://me.huanxung.cn

[B11] 生成数字序列 / 区间
来源：http://nx.panjiajie.cn

Py:   list(range(0, 10, 2))
来源：http://sc.huanxung.cn

PHP:  range(0, 10, 2);
来源：http://xo.colortex.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ma.asd995.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xr.szxytkj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qk.haigaiapp.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ld.huixiangedu.cn

Ruby: (0...10).step(2).to_a
来源：http://kj.bjjhwx.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fx.szxytkj.cn

[B12] 跳出多层循环
来源：http://hz.colortex.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ck.jctech888.com.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hn.shxzskj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xv.jianghongdianzi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vh.jctech888.com.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://oe.shxzskj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yh.szsharing.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zf.bjjhwx.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dd.hnjuh.cn

[B13] 判断是否为数字
来源：http://xt.nszjky.cn

Py:   isinstance(x, (int, float))
来源：http://wi.shtwfgs.cn

PHP:  is_numeric($x)
来源：http://wu.shxzukj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xr.colortex.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xx.szsharing.cn

Java: x instanceof Number
来源：http://ho.newstarts.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dp.asd995.cn

Ruby: x.is_a?(Numeric)
来源：http://lv.panjiajie.cn

C#:   x is int or double or decimal
来源：http://ka.yuexingan06.cn

[B14] 判断值是否在集合内
来源：http://bv.asd995.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cu.szxytkj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://up.nicolike.cn

JS:   [1, 2, 3].includes(x)
来源：http://mk.newstarts.cn

TS:   [1, 2, 3].includes(x)
来源：http://mk.asd995.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ha.gzmigu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fl.colortex.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cb.nicolike.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dy.asd995.cn

[B15] 布尔运算与取反
来源：http://ad.hahajie.cn

Py:   a and b or not c
来源：http://lp.nszjky.cn

PHP:  $a && $b || !$c
来源：http://go.haigaiapp.cn

JS:   a && b || !c
来源：http://le.bookmarksfly.cn

TS:   a && b || !c
来源：http://xt.jianghongdianzi.cn

Java: a && b || !c
来源：http://yp.asd995.cn

Go:   a && b || !c
来源：http://xl.newstarts.cn

Ruby: a && b || !c
来源：http://jk.jctech888.com.cn

C#:   a && b || !c
来源：http://jm.colortex.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lm.bookmarksfly.cn

Py:   if not data: return
来源：http://gp.chemitech.net.cn

PHP:  if (!$data) { return; }
来源：http://km.9csxet.cn

JS:   if (!data) return;
来源：http://uy.shtwfgs.cn

TS:   if (!data) return;
来源：http://md.shtwfgs.cn

Java: if (data == null) return;
来源：http://ma.shtwfgs.cn

Go:   if data == nil { return }
来源：http://pd.hnjuh.cn

Ruby: return if data.nil?
来源：http://jp.yuexingan06.cn

C#:   if (data == null) return;
来源：http://dp.lnxyls.cn

================================================================================
来源：http://sd.hnjuh.cn

C. 函数与作用域
来源：http://ah.haigaiapp.cn

================================================================================
来源：http://uk.521024.cn

[C01] 定义函数
来源：http://cl.szxytkj.cn

Py:   def add(a, b): return a + b
来源：http://lg.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jj.shtwfgs.cn

JS:   function add(a, b) { return a + b; }
来源：http://hn.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://za.yuexingan06.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dk.gzmigu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://uw.szxytkj.cn

Ruby: def add(a, b); a + b; end
来源：http://fe.bookmarksfly.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://op.521024.cn

[C02] 默认参数
来源：http://ee.chemitech.net.cn

Py:   def greet(name="World"): return name
来源：http://yz.521024.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yr.9csxet.cn

JS:   function greet(name = "World") { return name; }
来源：http://wf.9csxet.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cl.lnxyls.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://if.haigaiapp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ks.nszjky.cn

Ruby: def greet(name = "World") = name
来源：http://pt.szxytkj.cn

C#:   string Greet(string name = "World") => name;
来源：http://sp.hnjuh.cn

[C03] 可变参数
来源：http://ab.szxytkj.cn

Py:   def total(*args): return sum(args)
来源：http://gr.521024.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jh.yuexingan06.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sz.colortex.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yq.shxzskj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nn.colortex.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://iy.huixinmuqiang.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xg.bjjhwx.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://es.chemitech.net.cn

[C04] 命名参数 / 关键字参数
来源：http://uz.shxzukj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fq.jianghongdianzi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ai.shxzukj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jt.jctech888.com.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kp.wgjwhj.cn

Java: // 无：用 Builder 模式或 record
来源：http://gq.colortex.cn

Go:   // 无：用配置结构体参数
来源：http://ek.521024.cn

Ruby: f(a: 1, b: 2)
来源：http://us.chemitech.net.cn

C#:   f(a: 1, b: 2)
来源：http://mr.szxytkj.cn

[C05] 返回多个值
来源：http://wn.panjiajie.cn

Py:   return a, b
来源：http://tg.shxzskj.cn

PHP:  return [$a, $b];
来源：http://bf.hnjuh.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ei.panjiajie.cn

TS:   return { a, b };
来源：http://me.szsharing.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lu.huixiangedu.cn

Go:   return a, b
来源：http://jz.huixinmuqiang.cn

Ruby: return a, b
来源：http://ao.521024.cn

C#:   return (a, b);              // ValueTuple
来源：http://wj.huixinmuqiang.cn

[C06] 匿名函数 / lambda
来源：http://xz.hnjuh.cn

Py:   square = lambda x: x * x
来源：http://nk.yuntaijiaju.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://hw.huixinmuqiang.cn

JS:   const square = x => x * x;
来源：http://le.nszjky.cn

TS:   const square = (x: number): number => x * x;
来源：http://zy.jctech888.com.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://no.nicolike.cn

Go:   sq := func(x int) int { return x * x }
来源：http://cg.yuntaijiaju.cn

Ruby: square = ->(x) { x * x }
来源：http://nu.colortex.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ee.hnjuh.cn

[C07] 把函数作为参数传入
来源：http://nq.9csxet.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ut.huixinmuqiang.cn

PHP:  array_map("strtoupper", $arr);
来源：http://dc.newstarts.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lu.521024.cn

TS:   arr.map(String)
来源：http://hp.lnxyls.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://le.haigaiapp.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xp.jianghongdianzi.cn

Ruby: arr.map(&:upcase)
来源：http://kk.panjiajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wa.nicolike.cn

[C08] 闭包
来源：http://ug.yuexingan06.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ez.gzmigu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://oz.yuntaijiaju.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vz.szsharing.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://we.haigaiapp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ug.asd995.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lq.szxytkj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cm.nszjky.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://id.521024.cn

[C09] 递归
来源：http://qa.chemitech.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ff.521024.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gr.jctech888.com.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pc.hnjuh.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aj.shxzskj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pf.muxihuayi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cn.asd995.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bm.wgjwhj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mt.jctech888.com.cn

[C10] 变量作用域
来源：http://uv.9csxet.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ff.huanxung.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mb.bjjhwx.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://il.hahajie.cn

TS:   同 JS
来源：http://xv.shxzskj.cn

Java: 方法内为块级作用域
来源：http://bi.huixinmuqiang.cn

Go:   花括号块级作用域
来源：http://sv.colortex.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sd.haigaiapp.cn

C#:   块级作用域
来源：http://zx.bookmarksfly.cn

[C11] 模块导入与导出
来源：http://mf.bjjhwx.cn

Py:   from module import func
来源：http://yh.nszjky.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mg.asd995.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jl.hnjuh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yh.yuexingan06.cn

Java: import java.util.List;
来源：http://zh.hnjuh.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tl.panjiajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://lm.nszjky.cn

C#:   using System.Text;
来源：http://cc.bookmarksfly.cn

[C12] 立即执行函数 IIFE
来源：http://wj.hahajie.cn

Py:   (lambda: print("run"))()
来源：http://cj.hahajie.cn

PHP:  (function () { echo "run"; })();
来源：http://dm.huixinmuqiang.cn

JS:   (() => { console.log("run"); })();
来源：http://ai.huanxung.cn

TS:   (() => { console.log("run"); })();
来源：http://ss.szxytkj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hm.bookmarksfly.cn

Go:   func() { fmt.Println("run") }()
来源：http://rm.huixinmuqiang.cn

Ruby: -> { puts "run" }.call
来源：http://qm.jianghongdianzi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://oy.wgjwhj.cn

[C13] 类型声明 / 类型注解
来源：http://il.muxihuayi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://be.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vc.gzmigu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lk.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fk.shxzskj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://yz.muxihuayi.cn

Go:   func add(a, b int) int
来源：http://mz.bjjhwx.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bm.hnjuh.cn

C#:   int Add(int a, int b) => a + b;
来源：http://hf.huixiangedu.cn

[C14] 泛型函数
来源：http://im.shxzskj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kb.shtwfgs.cn

PHP:  // 无泛型
来源：http://ck.yuexingan06.cn

JS:   // 无泛型
来源：http://qh.colortex.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hw.shtwfgs.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hk.521024.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lm.gzmigu.cn

Ruby: # 无泛型
来源：http://gp.lnxyls.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xl.shtwfgs.cn

[C15] 解构 / 展开参数
来源：http://xh.szsharing.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ev.huixinmuqiang.cn

PHP:  [$a, $b] = $pair;
来源：http://ru.lnxyls.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vc.jianghongdianzi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ri.jctech888.com.cn

Java: // 无解构
来源：http://mt.huixinmuqiang.cn

Go:   // 无解构
来源：http://mw.szxytkj.cn

Ruby: a, b = pair
来源：http://dt.jianghongdianzi.cn

C#:   var (a, b) = pair;
来源：http://md.colortex.cn

[C16] 函数 / 方法重载
来源：http://gx.gzmigu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://co.muxihuayi.cn

PHP:  // 无重载
来源：http://lr.yuexingan06.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://am.muxihuayi.cn

TS:   // 用联合类型或重载签名声明
来源：http://la.nszjky.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://vg.shxzukj.cn

Go:   // 无重载：用不同函数名
来源：http://pm.wgjwhj.cn

Ruby: # 无重载：靠动态参数
来源：http://es.panjiajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qz.521024.cn

================================================================================
来源：http://ux.shtwfgs.cn

D. 数组 / 列表 / 集合
来源：http://rd.521024.cn

================================================================================
来源：http://cy.hahajie.cn

[D01] 创建数组 / 列表
来源：http://hd.shtwfgs.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ld.panjiajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vd.yuexingan06.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sw.szsharing.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ir.szxytkj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gs.huanxung.cn


<!-- 参考信息 -->