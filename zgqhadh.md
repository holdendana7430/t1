代发 wailian999

[A26] 类型转换总览
来源：http://pd.huixinmuqiang.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bt.nszjky.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qf.shxzukj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dd.asd995.cn

TS:   Number() String() Boolean() x as number
来源：http://hw.shxzskj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mt.521024.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cz.521024.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://bt.szxytkj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hr.bjjhwx.cn

================================================================================
来源：http://jg.colortex.cn

B. 流程控制
来源：http://un.muxihuayi.cn

================================================================================
来源：http://mu.yuntaijiaju.cn

[B01] 条件判断 if / else
来源：http://rf.panjiajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://rw.wgjwhj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ux.lnxyls.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ul.panjiajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kj.chemitech.net.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bm.bookmarksfly.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ad.szxytkj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://np.bookmarksfly.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cn.yuntaijiaju.cn

[B02] 多分支 else if / elif
来源：http://yp.yuexingan06.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tu.bjjhwx.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://az.shxzskj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hm.muxihuayi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cs.jctech888.com.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sq.yuexingan06.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ra.asd995.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rp.bjjhwx.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sk.521024.cn

[B03] switch / match / case
来源：http://fu.jianghongdianzi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wa.gzmigu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ay.shtwfgs.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pt.shxzukj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ez.jianghongdianzi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jt.nszjky.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://md.muxihuayi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ld.nicolike.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://oo.jianghongdianzi.cn

[B04] for 计数循环
来源：http://dn.521024.cn

Py:   for i in range(10): print(i)
来源：http://cb.newstarts.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lt.shtwfgs.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dw.521024.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ny.gzmigu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mk.muxihuayi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gu.gzmigu.cn

Ruby: 10.times { |i| puts i }
来源：http://bg.huixiangedu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dx.huixinmuqiang.cn

[B05] 遍历数组 / 列表
来源：http://rz.haigaiapp.cn

Py:   for item in arr: print(item)
来源：http://rd.colortex.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ka.huixinmuqiang.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ay.panjiajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ro.jctech888.com.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wv.yuexingan06.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zn.wgjwhj.cn

Ruby: arr.each { |item| puts item }
来源：http://vn.bjjhwx.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mv.panjiajie.cn

[B06] 遍历字典 / 对象
来源：http://yb.muxihuayi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ug.newstarts.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nt.lnxyls.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qg.huixinmuqiang.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fh.9csxet.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pv.newstarts.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xk.jianghongdianzi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yo.chemitech.net.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://og.huixinmuqiang.cn

[B07] while 循环
来源：http://xk.nszjky.cn

Py:   while i < 10: i += 1
来源：http://sp.chemitech.net.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ph.newstarts.cn

JS:   while (i < 10) { i++; }
来源：http://bd.haigaiapp.cn

TS:   while (i < 10) { i++; }
来源：http://em.asd995.cn

Java: while (i < 10) { i++; }
来源：http://yd.huixiangedu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cz.panjiajie.cn

Ruby: while i < 10; i += 1; end
来源：http://xr.bjjhwx.cn

C#:   while (i < 10) { i++; }
来源：http://ii.newstarts.cn

[B08] do-while（至少执行一次）
来源：http://dj.panjiajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://if.colortex.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ny.hahajie.cn

JS:   do { i++; } while (i < 10);
来源：http://qc.newstarts.cn

TS:   do { i++; } while (i < 10);
来源：http://uf.haigaiapp.cn

Java: do { i++; } while (i < 10);
来源：http://ym.wgjwhj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sc.wgjwhj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://et.shtwfgs.cn

C#:   do { i++; } while (i < 10);
来源：http://ux.asd995.cn

[B09] break 与 continue
来源：http://tj.9csxet.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://at.bjjhwx.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ji.yuexingan06.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mh.asd995.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://em.9csxet.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://an.huixinmuqiang.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jt.panjiajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://oj.muxihuayi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jn.lnxyls.cn

[B10] 遍历同时拿索引
来源：http://ag.9csxet.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gw.gzmigu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ry.nicolike.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rx.yuntaijiaju.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://id.colortex.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://el.bookmarksfly.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uu.jctech888.com.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bx.jctech888.com.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ge.asd995.cn

[B11] 生成数字序列 / 区间
来源：http://xq.bjjhwx.cn

Py:   list(range(0, 10, 2))
来源：http://us.panjiajie.cn

PHP:  range(0, 10, 2);
来源：http://xs.nicolike.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://co.wgjwhj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xs.szxytkj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hy.muxihuayi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zf.huixiangedu.cn

Ruby: (0...10).step(2).to_a
来源：http://lp.jctech888.com.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lo.shxzukj.cn

[B12] 跳出多层循环
来源：http://gb.521024.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ic.lnxyls.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://sl.jctech888.com.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://si.lnxyls.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xo.haigaiapp.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://um.gzmigu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jl.panjiajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bt.huixinmuqiang.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gz.jctech888.com.cn

