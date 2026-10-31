代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://en.shxzukj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hq.521024.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nh.yuntaijiaju.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ml.shxzukj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://si.wgjwhj.cn

================================================================================
来源：http://qu.521024.cn

B. 流程控制
来源：http://jv.shxzskj.cn

================================================================================
来源：http://zh.asd995.cn

[B01] 条件判断 if / else
来源：http://kc.jianghongdianzi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ao.lnxyls.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ne.521024.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vp.bookmarksfly.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://js.shxzskj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://fc.bjjhwx.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ik.shxzskj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ju.chemitech.net.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bt.yuntaijiaju.cn

[B02] 多分支 else if / elif
来源：http://vo.bookmarksfly.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cj.521024.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qs.yuntaijiaju.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://la.wgjwhj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ux.haigaiapp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vb.lnxyls.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ll.9csxet.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gb.huixinmuqiang.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xa.huanxung.cn

[B03] switch / match / case
来源：http://zf.hnjuh.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://go.jctech888.com.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qk.colortex.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hp.haigaiapp.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jw.huixinmuqiang.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bm.bjjhwx.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uu.wgjwhj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nh.nicolike.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wj.9csxet.cn

[B04] for 计数循环
来源：http://pr.muxihuayi.cn

Py:   for i in range(10): print(i)
来源：http://sk.muxihuayi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ty.huixinmuqiang.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sc.lnxyls.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://os.colortex.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jk.muxihuayi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://om.hahajie.cn

Ruby: 10.times { |i| puts i }
来源：http://dt.newstarts.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hy.hahajie.cn

[B05] 遍历数组 / 列表
来源：http://eu.521024.cn

Py:   for item in arr: print(item)
来源：http://dv.jianghongdianzi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pd.panjiajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://nt.bjjhwx.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ja.jianghongdianzi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qz.nszjky.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hv.shxzukj.cn

Ruby: arr.each { |item| puts item }
来源：http://xv.haigaiapp.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sg.szxytkj.cn

[B06] 遍历字典 / 对象
来源：http://oo.521024.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zt.hnjuh.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lv.jianghongdianzi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bq.huixinmuqiang.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nt.hnjuh.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pf.haigaiapp.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://op.hnjuh.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bm.haigaiapp.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gs.9csxet.cn

[B07] while 循环
来源：http://np.haigaiapp.cn

Py:   while i < 10: i += 1
来源：http://mx.yuexingan06.cn

PHP:  while ($i < 10) { $i++; }
来源：http://nl.bjjhwx.cn

JS:   while (i < 10) { i++; }
来源：http://lt.9csxet.cn

TS:   while (i < 10) { i++; }
来源：http://xh.shxzskj.cn

Java: while (i < 10) { i++; }
来源：http://ss.muxihuayi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mj.hnjuh.cn

Ruby: while i < 10; i += 1; end
来源：http://xj.nszjky.cn

C#:   while (i < 10) { i++; }
来源：http://fa.wgjwhj.cn

[B08] do-while（至少执行一次）
来源：http://ze.9csxet.cn

Py:   # 无 do-while：用 while True + break
来源：http://rw.shtwfgs.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qh.bookmarksfly.cn

JS:   do { i++; } while (i < 10);
来源：http://ug.wgjwhj.cn

TS:   do { i++; } while (i < 10);
来源：http://rq.hahajie.cn

Java: do { i++; } while (i < 10);
来源：http://wg.hnjuh.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://qj.shtwfgs.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mu.muxihuayi.cn

C#:   do { i++; } while (i < 10);
来源：http://mt.huixiangedu.cn

[B09] break 与 continue
来源：http://pn.huixinmuqiang.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fw.szsharing.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yu.hnjuh.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jd.panjiajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cx.huixinmuqiang.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wx.shxzukj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vm.hahajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xr.lnxyls.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ec.yuntaijiaju.cn

[B10] 遍历同时拿索引
来源：http://hk.colortex.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ea.asd995.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rh.shxzukj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qw.colortex.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://oh.panjiajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dr.hahajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ac.yuexingan06.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vi.colortex.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vo.gzmigu.cn

[B11] 生成数字序列 / 区间
来源：http://cz.shxzukj.cn

Py:   list(range(0, 10, 2))
来源：http://ak.9csxet.cn

PHP:  range(0, 10, 2);
来源：http://qk.jianghongdianzi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rw.wgjwhj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rh.yuexingan06.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ga.lnxyls.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pm.jctech888.com.cn

Ruby: (0...10).step(2).to_a
来源：http://vd.muxihuayi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uh.szxytkj.cn

[B12] 跳出多层循环
来源：http://fh.521024.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://uw.shxzskj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://lz.521024.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sh.nszjky.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fe.nicolike.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zv.colortex.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://os.szsharing.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hq.jianghongdianzi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xu.nicolike.cn

