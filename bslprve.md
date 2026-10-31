代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lh.yuexingan06.cn

================================================================================
来源：http://fx.huixinmuqiang.cn

B. 流程控制
来源：http://ml.jctech888.com.cn

================================================================================
来源：http://sy.chemitech.net.cn

[B01] 条件判断 if / else
来源：http://dq.szxytkj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hx.huixiangedu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://eg.bookmarksfly.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://be.bookmarksfly.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ez.szxytkj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://va.yuntaijiaju.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qn.szxytkj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ax.bookmarksfly.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://db.huixiangedu.cn

[B02] 多分支 else if / elif
来源：http://em.newstarts.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://db.gzmigu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rq.wgjwhj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oz.bjjhwx.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ob.shxzukj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tv.lnxyls.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://iz.chemitech.net.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jp.shxzukj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xh.asd995.cn

[B03] switch / match / case
来源：http://fy.asd995.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nm.yuntaijiaju.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ik.huixiangedu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jc.jctech888.com.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ur.panjiajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kj.colortex.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qn.huixinmuqiang.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sl.shxzskj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pc.wgjwhj.cn

[B04] for 计数循环
来源：http://dp.chemitech.net.cn

Py:   for i in range(10): print(i)
来源：http://yu.9csxet.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wa.colortex.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://md.shxzskj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://by.huixiangedu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ef.newstarts.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jn.521024.cn

Ruby: 10.times { |i| puts i }
来源：http://er.shxzskj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sf.nicolike.cn

[B05] 遍历数组 / 列表
来源：http://ge.bjjhwx.cn

Py:   for item in arr: print(item)
来源：http://vi.shxzukj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pm.hnjuh.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://cz.bjjhwx.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://sg.bjjhwx.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zz.asd995.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ip.nszjky.cn

Ruby: arr.each { |item| puts item }
来源：http://cn.szxytkj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jn.yuntaijiaju.cn

[B06] 遍历字典 / 对象
来源：http://wy.bookmarksfly.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://lt.panjiajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kr.bjjhwx.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ot.huanxung.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wv.nszjky.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wc.hahajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vp.chemitech.net.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sz.newstarts.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mf.newstarts.cn

[B07] while 循环
来源：http://yi.521024.cn

Py:   while i < 10: i += 1
来源：http://gc.wgjwhj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ph.chemitech.net.cn

JS:   while (i < 10) { i++; }
来源：http://hy.huixiangedu.cn

TS:   while (i < 10) { i++; }
来源：http://jr.szsharing.cn

Java: while (i < 10) { i++; }
来源：http://sk.huanxung.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zd.haigaiapp.cn

Ruby: while i < 10; i += 1; end
来源：http://wn.szxytkj.cn

C#:   while (i < 10) { i++; }
来源：http://uh.shxzukj.cn

[B08] do-while（至少执行一次）
来源：http://at.bookmarksfly.cn

Py:   # 无 do-while：用 while True + break
来源：http://de.panjiajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pa.jctech888.com.cn

JS:   do { i++; } while (i < 10);
来源：http://va.colortex.cn

TS:   do { i++; } while (i < 10);
来源：http://ol.hnjuh.cn

Java: do { i++; } while (i < 10);
来源：http://mw.yuntaijiaju.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://uv.muxihuayi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://sp.muxihuayi.cn

C#:   do { i++; } while (i < 10);
来源：http://wb.9csxet.cn

[B09] break 与 continue
来源：http://kd.colortex.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zi.huixiangedu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mg.bookmarksfly.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gk.shtwfgs.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tu.huixinmuqiang.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dx.jianghongdianzi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yi.huixiangedu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xy.nszjky.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ph.hahajie.cn

[B10] 遍历同时拿索引
来源：http://yv.hahajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mx.hahajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ru.wgjwhj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fb.521024.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bm.shtwfgs.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wf.hnjuh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pa.gzmigu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fn.panjiajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rr.bookmarksfly.cn

[B11] 生成数字序列 / 区间
来源：http://xa.shxzukj.cn

Py:   list(range(0, 10, 2))
来源：http://os.yuexingan06.cn

PHP:  range(0, 10, 2);
来源：http://ge.shxzukj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dg.wgjwhj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jq.nszjky.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dd.muxihuayi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pd.nicolike.cn

Ruby: (0...10).step(2).to_a
来源：http://ua.hahajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ur.szxytkj.cn

[B12] 跳出多层循环
来源：http://os.bjjhwx.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tt.gzmigu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mg.jianghongdianzi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dn.hahajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://op.521024.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ol.chemitech.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qw.yuntaijiaju.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nw.haigaiapp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ox.panjiajie.cn

[B13] 判断是否为数字
来源：http://dq.hnjuh.cn

Py:   isinstance(x, (int, float))
来源：http://ye.newstarts.cn

PHP:  is_numeric($x)
来源：http://zo.huixinmuqiang.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ou.9csxet.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yy.nszjky.cn

