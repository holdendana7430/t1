代发 wailian999

[A26] 类型转换总览
来源：http://br.yuexingan06.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ze.521024.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wr.asd995.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tm.lnxyls.cn

TS:   Number() String() Boolean() x as number
来源：http://oq.gzmigu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rn.colortex.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zk.newstarts.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ei.huixinmuqiang.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://iz.huixiangedu.cn

================================================================================
来源：http://dx.shxzukj.cn

B. 流程控制
来源：http://fx.colortex.cn

================================================================================
来源：http://ou.nicolike.cn

[B01] 条件判断 if / else
来源：http://kh.szsharing.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bt.yuntaijiaju.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rb.wgjwhj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nq.hnjuh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ls.9csxet.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xe.huanxung.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://eb.chemitech.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ai.huanxung.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bd.nicolike.cn

[B02] 多分支 else if / elif
来源：http://ey.shxzskj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://eu.newstarts.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xs.yuexingan06.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jz.9csxet.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://im.bookmarksfly.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ld.huixinmuqiang.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://id.szsharing.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qi.chemitech.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wn.huixinmuqiang.cn

[B03] switch / match / case
来源：http://rr.yuexingan06.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ji.szxytkj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zm.nicolike.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hf.muxihuayi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cs.yuntaijiaju.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://yg.asd995.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ma.521024.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qw.wgjwhj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kg.shxzukj.cn

[B04] for 计数循环
来源：http://db.9csxet.cn

Py:   for i in range(10): print(i)
来源：http://wr.hahajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rx.jctech888.com.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cq.colortex.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mo.lnxyls.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ij.haigaiapp.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rb.jianghongdianzi.cn

Ruby: 10.times { |i| puts i }
来源：http://em.haigaiapp.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ic.muxihuayi.cn

[B05] 遍历数组 / 列表
来源：http://en.huanxung.cn

Py:   for item in arr: print(item)
来源：http://nc.szxytkj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zb.muxihuayi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://se.yuntaijiaju.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tm.panjiajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://at.521024.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fj.hahajie.cn

Ruby: arr.each { |item| puts item }
来源：http://vl.shxzukj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://py.newstarts.cn

[B06] 遍历字典 / 对象
来源：http://kz.lnxyls.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://wa.szxytkj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wo.yuntaijiaju.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lm.chemitech.net.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oh.jianghongdianzi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zd.521024.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vr.nicolike.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hc.bjjhwx.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pl.521024.cn

[B07] while 循环
来源：http://fx.colortex.cn

Py:   while i < 10: i += 1
来源：http://dn.9csxet.cn

PHP:  while ($i < 10) { $i++; }
来源：http://oa.nszjky.cn

JS:   while (i < 10) { i++; }
来源：http://qe.bookmarksfly.cn

TS:   while (i < 10) { i++; }
来源：http://uq.jctech888.com.cn

Java: while (i < 10) { i++; }
来源：http://ph.gzmigu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vx.lnxyls.cn

Ruby: while i < 10; i += 1; end
来源：http://bz.huixiangedu.cn

C#:   while (i < 10) { i++; }
来源：http://rj.nicolike.cn

[B08] do-while（至少执行一次）
来源：http://lq.bookmarksfly.cn

Py:   # 无 do-while：用 while True + break
来源：http://be.nicolike.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xj.yuntaijiaju.cn

JS:   do { i++; } while (i < 10);
来源：http://xh.521024.cn

TS:   do { i++; } while (i < 10);
来源：http://mt.huanxung.cn

Java: do { i++; } while (i < 10);
来源：http://ud.shxzukj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ww.szsharing.cn

Ruby: begin; i += 1; end while i < 10
来源：http://yp.hnjuh.cn

C#:   do { i++; } while (i < 10);
来源：http://in.szxytkj.cn

[B09] break 与 continue
来源：http://ma.panjiajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zu.bookmarksfly.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cw.shxzukj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vc.muxihuayi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ts.muxihuayi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pw.huixinmuqiang.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://je.gzmigu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vq.colortex.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fm.colortex.cn

[B10] 遍历同时拿索引
来源：http://sa.szxytkj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pb.bjjhwx.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bc.hahajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ml.521024.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cz.newstarts.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.muxihuayi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vx.colortex.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kc.wgjwhj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kf.szsharing.cn

[B11] 生成数字序列 / 区间
来源：http://rs.newstarts.cn

Py:   list(range(0, 10, 2))
来源：http://sf.shxzskj.cn

PHP:  range(0, 10, 2);
来源：http://kt.huixinmuqiang.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wm.huixinmuqiang.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nm.bjjhwx.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pu.colortex.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://og.huixinmuqiang.cn

Ruby: (0...10).step(2).to_a
来源：http://eo.521024.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cg.jianghongdianzi.cn