[B13] 判断是否为数字
来源：http://sw.szsharing.cn

Py:   isinstance(x, (int, float))
来源：http://ls.nicolike.cn

PHP:  is_numeric($x)
来源：http://sl.szsharing.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tm.szsharing.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kq.asd995.cn

Java: x instanceof Number
来源：http://ud.newstarts.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kk.9csxet.cn

Ruby: x.is_a?(Numeric)
来源：http://ac.nszjky.cn

C#:   x is int or double or decimal
来源：http://lu.wgjwhj.cn

[B14] 判断值是否在集合内
来源：http://re.jianghongdianzi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kg.lnxyls.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ah.huixiangedu.cn

JS:   [1, 2, 3].includes(x)
来源：http://ix.nicolike.cn

TS:   [1, 2, 3].includes(x)
来源：http://hm.hnjuh.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://la.hnjuh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yz.jianghongdianzi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vv.chemitech.net.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mb.jianghongdianzi.cn

[B15] 布尔运算与取反
来源：http://ff.521024.cn

Py:   a and b or not c
来源：http://aq.huixinmuqiang.cn

PHP:  $a && $b || !$c
来源：http://gl.colortex.cn

JS:   a && b || !c
来源：http://cm.bjjhwx.cn

TS:   a && b || !c
来源：http://sa.jctech888.com.cn

Java: a && b || !c
来源：http://lo.hnjuh.cn

Go:   a && b || !c
来源：http://gm.bjjhwx.cn

Ruby: a && b || !c
来源：http://xm.bjjhwx.cn

C#:   a && b || !c
来源：http://sz.colortex.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hr.lnxyls.cn

Py:   if not data: return
来源：http://vf.shxzukj.cn

PHP:  if (!$data) { return; }
来源：http://fv.shxzskj.cn

JS:   if (!data) return;
来源：http://ik.chemitech.net.cn

TS:   if (!data) return;
来源：http://sh.hnjuh.cn

Java: if (data == null) return;
来源：http://af.bjjhwx.cn

Go:   if data == nil { return }
来源：http://wn.szsharing.cn

Ruby: return if data.nil?
来源：http://kc.huixinmuqiang.cn

C#:   if (data == null) return;
来源：http://bs.hnjuh.cn

================================================================================
来源：http://xv.wgjwhj.cn

C. 函数与作用域
来源：http://lk.jianghongdianzi.cn

================================================================================
来源：http://cq.yuntaijiaju.cn

[C01] 定义函数
来源：http://fv.bookmarksfly.cn

Py:   def add(a, b): return a + b
来源：http://vt.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://af.lnxyls.cn

JS:   function add(a, b) { return a + b; }
来源：http://wp.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vw.colortex.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://pa.shxzukj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://it.huixiangedu.cn

Ruby: def add(a, b); a + b; end
来源：http://bo.nszjky.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://eo.bjjhwx.cn

[C02] 默认参数
来源：http://vj.bjjhwx.cn

Py:   def greet(name="World"): return name
来源：http://wa.chemitech.net.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zr.bjjhwx.cn

JS:   function greet(name = "World") { return name; }
来源：http://wf.shxzukj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://im.chemitech.net.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ro.shxzukj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pg.9csxet.cn

Ruby: def greet(name = "World") = name
来源：http://fw.hnjuh.cn

C#:   string Greet(string name = "World") => name;
来源：http://gr.wgjwhj.cn

[C03] 可变参数
来源：http://iu.yuexingan06.cn

Py:   def total(*args): return sum(args)
来源：http://qp.hahajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://eq.bjjhwx.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://je.hahajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fv.muxihuayi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lk.jctech888.com.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rh.hahajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://az.szxytkj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ja.huanxung.cn

[C04] 命名参数 / 关键字参数
来源：http://sh.wgjwhj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ar.szxytkj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://uc.colortex.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qj.chemitech.net.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://iu.bjjhwx.cn

Java: // 无：用 Builder 模式或 record
来源：http://co.chemitech.net.cn

Go:   // 无：用配置结构体参数
来源：http://th.wgjwhj.cn

Ruby: f(a: 1, b: 2)
来源：http://ka.szxytkj.cn

C#:   f(a: 1, b: 2)
来源：http://ds.9csxet.cn

[C05] 返回多个值
来源：http://kd.haigaiapp.cn

Py:   return a, b
来源：http://za.shtwfgs.cn

PHP:  return [$a, $b];
来源：http://ru.gzmigu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://el.yuexingan06.cn

TS:   return { a, b };
来源：http://me.521024.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jk.shxzukj.cn

Go:   return a, b
来源：http://ha.wgjwhj.cn

Ruby: return a, b
来源：http://wv.521024.cn

C#:   return (a, b);              // ValueTuple
来源：http://po.gzmigu.cn

[C06] 匿名函数 / lambda
来源：http://sw.jctech888.com.cn

