代发 wailian999

[A26] 类型转换总览
来源：http://ki.shxzukj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xt.muxihuayi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ir.shxzukj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mf.shxzukj.cn

TS:   Number() String() Boolean() x as number
来源：http://og.nicolike.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xj.huixiangedu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ay.nszjky.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://en.jianghongdianzi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vv.lnxyls.cn

================================================================================
来源：http://ma.bookmarksfly.cn

B. 流程控制
来源：http://uj.newstarts.cn

================================================================================
来源：http://am.wgjwhj.cn

[B01] 条件判断 if / else
来源：http://mk.haigaiapp.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xl.szxytkj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ty.szxytkj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jh.shtwfgs.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kr.asd995.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ki.huanxung.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bw.wgjwhj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cq.521024.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hg.panjiajie.cn

[B02] 多分支 else if / elif
来源：http://md.huanxung.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://no.huixiangedu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fq.bjjhwx.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hr.bjjhwx.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sc.asd995.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oz.chemitech.net.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ud.huixiangedu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ch.asd995.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ol.huixinmuqiang.cn

[B03] switch / match / case
来源：http://wr.521024.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://if.lnxyls.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xg.shxzukj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vg.jianghongdianzi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mt.shxzskj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bg.wgjwhj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tw.nszjky.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://po.bjjhwx.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ey.haigaiapp.cn

[B04] for 计数循环
来源：http://xi.shxzukj.cn

Py:   for i in range(10): print(i)
来源：http://xn.szxytkj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xf.colortex.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ja.panjiajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wc.yuexingan06.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qd.nszjky.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bc.shtwfgs.cn

Ruby: 10.times { |i| puts i }
来源：http://up.muxihuayi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xt.nszjky.cn

[B05] 遍历数组 / 列表
来源：http://pa.haigaiapp.cn

Py:   for item in arr: print(item)
来源：http://dp.hahajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kl.muxihuayi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://sn.haigaiapp.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://zv.bjjhwx.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sl.asd995.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pz.shxzukj.cn

Ruby: arr.each { |item| puts item }
来源：http://tn.9csxet.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hf.huixiangedu.cn

[B06] 遍历字典 / 对象
来源：http://wd.gzmigu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pd.muxihuayi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pj.wgjwhj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dr.panjiajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ou.9csxet.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lf.shxzukj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pf.9csxet.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nr.lnxyls.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ap.huanxung.cn

[B07] while 循环
来源：http://ez.yuexingan06.cn

Py:   while i < 10: i += 1
来源：http://ls.newstarts.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gf.colortex.cn

JS:   while (i < 10) { i++; }
来源：http://ld.gzmigu.cn

TS:   while (i < 10) { i++; }
来源：http://ng.muxihuayi.cn

Java: while (i < 10) { i++; }
来源：http://lv.shtwfgs.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bg.jctech888.com.cn

Ruby: while i < 10; i += 1; end
来源：http://kk.lnxyls.cn

C#:   while (i < 10) { i++; }
来源：http://be.panjiajie.cn

[B08] do-while（至少执行一次）
来源：http://ui.9csxet.cn

Py:   # 无 do-while：用 while True + break
来源：http://vo.haigaiapp.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://af.lnxyls.cn

JS:   do { i++; } while (i < 10);
来源：http://zp.szsharing.cn

TS:   do { i++; } while (i < 10);
来源：http://bd.jctech888.com.cn

Java: do { i++; } while (i < 10);
来源：http://cg.colortex.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jd.szsharing.cn

Ruby: begin; i += 1; end while i < 10
来源：http://iq.nszjky.cn

C#:   do { i++; } while (i < 10);
来源：http://kd.yuntaijiaju.cn

[B09] break 与 continue
来源：http://qv.521024.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ga.szsharing.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://oz.gzmigu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://us.hahajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hk.asd995.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wc.haigaiapp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://of.shtwfgs.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fa.lnxyls.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xy.haigaiapp.cn

[B10] 遍历同时拿索引
来源：http://uq.gzmigu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mf.bookmarksfly.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ev.muxihuayi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sj.yuexingan06.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kp.newstarts.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qx.haigaiapp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hn.hahajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sm.newstarts.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vq.newstarts.cn

[B11] 生成数字序列 / 区间
来源：http://kv.bjjhwx.cn

Py:   list(range(0, 10, 2))
来源：http://ay.hnjuh.cn

PHP:  range(0, 10, 2);
来源：http://oy.asd995.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ku.huixiangedu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xh.nicolike.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tr.wgjwhj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xi.huixiangedu.cn

Ruby: (0...10).step(2).to_a
来源：http://wf.nicolike.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fx.shtwfgs.cn

[B12] 跳出多层循环
来源：http://yo.szsharing.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ch.521024.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://lb.asd995.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wy.hnjuh.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dq.nicolike.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ve.colortex.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qe.gzmigu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nc.shxzskj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tp.jctech888.com.cn

