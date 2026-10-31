代发 wailian999

[A26] 类型转换总览
来源：http://ej.lnxyls.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bp.bjjhwx.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qe.gzmigu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bu.panjiajie.cn

TS:   Number() String() Boolean() x as number
来源：http://dp.nszjky.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://on.huixinmuqiang.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ze.huixiangedu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zl.panjiajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kf.muxihuayi.cn

================================================================================
来源：http://dp.asd995.cn

B. 流程控制
来源：http://an.nszjky.cn

================================================================================
来源：http://vi.chemitech.net.cn

[B01] 条件判断 if / else
来源：http://ng.jctech888.com.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://uw.chemitech.net.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fr.newstarts.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cf.bookmarksfly.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hb.bjjhwx.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://os.yuexingan06.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gb.bjjhwx.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qm.szsharing.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zt.gzmigu.cn

[B02] 多分支 else if / elif
来源：http://pb.chemitech.net.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://uf.shxzskj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dx.shtwfgs.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cl.lnxyls.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xx.haigaiapp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://al.huanxung.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fo.shxzukj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fz.colortex.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rh.521024.cn

[B03] switch / match / case
来源：http://ft.newstarts.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sp.9csxet.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nk.9csxet.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://io.hnjuh.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uh.jianghongdianzi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://yq.chemitech.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://my.newstarts.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ot.521024.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ei.newstarts.cn

[B04] for 计数循环
来源：http://vz.chemitech.net.cn

Py:   for i in range(10): print(i)
来源：http://aj.nicolike.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yq.panjiajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pc.haigaiapp.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ak.huanxung.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fw.hahajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fp.huixinmuqiang.cn

Ruby: 10.times { |i| puts i }
来源：http://kf.asd995.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://do.jianghongdianzi.cn

[B05] 遍历数组 / 列表
来源：http://km.shtwfgs.cn

Py:   for item in arr: print(item)
来源：http://sa.szxytkj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vn.9csxet.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ux.szsharing.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://wi.huixiangedu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ue.yuexingan06.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://io.haigaiapp.cn

Ruby: arr.each { |item| puts item }
来源：http://bl.hnjuh.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yp.jctech888.com.cn

[B06] 遍历字典 / 对象
来源：http://cg.szsharing.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ke.nszjky.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yb.bjjhwx.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mp.jctech888.com.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uf.szsharing.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sg.nicolike.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pb.hahajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zt.haigaiapp.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hh.gzmigu.cn

[B07] while 循环
来源：http://fj.asd995.cn

Py:   while i < 10: i += 1
来源：http://tj.szxytkj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ux.bookmarksfly.cn

JS:   while (i < 10) { i++; }
来源：http://cc.9csxet.cn

TS:   while (i < 10) { i++; }
来源：http://da.bookmarksfly.cn

Java: while (i < 10) { i++; }
来源：http://cv.shxzukj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://oe.chemitech.net.cn

Ruby: while i < 10; i += 1; end
来源：http://ii.huixinmuqiang.cn

C#:   while (i < 10) { i++; }
来源：http://ja.szsharing.cn

[B08] do-while（至少执行一次）
来源：http://ig.yuntaijiaju.cn

Py:   # 无 do-while：用 while True + break
来源：http://jw.hnjuh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ep.huixiangedu.cn

JS:   do { i++; } while (i < 10);
来源：http://di.wgjwhj.cn

TS:   do { i++; } while (i < 10);
来源：http://si.chemitech.net.cn

Java: do { i++; } while (i < 10);
来源：http://gx.bjjhwx.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jz.wgjwhj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jo.shtwfgs.cn

C#:   do { i++; } while (i < 10);
来源：http://ps.shxzskj.cn

[B09] break 与 continue
来源：http://sw.bookmarksfly.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bq.bookmarksfly.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ij.lnxyls.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nz.huixiangedu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ex.jianghongdianzi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sf.wgjwhj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qt.shtwfgs.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ta.yuntaijiaju.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tz.nicolike.cn

[B10] 遍历同时拿索引
来源：http://cm.hnjuh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xt.huixiangedu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kb.9csxet.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ym.huixinmuqiang.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://br.nicolike.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hn.521024.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cp.huanxung.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dv.nicolike.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zn.gzmigu.cn

[B11] 生成数字序列 / 区间
来源：http://ta.huixiangedu.cn

Py:   list(range(0, 10, 2))
来源：http://dc.muxihuayi.cn

PHP:  range(0, 10, 2);
来源：http://tq.huanxung.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rm.lnxyls.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bk.bookmarksfly.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vv.bjjhwx.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zd.huixinmuqiang.cn

Ruby: (0...10).step(2).to_a
来源：http://sj.szsharing.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jo.muxihuayi.cn

[B12] 跳出多层循环
来源：http://gn.wgjwhj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ir.nszjky.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hx.muxihuayi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://df.huixinmuqiang.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ug.muxihuayi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hi.asd995.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xl.szxytkj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mv.newstarts.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xm.bjjhwx.cn