Java: x instanceof Number
来源：http://vx.nszjky.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lm.nszjky.cn

Ruby: x.is_a?(Numeric)
来源：http://qq.szxytkj.cn

C#:   x is int or double or decimal
来源：http://eq.haigaiapp.cn

[B14] 判断值是否在集合内
来源：http://up.wgjwhj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jl.huanxung.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lz.wgjwhj.cn

JS:   [1, 2, 3].includes(x)
来源：http://kc.haigaiapp.cn

TS:   [1, 2, 3].includes(x)
来源：http://zm.huixiangedu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://nq.szxytkj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ng.jctech888.com.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cu.jctech888.com.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wd.yuntaijiaju.cn

[B15] 布尔运算与取反
来源：http://ma.shxzskj.cn

Py:   a and b or not c
来源：http://lh.asd995.cn

PHP:  $a && $b || !$c
来源：http://uh.nszjky.cn

JS:   a && b || !c
来源：http://nu.shtwfgs.cn

TS:   a && b || !c
来源：http://sh.panjiajie.cn

Java: a && b || !c
来源：http://gv.huixiangedu.cn

Go:   a && b || !c
来源：http://hm.panjiajie.cn

Ruby: a && b || !c
来源：http://lt.nicolike.cn

C#:   a && b || !c
来源：http://sh.huixinmuqiang.cn

[B16] 卫语句：不满足条件提前返回
来源：http://mg.yuntaijiaju.cn

Py:   if not data: return
来源：http://wg.huixiangedu.cn

PHP:  if (!$data) { return; }
来源：http://ic.nszjky.cn

JS:   if (!data) return;
来源：http://mp.colortex.cn

TS:   if (!data) return;
来源：http://kv.nszjky.cn

Java: if (data == null) return;
来源：http://ra.jctech888.com.cn

Go:   if data == nil { return }
来源：http://bc.szxytkj.cn

Ruby: return if data.nil?
来源：http://qe.szsharing.cn

C#:   if (data == null) return;
来源：http://rw.huixiangedu.cn

================================================================================
来源：http://lc.colortex.cn

C. 函数与作用域
来源：http://im.huixinmuqiang.cn

================================================================================
来源：http://hy.chemitech.net.cn

[C01] 定义函数
来源：http://uh.9csxet.cn

Py:   def add(a, b): return a + b
来源：http://go.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qr.jctech888.com.cn

JS:   function add(a, b) { return a + b; }
来源：http://sy.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ct.colortex.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wq.nszjky.cn

Go:   func add(a, b int) int { return a + b }
来源：http://fp.yuexingan06.cn

Ruby: def add(a, b); a + b; end
来源：http://ll.shtwfgs.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rg.9csxet.cn

[C02] 默认参数
来源：http://lr.wgjwhj.cn

Py:   def greet(name="World"): return name
来源：http://hl.huixiangedu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ba.gzmigu.cn

JS:   function greet(name = "World") { return name; }
来源：http://xf.newstarts.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rq.shxzskj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ae.colortex.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pu.panjiajie.cn

Ruby: def greet(name = "World") = name
来源：http://yf.chemitech.net.cn

C#:   string Greet(string name = "World") => name;
来源：http://ee.shxzukj.cn

[C03] 可变参数
来源：http://lk.szsharing.cn

Py:   def total(*args): return sum(args)
来源：http://yf.hnjuh.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ca.521024.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fp.hnjuh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jg.yuntaijiaju.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://za.nicolike.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://od.yuntaijiaju.cn

Ruby: def total(*nums); nums.sum; end
来源：http://or.yuntaijiaju.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://is.bookmarksfly.cn

[C04] 命名参数 / 关键字参数
来源：http://hh.jianghongdianzi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://aw.huixinmuqiang.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jr.panjiajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nb.newstarts.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qs.yuexingan06.cn

Java: // 无：用 Builder 模式或 record
来源：http://jw.muxihuayi.cn

Go:   // 无：用配置结构体参数
来源：http://cf.muxihuayi.cn

Ruby: f(a: 1, b: 2)
来源：http://sg.asd995.cn

C#:   f(a: 1, b: 2)
来源：http://mi.yuexingan06.cn

[C05] 返回多个值
来源：http://fc.bookmarksfly.cn

Py:   return a, b
来源：http://bn.huixiangedu.cn

PHP:  return [$a, $b];
来源：http://ip.asd995.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://oc.shtwfgs.cn

TS:   return { a, b };
来源：http://el.shxzukj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vc.panjiajie.cn

Go:   return a, b
来源：http://if.shxzukj.cn

Ruby: return a, b
来源：http://wx.huixiangedu.cn

C#:   return (a, b);              // ValueTuple
来源：http://ow.huixinmuqiang.cn

[C06] 匿名函数 / lambda
来源：http://za.shxzukj.cn

Py:   square = lambda x: x * x
来源：http://nq.yuexingan06.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://lm.wgjwhj.cn

JS:   const square = x => x * x;
来源：http://xq.szxytkj.cn

