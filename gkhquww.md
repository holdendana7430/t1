代发 wailian999

[A26] 类型转换总览
来源：http://ot.jctech888.com.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kx.muxihuayi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yv.szxytkj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gm.huixinmuqiang.cn

TS:   Number() String() Boolean() x as number
来源：http://fz.chemitech.net.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gk.bjjhwx.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vj.hnjuh.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lg.yuntaijiaju.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pz.bjjhwx.cn

================================================================================
来源：http://ar.colortex.cn

B. 流程控制
来源：http://go.newstarts.cn

================================================================================
来源：http://yt.chemitech.net.cn

[B01] 条件判断 if / else
来源：http://io.yuntaijiaju.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://tw.bookmarksfly.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lf.yuntaijiaju.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wh.9csxet.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pq.chemitech.net.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://lx.nszjky.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lj.gzmigu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pn.chemitech.net.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bd.huixiangedu.cn

[B02] 多分支 else if / elif
来源：http://no.shxzukj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ps.huanxung.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://uv.newstarts.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ae.haigaiapp.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ve.nicolike.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yh.jctech888.com.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ss.wgjwhj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://br.panjiajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://of.9csxet.cn

[B03] switch / match / case
来源：http://yo.yuntaijiaju.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bb.yuexingan06.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qr.huanxung.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nx.huixinmuqiang.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://an.muxihuayi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ts.9csxet.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://is.szxytkj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xw.gzmigu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xy.shxzukj.cn

[B04] for 计数循环
来源：http://sg.wgjwhj.cn

Py:   for i in range(10): print(i)
来源：http://vd.shxzskj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://iq.jianghongdianzi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ns.gzmigu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tb.huixiangedu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://md.nszjky.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bp.szxytkj.cn

Ruby: 10.times { |i| puts i }
来源：http://bl.shxzukj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hn.panjiajie.cn

[B05] 遍历数组 / 列表
来源：http://sc.shtwfgs.cn

Py:   for item in arr: print(item)
来源：http://ch.wgjwhj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zg.shxzukj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://vg.muxihuayi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fh.szsharing.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xo.huanxung.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xh.huanxung.cn

Ruby: arr.each { |item| puts item }
来源：http://zb.haigaiapp.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mu.huixinmuqiang.cn

[B06] 遍历字典 / 对象
来源：http://il.shxzukj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://nj.wgjwhj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yy.chemitech.net.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ic.huixiangedu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vt.huixinmuqiang.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qf.hnjuh.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://og.shtwfgs.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://oq.asd995.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wl.szxytkj.cn

[B07] while 循环
来源：http://on.muxihuayi.cn

Py:   while i < 10: i += 1
来源：http://sq.yuexingan06.cn

PHP:  while ($i < 10) { $i++; }
来源：http://db.chemitech.net.cn

JS:   while (i < 10) { i++; }
来源：http://sy.haigaiapp.cn

TS:   while (i < 10) { i++; }
来源：http://tu.bookmarksfly.cn

Java: while (i < 10) { i++; }
来源：http://es.nicolike.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hp.hahajie.cn

Ruby: while i < 10; i += 1; end
来源：http://cj.szsharing.cn

C#:   while (i < 10) { i++; }
来源：http://ry.gzmigu.cn

[B08] do-while（至少执行一次）
来源：http://to.asd995.cn

Py:   # 无 do-while：用 while True + break
来源：http://da.newstarts.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://br.shxzskj.cn

JS:   do { i++; } while (i < 10);
来源：http://tl.szxytkj.cn

TS:   do { i++; } while (i < 10);
来源：http://cm.lnxyls.cn

Java: do { i++; } while (i < 10);
来源：http://zs.nszjky.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wt.shxzskj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ax.szsharing.cn

C#:   do { i++; } while (i < 10);
来源：http://vj.chemitech.net.cn

[B09] break 与 continue
来源：http://mw.jctech888.com.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cq.szxytkj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://br.lnxyls.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gu.huanxung.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://az.huanxung.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nc.colortex.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://df.huixinmuqiang.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lz.muxihuayi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wa.wgjwhj.cn

[B10] 遍历同时拿索引
来源：http://bk.muxihuayi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fp.shxzskj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cx.yuexingan06.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sv.huanxung.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ea.muxihuayi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://al.huanxung.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qr.521024.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jv.shxzukj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ph.haigaiapp.cn

[B11] 生成数字序列 / 区间
来源：http://lj.bjjhwx.cn

Py:   list(range(0, 10, 2))
来源：http://ne.shxzskj.cn

PHP:  range(0, 10, 2);
来源：http://hg.shxzukj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gb.521024.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qa.jctech888.com.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zy.yuntaijiaju.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pf.521024.cn

Ruby: (0...10).step(2).to_a
来源：http://jz.9csxet.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dd.lnxyls.cn

