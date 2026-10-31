代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://iy.shxzskj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://si.521024.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nu.shxzskj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mn.huanxung.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dg.chemitech.net.cn

================================================================================
来源：http://no.nicolike.cn

B. 流程控制
来源：http://yu.huanxung.cn

================================================================================
来源：http://ev.huanxung.cn

[B01] 条件判断 if / else
来源：http://gl.yuntaijiaju.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bb.shxzskj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://le.muxihuayi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://di.gzmigu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bb.shtwfgs.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ln.nszjky.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://sg.nszjky.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fv.jctech888.com.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rv.chemitech.net.cn

[B02] 多分支 else if / elif
来源：http://tj.hnjuh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qi.jctech888.com.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rs.nicolike.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ia.haigaiapp.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cb.shxzukj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pu.haigaiapp.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tt.szsharing.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hf.hnjuh.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tm.yuexingan06.cn

[B03] switch / match / case
来源：http://jz.szsharing.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nt.gzmigu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vj.shtwfgs.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wt.huixiangedu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gf.yuexingan06.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tv.colortex.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lq.521024.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pd.muxihuayi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kv.shtwfgs.cn

[B04] for 计数循环
来源：http://ly.jianghongdianzi.cn

Py:   for i in range(10): print(i)
来源：http://uu.shtwfgs.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://be.nszjky.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zc.yuexingan06.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fu.lnxyls.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gg.hahajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cn.bjjhwx.cn

Ruby: 10.times { |i| puts i }
来源：http://ua.newstarts.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jp.huixiangedu.cn

[B05] 遍历数组 / 列表
来源：http://mj.yuntaijiaju.cn

Py:   for item in arr: print(item)
来源：http://zo.bjjhwx.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ak.9csxet.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yt.colortex.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xv.shtwfgs.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ds.muxihuayi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tr.yuexingan06.cn

Ruby: arr.each { |item| puts item }
来源：http://qz.asd995.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hs.szsharing.cn

[B06] 遍历字典 / 对象
来源：http://yz.yuntaijiaju.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://nj.9csxet.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tq.jctech888.com.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gw.lnxyls.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kk.huanxung.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gg.shtwfgs.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yf.lnxyls.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mt.nszjky.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vu.jianghongdianzi.cn

[B07] while 循环
来源：http://tc.bjjhwx.cn

Py:   while i < 10: i += 1
来源：http://gm.wgjwhj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://su.muxihuayi.cn

JS:   while (i < 10) { i++; }
来源：http://mf.haigaiapp.cn

TS:   while (i < 10) { i++; }
来源：http://sp.haigaiapp.cn

Java: while (i < 10) { i++; }
来源：http://ig.jianghongdianzi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sc.bjjhwx.cn

Ruby: while i < 10; i += 1; end
来源：http://lz.shtwfgs.cn

C#:   while (i < 10) { i++; }
来源：http://ix.lnxyls.cn

[B08] do-while（至少执行一次）
来源：http://gh.newstarts.cn

Py:   # 无 do-while：用 while True + break
来源：http://nm.huanxung.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://fh.panjiajie.cn

JS:   do { i++; } while (i < 10);
来源：http://ts.newstarts.cn

TS:   do { i++; } while (i < 10);
来源：http://tx.newstarts.cn

Java: do { i++; } while (i < 10);
来源：http://vh.shxzukj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vx.gzmigu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zq.huanxung.cn

C#:   do { i++; } while (i < 10);
来源：http://xm.shxzukj.cn

[B09] break 与 continue
来源：http://qd.9csxet.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pq.huixiangedu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fu.wgjwhj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lt.shxzskj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aa.9csxet.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ho.shtwfgs.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lx.asd995.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hq.yuexingan06.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ak.colortex.cn

[B10] 遍历同时拿索引
来源：http://kt.521024.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://di.huanxung.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rx.yuntaijiaju.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mw.nicolike.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cj.jctech888.com.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gk.hnjuh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ax.shxzukj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qs.bookmarksfly.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ds.yuexingan06.cn

[B11] 生成数字序列 / 区间
来源：http://fk.bookmarksfly.cn

Py:   list(range(0, 10, 2))
来源：http://tz.panjiajie.cn

PHP:  range(0, 10, 2);
来源：http://kl.shtwfgs.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uj.bookmarksfly.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://js.panjiajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dc.huixiangedu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nx.521024.cn

Ruby: (0...10).step(2).to_a
来源：http://qx.jctech888.com.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ay.huanxung.cn

[B12] 跳出多层循环
来源：http://io.haigaiapp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://om.huanxung.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://le.haigaiapp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cs.newstarts.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pu.nicolike.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rj.szsharing.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rz.521024.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lf.szsharing.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wt.huanxung.cn

[B13] 判断是否为数字
来源：http://pl.haigaiapp.cn

Py:   isinstance(x, (int, float))
来源：http://ex.shxzskj.cn