[B13] 判断是否为数字
来源：http://el.szxytkj.cn

Py:   isinstance(x, (int, float))
来源：http://vs.yuntaijiaju.cn

PHP:  is_numeric($x)
来源：http://nk.9csxet.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lv.nicolike.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://un.gzmigu.cn

Java: x instanceof Number
来源：http://dd.hahajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wt.haigaiapp.cn

Ruby: x.is_a?(Numeric)
来源：http://ad.wgjwhj.cn

C#:   x is int or double or decimal
来源：http://wz.szsharing.cn

[B14] 判断值是否在集合内
来源：http://mg.nszjky.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tt.szsharing.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://db.muxihuayi.cn

JS:   [1, 2, 3].includes(x)
来源：http://sd.muxihuayi.cn

TS:   [1, 2, 3].includes(x)
来源：http://cc.hnjuh.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ip.bjjhwx.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ek.huixinmuqiang.cn

Ruby: [1, 2, 3].include?(x)
来源：http://id.chemitech.net.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cy.huixiangedu.cn

[B15] 布尔运算与取反
来源：http://sx.shxzukj.cn

Py:   a and b or not c
来源：http://bd.chemitech.net.cn

PHP:  $a && $b || !$c
来源：http://hy.asd995.cn

JS:   a && b || !c
来源：http://ap.szxytkj.cn

TS:   a && b || !c
来源：http://la.521024.cn

Java: a && b || !c
来源：http://lb.jianghongdianzi.cn

Go:   a && b || !c
来源：http://la.huixinmuqiang.cn

Ruby: a && b || !c
来源：http://xj.shtwfgs.cn

C#:   a && b || !c
来源：http://rm.nszjky.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gz.shtwfgs.cn

Py:   if not data: return
来源：http://ew.shtwfgs.cn

PHP:  if (!$data) { return; }
来源：http://mf.szsharing.cn

JS:   if (!data) return;
来源：http://nq.newstarts.cn

TS:   if (!data) return;
来源：http://dy.szxytkj.cn

Java: if (data == null) return;
来源：http://vl.shxzskj.cn

Go:   if data == nil { return }
来源：http://dh.hahajie.cn

Ruby: return if data.nil?
来源：http://vk.bjjhwx.cn

C#:   if (data == null) return;
来源：http://we.nszjky.cn

================================================================================
来源：http://gg.jctech888.com.cn

C. 函数与作用域
来源：http://nd.jianghongdianzi.cn

================================================================================
来源：http://ii.9csxet.cn

[C01] 定义函数
来源：http://sb.lnxyls.cn

Py:   def add(a, b): return a + b
来源：http://lx.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bv.nicolike.cn

JS:   function add(a, b) { return a + b; }
来源：http://gz.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jg.panjiajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mv.huanxung.cn

Go:   func add(a, b int) int { return a + b }
来源：http://fo.9csxet.cn

Ruby: def add(a, b); a + b; end
来源：http://qi.yuexingan06.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://eg.wgjwhj.cn

[C02] 默认参数
来源：http://gi.szxytkj.cn

Py:   def greet(name="World"): return name
来源：http://zs.panjiajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ut.muxihuayi.cn

JS:   function greet(name = "World") { return name; }
来源：http://dm.shxzskj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fe.asd995.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ge.yuexingan06.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vu.shxzskj.cn

Ruby: def greet(name = "World") = name
来源：http://kz.yuexingan06.cn

C#:   string Greet(string name = "World") => name;
来源：http://ki.bookmarksfly.cn

[C03] 可变参数
来源：http://cs.nicolike.cn

Py:   def total(*args): return sum(args)
来源：http://mx.panjiajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pr.huanxung.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ht.bjjhwx.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ug.muxihuayi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vc.yuntaijiaju.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://up.jianghongdianzi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://po.bookmarksfly.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zo.521024.cn

[C04] 命名参数 / 关键字参数
来源：http://fv.muxihuayi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sz.bookmarksfly.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ue.bookmarksfly.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xa.huixiangedu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://eu.lnxyls.cn

Java: // 无：用 Builder 模式或 record
来源：http://tu.wgjwhj.cn

Go:   // 无：用配置结构体参数
来源：http://qn.wgjwhj.cn

Ruby: f(a: 1, b: 2)
来源：http://wn.hahajie.cn

C#:   f(a: 1, b: 2)
来源：http://wh.jctech888.com.cn

[C05] 返回多个值
来源：http://lf.yuexingan06.cn

Py:   return a, b
来源：http://da.szsharing.cn

PHP:  return [$a, $b];
来源：http://ie.gzmigu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ut.shtwfgs.cn

TS:   return { a, b };
来源：http://bj.shxzskj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xt.bjjhwx.cn