[B13] 判断是否为数字
来源：http://oz.bookmarksfly.cn

Py:   isinstance(x, (int, float))
来源：http://bo.asd995.cn

PHP:  is_numeric($x)
来源：http://ok.muxihuayi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oo.asd995.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wl.huixiangedu.cn

Java: x instanceof Number
来源：http://uw.shxzukj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nv.szsharing.cn

Ruby: x.is_a?(Numeric)
来源：http://he.newstarts.cn

C#:   x is int or double or decimal
来源：http://sf.newstarts.cn

[B14] 判断值是否在集合内
来源：http://da.panjiajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nj.colortex.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fz.newstarts.cn

JS:   [1, 2, 3].includes(x)
来源：http://qy.jianghongdianzi.cn

TS:   [1, 2, 3].includes(x)
来源：http://bh.nicolike.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ic.nicolike.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cz.jianghongdianzi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ft.yuntaijiaju.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uz.newstarts.cn

[B15] 布尔运算与取反
来源：http://qy.colortex.cn

Py:   a and b or not c
来源：http://tc.jianghongdianzi.cn

PHP:  $a && $b || !$c
来源：http://lv.521024.cn

JS:   a && b || !c
来源：http://um.muxihuayi.cn

TS:   a && b || !c
来源：http://xi.yuntaijiaju.cn

Java: a && b || !c
来源：http://rv.huanxung.cn

Go:   a && b || !c
来源：http://jj.haigaiapp.cn

Ruby: a && b || !c
来源：http://pf.bjjhwx.cn

C#:   a && b || !c
来源：http://yi.chemitech.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://pm.muxihuayi.cn

Py:   if not data: return
来源：http://yz.jctech888.com.cn

PHP:  if (!$data) { return; }
来源：http://jc.wgjwhj.cn

JS:   if (!data) return;
来源：http://ss.colortex.cn

TS:   if (!data) return;
来源：http://ak.shxzukj.cn

Java: if (data == null) return;
来源：http://zs.muxihuayi.cn

Go:   if data == nil { return }
来源：http://iy.wgjwhj.cn

Ruby: return if data.nil?
来源：http://qv.lnxyls.cn

C#:   if (data == null) return;
来源：http://co.yuexingan06.cn

================================================================================
来源：http://go.chemitech.net.cn

C. 函数与作用域
来源：http://gh.haigaiapp.cn

================================================================================
来源：http://qk.huixiangedu.cn

[C01] 定义函数
来源：http://vj.nszjky.cn

Py:   def add(a, b): return a + b
来源：http://jt.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ul.yuexingan06.cn

JS:   function add(a, b) { return a + b; }
来源：http://wu.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nm.yuntaijiaju.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wc.hnjuh.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ye.shxzukj.cn

Ruby: def add(a, b); a + b; end
来源：http://jt.panjiajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hs.huixinmuqiang.cn

[C02] 默认参数
来源：http://ms.nicolike.cn

Py:   def greet(name="World"): return name
来源：http://qv.yuexingan06.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tk.wgjwhj.cn

JS:   function greet(name = "World") { return name; }
来源：http://dw.haigaiapp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yi.haigaiapp.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://mx.haigaiapp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://oa.gzmigu.cn

Ruby: def greet(name = "World") = name
来源：http://xm.newstarts.cn

C#:   string Greet(string name = "World") => name;
来源：http://ha.muxihuayi.cn

[C03] 可变参数
来源：http://vu.newstarts.cn

Py:   def total(*args): return sum(args)
来源：http://io.nszjky.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qv.nicolike.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dc.asd995.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uv.haigaiapp.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ms.jianghongdianzi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vr.newstarts.cn

Ruby: def total(*nums); nums.sum; end
来源：http://uw.szxytkj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hg.nicolike.cn

[C04] 命名参数 / 关键字参数
来源：http://zt.yuexingan06.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hy.nicolike.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://av.yuntaijiaju.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wd.haigaiapp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://an.colortex.cn

Java: // 无：用 Builder 模式或 record
来源：http://kf.wgjwhj.cn

Go:   // 无：用配置结构体参数
来源：http://dx.gzmigu.cn

Ruby: f(a: 1, b: 2)
来源：http://wq.lnxyls.cn

C#:   f(a: 1, b: 2)
来源：http://ks.szxytkj.cn

[C05] 返回多个值
来源：http://dz.yuexingan06.cn

Py:   return a, b
来源：http://vj.asd995.cn

PHP:  return [$a, $b];
来源：http://bs.shtwfgs.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://bm.nicolike.cn

TS:   return { a, b };
来源：http://pk.jianghongdianzi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://za.yuexingan06.cn

Go:   return a, b
来源：http://qo.newstarts.cn

Ruby: return a, b
来源：http://ii.lnxyls.cn