PHP:  is_numeric($x)
来源：http://jx.nicolike.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mv.haigaiapp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gv.jctech888.com.cn

Java: x instanceof Number
来源：http://bg.bookmarksfly.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kq.shtwfgs.cn

Ruby: x.is_a?(Numeric)
来源：http://rc.shxzukj.cn

C#:   x is int or double or decimal
来源：http://kw.nszjky.cn

[B14] 判断值是否在集合内
来源：http://jf.huixinmuqiang.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://oc.nszjky.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gx.szxytkj.cn

JS:   [1, 2, 3].includes(x)
来源：http://nz.chemitech.net.cn

TS:   [1, 2, 3].includes(x)
来源：http://wq.shxzukj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://cs.shtwfgs.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tc.jctech888.com.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gl.szxytkj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hg.huanxung.cn

[B15] 布尔运算与取反
来源：http://hp.bookmarksfly.cn

Py:   a and b or not c
来源：http://nx.szsharing.cn

PHP:  $a && $b || !$c
来源：http://me.521024.cn

JS:   a && b || !c
来源：http://ts.shtwfgs.cn

TS:   a && b || !c
来源：http://uj.shxzskj.cn

Java: a && b || !c
来源：http://an.lnxyls.cn

Go:   a && b || !c
来源：http://xz.yuntaijiaju.cn

Ruby: a && b || !c
来源：http://ny.bookmarksfly.cn

C#:   a && b || !c
来源：http://ng.yuntaijiaju.cn

[B16] 卫语句：不满足条件提前返回
来源：http://db.colortex.cn

Py:   if not data: return
来源：http://qi.gzmigu.cn

PHP:  if (!$data) { return; }
来源：http://ku.shxzukj.cn

JS:   if (!data) return;
来源：http://qr.lnxyls.cn

TS:   if (!data) return;
来源：http://ui.shtwfgs.cn

Java: if (data == null) return;
来源：http://eq.szxytkj.cn

Go:   if data == nil { return }
来源：http://ve.muxihuayi.cn

Ruby: return if data.nil?
来源：http://jh.huixinmuqiang.cn

C#:   if (data == null) return;
来源：http://le.jctech888.com.cn

================================================================================
来源：http://xd.nszjky.cn

C. 函数与作用域
来源：http://oi.hnjuh.cn

================================================================================
来源：http://vx.asd995.cn

[C01] 定义函数
来源：http://ft.jianghongdianzi.cn

Py:   def add(a, b): return a + b
来源：http://dk.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kt.shxzukj.cn

JS:   function add(a, b) { return a + b; }
来源：http://xb.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gr.wgjwhj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://da.bookmarksfly.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jt.muxihuayi.cn

Ruby: def add(a, b); a + b; end
来源：http://op.szxytkj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uy.nicolike.cn

[C02] 默认参数
来源：http://li.bookmarksfly.cn

Py:   def greet(name="World"): return name
来源：http://es.huanxung.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://om.huixinmuqiang.cn

JS:   function greet(name = "World") { return name; }
来源：http://lq.nicolike.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bx.muxihuayi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ec.jctech888.com.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gb.asd995.cn

Ruby: def greet(name = "World") = name
来源：http://dc.shxzukj.cn

C#:   string Greet(string name = "World") => name;
来源：http://wx.bjjhwx.cn

[C03] 可变参数
来源：http://jw.bookmarksfly.cn

Py:   def total(*args): return sum(args)
来源：http://bs.jctech888.com.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bf.lnxyls.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sm.lnxyls.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qk.hnjuh.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ea.nicolike.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cy.bjjhwx.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fu.shxzskj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tr.huixinmuqiang.cn

[C04] 命名参数 / 关键字参数
来源：http://gc.bookmarksfly.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://am.9csxet.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rw.bjjhwx.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://px.hahajie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://du.lnxyls.cn

Java: // 无：用 Builder 模式或 record
来源：http://ld.hnjuh.cn

Go:   // 无：用配置结构体参数
来源：http://tb.jianghongdianzi.cn

Ruby: f(a: 1, b: 2)
来源：http://xf.huixinmuqiang.cn

C#:   f(a: 1, b: 2)
来源：http://lc.shxzukj.cn

[C05] 返回多个值
来源：http://sr.hnjuh.cn

Py:   return a, b
来源：http://fq.gzmigu.cn

PHP:  return [$a, $b];
来源：http://mp.hnjuh.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://mb.shtwfgs.cn

TS:   return { a, b };
来源：http://xq.shxzskj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pp.szsharing.cn

Go:   return a, b
来源：http://pg.nszjky.cn

Ruby: return a, b
来源：http://hp.bjjhwx.cn

C#:   return (a, b);              // ValueTuple
来源：http://qu.huixiangedu.cn

[C06] 匿名函数 / lambda
来源：http://oe.hahajie.cn

Py:   square = lambda x: x * x
来源：http://dz.nicolike.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qf.nicolike.cn