[B12] 跳出多层循环
来源：http://hv.szsharing.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://qq.jianghongdianzi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://kv.panjiajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lz.gzmigu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fh.asd995.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ni.haigaiapp.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cf.huixinmuqiang.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://my.szsharing.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cz.521024.cn

[B13] 判断是否为数字
来源：http://zl.chemitech.net.cn

Py:   isinstance(x, (int, float))
来源：http://rp.jctech888.com.cn

PHP:  is_numeric($x)
来源：http://ea.yuexingan06.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fr.9csxet.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xa.hahajie.cn

Java: x instanceof Number
来源：http://st.nicolike.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ml.bjjhwx.cn

Ruby: x.is_a?(Numeric)
来源：http://yc.hahajie.cn

C#:   x is int or double or decimal
来源：http://od.haigaiapp.cn

[B14] 判断值是否在集合内
来源：http://jp.521024.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://os.shxzskj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vi.panjiajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://vc.chemitech.net.cn

TS:   [1, 2, 3].includes(x)
来源：http://ou.gzmigu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://sv.521024.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xl.huanxung.cn

Ruby: [1, 2, 3].include?(x)
来源：http://em.wgjwhj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ku.chemitech.net.cn

[B15] 布尔运算与取反
来源：http://gm.newstarts.cn

Py:   a and b or not c
来源：http://xt.hnjuh.cn

PHP:  $a && $b || !$c
来源：http://bl.hnjuh.cn

JS:   a && b || !c
来源：http://be.chemitech.net.cn

TS:   a && b || !c
来源：http://ep.szxytkj.cn

Java: a && b || !c
来源：http://rv.asd995.cn

Go:   a && b || !c
来源：http://gb.wgjwhj.cn

Ruby: a && b || !c
来源：http://ul.haigaiapp.cn

C#:   a && b || !c
来源：http://pa.colortex.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xr.wgjwhj.cn

Py:   if not data: return
来源：http://ax.newstarts.cn

PHP:  if (!$data) { return; }
来源：http://rd.nszjky.cn

JS:   if (!data) return;
来源：http://gz.asd995.cn

TS:   if (!data) return;
来源：http://cf.bookmarksfly.cn

Java: if (data == null) return;
来源：http://tl.521024.cn

Go:   if data == nil { return }
来源：http://qt.muxihuayi.cn

Ruby: return if data.nil?
来源：http://mu.nszjky.cn

C#:   if (data == null) return;
来源：http://go.nicolike.cn

================================================================================
来源：http://wf.chemitech.net.cn

C. 函数与作用域
来源：http://pl.haigaiapp.cn

================================================================================
来源：http://ys.shxzukj.cn

[C01] 定义函数
来源：http://fc.huanxung.cn

Py:   def add(a, b): return a + b
来源：http://ff.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iv.huixinmuqiang.cn

JS:   function add(a, b) { return a + b; }
来源：http://gq.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ak.haigaiapp.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://cn.521024.cn

Go:   func add(a, b int) int { return a + b }
来源：http://kk.gzmigu.cn

Ruby: def add(a, b); a + b; end
来源：http://jw.9csxet.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lu.jianghongdianzi.cn

[C02] 默认参数
来源：http://vy.colortex.cn

Py:   def greet(name="World"): return name
来源：http://eb.521024.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dc.yuexingan06.cn

JS:   function greet(name = "World") { return name; }
来源：http://fm.hahajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zr.hahajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://mv.haigaiapp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wx.lnxyls.cn

Ruby: def greet(name = "World") = name
来源：http://ce.huixiangedu.cn

C#:   string Greet(string name = "World") => name;
来源：http://iz.521024.cn

[C03] 可变参数
来源：http://zx.hnjuh.cn

Py:   def total(*args): return sum(args)
来源：http://ew.huixinmuqiang.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yd.haigaiapp.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bv.newstarts.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mo.9csxet.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bn.szsharing.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kc.huixinmuqiang.cn

Ruby: def total(*nums); nums.sum; end
来源：http://aq.lnxyls.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ly.lnxyls.cn

[C04] 命名参数 / 关键字参数
来源：http://iv.jctech888.com.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vw.9csxet.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://aq.newstarts.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yg.shxzskj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jg.hahajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://es.shxzskj.cn

Go:   // 无：用配置结构体参数
来源：http://fd.chemitech.net.cn

Ruby: f(a: 1, b: 2)
来源：http://df.jianghongdianzi.cn

C#:   f(a: 1, b: 2)
来源：http://xh.hahajie.cn

[C05] 返回多个值
来源：http://rc.hahajie.cn

Py:   return a, b
来源：http://mx.chemitech.net.cn

PHP:  return [$a, $b];
来源：http://ha.bookmarksfly.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fz.521024.cn

TS:   return { a, b };
来源：http://bo.nszjky.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qy.panjiajie.cn

Go:   return a, b
来源：http://qi.huanxung.cn

