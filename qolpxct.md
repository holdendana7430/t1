代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jz.huanxung.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nr.hahajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://nk.huixiangedu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zq.szxytkj.cn

[A26] 类型转换总览
来源：http://vg.nicolike.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://se.yuntaijiaju.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sa.gzmigu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://lc.hahajie.cn

TS:   Number() String() Boolean() x as number
来源：http://ih.muxihuayi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qx.9csxet.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sm.wgjwhj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mv.hnjuh.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://en.chemitech.net.cn

================================================================================
来源：http://yt.yuexingan06.cn

B. 流程控制
来源：http://jj.nszjky.cn

================================================================================
来源：http://mr.shxzukj.cn

[B01] 条件判断 if / else
来源：http://kt.bjjhwx.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ru.521024.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pu.hnjuh.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cz.gzmigu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bi.huixinmuqiang.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://la.chemitech.net.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://uh.wgjwhj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gp.gzmigu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ro.haigaiapp.cn

[B02] 多分支 else if / elif
来源：http://wa.9csxet.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rg.bjjhwx.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jo.chemitech.net.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hl.shtwfgs.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://om.asd995.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rr.colortex.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lf.shxzukj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://sd.huixiangedu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ch.521024.cn

[B03] switch / match / case
来源：http://gp.9csxet.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mh.hahajie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dj.newstarts.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cj.chemitech.net.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tr.nicolike.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kl.yuntaijiaju.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ed.chemitech.net.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bw.jianghongdianzi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ia.muxihuayi.cn

[B04] for 计数循环
来源：http://ng.9csxet.cn

Py:   for i in range(10): print(i)
来源：http://ps.9csxet.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bl.hahajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yf.bjjhwx.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vf.yuexingan06.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fj.jianghongdianzi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dg.gzmigu.cn

Ruby: 10.times { |i| puts i }
来源：http://gr.chemitech.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yy.haigaiapp.cn

[B05] 遍历数组 / 列表
来源：http://sn.hnjuh.cn

Py:   for item in arr: print(item)
来源：http://gi.bjjhwx.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://oc.521024.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://lu.colortex.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://eg.wgjwhj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ve.haigaiapp.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mh.shxzukj.cn

Ruby: arr.each { |item| puts item }
来源：http://su.yuntaijiaju.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ko.yuexingan06.cn

[B06] 遍历字典 / 对象
来源：http://ge.shxzskj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://nr.nszjky.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ip.szsharing.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://be.bookmarksfly.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wp.shtwfgs.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mr.bookmarksfly.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yq.wgjwhj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ja.shxzukj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://za.nicolike.cn

[B07] while 循环
来源：http://mf.yuntaijiaju.cn

Py:   while i < 10: i += 1
来源：http://po.wgjwhj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ds.huixinmuqiang.cn

JS:   while (i < 10) { i++; }
来源：http://lf.colortex.cn

TS:   while (i < 10) { i++; }
来源：http://ko.shxzukj.cn

Java: while (i < 10) { i++; }
来源：http://pu.szsharing.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gt.huixiangedu.cn

Ruby: while i < 10; i += 1; end
来源：http://kq.jctech888.com.cn

C#:   while (i < 10) { i++; }
来源：http://mj.shtwfgs.cn

[B08] do-while（至少执行一次）
来源：http://jr.lnxyls.cn

Py:   # 无 do-while：用 while True + break
来源：http://rg.shtwfgs.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://tg.huixinmuqiang.cn

JS:   do { i++; } while (i < 10);
来源：http://vs.wgjwhj.cn

TS:   do { i++; } while (i < 10);
来源：http://hf.nszjky.cn

Java: do { i++; } while (i < 10);
来源：http://kl.wgjwhj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bh.jianghongdianzi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zj.hnjuh.cn

C#:   do { i++; } while (i < 10);
来源：http://qh.nicolike.cn

[B09] break 与 continue
来源：http://gi.huanxung.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sz.hahajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pw.nszjky.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lq.jctech888.com.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sc.bjjhwx.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ai.bookmarksfly.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://by.huanxung.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mc.huixiangedu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bu.colortex.cn

[B10] 遍历同时拿索引
来源：http://vc.yuexingan06.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://at.newstarts.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ay.szsharing.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dx.huanxung.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sd.lnxyls.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mi.szxytkj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fg.521024.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pj.hnjuh.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://it.colortex.cn

[B11] 生成数字序列 / 区间
来源：http://mq.bjjhwx.cn

Py:   list(range(0, 10, 2))
来源：http://jm.gzmigu.cn

PHP:  range(0, 10, 2);
来源：http://xk.colortex.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kd.hahajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nn.colortex.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bs.newstarts.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pu.huixinmuqiang.cn

Ruby: (0...10).step(2).to_a
来源：http://ec.newstarts.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bo.hahajie.cn

