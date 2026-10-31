代发 wailian999

[A26] 类型转换总览
来源：http://lk.newstarts.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://iv.newstarts.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lf.newstarts.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://oa.asd995.cn

TS:   Number() String() Boolean() x as number
来源：http://xg.wgjwhj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yj.9csxet.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rm.bookmarksfly.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://di.shxzskj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://in.hahajie.cn

================================================================================
来源：http://aq.panjiajie.cn

B. 流程控制
来源：http://ac.bookmarksfly.cn

================================================================================
来源：http://uz.lnxyls.cn

[B01] 条件判断 if / else
来源：http://mg.szxytkj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://rr.colortex.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://au.jctech888.com.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vq.wgjwhj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qt.hnjuh.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vw.newstarts.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://py.nicolike.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ls.shtwfgs.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://uf.hahajie.cn

[B02] 多分支 else if / elif
来源：http://xn.haigaiapp.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dt.bjjhwx.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gk.hnjuh.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gj.huixiangedu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dx.nicolike.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vt.panjiajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ls.newstarts.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://it.jianghongdianzi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://of.jianghongdianzi.cn

[B03] switch / match / case
来源：http://ko.hahajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qv.haigaiapp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qv.bookmarksfly.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ma.gzmigu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lq.huixinmuqiang.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zm.nszjky.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://je.9csxet.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sz.jianghongdianzi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rm.colortex.cn

[B04] for 计数循环
来源：http://uy.haigaiapp.cn

Py:   for i in range(10): print(i)
来源：http://ma.shxzskj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mq.yuntaijiaju.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rb.shxzskj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://de.shtwfgs.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://as.shxzukj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vu.bjjhwx.cn

Ruby: 10.times { |i| puts i }
来源：http://hg.colortex.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ds.nicolike.cn

[B05] 遍历数组 / 列表
来源：http://po.nicolike.cn

Py:   for item in arr: print(item)
来源：http://nd.panjiajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wz.huanxung.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zy.wgjwhj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://om.hnjuh.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sy.gzmigu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wx.shxzskj.cn

Ruby: arr.each { |item| puts item }
来源：http://nr.lnxyls.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xi.haigaiapp.cn

[B06] 遍历字典 / 对象
来源：http://rh.hahajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://am.colortex.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dc.huixiangedu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tf.wgjwhj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pa.huanxung.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gv.jianghongdianzi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://af.chemitech.net.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://en.shxzskj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wq.nszjky.cn

[B07] while 循环
来源：http://qw.jctech888.com.cn

Py:   while i < 10: i += 1
来源：http://qz.shxzskj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ms.chemitech.net.cn

JS:   while (i < 10) { i++; }
来源：http://ji.huanxung.cn

TS:   while (i < 10) { i++; }
来源：http://kd.muxihuayi.cn

Java: while (i < 10) { i++; }
来源：http://hn.hnjuh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wl.asd995.cn

Ruby: while i < 10; i += 1; end
来源：http://vo.muxihuayi.cn

C#:   while (i < 10) { i++; }
来源：http://pf.521024.cn

[B08] do-while（至少执行一次）
来源：http://dt.nszjky.cn

Py:   # 无 do-while：用 while True + break
来源：http://rh.hahajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://bq.yuntaijiaju.cn

JS:   do { i++; } while (i < 10);
来源：http://vv.szxytkj.cn

TS:   do { i++; } while (i < 10);
来源：http://ro.huanxung.cn

Java: do { i++; } while (i < 10);
来源：http://id.bjjhwx.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ek.nicolike.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pi.huixinmuqiang.cn

C#:   do { i++; } while (i < 10);
来源：http://mf.haigaiapp.cn

[B09] break 与 continue
来源：http://zk.yuexingan06.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ks.jctech888.com.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ib.szxytkj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tj.huixinmuqiang.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xx.yuexingan06.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jk.bjjhwx.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tf.yuntaijiaju.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://og.nicolike.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uq.asd995.cn

[B10] 遍历同时拿索引
来源：http://tu.panjiajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zd.9csxet.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ny.521024.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://je.yuntaijiaju.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bx.lnxyls.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://oc.panjiajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fc.shtwfgs.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ui.chemitech.net.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vd.yuexingan06.cn

[B11] 生成数字序列 / 区间
来源：http://gh.yuexingan06.cn

Py:   list(range(0, 10, 2))
来源：http://zx.huixinmuqiang.cn

PHP:  range(0, 10, 2);
来源：http://yf.newstarts.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ic.newstarts.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mz.muxihuayi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ze.nicolike.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zh.haigaiapp.cn

Ruby: (0...10).step(2).to_a
来源：http://ps.hahajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hy.muxihuayi.cn

