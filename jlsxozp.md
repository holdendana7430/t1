代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://mu.panjiajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lw.wgjwhj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ph.haigaiapp.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://hd.chemitech.net.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tz.bookmarksfly.cn

================================================================================
来源：http://ec.gzmigu.cn

B. 流程控制
来源：http://nk.hnjuh.cn

================================================================================
来源：http://ke.hnjuh.cn

[B01] 条件判断 if / else
来源：http://xo.bjjhwx.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ge.yuntaijiaju.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://uq.9csxet.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tj.huanxung.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pn.szxytkj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://sk.lnxyls.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cp.szxytkj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mr.panjiajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yn.huixiangedu.cn

[B02] 多分支 else if / elif
来源：http://kd.huixiangedu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ju.chemitech.net.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qe.hnjuh.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fi.haigaiapp.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sc.521024.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ju.jctech888.com.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wy.bookmarksfly.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zn.huanxung.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bv.gzmigu.cn

[B03] switch / match / case
来源：http://we.gzmigu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vh.yuexingan06.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cw.asd995.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ps.bjjhwx.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ue.shxzukj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zs.colortex.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hh.jianghongdianzi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mw.colortex.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kh.szsharing.cn

[B04] for 计数循环
来源：http://jl.muxihuayi.cn

Py:   for i in range(10): print(i)
来源：http://iy.shxzukj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rz.nszjky.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jy.hahajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rg.muxihuayi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fu.shxzukj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rh.colortex.cn

Ruby: 10.times { |i| puts i }
来源：http://hv.colortex.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fs.shtwfgs.cn

[B05] 遍历数组 / 列表
来源：http://kw.huixinmuqiang.cn

Py:   for item in arr: print(item)
来源：http://bh.huixinmuqiang.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ni.colortex.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://rn.szxytkj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ii.huanxung.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gz.haigaiapp.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ss.szxytkj.cn

Ruby: arr.each { |item| puts item }
来源：http://ux.yuntaijiaju.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://us.haigaiapp.cn

[B06] 遍历字典 / 对象
来源：http://xd.muxihuayi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mu.chemitech.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vs.nszjky.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xo.chemitech.net.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ga.haigaiapp.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jt.shxzskj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zn.bookmarksfly.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ow.nicolike.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dd.yuntaijiaju.cn

[B07] while 循环
来源：http://wr.jctech888.com.cn

Py:   while i < 10: i += 1
来源：http://sy.bookmarksfly.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zj.wgjwhj.cn

JS:   while (i < 10) { i++; }
来源：http://xt.huixinmuqiang.cn

TS:   while (i < 10) { i++; }
来源：http://kp.asd995.cn

Java: while (i < 10) { i++; }
来源：http://rc.muxihuayi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qw.haigaiapp.cn

Ruby: while i < 10; i += 1; end
来源：http://zy.yuexingan06.cn

C#:   while (i < 10) { i++; }
来源：http://qz.shtwfgs.cn

[B08] do-while（至少执行一次）
来源：http://wg.colortex.cn

Py:   # 无 do-while：用 while True + break
来源：http://lh.hahajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://hu.huixinmuqiang.cn

JS:   do { i++; } while (i < 10);
来源：http://ic.521024.cn

TS:   do { i++; } while (i < 10);
来源：http://qm.bjjhwx.cn

Java: do { i++; } while (i < 10);
来源：http://mg.muxihuayi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://rl.yuntaijiaju.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qu.521024.cn

C#:   do { i++; } while (i < 10);
来源：http://bq.asd995.cn

[B09] break 与 continue
来源：http://ej.shxzskj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ui.huixiangedu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://su.shxzskj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vu.shxzskj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fc.asd995.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ur.9csxet.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qs.asd995.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://es.shtwfgs.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bb.panjiajie.cn

[B10] 遍历同时拿索引
来源：http://mt.szsharing.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pr.nicolike.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kl.hahajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hb.lnxyls.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ug.shxzskj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qz.yuntaijiaju.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xa.521024.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://da.szxytkj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rc.haigaiapp.cn

[B11] 生成数字序列 / 区间
来源：http://ht.wgjwhj.cn

Py:   list(range(0, 10, 2))
来源：http://os.shxzukj.cn

PHP:  range(0, 10, 2);
来源：http://xr.bookmarksfly.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yz.huixinmuqiang.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uc.colortex.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hw.shtwfgs.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nq.jianghongdianzi.cn

Ruby: (0...10).step(2).to_a
来源：http://rs.jctech888.com.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cy.wgjwhj.cn

[B12] 跳出多层循环
来源：http://di.haigaiapp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yo.jctech888.com.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ll.szxytkj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vr.huixinmuqiang.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pv.yuexingan06.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vd.huanxung.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jo.shtwfgs.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sn.9csxet.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dg.wgjwhj.cn