TS:   const square = (x: number): number => x * x;
来源：http://sq.szxytkj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bm.jctech888.com.cn

Go:   sq := func(x int) int { return x * x }
来源：http://mw.jctech888.com.cn

Ruby: square = ->(x) { x * x }
来源：http://fp.yuexingan06.cn

C#:   Func<int, int> square = x => x * x;
来源：http://vs.shxzukj.cn

[C07] 把函数作为参数传入
来源：http://ba.newstarts.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dv.shxzukj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://sp.shxzukj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qf.wgjwhj.cn

TS:   arr.map(String)
来源：http://cw.jctech888.com.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://os.lnxyls.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://od.yuexingan06.cn

Ruby: arr.map(&:upcase)
来源：http://lw.521024.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pq.jianghongdianzi.cn

[C08] 闭包
来源：http://pt.huanxung.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ia.haigaiapp.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zv.jianghongdianzi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qu.521024.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mi.nicolike.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ju.9csxet.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qw.jctech888.com.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ia.chemitech.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tr.jctech888.com.cn

[C09] 递归
来源：http://cu.wgjwhj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jt.yuexingan06.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yz.521024.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ks.shtwfgs.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kv.colortex.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uy.bjjhwx.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://na.shxzukj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nv.huixinmuqiang.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pp.521024.cn

[C10] 变量作用域
来源：http://hn.muxihuayi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://by.huanxung.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jr.szsharing.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tt.521024.cn

TS:   同 JS
来源：http://ci.lnxyls.cn

Java: 方法内为块级作用域
来源：http://gf.yuexingan06.cn

Go:   花括号块级作用域
来源：http://cl.szxytkj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fh.colortex.cn

C#:   块级作用域
来源：http://gq.szxytkj.cn

[C11] 模块导入与导出
来源：http://ew.hnjuh.cn

Py:   from module import func
来源：http://ke.shxzskj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ow.wgjwhj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://he.521024.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xh.newstarts.cn

Java: import java.util.List;
来源：http://hf.jctech888.com.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yg.yuntaijiaju.cn

Ruby: require "json"; require_relative "./util"
来源：http://id.jianghongdianzi.cn

C#:   using System.Text;
来源：http://ba.asd995.cn

[C12] 立即执行函数 IIFE
来源：http://uu.9csxet.cn

Py:   (lambda: print("run"))()
来源：http://dx.yuexingan06.cn

PHP:  (function () { echo "run"; })();
来源：http://dc.gzmigu.cn

JS:   (() => { console.log("run"); })();
来源：http://rm.nicolike.cn

TS:   (() => { console.log("run"); })();
来源：http://zj.9csxet.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jz.panjiajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://re.szsharing.cn

Ruby: -> { puts "run" }.call
来源：http://kz.asd995.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pi.nszjky.cn

[C13] 类型声明 / 类型注解
来源：http://pe.lnxyls.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bk.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eq.hnjuh.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rn.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xq.shtwfgs.cn

Java: int add(int a, int b) { return a + b; }
来源：http://zl.huixiangedu.cn

Go:   func add(a, b int) int
来源：http://nl.nicolike.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yh.huanxung.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nd.szxytkj.cn

[C14] 泛型函数
来源：http://ky.panjiajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vm.chemitech.net.cn

PHP:  // 无泛型
来源：http://ip.lnxyls.cn

JS:   // 无泛型
来源：http://xn.gzmigu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qf.asd995.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ry.lnxyls.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://iy.9csxet.cn

Ruby: # 无泛型
来源：http://wf.chemitech.net.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pw.huixinmuqiang.cn

[C15] 解构 / 展开参数
来源：http://nt.bookmarksfly.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pm.chemitech.net.cn

PHP:  [$a, $b] = $pair;
来源：http://fh.shxzskj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ry.bookmarksfly.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cz.jianghongdianzi.cn

Java: // 无解构
来源：http://xu.yuexingan06.cn

Go:   // 无解构
来源：http://rc.nszjky.cn

Ruby: a, b = pair
来源：http://gy.hnjuh.cn

C#:   var (a, b) = pair;
来源：http://ub.shxzukj.cn

[C16] 函数 / 方法重载
来源：http://pg.yuexingan06.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ah.huixinmuqiang.cn

PHP:  // 无重载
来源：http://il.wgjwhj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ma.bookmarksfly.cn

TS:   // 用联合类型或重载签名声明
来源：http://lr.szxytkj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://nc.hahajie.cn

Go:   // 无重载：用不同函数名
来源：http://it.shxzskj.cn

Ruby: # 无重载：靠动态参数
来源：http://ku.yuexingan06.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://oe.wgjwhj.cn

================================================================================
来源：http://pt.jctech888.com.cn

D. 数组 / 列表 / 集合
来源：http://wl.huanxung.cn

================================================================================
来源：http://ja.bjjhwx.cn

[D01] 创建数组 / 列表
来源：http://hs.nszjky.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://il.jctech888.com.cn


<!-- 参考信息 -->