Go:   return a, b
来源：http://nl.newstarts.cn

Ruby: return a, b
来源：http://pf.asd995.cn

C#:   return (a, b);              // ValueTuple
来源：http://yb.9csxet.cn

[C06] 匿名函数 / lambda
来源：http://jq.nszjky.cn

Py:   square = lambda x: x * x
来源：http://rm.9csxet.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ar.huixiangedu.cn

JS:   const square = x => x * x;
来源：http://ey.hahajie.cn

TS:   const square = (x: number): number => x * x;
来源：http://ev.panjiajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://es.jianghongdianzi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rw.shxzukj.cn

Ruby: square = ->(x) { x * x }
来源：http://ub.bjjhwx.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fd.hnjuh.cn

[C07] 把函数作为参数传入
来源：http://ui.huanxung.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ju.shxzukj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://va.hahajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xn.hahajie.cn

TS:   arr.map(String)
来源：http://sz.szxytkj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xo.lnxyls.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jg.shxzukj.cn

Ruby: arr.map(&:upcase)
来源：http://ph.yuexingan06.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mh.huanxung.cn

[C08] 闭包
来源：http://yk.shxzskj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ql.haigaiapp.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gb.asd995.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zf.yuntaijiaju.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vf.newstarts.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rc.lnxyls.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ch.lnxyls.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dj.huixinmuqiang.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gx.jctech888.com.cn

[C09] 递归
来源：http://jj.huixinmuqiang.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tm.asd995.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://iz.nszjky.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yf.bjjhwx.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yw.hahajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tp.9csxet.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cm.jctech888.com.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rs.lnxyls.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wj.nicolike.cn

[C10] 变量作用域
来源：http://rp.yuntaijiaju.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yh.shxzskj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jj.yuntaijiaju.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://on.nicolike.cn

TS:   同 JS
来源：http://zg.521024.cn

Java: 方法内为块级作用域
来源：http://sj.nszjky.cn

Go:   花括号块级作用域
来源：http://ma.9csxet.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zv.hahajie.cn

C#:   块级作用域
来源：http://hl.gzmigu.cn

[C11] 模块导入与导出
来源：http://pt.bookmarksfly.cn

Py:   from module import func
来源：http://ab.jianghongdianzi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wl.shxzukj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://xt.yuntaijiaju.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://it.yuntaijiaju.cn

Java: import java.util.List;
来源：http://ba.newstarts.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vj.jctech888.com.cn

Ruby: require "json"; require_relative "./util"
来源：http://no.9csxet.cn

C#:   using System.Text;
来源：http://jf.haigaiapp.cn

[C12] 立即执行函数 IIFE
来源：http://ny.9csxet.cn

Py:   (lambda: print("run"))()
来源：http://os.hahajie.cn

PHP:  (function () { echo "run"; })();
来源：http://yb.yuntaijiaju.cn

JS:   (() => { console.log("run"); })();
来源：http://bg.asd995.cn

TS:   (() => { console.log("run"); })();
来源：http://sr.lnxyls.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rn.wgjwhj.cn

Go:   func() { fmt.Println("run") }()
来源：http://pr.521024.cn

Ruby: -> { puts "run" }.call
来源：http://zg.bookmarksfly.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pw.muxihuayi.cn

[C13] 类型声明 / 类型注解
来源：http://zn.bjjhwx.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kw.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://id.panjiajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://oq.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qd.chemitech.net.cn

Java: int add(int a, int b) { return a + b; }
来源：http://gz.9csxet.cn

Go:   func add(a, b int) int
来源：http://uw.hahajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bj.lnxyls.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fl.bjjhwx.cn

[C14] 泛型函数
来源：http://up.muxihuayi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fg.huixinmuqiang.cn

PHP:  // 无泛型
来源：http://gz.shxzukj.cn

JS:   // 无泛型
来源：http://mz.newstarts.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ii.9csxet.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jd.huixinmuqiang.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dq.szsharing.cn

Ruby: # 无泛型
来源：http://xe.gzmigu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ku.asd995.cn

[C15] 解构 / 展开参数
来源：http://pz.huanxung.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tv.hahajie.cn

PHP:  [$a, $b] = $pair;
来源：http://je.szsharing.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bi.yuexingan06.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wf.521024.cn

Java: // 无解构
来源：http://wm.yuntaijiaju.cn

Go:   // 无解构
来源：http://iz.yuexingan06.cn

Ruby: a, b = pair
来源：http://ze.gzmigu.cn

C#:   var (a, b) = pair;
来源：http://hq.hahajie.cn

[C16] 函数 / 方法重载
来源：http://mq.muxihuayi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fw.lnxyls.cn

PHP:  // 无重载
来源：http://ko.newstarts.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://um.huanxung.cn

TS:   // 用联合类型或重载签名声明
来源：http://za.colortex.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://fy.bjjhwx.cn


<!-- 参考信息 -->