[B13] 判断是否为数字
来源：http://sp.chemitech.net.cn

Py:   isinstance(x, (int, float))
来源：http://jj.shxzukj.cn

PHP:  is_numeric($x)
来源：http://bp.yuntaijiaju.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ll.yuntaijiaju.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gc.bookmarksfly.cn

Java: x instanceof Number
来源：http://sv.huixiangedu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zi.szsharing.cn

Ruby: x.is_a?(Numeric)
来源：http://rm.shxzskj.cn

C#:   x is int or double or decimal
来源：http://mv.shtwfgs.cn

[B14] 判断值是否在集合内
来源：http://qx.shtwfgs.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vq.yuntaijiaju.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lz.yuntaijiaju.cn

JS:   [1, 2, 3].includes(x)
来源：http://mf.huixinmuqiang.cn

TS:   [1, 2, 3].includes(x)
来源：http://ay.yuexingan06.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://mc.bookmarksfly.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://am.chemitech.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qe.newstarts.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sf.jianghongdianzi.cn

[B15] 布尔运算与取反
来源：http://fb.muxihuayi.cn

Py:   a and b or not c
来源：http://qn.gzmigu.cn

PHP:  $a && $b || !$c
来源：http://xi.nszjky.cn

JS:   a && b || !c
来源：http://vy.asd995.cn

TS:   a && b || !c
来源：http://ut.haigaiapp.cn

Java: a && b || !c
来源：http://uw.hnjuh.cn

Go:   a && b || !c
来源：http://ae.asd995.cn

Ruby: a && b || !c
来源：http://fl.szxytkj.cn

C#:   a && b || !c
来源：http://ry.haigaiapp.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gv.newstarts.cn

Py:   if not data: return
来源：http://es.jctech888.com.cn

PHP:  if (!$data) { return; }
来源：http://zq.521024.cn

JS:   if (!data) return;
来源：http://rw.asd995.cn

TS:   if (!data) return;
来源：http://sh.muxihuayi.cn

Java: if (data == null) return;
来源：http://ic.szsharing.cn

Go:   if data == nil { return }
来源：http://xd.szxytkj.cn

Ruby: return if data.nil?
来源：http://sd.yuntaijiaju.cn

C#:   if (data == null) return;
来源：http://pw.9csxet.cn

================================================================================
来源：http://jg.huixinmuqiang.cn

C. 函数与作用域
来源：http://ww.jianghongdianzi.cn

================================================================================
来源：http://fy.nszjky.cn

[C01] 定义函数
来源：http://hd.yuntaijiaju.cn

Py:   def add(a, b): return a + b
来源：http://bc.haigaiapp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bu.jianghongdianzi.cn

JS:   function add(a, b) { return a + b; }
来源：http://yp.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bh.yuexingan06.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bw.haigaiapp.cn

Go:   func add(a, b int) int { return a + b }
来源：http://va.colortex.cn

Ruby: def add(a, b); a + b; end
来源：http://nl.haigaiapp.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ra.huixinmuqiang.cn

[C02] 默认参数
来源：http://nz.szsharing.cn

Py:   def greet(name="World"): return name
来源：http://ik.panjiajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://np.szsharing.cn

JS:   function greet(name = "World") { return name; }
来源：http://fm.jianghongdianzi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vu.521024.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://si.9csxet.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xl.gzmigu.cn

Ruby: def greet(name = "World") = name
来源：http://pl.jianghongdianzi.cn

C#:   string Greet(string name = "World") => name;
来源：http://bh.chemitech.net.cn

[C03] 可变参数
来源：http://yt.huanxung.cn

Py:   def total(*args): return sum(args)
来源：http://ds.hnjuh.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://se.colortex.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fo.huixiangedu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gk.chemitech.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qs.shxzukj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tt.huanxung.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gh.hahajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xy.asd995.cn

[C04] 命名参数 / 关键字参数
来源：http://ue.yuntaijiaju.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wq.newstarts.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kz.huixinmuqiang.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ui.bjjhwx.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xk.jianghongdianzi.cn

Java: // 无：用 Builder 模式或 record
来源：http://of.muxihuayi.cn

Go:   // 无：用配置结构体参数
来源：http://om.bjjhwx.cn

Ruby: f(a: 1, b: 2)
来源：http://rz.hahajie.cn

C#:   f(a: 1, b: 2)
来源：http://dm.wgjwhj.cn

[C05] 返回多个值
来源：http://nl.shtwfgs.cn

Py:   return a, b
来源：http://ew.bookmarksfly.cn

PHP:  return [$a, $b];
来源：http://vc.huixiangedu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jh.szsharing.cn

TS:   return { a, b };
来源：http://do.shxzukj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kn.gzmigu.cn

Go:   return a, b
来源：http://yj.gzmigu.cn

