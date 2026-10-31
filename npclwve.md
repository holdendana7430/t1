代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://xh.gzmigu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cg.huanxung.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yt.shxzukj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://jx.9csxet.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://sf.gzmigu.cn

================================================================================
来源：http://go.shtwfgs.cn

B. 流程控制
来源：http://cf.521024.cn

================================================================================
来源：http://os.lnxyls.cn

[B01] 条件判断 if / else
来源：http://eb.lnxyls.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://we.chemitech.net.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ai.nicolike.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sd.shxzukj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://of.asd995.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xb.asd995.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ct.bookmarksfly.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://om.hnjuh.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cb.yuexingan06.cn

[B02] 多分支 else if / elif
来源：http://li.szsharing.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://va.nszjky.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bx.lnxyls.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://di.bjjhwx.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tp.chemitech.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://py.shxzukj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xx.huanxung.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hp.hahajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lk.yuntaijiaju.cn

[B03] switch / match / case
来源：http://if.chemitech.net.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ox.hnjuh.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mc.gzmigu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://za.hnjuh.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dc.lnxyls.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ul.szsharing.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rp.wgjwhj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mk.shxzskj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yd.huixinmuqiang.cn

[B04] for 计数循环
来源：http://wo.haigaiapp.cn

Py:   for i in range(10): print(i)
来源：http://wy.gzmigu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qb.chemitech.net.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pd.szxytkj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ku.haigaiapp.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dl.szsharing.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dy.jctech888.com.cn

Ruby: 10.times { |i| puts i }
来源：http://db.jianghongdianzi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pd.521024.cn

[B05] 遍历数组 / 列表
来源：http://sv.jctech888.com.cn

Py:   for item in arr: print(item)
来源：http://nw.shxzukj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://md.huixiangedu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ku.shxzukj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://km.huixiangedu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pn.jianghongdianzi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://in.wgjwhj.cn

Ruby: arr.each { |item| puts item }
来源：http://mf.huanxung.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xt.szxytkj.cn

[B06] 遍历字典 / 对象
来源：http://wj.huixinmuqiang.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ux.newstarts.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://no.yuntaijiaju.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lp.panjiajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://om.newstarts.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vg.nszjky.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ta.chemitech.net.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ls.panjiajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sj.panjiajie.cn

[B07] while 循环
来源：http://mi.chemitech.net.cn

Py:   while i < 10: i += 1
来源：http://fr.newstarts.cn

PHP:  while ($i < 10) { $i++; }
来源：http://co.521024.cn

JS:   while (i < 10) { i++; }
来源：http://pv.gzmigu.cn

TS:   while (i < 10) { i++; }
来源：http://tl.asd995.cn

Java: while (i < 10) { i++; }
来源：http://nu.hnjuh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xx.asd995.cn

Ruby: while i < 10; i += 1; end
来源：http://af.hnjuh.cn

C#:   while (i < 10) { i++; }
来源：http://hk.shxzukj.cn

[B08] do-while（至少执行一次）
来源：http://jx.szxytkj.cn

Py:   # 无 do-while：用 while True + break
来源：http://fk.lnxyls.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://br.muxihuayi.cn

JS:   do { i++; } while (i < 10);
来源：http://km.wgjwhj.cn

TS:   do { i++; } while (i < 10);
来源：http://rl.muxihuayi.cn

Java: do { i++; } while (i < 10);
来源：http://ig.chemitech.net.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xr.yuexingan06.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ar.bjjhwx.cn

C#:   do { i++; } while (i < 10);
来源：http://qg.muxihuayi.cn

[B09] break 与 continue
来源：http://dv.bookmarksfly.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://db.haigaiapp.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wa.nicolike.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://no.asd995.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ki.hahajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yc.haigaiapp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rd.muxihuayi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ur.gzmigu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zq.colortex.cn

[B10] 遍历同时拿索引
来源：http://zf.yuexingan06.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fv.huixiangedu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vi.yuntaijiaju.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fz.wgjwhj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xf.nicolike.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://oc.szsharing.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://as.yuntaijiaju.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mk.hahajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ko.521024.cn

[B11] 生成数字序列 / 区间
来源：http://kh.lnxyls.cn

Py:   list(range(0, 10, 2))
来源：http://aj.bjjhwx.cn

PHP:  range(0, 10, 2);
来源：http://wv.gzmigu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zg.shxzukj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xf.521024.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sw.hahajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qj.colortex.cn

Ruby: (0...10).step(2).to_a
来源：http://ah.yuntaijiaju.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sm.huixinmuqiang.cn

[B12] 跳出多层循环
来源：http://ac.newstarts.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://sx.panjiajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://xy.shxzukj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gs.jianghongdianzi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tx.gzmigu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://an.muxihuayi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cf.9csxet.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wv.yuntaijiaju.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zt.nszjky.cn

[B13] 判断是否为数字
来源：http://mj.asd995.cn