Ruby: return a, b
来源：http://sk.shtwfgs.cn

C#:   return (a, b);              // ValueTuple
来源：http://xj.hahajie.cn

[C06] 匿名函数 / lambda
来源：http://xq.9csxet.cn

Py:   square = lambda x: x * x
来源：http://ya.szsharing.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://hn.shtwfgs.cn

JS:   const square = x => x * x;
来源：http://rx.jianghongdianzi.cn

TS:   const square = (x: number): number => x * x;
来源：http://ry.yuntaijiaju.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://li.bookmarksfly.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wp.szxytkj.cn

Ruby: square = ->(x) { x * x }
来源：http://rg.chemitech.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dq.asd995.cn

[C07] 把函数作为参数传入
来源：http://cr.huixinmuqiang.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ss.chemitech.net.cn

PHP:  array_map("strtoupper", $arr);
来源：http://dl.shxzskj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://op.muxihuayi.cn

TS:   arr.map(String)
来源：http://tc.chemitech.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kz.bookmarksfly.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xa.huixiangedu.cn

Ruby: arr.map(&:upcase)
来源：http://hm.521024.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://kv.shtwfgs.cn

[C08] 闭包
来源：http://us.bjjhwx.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cl.muxihuayi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ef.hahajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kv.asd995.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ot.lnxyls.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ti.shxzskj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wd.bjjhwx.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ba.9csxet.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wd.shxzskj.cn

[C09] 递归
来源：http://em.bjjhwx.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qz.jianghongdianzi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ow.huixiangedu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tf.haigaiapp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://go.9csxet.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sn.hahajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mg.yuntaijiaju.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://je.521024.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wi.gzmigu.cn

[C10] 变量作用域
来源：http://ny.bjjhwx.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ae.jianghongdianzi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://uv.chemitech.net.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mj.newstarts.cn

TS:   同 JS
来源：http://na.shxzskj.cn

Java: 方法内为块级作用域
来源：http://dl.huixinmuqiang.cn

Go:   花括号块级作用域
来源：http://rr.521024.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jp.hahajie.cn

C#:   块级作用域
来源：http://dz.muxihuayi.cn

[C11] 模块导入与导出
来源：http://ys.nszjky.cn

Py:   from module import func
来源：http://us.shxzukj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://av.shtwfgs.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hv.521024.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lz.yuntaijiaju.cn

Java: import java.util.List;
来源：http://ok.hnjuh.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sy.shxzskj.cn

Ruby: require "json"; require_relative "./util"
来源：http://hp.asd995.cn

C#:   using System.Text;
来源：http://ax.huixinmuqiang.cn

[C12] 立即执行函数 IIFE
来源：http://eu.szsharing.cn

Py:   (lambda: print("run"))()
来源：http://qr.9csxet.cn

PHP:  (function () { echo "run"; })();
来源：http://ge.shxzukj.cn

JS:   (() => { console.log("run"); })();
来源：http://kd.gzmigu.cn

TS:   (() => { console.log("run"); })();
来源：http://nz.jianghongdianzi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bx.gzmigu.cn

Go:   func() { fmt.Println("run") }()
来源：http://ui.hnjuh.cn

Ruby: -> { puts "run" }.call
来源：http://cp.haigaiapp.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zg.panjiajie.cn

[C13] 类型声明 / 类型注解
来源：http://nh.huixiangedu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gy.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qv.shxzukj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dw.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tc.yuexingan06.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fp.nszjky.cn

Go:   func add(a, b int) int
来源：http://pa.haigaiapp.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://aq.yuntaijiaju.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ut.huanxung.cn

[C14] 泛型函数
来源：http://zs.nszjky.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ex.521024.cn

PHP:  // 无泛型
来源：http://ao.huanxung.cn

JS:   // 无泛型
来源：http://ny.shtwfgs.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ru.hnjuh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rb.jctech888.com.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gx.asd995.cn

Ruby: # 无泛型
来源：http://kj.panjiajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ut.shtwfgs.cn

[C15] 解构 / 展开参数
来源：http://xp.huixiangedu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zf.lnxyls.cn

PHP:  [$a, $b] = $pair;
来源：http://gn.nicolike.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xm.lnxyls.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ft.asd995.cn

Java: // 无解构
来源：http://dv.jctech888.com.cn

Go:   // 无解构
来源：http://gm.jctech888.com.cn

Ruby: a, b = pair
来源：http://je.lnxyls.cn

C#:   var (a, b) = pair;
来源：http://va.huanxung.cn

[C16] 函数 / 方法重载
来源：http://rw.gzmigu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vv.chemitech.net.cn

PHP:  // 无重载
来源：http://sx.gzmigu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ac.wgjwhj.cn

TS:   // 用联合类型或重载签名声明
来源：http://ig.chemitech.net.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gb.szxytkj.cn


<!-- 参考信息 -->