Ruby: return a, b
来源：http://mr.panjiajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://yt.szxytkj.cn

[C06] 匿名函数 / lambda
来源：http://aw.nicolike.cn

Py:   square = lambda x: x * x
来源：http://dq.jctech888.com.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://vh.szxytkj.cn

JS:   const square = x => x * x;
来源：http://bm.newstarts.cn

TS:   const square = (x: number): number => x * x;
来源：http://iq.szxytkj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jn.521024.cn

Go:   sq := func(x int) int { return x * x }
来源：http://br.huixinmuqiang.cn

Ruby: square = ->(x) { x * x }
来源：http://ha.huixinmuqiang.cn

C#:   Func<int, int> square = x => x * x;
来源：http://us.nszjky.cn

[C07] 把函数作为参数传入
来源：http://dp.huanxung.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ij.nszjky.cn

PHP:  array_map("strtoupper", $arr);
来源：http://fe.shxzukj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://il.jianghongdianzi.cn

TS:   arr.map(String)
来源：http://pz.colortex.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cj.9csxet.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gd.panjiajie.cn

Ruby: arr.map(&:upcase)
来源：http://cv.muxihuayi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://vh.asd995.cn

[C08] 闭包
来源：http://qd.newstarts.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mn.bookmarksfly.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dd.lnxyls.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vc.colortex.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uk.nicolike.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ov.hnjuh.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ty.bjjhwx.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pv.shxzskj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tp.chemitech.net.cn

[C09] 递归
来源：http://vr.521024.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cb.colortex.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fh.newstarts.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://by.huixiangedu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ym.huanxung.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rj.yuexingan06.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://yq.haigaiapp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tw.hnjuh.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kj.bookmarksfly.cn

[C10] 变量作用域
来源：http://yl.szxytkj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dv.9csxet.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jt.shxzukj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ci.wgjwhj.cn

TS:   同 JS
来源：http://ls.asd995.cn

Java: 方法内为块级作用域
来源：http://pb.szxytkj.cn

Go:   花括号块级作用域
来源：http://uj.newstarts.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jt.521024.cn

C#:   块级作用域
来源：http://bi.jctech888.com.cn

[C11] 模块导入与导出
来源：http://ou.jctech888.com.cn

Py:   from module import func
来源：http://fk.521024.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qy.nicolike.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://az.yuntaijiaju.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fq.haigaiapp.cn

Java: import java.util.List;
来源：http://ia.wgjwhj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zc.szxytkj.cn

Ruby: require "json"; require_relative "./util"
来源：http://kn.bookmarksfly.cn

C#:   using System.Text;
来源：http://xn.9csxet.cn

[C12] 立即执行函数 IIFE
来源：http://ii.huixiangedu.cn

Py:   (lambda: print("run"))()
来源：http://vr.newstarts.cn

PHP:  (function () { echo "run"; })();
来源：http://tj.szsharing.cn

JS:   (() => { console.log("run"); })();
来源：http://op.yuexingan06.cn

TS:   (() => { console.log("run"); })();
来源：http://ue.nicolike.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://py.nszjky.cn

Go:   func() { fmt.Println("run") }()
来源：http://lu.wgjwhj.cn

Ruby: -> { puts "run" }.call
来源：http://gq.9csxet.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://uu.newstarts.cn

[C13] 类型声明 / 类型注解
来源：http://jn.bjjhwx.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ub.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hu.newstarts.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://le.panjiajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zh.lnxyls.cn

Java: int add(int a, int b) { return a + b; }
来源：http://iu.szxytkj.cn

Go:   func add(a, b int) int
来源：http://ow.gzmigu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qt.huanxung.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gn.shxzukj.cn

[C14] 泛型函数
来源：http://kx.521024.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://aa.gzmigu.cn

PHP:  // 无泛型
来源：http://it.yuexingan06.cn

JS:   // 无泛型
来源：http://la.bjjhwx.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sa.asd995.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mo.shxzskj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gm.wgjwhj.cn

Ruby: # 无泛型
来源：http://yq.521024.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ce.asd995.cn

[C15] 解构 / 展开参数
来源：http://bt.hahajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ot.shtwfgs.cn

PHP:  [$a, $b] = $pair;
来源：http://et.yuntaijiaju.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ig.nicolike.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://db.huanxung.cn

Java: // 无解构
来源：http://pj.shxzskj.cn

Go:   // 无解构
来源：http://bz.bjjhwx.cn

Ruby: a, b = pair
来源：http://ir.yuexingan06.cn

C#:   var (a, b) = pair;
来源：http://ia.newstarts.cn

[C16] 函数 / 方法重载
来源：http://ap.haigaiapp.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xg.shxzskj.cn

PHP:  // 无重载
来源：http://po.lnxyls.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://tm.panjiajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://xo.9csxet.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jh.521024.cn


<!-- 参考信息 -->