Py:   isinstance(x, (int, float))
来源：http://cs.gzmigu.cn

PHP:  is_numeric($x)
来源：http://sf.hahajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qs.gzmigu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rw.huixinmuqiang.cn

Java: x instanceof Number
来源：http://zw.szxytkj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uf.wgjwhj.cn

Ruby: x.is_a?(Numeric)
来源：http://hd.jctech888.com.cn

C#:   x is int or double or decimal
来源：http://vo.521024.cn

[B14] 判断值是否在集合内
来源：http://uk.haigaiapp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cm.huixiangedu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ex.szxytkj.cn

JS:   [1, 2, 3].includes(x)
来源：http://fs.jianghongdianzi.cn

TS:   [1, 2, 3].includes(x)
来源：http://rw.9csxet.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vh.jctech888.com.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dn.bookmarksfly.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ra.shxzukj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gw.newstarts.cn

[B15] 布尔运算与取反
来源：http://wd.hahajie.cn

Py:   a and b or not c
来源：http://em.panjiajie.cn

PHP:  $a && $b || !$c
来源：http://el.colortex.cn

JS:   a && b || !c
来源：http://dq.huixiangedu.cn

TS:   a && b || !c
来源：http://ml.shxzukj.cn

Java: a && b || !c
来源：http://cj.bookmarksfly.cn

Go:   a && b || !c
来源：http://lk.szsharing.cn

Ruby: a && b || !c
来源：http://ue.yuexingan06.cn

C#:   a && b || !c
来源：http://zr.muxihuayi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lm.newstarts.cn

Py:   if not data: return
来源：http://jr.hahajie.cn

PHP:  if (!$data) { return; }
来源：http://ea.bjjhwx.cn

JS:   if (!data) return;
来源：http://mk.huixinmuqiang.cn

TS:   if (!data) return;
来源：http://tf.jctech888.com.cn

Java: if (data == null) return;
来源：http://tt.huanxung.cn

Go:   if data == nil { return }
来源：http://oo.yuexingan06.cn

Ruby: return if data.nil?
来源：http://qh.yuexingan06.cn

C#:   if (data == null) return;
来源：http://ku.nicolike.cn

================================================================================
来源：http://lq.gzmigu.cn

C. 函数与作用域
来源：http://hm.521024.cn

================================================================================
来源：http://as.9csxet.cn

[C01] 定义函数
来源：http://ms.haigaiapp.cn

Py:   def add(a, b): return a + b
来源：http://ab.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pr.jianghongdianzi.cn

JS:   function add(a, b) { return a + b; }
来源：http://oh.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hj.jctech888.com.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://jx.521024.cn

Go:   func add(a, b int) int { return a + b }
来源：http://bk.hnjuh.cn

Ruby: def add(a, b); a + b; end
来源：http://fs.9csxet.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dk.shtwfgs.cn

[C02] 默认参数
来源：http://zn.hahajie.cn

Py:   def greet(name="World"): return name
来源：http://xu.jianghongdianzi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yj.yuexingan06.cn

JS:   function greet(name = "World") { return name; }
来源：http://dy.nszjky.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bz.asd995.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://sk.hahajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dc.jctech888.com.cn

Ruby: def greet(name = "World") = name
来源：http://jv.huixiangedu.cn

C#:   string Greet(string name = "World") => name;
来源：http://dm.9csxet.cn

[C03] 可变参数
来源：http://te.bjjhwx.cn

Py:   def total(*args): return sum(args)
来源：http://dr.muxihuayi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pz.bookmarksfly.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sg.muxihuayi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fd.newstarts.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yz.panjiajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hk.shxzukj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://lg.chemitech.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dj.jianghongdianzi.cn

[C04] 命名参数 / 关键字参数
来源：http://jc.gzmigu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wu.szsharing.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kt.jianghongdianzi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hy.haigaiapp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zs.jianghongdianzi.cn

Java: // 无：用 Builder 模式或 record
来源：http://fh.muxihuayi.cn

Go:   // 无：用配置结构体参数
来源：http://pw.yuexingan06.cn

Ruby: f(a: 1, b: 2)
来源：http://sx.wgjwhj.cn

C#:   f(a: 1, b: 2)
来源：http://co.nicolike.cn

[C05] 返回多个值
来源：http://xr.huixinmuqiang.cn

Py:   return a, b
来源：http://fn.9csxet.cn

PHP:  return [$a, $b];
来源：http://fb.521024.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://iq.szsharing.cn

TS:   return { a, b };
来源：http://jb.nszjky.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vj.colortex.cn

Go:   return a, b
来源：http://zd.huixinmuqiang.cn

Ruby: return a, b
来源：http://er.hnjuh.cn

C#:   return (a, b);              // ValueTuple
来源：http://id.asd995.cn

[C06] 匿名函数 / lambda
来源：http://kj.yuntaijiaju.cn

Py:   square = lambda x: x * x
来源：http://sb.shtwfgs.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fz.521024.cn