JS:   const square = x => x * x;
来源：http://pq.haigaiapp.cn

TS:   const square = (x: number): number => x * x;
来源：http://sg.jianghongdianzi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mp.huixinmuqiang.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ml.szsharing.cn

Ruby: square = ->(x) { x * x }
来源：http://uf.jctech888.com.cn

C#:   Func<int, int> square = x => x * x;
来源：http://cs.yuexingan06.cn

[C07] 把函数作为参数传入
来源：http://zl.bookmarksfly.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tc.huixinmuqiang.cn

PHP:  array_map("strtoupper", $arr);
来源：http://it.bookmarksfly.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fw.jctech888.com.cn

TS:   arr.map(String)
来源：http://aw.huixiangedu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lr.lnxyls.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gq.jctech888.com.cn

Ruby: arr.map(&:upcase)
来源：http://vt.shtwfgs.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gs.huanxung.cn

[C08] 闭包
来源：http://zu.haigaiapp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yl.asd995.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ao.panjiajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lx.521024.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rr.hahajie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pk.yuexingan06.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kl.521024.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sj.shxzukj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://br.shxzskj.cn

[C09] 递归
来源：http://wy.huanxung.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lk.jctech888.com.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rq.lnxyls.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cw.jctech888.com.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uv.shxzskj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mz.lnxyls.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wb.panjiajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lk.newstarts.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ht.panjiajie.cn

[C10] 变量作用域
来源：http://uf.gzmigu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xh.nszjky.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://oz.9csxet.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qc.huixinmuqiang.cn

TS:   同 JS
来源：http://dx.bjjhwx.cn

Java: 方法内为块级作用域
来源：http://oo.bookmarksfly.cn

Go:   花括号块级作用域
来源：http://ld.szxytkj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://to.jianghongdianzi.cn

C#:   块级作用域
来源：http://dr.bookmarksfly.cn

[C11] 模块导入与导出
来源：http://ux.shtwfgs.cn

Py:   from module import func
来源：http://sg.nszjky.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://se.shxzskj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ss.shtwfgs.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xc.hahajie.cn

Java: import java.util.List;
来源：http://df.newstarts.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wt.nszjky.cn

Ruby: require "json"; require_relative "./util"
来源：http://gj.gzmigu.cn

C#:   using System.Text;
来源：http://ea.newstarts.cn

[C12] 立即执行函数 IIFE
来源：http://po.521024.cn

Py:   (lambda: print("run"))()
来源：http://qi.hahajie.cn

PHP:  (function () { echo "run"; })();
来源：http://oh.yuexingan06.cn

JS:   (() => { console.log("run"); })();
来源：http://bu.jctech888.com.cn

TS:   (() => { console.log("run"); })();
来源：http://gx.hnjuh.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nq.shxzskj.cn

Go:   func() { fmt.Println("run") }()
来源：http://pw.asd995.cn

Ruby: -> { puts "run" }.call
来源：http://ev.haigaiapp.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://yb.nszjky.cn

[C13] 类型声明 / 类型注解
来源：http://ei.chemitech.net.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rb.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sf.colortex.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kb.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yo.9csxet.cn

Java: int add(int a, int b) { return a + b; }
来源：http://zo.hahajie.cn

Go:   func add(a, b int) int
来源：http://pk.wgjwhj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://id.shtwfgs.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fl.shxzskj.cn

[C14] 泛型函数
来源：http://ak.huixiangedu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jl.jctech888.com.cn

PHP:  // 无泛型
来源：http://ry.hnjuh.cn

JS:   // 无泛型
来源：http://eb.9csxet.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://af.jianghongdianzi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ce.nicolike.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bk.9csxet.cn

Ruby: # 无泛型
来源：http://nz.jctech888.com.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dz.huixiangedu.cn

[C15] 解构 / 展开参数
来源：http://vq.nicolike.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xm.haigaiapp.cn

PHP:  [$a, $b] = $pair;
来源：http://sq.szsharing.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xr.nszjky.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qy.gzmigu.cn

Java: // 无解构
来源：http://oe.szxytkj.cn

Go:   // 无解构
来源：http://rc.nszjky.cn

Ruby: a, b = pair
来源：http://bp.shxzskj.cn

C#:   var (a, b) = pair;
来源：http://wc.wgjwhj.cn

[C16] 函数 / 方法重载
来源：http://sc.yuntaijiaju.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jm.hahajie.cn

PHP:  // 无重载
来源：http://gn.lnxyls.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://cy.huixinmuqiang.cn

TS:   // 用联合类型或重载签名声明
来源：http://er.yuexingan06.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://bv.huixiangedu.cn

Go:   // 无重载：用不同函数名
来源：http://zs.chemitech.net.cn

Ruby: # 无重载：靠动态参数
来源：http://hj.jctech888.com.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zi.9csxet.cn

================================================================================
来源：http://yw.newstarts.cn


<!-- 参考信息 -->