[B12] 跳出多层循环
来源：http://rj.panjiajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fj.asd995.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://co.huixiangedu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lw.9csxet.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bq.huixiangedu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wk.muxihuayi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gc.shtwfgs.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://el.huixinmuqiang.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ic.lnxyls.cn

[B13] 判断是否为数字
来源：http://kx.shtwfgs.cn

Py:   isinstance(x, (int, float))
来源：http://eb.nicolike.cn

PHP:  is_numeric($x)
来源：http://ud.szxytkj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xm.jianghongdianzi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xb.521024.cn

Java: x instanceof Number
来源：http://eq.muxihuayi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dc.panjiajie.cn

Ruby: x.is_a?(Numeric)
来源：http://od.hahajie.cn

C#:   x is int or double or decimal
来源：http://wq.shxzukj.cn

[B14] 判断值是否在集合内
来源：http://ac.hnjuh.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kt.chemitech.net.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yc.wgjwhj.cn

JS:   [1, 2, 3].includes(x)
来源：http://tq.huanxung.cn

TS:   [1, 2, 3].includes(x)
来源：http://ui.nicolike.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://yf.jctech888.com.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hb.nszjky.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vs.yuexingan06.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tk.colortex.cn

[B15] 布尔运算与取反
来源：http://ne.huixiangedu.cn

Py:   a and b or not c
来源：http://bw.hahajie.cn

PHP:  $a && $b || !$c
来源：http://kr.muxihuayi.cn

JS:   a && b || !c
来源：http://ua.gzmigu.cn

TS:   a && b || !c
来源：http://vh.panjiajie.cn

Java: a && b || !c
来源：http://xs.521024.cn

Go:   a && b || !c
来源：http://wu.szxytkj.cn

Ruby: a && b || !c
来源：http://lr.yuntaijiaju.cn

C#:   a && b || !c
来源：http://co.shxzukj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://sa.colortex.cn

Py:   if not data: return
来源：http://hg.panjiajie.cn

PHP:  if (!$data) { return; }
来源：http://km.newstarts.cn

JS:   if (!data) return;
来源：http://zl.colortex.cn

TS:   if (!data) return;
来源：http://fx.bookmarksfly.cn

Java: if (data == null) return;
来源：http://fy.jianghongdianzi.cn

Go:   if data == nil { return }
来源：http://se.szxytkj.cn

Ruby: return if data.nil?
来源：http://xi.nszjky.cn

C#:   if (data == null) return;
来源：http://at.bjjhwx.cn

================================================================================
来源：http://eu.bjjhwx.cn

C. 函数与作用域
来源：http://de.colortex.cn

================================================================================
来源：http://gl.yuntaijiaju.cn

[C01] 定义函数
来源：http://va.asd995.cn

Py:   def add(a, b): return a + b
来源：http://nt.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qk.huixinmuqiang.cn

JS:   function add(a, b) { return a + b; }
来源：http://zq.huixinmuqiang.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ol.huixinmuqiang.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://io.panjiajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ef.panjiajie.cn

Ruby: def add(a, b); a + b; end
来源：http://pp.nszjky.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gq.haigaiapp.cn

[C02] 默认参数
来源：http://hj.gzmigu.cn

Py:   def greet(name="World"): return name
来源：http://uo.jctech888.com.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://rf.huixinmuqiang.cn

JS:   function greet(name = "World") { return name; }
来源：http://hh.9csxet.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zx.shxzukj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cf.newstarts.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bl.yuntaijiaju.cn

Ruby: def greet(name = "World") = name
来源：http://kr.shtwfgs.cn

C#:   string Greet(string name = "World") => name;
来源：http://tu.nszjky.cn

[C03] 可变参数
来源：http://cu.hahajie.cn

Py:   def total(*args): return sum(args)
来源：http://if.muxihuayi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hd.gzmigu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zs.yuntaijiaju.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tm.shxzskj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ou.szsharing.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.nicolike.cn

Ruby: def total(*nums); nums.sum; end
来源：http://bw.lnxyls.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://te.huixiangedu.cn

[C04] 命名参数 / 关键字参数
来源：http://ka.lnxyls.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://em.nszjky.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ya.yuntaijiaju.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ru.9csxet.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bt.521024.cn

Java: // 无：用 Builder 模式或 record
来源：http://ck.haigaiapp.cn

Go:   // 无：用配置结构体参数
来源：http://ui.jianghongdianzi.cn

Ruby: f(a: 1, b: 2)
来源：http://pe.shxzskj.cn

C#:   f(a: 1, b: 2)
来源：http://ej.jctech888.com.cn

[C05] 返回多个值
来源：http://pb.szxytkj.cn

Py:   return a, b
来源：http://mf.nszjky.cn

PHP:  return [$a, $b];
来源：http://sk.bookmarksfly.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://rj.panjiajie.cn