C#:   return (a, b);              // ValueTuple
来源：http://pt.asd995.cn

[C06] 匿名函数 / lambda
来源：http://tk.colortex.cn

Py:   square = lambda x: x * x
来源：http://ve.asd995.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://uf.yuexingan06.cn

JS:   const square = x => x * x;
来源：http://dp.muxihuayi.cn

TS:   const square = (x: number): number => x * x;
来源：http://uk.shtwfgs.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://en.bookmarksfly.cn

Go:   sq := func(x int) int { return x * x }
来源：http://um.asd995.cn

Ruby: square = ->(x) { x * x }
来源：http://hm.hnjuh.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ja.shxzukj.cn

[C07] 把函数作为参数传入
来源：http://ek.muxihuayi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mf.hahajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://gf.haigaiapp.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ad.gzmigu.cn

TS:   arr.map(String)
来源：http://sn.jianghongdianzi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xe.asd995.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rk.shxzukj.cn

Ruby: arr.map(&:upcase)
来源：http://pd.bookmarksfly.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://de.colortex.cn

[C08] 闭包
来源：http://rk.chemitech.net.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://by.wgjwhj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ug.gzmigu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://je.huanxung.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zj.nicolike.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mt.huanxung.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ej.panjiajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dw.bjjhwx.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gq.chemitech.net.cn

[C09] 递归
来源：http://jf.szxytkj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://iw.bookmarksfly.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hs.chemitech.net.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ja.gzmigu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kw.newstarts.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bh.huixinmuqiang.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ki.muxihuayi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://de.nszjky.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://br.yuexingan06.cn

[C10] 变量作用域
来源：http://hj.521024.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xq.chemitech.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hf.bjjhwx.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hy.lnxyls.cn

TS:   同 JS
来源：http://ic.yuntaijiaju.cn

Java: 方法内为块级作用域
来源：http://ih.gzmigu.cn

Go:   花括号块级作用域
来源：http://zh.yuntaijiaju.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xf.bjjhwx.cn

C#:   块级作用域
来源：http://ps.yuexingan06.cn

[C11] 模块导入与导出
来源：http://hh.muxihuayi.cn

Py:   from module import func
来源：http://be.panjiajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bc.asd995.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://wy.szxytkj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gq.shxzskj.cn

Java: import java.util.List;
来源：http://ys.panjiajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pe.newstarts.cn

Ruby: require "json"; require_relative "./util"
来源：http://kc.gzmigu.cn

C#:   using System.Text;
来源：http://gc.lnxyls.cn

[C12] 立即执行函数 IIFE
来源：http://rk.asd995.cn

Py:   (lambda: print("run"))()
来源：http://rs.521024.cn

PHP:  (function () { echo "run"; })();
来源：http://jd.nicolike.cn

JS:   (() => { console.log("run"); })();
来源：http://pe.asd995.cn

TS:   (() => { console.log("run"); })();
来源：http://eh.shtwfgs.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bi.asd995.cn

Go:   func() { fmt.Println("run") }()
来源：http://pa.bjjhwx.cn

Ruby: -> { puts "run" }.call
来源：http://ac.yuexingan06.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ei.huanxung.cn

[C13] 类型声明 / 类型注解
来源：http://gi.huanxung.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jg.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ql.panjiajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ej.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mc.colortex.cn

Java: int add(int a, int b) { return a + b; }
来源：http://gd.huanxung.cn

Go:   func add(a, b int) int
来源：http://lp.huixiangedu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uw.huixinmuqiang.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fn.yuexingan06.cn

[C14] 泛型函数
来源：http://fu.9csxet.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bg.huixinmuqiang.cn

PHP:  // 无泛型
来源：http://fe.hnjuh.cn

JS:   // 无泛型
来源：http://nl.huixinmuqiang.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jt.colortex.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ik.haigaiapp.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fl.asd995.cn

Ruby: # 无泛型
来源：http://hl.wgjwhj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ki.nicolike.cn

[C15] 解构 / 展开参数
来源：http://os.nicolike.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qq.huixinmuqiang.cn

PHP:  [$a, $b] = $pair;
来源：http://ka.yuntaijiaju.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zd.huixiangedu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wa.szsharing.cn

Java: // 无解构
来源：http://ol.jianghongdianzi.cn

Go:   // 无解构
来源：http://jq.wgjwhj.cn

Ruby: a, b = pair
来源：http://ce.huixinmuqiang.cn

C#:   var (a, b) = pair;
来源：http://rp.nicolike.cn

[C16] 函数 / 方法重载
来源：http://tp.huanxung.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ov.chemitech.net.cn

PHP:  // 无重载
来源：http://ux.wgjwhj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zp.jctech888.com.cn

TS:   // 用联合类型或重载签名声明
来源：http://pv.shxzskj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://kl.huixinmuqiang.cn


<!-- 参考信息 -->