[B12] 跳出多层循环
来源：http://hm.huanxung.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://uz.521024.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zd.nszjky.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yp.newstarts.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wd.huanxung.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bc.muxihuayi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://li.jianghongdianzi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wx.wgjwhj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zv.9csxet.cn

[B13] 判断是否为数字
来源：http://tu.9csxet.cn

Py:   isinstance(x, (int, float))
来源：http://az.muxihuayi.cn

PHP:  is_numeric($x)
来源：http://fu.shtwfgs.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ac.wgjwhj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kb.muxihuayi.cn

Java: x instanceof Number
来源：http://dd.yuntaijiaju.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yu.hnjuh.cn

Ruby: x.is_a?(Numeric)
来源：http://qf.colortex.cn

C#:   x is int or double or decimal
来源：http://xn.newstarts.cn

[B14] 判断值是否在集合内
来源：http://sl.szsharing.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ee.shtwfgs.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tu.chemitech.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://kq.lnxyls.cn

TS:   [1, 2, 3].includes(x)
来源：http://up.szxytkj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://bs.shxzskj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://oz.jianghongdianzi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://wq.muxihuayi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yr.huixiangedu.cn

[B15] 布尔运算与取反
来源：http://yp.jianghongdianzi.cn

Py:   a and b or not c
来源：http://xy.shtwfgs.cn

PHP:  $a && $b || !$c
来源：http://nt.hahajie.cn

JS:   a && b || !c
来源：http://va.hahajie.cn

TS:   a && b || !c
来源：http://ip.hahajie.cn

Java: a && b || !c
来源：http://fl.9csxet.cn

Go:   a && b || !c
来源：http://ht.bookmarksfly.cn

Ruby: a && b || !c
来源：http://cz.szxytkj.cn

C#:   a && b || !c
来源：http://rb.newstarts.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fm.hnjuh.cn

Py:   if not data: return
来源：http://uf.chemitech.net.cn

PHP:  if (!$data) { return; }
来源：http://op.chemitech.net.cn

JS:   if (!data) return;
来源：http://eb.hnjuh.cn

TS:   if (!data) return;
来源：http://eb.shxzukj.cn

Java: if (data == null) return;
来源：http://pn.colortex.cn

Go:   if data == nil { return }
来源：http://un.panjiajie.cn

Ruby: return if data.nil?
来源：http://aq.muxihuayi.cn

C#:   if (data == null) return;
来源：http://sb.asd995.cn

================================================================================
来源：http://jl.jianghongdianzi.cn

C. 函数与作用域
来源：http://xs.colortex.cn

================================================================================
来源：http://dy.jctech888.com.cn

[C01] 定义函数
来源：http://vx.hahajie.cn

Py:   def add(a, b): return a + b
来源：http://zh.muxihuayi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lh.bjjhwx.cn

JS:   function add(a, b) { return a + b; }
来源：http://qm.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mu.huixiangedu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bs.nicolike.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ed.panjiajie.cn

Ruby: def add(a, b); a + b; end
来源：http://sv.bookmarksfly.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jr.yuntaijiaju.cn

[C02] 默认参数
来源：http://qs.bjjhwx.cn

Py:   def greet(name="World"): return name
来源：http://rx.521024.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wr.asd995.cn

JS:   function greet(name = "World") { return name; }
来源：http://kr.9csxet.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fq.bjjhwx.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://sk.hahajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://la.bookmarksfly.cn

Ruby: def greet(name = "World") = name
来源：http://dc.shxzukj.cn

C#:   string Greet(string name = "World") => name;
来源：http://kr.bjjhwx.cn

[C03] 可变参数
来源：http://ud.shxzukj.cn

Py:   def total(*args): return sum(args)
来源：http://cl.szsharing.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yz.yuntaijiaju.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nz.huixiangedu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ef.nszjky.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ws.yuntaijiaju.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://oh.szsharing.cn

Ruby: def total(*nums); nums.sum; end
来源：http://mz.huixiangedu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hu.nicolike.cn

[C04] 命名参数 / 关键字参数
来源：http://hp.huanxung.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jh.huixiangedu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lv.hahajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://px.colortex.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://un.szxytkj.cn

Java: // 无：用 Builder 模式或 record
来源：http://up.huixiangedu.cn

Go:   // 无：用配置结构体参数
来源：http://tq.hahajie.cn

Ruby: f(a: 1, b: 2)
来源：http://wt.9csxet.cn

C#:   f(a: 1, b: 2)
来源：http://so.chemitech.net.cn

[C05] 返回多个值
来源：http://td.bjjhwx.cn

Py:   return a, b
来源：http://ui.shtwfgs.cn

PHP:  return [$a, $b];
来源：http://bn.nicolike.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wo.yuntaijiaju.cn

TS:   return { a, b };
来源：http://sp.szxytkj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://aq.9csxet.cn

Go:   return a, b
来源：http://pg.newstarts.cn

Ruby: return a, b
来源：http://it.jianghongdianzi.cn

C#:   return (a, b);              // ValueTuple
来源：http://qc.huixinmuqiang.cn