[B12] 跳出多层循环
来源：http://pc.bookmarksfly.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wq.wgjwhj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://bi.shxzskj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tf.yuntaijiaju.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://we.hnjuh.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nc.bookmarksfly.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ih.9csxet.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xg.huixiangedu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mv.newstarts.cn

[B13] 判断是否为数字
来源：http://ql.szxytkj.cn

Py:   isinstance(x, (int, float))
来源：http://dv.jianghongdianzi.cn

PHP:  is_numeric($x)
来源：http://lf.hahajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ye.gzmigu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ud.nszjky.cn

Java: x instanceof Number
来源：http://kw.szxytkj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tg.hnjuh.cn

Ruby: x.is_a?(Numeric)
来源：http://uj.panjiajie.cn

C#:   x is int or double or decimal
来源：http://sp.9csxet.cn

[B14] 判断值是否在集合内
来源：http://fw.521024.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dp.shxzskj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://np.gzmigu.cn

JS:   [1, 2, 3].includes(x)
来源：http://yn.bjjhwx.cn

TS:   [1, 2, 3].includes(x)
来源：http://ne.jctech888.com.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://uh.muxihuayi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yn.chemitech.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://hg.521024.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mt.jianghongdianzi.cn

[B15] 布尔运算与取反
来源：http://zq.bjjhwx.cn

Py:   a and b or not c
来源：http://wb.panjiajie.cn

PHP:  $a && $b || !$c
来源：http://ky.huixinmuqiang.cn

JS:   a && b || !c
来源：http://ci.hahajie.cn

TS:   a && b || !c
来源：http://ae.jianghongdianzi.cn

Java: a && b || !c
来源：http://sa.colortex.cn

Go:   a && b || !c
来源：http://nw.hahajie.cn

Ruby: a && b || !c
来源：http://dz.yuntaijiaju.cn

C#:   a && b || !c
来源：http://bp.wgjwhj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://rd.huixinmuqiang.cn

Py:   if not data: return
来源：http://ji.huixinmuqiang.cn

PHP:  if (!$data) { return; }
来源：http://xj.asd995.cn

JS:   if (!data) return;
来源：http://ot.9csxet.cn

TS:   if (!data) return;
来源：http://bv.jctech888.com.cn

Java: if (data == null) return;
来源：http://vf.panjiajie.cn

Go:   if data == nil { return }
来源：http://mi.nszjky.cn

Ruby: return if data.nil?
来源：http://ux.shxzskj.cn

C#:   if (data == null) return;
来源：http://ws.shxzukj.cn

================================================================================
来源：http://ti.bjjhwx.cn

C. 函数与作用域
来源：http://ek.hahajie.cn

================================================================================
来源：http://ls.colortex.cn

[C01] 定义函数
来源：http://hl.521024.cn

Py:   def add(a, b): return a + b
来源：http://ep.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vv.wgjwhj.cn

JS:   function add(a, b) { return a + b; }
来源：http://sg.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lp.lnxyls.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lh.shxzskj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mj.wgjwhj.cn

Ruby: def add(a, b); a + b; end
来源：http://fp.panjiajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ne.shxzskj.cn

[C02] 默认参数
来源：http://hi.haigaiapp.cn

Py:   def greet(name="World"): return name
来源：http://tn.lnxyls.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qk.yuntaijiaju.cn

JS:   function greet(name = "World") { return name; }
来源：http://ms.chemitech.net.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://py.shxzskj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ra.haigaiapp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yr.jctech888.com.cn

Ruby: def greet(name = "World") = name
来源：http://dt.gzmigu.cn

C#:   string Greet(string name = "World") => name;
来源：http://ze.bookmarksfly.cn

[C03] 可变参数
来源：http://av.bjjhwx.cn

Py:   def total(*args): return sum(args)
来源：http://fe.jctech888.com.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qu.huixinmuqiang.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://we.chemitech.net.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://oa.panjiajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yv.nicolike.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zz.shxzskj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ez.newstarts.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cf.lnxyls.cn

[C04] 命名参数 / 关键字参数
来源：http://cx.hnjuh.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jo.szsharing.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tk.asd995.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ma.521024.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qj.lnxyls.cn

Java: // 无：用 Builder 模式或 record
来源：http://bb.huixinmuqiang.cn

Go:   // 无：用配置结构体参数
来源：http://ht.nszjky.cn

Ruby: f(a: 1, b: 2)
来源：http://sq.shxzukj.cn

C#:   f(a: 1, b: 2)
来源：http://xn.huixinmuqiang.cn

[C05] 返回多个值
来源：http://da.newstarts.cn

Py:   return a, b
来源：http://xr.hahajie.cn

PHP:  return [$a, $b];
来源：http://hl.panjiajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://cc.muxihuayi.cn

TS:   return { a, b };
来源：http://ds.wgjwhj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ja.wgjwhj.cn

Go:   return a, b
来源：http://lf.gzmigu.cn

Ruby: return a, b
来源：http://vk.chemitech.net.cn