[B13] 判断是否为数字
来源：http://eq.shxzskj.cn

Py:   isinstance(x, (int, float))
来源：http://jw.nszjky.cn

PHP:  is_numeric($x)
来源：http://ue.shxzukj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://km.yuexingan06.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mm.huixiangedu.cn

Java: x instanceof Number
来源：http://dw.hahajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://oy.jianghongdianzi.cn

Ruby: x.is_a?(Numeric)
来源：http://st.chemitech.net.cn

C#:   x is int or double or decimal
来源：http://xt.huanxung.cn

[B14] 判断值是否在集合内
来源：http://hg.szxytkj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://np.yuexingan06.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wv.jctech888.com.cn

JS:   [1, 2, 3].includes(x)
来源：http://tw.shxzukj.cn

TS:   [1, 2, 3].includes(x)
来源：http://nd.521024.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://yf.9csxet.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mj.asd995.cn

Ruby: [1, 2, 3].include?(x)
来源：http://pz.yuexingan06.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://um.lnxyls.cn

[B15] 布尔运算与取反
来源：http://aw.szxytkj.cn

Py:   a and b or not c
来源：http://gv.521024.cn

PHP:  $a && $b || !$c
来源：http://ir.haigaiapp.cn

JS:   a && b || !c
来源：http://wd.huanxung.cn

TS:   a && b || !c
来源：http://zb.panjiajie.cn

Java: a && b || !c
来源：http://dm.asd995.cn

Go:   a && b || !c
来源：http://vl.szxytkj.cn

Ruby: a && b || !c
来源：http://uq.jianghongdianzi.cn

C#:   a && b || !c
来源：http://oy.wgjwhj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xk.panjiajie.cn

Py:   if not data: return
来源：http://hc.jctech888.com.cn

PHP:  if (!$data) { return; }
来源：http://kn.shtwfgs.cn

JS:   if (!data) return;
来源：http://fk.huanxung.cn

TS:   if (!data) return;
来源：http://ed.shtwfgs.cn

Java: if (data == null) return;
来源：http://ik.haigaiapp.cn

Go:   if data == nil { return }
来源：http://ln.521024.cn

Ruby: return if data.nil?
来源：http://ut.huixinmuqiang.cn

C#:   if (data == null) return;
来源：http://bn.newstarts.cn

================================================================================
来源：http://si.huixiangedu.cn

C. 函数与作用域
来源：http://cx.wgjwhj.cn

================================================================================
来源：http://bx.newstarts.cn

[C01] 定义函数
来源：http://ou.lnxyls.cn

Py:   def add(a, b): return a + b
来源：http://ps.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cf.panjiajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://aq.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ub.521024.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://as.chemitech.net.cn

Go:   func add(a, b int) int { return a + b }
来源：http://kr.shxzukj.cn

Ruby: def add(a, b); a + b; end
来源：http://lf.shxzukj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pq.szxytkj.cn

[C02] 默认参数
来源：http://xw.bookmarksfly.cn

Py:   def greet(name="World"): return name
来源：http://vg.chemitech.net.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ms.panjiajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://ts.shxzukj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bf.szsharing.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ri.521024.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://oh.huanxung.cn

Ruby: def greet(name = "World") = name
来源：http://nb.lnxyls.cn

C#:   string Greet(string name = "World") => name;
来源：http://tr.haigaiapp.cn

[C03] 可变参数
来源：http://aj.bookmarksfly.cn

Py:   def total(*args): return sum(args)
来源：http://ya.hahajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bw.chemitech.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dz.szsharing.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hy.bjjhwx.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://na.wgjwhj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rd.bjjhwx.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gn.szsharing.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tl.nicolike.cn

[C04] 命名参数 / 关键字参数
来源：http://zo.9csxet.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://iv.9csxet.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://uh.hahajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dn.nszjky.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ei.nszjky.cn

Java: // 无：用 Builder 模式或 record
来源：http://fh.bookmarksfly.cn

Go:   // 无：用配置结构体参数
来源：http://ut.nszjky.cn

Ruby: f(a: 1, b: 2)
来源：http://wx.huixiangedu.cn

C#:   f(a: 1, b: 2)
来源：http://vc.huixiangedu.cn

[C05] 返回多个值
来源：http://wn.chemitech.net.cn

Py:   return a, b
来源：http://hw.hnjuh.cn

PHP:  return [$a, $b];
来源：http://ip.huixiangedu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yo.yuexingan06.cn

TS:   return { a, b };
来源：http://aa.yuexingan06.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sb.jctech888.com.cn

Go:   return a, b
来源：http://mn.shxzukj.cn

Ruby: return a, b
来源：http://je.9csxet.cn

C#:   return (a, b);              // ValueTuple
来源：http://ag.shxzskj.cn

[C06] 匿名函数 / lambda
来源：http://on.jctech888.com.cn