Py:   square = lambda x: x * x
来源：http://tp.shxzskj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ms.521024.cn

JS:   const square = x => x * x;
来源：http://ry.newstarts.cn

TS:   const square = (x: number): number => x * x;
来源：http://af.huixiangedu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yw.haigaiapp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gg.muxihuayi.cn

Ruby: square = ->(x) { x * x }
来源：http://uh.lnxyls.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qu.panjiajie.cn

[C07] 把函数作为参数传入
来源：http://cb.newstarts.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gs.hnjuh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://cm.chemitech.net.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lv.bookmarksfly.cn

TS:   arr.map(String)
来源：http://wa.muxihuayi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://iv.huixinmuqiang.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yh.gzmigu.cn

Ruby: arr.map(&:upcase)
来源：http://vg.shxzukj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://js.nicolike.cn

[C08] 闭包
来源：http://ck.bookmarksfly.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ke.9csxet.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qu.nszjky.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ph.gzmigu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dr.asd995.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://le.huanxung.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kh.gzmigu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qp.9csxet.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mx.chemitech.net.cn

[C09] 递归
来源：http://js.yuexingan06.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hu.gzmigu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://iw.chemitech.net.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fs.szsharing.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qt.szxytkj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wd.panjiajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fa.shxzskj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://px.jianghongdianzi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ai.chemitech.net.cn

[C10] 变量作用域
来源：http://kq.shxzukj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://py.huixiangedu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vk.jianghongdianzi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gi.hahajie.cn

TS:   同 JS
来源：http://lb.bookmarksfly.cn

Java: 方法内为块级作用域
来源：http://fq.szsharing.cn

Go:   花括号块级作用域
来源：http://ne.szsharing.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://eh.bjjhwx.cn

C#:   块级作用域
来源：http://dl.yuntaijiaju.cn

[C11] 模块导入与导出
来源：http://sw.shtwfgs.cn

Py:   from module import func
来源：http://fl.hnjuh.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://py.huixinmuqiang.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://to.bookmarksfly.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zn.jctech888.com.cn

Java: import java.util.List;
来源：http://ok.wgjwhj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tp.szxytkj.cn

Ruby: require "json"; require_relative "./util"
来源：http://mh.huixiangedu.cn

C#:   using System.Text;
来源：http://ou.szsharing.cn

[C12] 立即执行函数 IIFE
来源：http://lf.newstarts.cn

Py:   (lambda: print("run"))()
来源：http://ni.szsharing.cn

PHP:  (function () { echo "run"; })();
来源：http://fd.521024.cn

JS:   (() => { console.log("run"); })();
来源：http://tn.shxzskj.cn

TS:   (() => { console.log("run"); })();
来源：http://aq.chemitech.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bo.colortex.cn

Go:   func() { fmt.Println("run") }()
来源：http://jl.szxytkj.cn

Ruby: -> { puts "run" }.call
来源：http://yn.521024.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://is.nicolike.cn

[C13] 类型声明 / 类型注解
来源：http://yp.nicolike.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zg.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eo.jctech888.com.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://az.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://et.panjiajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://rp.nicolike.cn

Go:   func add(a, b int) int
来源：http://ie.huanxung.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://li.asd995.cn

C#:   int Add(int a, int b) => a + b;
来源：http://om.asd995.cn

[C14] 泛型函数
来源：http://hk.gzmigu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sj.gzmigu.cn

PHP:  // 无泛型
来源：http://bg.yuexingan06.cn

JS:   // 无泛型
来源：http://ht.haigaiapp.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tm.panjiajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jc.panjiajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gj.asd995.cn

Ruby: # 无泛型
来源：http://ry.nicolike.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pk.gzmigu.cn

[C15] 解构 / 展开参数
来源：http://nn.huixiangedu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zk.haigaiapp.cn

PHP:  [$a, $b] = $pair;
来源：http://pg.9csxet.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://oo.jianghongdianzi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lk.panjiajie.cn

Java: // 无解构
来源：http://xo.colortex.cn

Go:   // 无解构
来源：http://rh.huixinmuqiang.cn

Ruby: a, b = pair
来源：http://sw.bookmarksfly.cn

C#:   var (a, b) = pair;
来源：http://av.chemitech.net.cn

[C16] 函数 / 方法重载
来源：http://nt.9csxet.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zy.shxzukj.cn

PHP:  // 无重载
来源：http://lq.9csxet.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://sg.shxzskj.cn

TS:   // 用联合类型或重载签名声明
来源：http://nf.hahajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://zc.9csxet.cn

Go:   // 无重载：用不同函数名
来源：http://wx.nicolike.cn

Ruby: # 无重载：靠动态参数
来源：http://wz.panjiajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://uj.szxytkj.cn

================================================================================
来源：http://ll.hahajie.cn


<!-- 参考信息 -->