[C06] 匿名函数 / lambda
来源：http://fz.yuntaijiaju.cn

Py:   square = lambda x: x * x
来源：http://fc.lnxyls.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xq.szxytkj.cn

JS:   const square = x => x * x;
来源：http://bo.chemitech.net.cn

TS:   const square = (x: number): number => x * x;
来源：http://mh.nszjky.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://uq.newstarts.cn

Go:   sq := func(x int) int { return x * x }
来源：http://oy.bookmarksfly.cn

Ruby: square = ->(x) { x * x }
来源：http://hi.bookmarksfly.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zz.huixinmuqiang.cn

[C07] 把函数作为参数传入
来源：http://mh.jctech888.com.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pa.huixinmuqiang.cn

PHP:  array_map("strtoupper", $arr);
来源：http://yo.huixiangedu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ts.chemitech.net.cn

TS:   arr.map(String)
来源：http://zv.hnjuh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://io.shtwfgs.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uy.hahajie.cn

Ruby: arr.map(&:upcase)
来源：http://tn.nicolike.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xv.yuexingan06.cn

[C08] 闭包
来源：http://ey.521024.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zj.wgjwhj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://un.yuexingan06.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bj.jctech888.com.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mg.shtwfgs.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dv.nszjky.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://po.hnjuh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qg.shxzskj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vw.newstarts.cn

[C09] 递归
来源：http://zs.bookmarksfly.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sd.lnxyls.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://za.huanxung.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qd.szsharing.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dy.lnxyls.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jx.yuntaijiaju.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vn.bookmarksfly.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sz.9csxet.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zk.colortex.cn

[C10] 变量作用域
来源：http://oh.jctech888.com.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://as.shtwfgs.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://od.shxzukj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zg.jctech888.com.cn

TS:   同 JS
来源：http://lh.bjjhwx.cn

Java: 方法内为块级作用域
来源：http://vy.hahajie.cn

Go:   花括号块级作用域
来源：http://bo.asd995.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gi.9csxet.cn

C#:   块级作用域
来源：http://is.hahajie.cn

[C11] 模块导入与导出
来源：http://pd.szxytkj.cn

Py:   from module import func
来源：http://mv.colortex.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://yv.9csxet.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://za.lnxyls.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hu.colortex.cn

Java: import java.util.List;
来源：http://nh.haigaiapp.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jn.9csxet.cn

Ruby: require "json"; require_relative "./util"
来源：http://mf.9csxet.cn

C#:   using System.Text;
来源：http://qv.lnxyls.cn

[C12] 立即执行函数 IIFE
来源：http://mw.newstarts.cn

Py:   (lambda: print("run"))()
来源：http://vn.bookmarksfly.cn

PHP:  (function () { echo "run"; })();
来源：http://xp.huixinmuqiang.cn

JS:   (() => { console.log("run"); })();
来源：http://nf.shxzukj.cn

TS:   (() => { console.log("run"); })();
来源：http://pp.gzmigu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mb.gzmigu.cn

Go:   func() { fmt.Println("run") }()
来源：http://ou.jianghongdianzi.cn

Ruby: -> { puts "run" }.call
来源：http://pt.chemitech.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://vi.panjiajie.cn

[C13] 类型声明 / 类型注解
来源：http://bg.nszjky.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rp.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://th.nicolike.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://iq.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ib.szsharing.cn

Java: int add(int a, int b) { return a + b; }
来源：http://yu.nszjky.cn

Go:   func add(a, b int) int
来源：http://jk.panjiajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ie.bookmarksfly.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nu.wgjwhj.cn

[C14] 泛型函数
来源：http://yp.nszjky.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sa.shxzskj.cn

PHP:  // 无泛型
来源：http://kv.haigaiapp.cn

JS:   // 无泛型
来源：http://mg.yuntaijiaju.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xg.newstarts.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ny.huixinmuqiang.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ku.shxzukj.cn

Ruby: # 无泛型
来源：http://ei.521024.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gr.yuntaijiaju.cn

[C15] 解构 / 展开参数
来源：http://gv.panjiajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://uu.panjiajie.cn

PHP:  [$a, $b] = $pair;
来源：http://uf.yuntaijiaju.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ik.bjjhwx.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://we.haigaiapp.cn

Java: // 无解构
来源：http://wt.nszjky.cn

Go:   // 无解构
来源：http://tt.nicolike.cn

Ruby: a, b = pair
来源：http://pz.yuntaijiaju.cn

C#:   var (a, b) = pair;
来源：http://en.wgjwhj.cn

[C16] 函数 / 方法重载
来源：http://nh.colortex.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://as.9csxet.cn

PHP:  // 无重载
来源：http://dv.huixiangedu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://yr.colortex.cn

TS:   // 用联合类型或重载签名声明
来源：http://ih.hahajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ns.jianghongdianzi.cn


<!-- 参考信息 -->