C#:   return (a, b);              // ValueTuple
来源：http://lp.hnjuh.cn

[C06] 匿名函数 / lambda
来源：http://wz.gzmigu.cn

Py:   square = lambda x: x * x
来源：http://aw.huixiangedu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xp.asd995.cn

JS:   const square = x => x * x;
来源：http://yk.hnjuh.cn

TS:   const square = (x: number): number => x * x;
来源：http://kj.9csxet.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://re.lnxyls.cn

Go:   sq := func(x int) int { return x * x }
来源：http://lo.lnxyls.cn

Ruby: square = ->(x) { x * x }
来源：http://qy.wgjwhj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ow.asd995.cn

[C07] 把函数作为参数传入
来源：http://rd.asd995.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ay.haigaiapp.cn

PHP:  array_map("strtoupper", $arr);
来源：http://pd.muxihuayi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://do.nszjky.cn

TS:   arr.map(String)
来源：http://zh.asd995.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wi.shtwfgs.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nv.huixinmuqiang.cn

Ruby: arr.map(&:upcase)
来源：http://em.szsharing.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://au.wgjwhj.cn

[C08] 闭包
来源：http://of.colortex.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hq.newstarts.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uo.asd995.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ik.521024.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hf.bjjhwx.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://or.huanxung.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jz.muxihuayi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ch.shxzskj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xe.szxytkj.cn

[C09] 递归
来源：http://qe.yuntaijiaju.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hy.bjjhwx.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zs.yuntaijiaju.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gu.hahajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ub.colortex.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yi.szxytkj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uh.shxzukj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sf.asd995.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ff.asd995.cn

[C10] 变量作用域
来源：http://dn.hahajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dk.9csxet.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zh.chemitech.net.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kb.jianghongdianzi.cn

TS:   同 JS
来源：http://ub.jctech888.com.cn

Java: 方法内为块级作用域
来源：http://uc.nicolike.cn

Go:   花括号块级作用域
来源：http://yo.521024.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tf.bjjhwx.cn

C#:   块级作用域
来源：http://jo.huanxung.cn

[C11] 模块导入与导出
来源：http://fk.muxihuayi.cn

Py:   from module import func
来源：http://gm.haigaiapp.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ls.newstarts.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ss.521024.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uy.yuntaijiaju.cn

Java: import java.util.List;
来源：http://jn.colortex.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://um.huanxung.cn

Ruby: require "json"; require_relative "./util"
来源：http://zq.shxzskj.cn

C#:   using System.Text;
来源：http://er.hnjuh.cn

[C12] 立即执行函数 IIFE
来源：http://bt.yuexingan06.cn

Py:   (lambda: print("run"))()
来源：http://ru.shxzukj.cn

PHP:  (function () { echo "run"; })();
来源：http://jf.lnxyls.cn

JS:   (() => { console.log("run"); })();
来源：http://ol.chemitech.net.cn

TS:   (() => { console.log("run"); })();
来源：http://la.bjjhwx.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ft.muxihuayi.cn

Go:   func() { fmt.Println("run") }()
来源：http://fh.shtwfgs.cn

Ruby: -> { puts "run" }.call
来源：http://ms.nszjky.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://kz.yuexingan06.cn

[C13] 类型声明 / 类型注解
来源：http://xn.muxihuayi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qw.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://un.lnxyls.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://my.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qx.colortex.cn

Java: int add(int a, int b) { return a + b; }
来源：http://zs.asd995.cn

Go:   func add(a, b int) int
来源：http://bt.yuntaijiaju.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zn.szxytkj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ds.newstarts.cn

[C14] 泛型函数
来源：http://ep.hahajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ps.521024.cn

PHP:  // 无泛型
来源：http://gp.hnjuh.cn

JS:   // 无泛型
来源：http://nq.asd995.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tx.wgjwhj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fv.haigaiapp.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ri.hnjuh.cn

Ruby: # 无泛型
来源：http://tj.gzmigu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yc.lnxyls.cn

[C15] 解构 / 展开参数
来源：http://ta.szsharing.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fb.panjiajie.cn

PHP:  [$a, $b] = $pair;
来源：http://sg.nszjky.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pt.jctech888.com.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yt.shtwfgs.cn

Java: // 无解构
来源：http://ey.colortex.cn

Go:   // 无解构
来源：http://ta.lnxyls.cn

Ruby: a, b = pair
来源：http://rw.haigaiapp.cn

C#:   var (a, b) = pair;
来源：http://ae.colortex.cn

[C16] 函数 / 方法重载
来源：http://xj.huixiangedu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bu.shxzukj.cn

PHP:  // 无重载
来源：http://ij.lnxyls.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://vh.huixiangedu.cn

TS:   // 用联合类型或重载签名声明
来源：http://gs.hnjuh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://yb.newstarts.cn


<!-- 参考信息 -->