Py:   square = lambda x: x * x
来源：http://oc.nicolike.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://yf.huanxung.cn

JS:   const square = x => x * x;
来源：http://zo.jctech888.com.cn

TS:   const square = (x: number): number => x * x;
来源：http://jy.asd995.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cb.shxzukj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ig.colortex.cn

Ruby: square = ->(x) { x * x }
来源：http://dj.yuntaijiaju.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ch.hahajie.cn

[C07] 把函数作为参数传入
来源：http://fv.huixinmuqiang.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sy.521024.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ws.szsharing.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://br.panjiajie.cn

TS:   arr.map(String)
来源：http://ii.jctech888.com.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xz.chemitech.net.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pj.shxzukj.cn

Ruby: arr.map(&:upcase)
来源：http://au.panjiajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://oc.bjjhwx.cn

[C08] 闭包
来源：http://oc.muxihuayi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ty.szsharing.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wq.gzmigu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zz.bjjhwx.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fo.bookmarksfly.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ld.yuntaijiaju.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fu.lnxyls.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vc.shxzskj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rj.gzmigu.cn

[C09] 递归
来源：http://tp.jianghongdianzi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jq.yuexingan06.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jc.hnjuh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sf.shxzskj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gm.shxzskj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fr.szxytkj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://df.gzmigu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pn.wgjwhj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dd.hnjuh.cn

[C10] 变量作用域
来源：http://wx.colortex.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wl.9csxet.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wi.shxzskj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ws.colortex.cn

TS:   同 JS
来源：http://il.szxytkj.cn

Java: 方法内为块级作用域
来源：http://aa.shxzskj.cn

Go:   花括号块级作用域
来源：http://hl.shtwfgs.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ey.nszjky.cn

C#:   块级作用域
来源：http://ju.szxytkj.cn

[C11] 模块导入与导出
来源：http://xi.yuexingan06.cn

Py:   from module import func
来源：http://sj.asd995.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ag.bjjhwx.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://au.bookmarksfly.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pb.lnxyls.cn

Java: import java.util.List;
来源：http://ym.jianghongdianzi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zd.szsharing.cn

Ruby: require "json"; require_relative "./util"
来源：http://bp.nicolike.cn

C#:   using System.Text;
来源：http://ol.521024.cn

[C12] 立即执行函数 IIFE
来源：http://td.yuexingan06.cn

Py:   (lambda: print("run"))()
来源：http://jt.521024.cn

PHP:  (function () { echo "run"; })();
来源：http://fc.asd995.cn

JS:   (() => { console.log("run"); })();
来源：http://uh.bjjhwx.cn

TS:   (() => { console.log("run"); })();
来源：http://mb.asd995.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pf.shxzukj.cn

Go:   func() { fmt.Println("run") }()
来源：http://fr.colortex.cn

Ruby: -> { puts "run" }.call
来源：http://vb.lnxyls.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://na.panjiajie.cn

[C13] 类型声明 / 类型注解
来源：http://ol.muxihuayi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gy.muxihuayi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bf.shtwfgs.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rq.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ho.panjiajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://du.jctech888.com.cn

Go:   func add(a, b int) int
来源：http://ow.jianghongdianzi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://an.colortex.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ok.521024.cn

[C14] 泛型函数
来源：http://rg.shtwfgs.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://oi.shxzukj.cn

PHP:  // 无泛型
来源：http://qa.huixinmuqiang.cn

JS:   // 无泛型
来源：http://ki.huixinmuqiang.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hf.szsharing.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ms.chemitech.net.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ga.jianghongdianzi.cn

Ruby: # 无泛型
来源：http://ax.jianghongdianzi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vh.yuntaijiaju.cn

[C15] 解构 / 展开参数
来源：http://do.wgjwhj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lu.huixiangedu.cn

PHP:  [$a, $b] = $pair;
来源：http://tk.huanxung.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jq.haigaiapp.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gn.521024.cn

Java: // 无解构
来源：http://du.szsharing.cn

Go:   // 无解构
来源：http://od.wgjwhj.cn

Ruby: a, b = pair
来源：http://cp.shtwfgs.cn

C#:   var (a, b) = pair;
来源：http://ti.huanxung.cn

[C16] 函数 / 方法重载
来源：http://le.bjjhwx.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gx.jctech888.com.cn

PHP:  // 无重载
来源：http://ic.9csxet.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://mf.haigaiapp.cn

TS:   // 用联合类型或重载签名声明
来源：http://is.szxytkj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gj.hahajie.cn

Go:   // 无重载：用不同函数名
来源：http://rm.wgjwhj.cn

Ruby: # 无重载：靠动态参数
来源：http://eq.521024.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://os.muxihuayi.cn

================================================================================
来源：http://py.szsharing.cn


<!-- 参考信息 -->