TS:   return { a, b };
来源：http://bd.huanxung.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tr.bookmarksfly.cn

Go:   return a, b
来源：http://qt.bjjhwx.cn

Ruby: return a, b
来源：http://mg.szxytkj.cn

C#:   return (a, b);              // ValueTuple
来源：http://yv.hahajie.cn

[C06] 匿名函数 / lambda
来源：http://yj.nszjky.cn

Py:   square = lambda x: x * x
来源：http://xz.hnjuh.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://po.jctech888.com.cn

JS:   const square = x => x * x;
来源：http://yf.muxihuayi.cn

TS:   const square = (x: number): number => x * x;
来源：http://jj.jctech888.com.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qk.chemitech.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://cb.huanxung.cn

Ruby: square = ->(x) { x * x }
来源：http://dn.panjiajie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ox.shxzskj.cn

[C07] 把函数作为参数传入
来源：http://sh.hahajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pq.haigaiapp.cn

PHP:  array_map("strtoupper", $arr);
来源：http://pe.hahajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rn.szsharing.cn

TS:   arr.map(String)
来源：http://ds.huanxung.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hw.chemitech.net.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jq.huixinmuqiang.cn

Ruby: arr.map(&:upcase)
来源：http://ct.wgjwhj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qr.huixinmuqiang.cn

[C08] 闭包
来源：http://tp.521024.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://db.nszjky.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ku.szsharing.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qv.shxzukj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yc.jctech888.com.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vh.yuexingan06.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ux.haigaiapp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gd.shxzskj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pf.szxytkj.cn

[C09] 递归
来源：http://ss.huixinmuqiang.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dr.yuexingan06.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xy.bjjhwx.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zt.muxihuayi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nx.yuntaijiaju.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zu.szxytkj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xm.newstarts.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nb.hahajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://se.jctech888.com.cn

[C10] 变量作用域
来源：http://bn.bookmarksfly.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lg.bjjhwx.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kx.gzmigu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pr.jctech888.com.cn

TS:   同 JS
来源：http://th.jctech888.com.cn

Java: 方法内为块级作用域
来源：http://qs.nicolike.cn

Go:   花括号块级作用域
来源：http://gw.newstarts.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gj.jianghongdianzi.cn

C#:   块级作用域
来源：http://js.asd995.cn

[C11] 模块导入与导出
来源：http://lr.szsharing.cn

Py:   from module import func
来源：http://zm.haigaiapp.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://nn.szsharing.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://td.shtwfgs.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ir.huixiangedu.cn

Java: import java.util.List;
来源：http://ta.szsharing.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ou.szsharing.cn

Ruby: require "json"; require_relative "./util"
来源：http://ut.bookmarksfly.cn

C#:   using System.Text;
来源：http://sr.bookmarksfly.cn

[C12] 立即执行函数 IIFE
来源：http://cz.chemitech.net.cn

Py:   (lambda: print("run"))()
来源：http://zz.yuntaijiaju.cn

PHP:  (function () { echo "run"; })();
来源：http://lr.szsharing.cn

JS:   (() => { console.log("run"); })();
来源：http://pz.panjiajie.cn

TS:   (() => { console.log("run"); })();
来源：http://er.521024.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gu.huanxung.cn

Go:   func() { fmt.Println("run") }()
来源：http://hf.lnxyls.cn

Ruby: -> { puts "run" }.call
来源：http://lb.huanxung.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gh.bjjhwx.cn

[C13] 类型声明 / 类型注解
来源：http://ka.shxzukj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kp.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bd.muxihuayi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bh.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ec.bjjhwx.cn

Java: int add(int a, int b) { return a + b; }
来源：http://lm.521024.cn

Go:   func add(a, b int) int
来源：http://mu.colortex.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wh.gzmigu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qb.bjjhwx.cn

[C14] 泛型函数
来源：http://dr.521024.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hm.521024.cn

PHP:  // 无泛型
来源：http://yv.shtwfgs.cn

JS:   // 无泛型
来源：http://kv.huixinmuqiang.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yh.nicolike.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://oz.newstarts.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cq.shxzskj.cn

Ruby: # 无泛型
来源：http://gf.yuntaijiaju.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xz.huanxung.cn

[C15] 解构 / 展开参数
来源：http://tk.521024.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ri.panjiajie.cn

PHP:  [$a, $b] = $pair;
来源：http://ss.nszjky.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hc.jianghongdianzi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sl.hnjuh.cn

Java: // 无解构
来源：http://ex.panjiajie.cn

Go:   // 无解构
来源：http://dz.huanxung.cn

Ruby: a, b = pair
来源：http://cn.chemitech.net.cn

C#:   var (a, b) = pair;
来源：http://sf.muxihuayi.cn

[C16] 函数 / 方法重载
来源：http://pu.nicolike.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yf.nszjky.cn


<!-- 参考信息 -->