JS:   const square = x => x * x;
来源：http://zs.chemitech.net.cn

TS:   const square = (x: number): number => x * x;
来源：http://sc.panjiajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mz.szxytkj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://bc.szxytkj.cn

Ruby: square = ->(x) { x * x }
来源：http://rp.jctech888.com.cn

C#:   Func<int, int> square = x => x * x;
来源：http://yw.colortex.cn

[C07] 把函数作为参数传入
来源：http://ou.hnjuh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zh.yuntaijiaju.cn

PHP:  array_map("strtoupper", $arr);
来源：http://am.shtwfgs.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rk.gzmigu.cn

TS:   arr.map(String)
来源：http://jt.hahajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ys.hnjuh.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ul.shxzukj.cn

Ruby: arr.map(&:upcase)
来源：http://dr.yuntaijiaju.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://bo.huanxung.cn

[C08] 闭包
来源：http://ph.nszjky.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nd.shxzukj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mx.lnxyls.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ah.panjiajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wx.szsharing.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jj.haigaiapp.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gw.panjiajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nm.asd995.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xm.huanxung.cn

[C09] 递归
来源：http://ln.newstarts.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bs.bookmarksfly.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qa.colortex.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://os.yuexingan06.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rc.bookmarksfly.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sp.521024.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://aq.gzmigu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tw.asd995.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xy.wgjwhj.cn

[C10] 变量作用域
来源：http://cw.jianghongdianzi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://br.panjiajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ei.lnxyls.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://al.huixiangedu.cn

TS:   同 JS
来源：http://lj.szxytkj.cn

Java: 方法内为块级作用域
来源：http://za.haigaiapp.cn

Go:   花括号块级作用域
来源：http://en.colortex.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kc.yuntaijiaju.cn

C#:   块级作用域
来源：http://hq.gzmigu.cn

[C11] 模块导入与导出
来源：http://je.shtwfgs.cn

Py:   from module import func
来源：http://ia.hnjuh.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://dl.chemitech.net.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jy.wgjwhj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jg.yuntaijiaju.cn

Java: import java.util.List;
来源：http://wl.asd995.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bc.haigaiapp.cn

Ruby: require "json"; require_relative "./util"
来源：http://gw.hnjuh.cn

C#:   using System.Text;
来源：http://im.shtwfgs.cn

[C12] 立即执行函数 IIFE
来源：http://de.bjjhwx.cn

Py:   (lambda: print("run"))()
来源：http://wt.gzmigu.cn

PHP:  (function () { echo "run"; })();
来源：http://aq.gzmigu.cn

JS:   (() => { console.log("run"); })();
来源：http://cb.huixiangedu.cn

TS:   (() => { console.log("run"); })();
来源：http://uy.yuntaijiaju.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gy.jctech888.com.cn

Go:   func() { fmt.Println("run") }()
来源：http://fg.hahajie.cn

Ruby: -> { puts "run" }.call
来源：http://kq.521024.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xu.9csxet.cn

[C13] 类型声明 / 类型注解
来源：http://lq.huanxung.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bw.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bj.szxytkj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://um.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bd.lnxyls.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wp.shxzukj.cn

Go:   func add(a, b int) int
来源：http://ml.lnxyls.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://id.bjjhwx.cn

C#:   int Add(int a, int b) => a + b;
来源：http://at.panjiajie.cn

[C14] 泛型函数
来源：http://jy.asd995.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yx.panjiajie.cn

PHP:  // 无泛型
来源：http://pv.9csxet.cn

JS:   // 无泛型
来源：http://gd.gzmigu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ar.muxihuayi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bk.chemitech.net.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gv.hahajie.cn

Ruby: # 无泛型
来源：http://vx.shxzukj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nq.muxihuayi.cn

[C15] 解构 / 展开参数
来源：http://dt.shtwfgs.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xj.bjjhwx.cn

PHP:  [$a, $b] = $pair;
来源：http://tv.shxzukj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rh.haigaiapp.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uu.shxzskj.cn

Java: // 无解构
来源：http://zz.huanxung.cn

Go:   // 无解构
来源：http://in.jianghongdianzi.cn

Ruby: a, b = pair
来源：http://pt.nszjky.cn

C#:   var (a, b) = pair;
来源：http://mg.szsharing.cn

[C16] 函数 / 方法重载
来源：http://yt.hnjuh.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pk.jianghongdianzi.cn

PHP:  // 无重载
来源：http://bs.jctech888.com.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qk.shxzukj.cn

TS:   // 用联合类型或重载签名声明
来源：http://ac.newstarts.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://sj.yuntaijiaju.cn

Go:   // 无重载：用不同函数名
来源：http://ol.hnjuh.cn

Ruby: # 无重载：靠动态参数
来源：http://ce.muxihuayi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zh.szxytkj.cn

================================================================================
来源：http://qw.9csxet.cn


<!-- 参考信息 -->