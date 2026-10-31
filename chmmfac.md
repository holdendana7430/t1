代发 wailian999

[A26] 类型转换总览
来源：http://ec.newstarts.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jm.jctech888.com.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pz.bookmarksfly.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kt.gzmigu.cn

TS:   Number() String() Boolean() x as number
来源：http://wf.gzmigu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://af.haigaiapp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fj.panjiajie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://nc.bjjhwx.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fm.nszjky.cn

================================================================================
来源：http://uq.szsharing.cn

B. 流程控制
来源：http://qp.huanxung.cn

================================================================================
来源：http://mj.yuexingan06.cn

[B01] 条件判断 if / else
来源：http://uu.huanxung.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://cs.panjiajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qt.lnxyls.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gl.jianghongdianzi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wu.hnjuh.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://hj.chemitech.net.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ex.newstarts.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xd.nicolike.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fb.chemitech.net.cn

[B02] 多分支 else if / elif
来源：http://tk.gzmigu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bm.szxytkj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zq.shxzukj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qz.colortex.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qx.asd995.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yy.bookmarksfly.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hj.jctech888.com.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://em.521024.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://my.jctech888.com.cn

[B03] switch / match / case
来源：http://xs.yuntaijiaju.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xq.9csxet.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tz.huixinmuqiang.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zh.lnxyls.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bt.jianghongdianzi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bi.szsharing.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://le.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cs.huixinmuqiang.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://na.shxzskj.cn

[B04] for 计数循环
来源：http://sf.hahajie.cn

Py:   for i in range(10): print(i)
来源：http://ky.szsharing.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ci.nszjky.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pb.yuntaijiaju.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lk.jctech888.com.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dd.shtwfgs.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://su.huixiangedu.cn

Ruby: 10.times { |i| puts i }
来源：http://qy.521024.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qk.nicolike.cn

[B05] 遍历数组 / 列表
来源：http://iw.chemitech.net.cn

Py:   for item in arr: print(item)
来源：http://uy.yuntaijiaju.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lj.shxzskj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://mc.gzmigu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://lm.nszjky.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ol.bookmarksfly.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pq.shxzukj.cn

Ruby: arr.each { |item| puts item }
来源：http://uw.521024.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cq.szxytkj.cn

[B06] 遍历字典 / 对象
来源：http://sw.gzmigu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://du.hnjuh.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rh.lnxyls.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dc.gzmigu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nj.shxzskj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://au.gzmigu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ic.haigaiapp.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gi.colortex.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jf.bjjhwx.cn

[B07] while 循环
来源：http://cg.jctech888.com.cn

Py:   while i < 10: i += 1
来源：http://ov.haigaiapp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://nf.shtwfgs.cn

JS:   while (i < 10) { i++; }
来源：http://ea.szxytkj.cn

TS:   while (i < 10) { i++; }
来源：http://za.bookmarksfly.cn

Java: while (i < 10) { i++; }
来源：http://rp.wgjwhj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ym.nicolike.cn

Ruby: while i < 10; i += 1; end
来源：http://rw.hnjuh.cn

C#:   while (i < 10) { i++; }
来源：http://mv.colortex.cn

[B08] do-while（至少执行一次）
来源：http://ku.asd995.cn

Py:   # 无 do-while：用 while True + break
来源：http://ci.haigaiapp.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ir.shxzukj.cn

JS:   do { i++; } while (i < 10);
来源：http://up.nszjky.cn

TS:   do { i++; } while (i < 10);
来源：http://oo.9csxet.cn

Java: do { i++; } while (i < 10);
来源：http://xg.lnxyls.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://kd.chemitech.net.cn

Ruby: begin; i += 1; end while i < 10
来源：http://tj.colortex.cn

C#:   do { i++; } while (i < 10);
来源：http://ma.yuntaijiaju.cn

[B09] break 与 continue
来源：http://ou.hahajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://do.huanxung.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lk.haigaiapp.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ld.asd995.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://os.yuntaijiaju.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jz.shxzskj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cx.nicolike.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xv.haigaiapp.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ss.nicolike.cn

[B10] 遍历同时拿索引
来源：http://yy.huixiangedu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mh.yuexingan06.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zw.wgjwhj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vk.huixinmuqiang.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nb.shxzskj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sv.521024.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://by.nszjky.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://aj.521024.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jb.bjjhwx.cn

[B11] 生成数字序列 / 区间
来源：http://pw.nszjky.cn

Py:   list(range(0, 10, 2))
来源：http://zy.huixiangedu.cn

PHP:  range(0, 10, 2);
来源：http://pc.nszjky.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kp.521024.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lb.hnjuh.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wq.wgjwhj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://br.huixinmuqiang.cn

Ruby: (0...10).step(2).to_a
来源：http://wx.jianghongdianzi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bi.shxzukj.cn

[B12] 跳出多层循环
来源：http://dh.shxzskj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tg.shxzukj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://db.asd995.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lb.yuntaijiaju.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qd.huixinmuqiang.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nu.szxytkj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hu.shtwfgs.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kc.521024.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://th.nicolike.cn

[B13] 判断是否为数字
来源：http://en.haigaiapp.cn

Py:   isinstance(x, (int, float))
来源：http://wg.shxzukj.cn

PHP:  is_numeric($x)
来源：http://tc.jctech888.com.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zu.yuntaijiaju.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mg.nszjky.cn

Java: x instanceof Number
来源：http://wa.lnxyls.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ha.szxytkj.cn

Ruby: x.is_a?(Numeric)
来源：http://uv.hnjuh.cn

C#:   x is int or double or decimal
来源：http://ep.shtwfgs.cn

[B14] 判断值是否在集合内
来源：http://io.shtwfgs.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kj.asd995.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tb.haigaiapp.cn

JS:   [1, 2, 3].includes(x)
来源：http://st.521024.cn

TS:   [1, 2, 3].includes(x)
来源：http://kr.bjjhwx.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://nw.nszjky.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cg.shxzukj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://at.lnxyls.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jq.521024.cn

[B15] 布尔运算与取反
来源：http://jx.shxzukj.cn

Py:   a and b or not c
来源：http://xv.szxytkj.cn

PHP:  $a && $b || !$c
来源：http://xi.haigaiapp.cn

JS:   a && b || !c
来源：http://mm.nszjky.cn

TS:   a && b || !c
来源：http://zh.colortex.cn

Java: a && b || !c
来源：http://ak.yuexingan06.cn

Go:   a && b || !c
来源：http://ty.huanxung.cn

Ruby: a && b || !c
来源：http://ub.bjjhwx.cn

C#:   a && b || !c
来源：http://ij.colortex.cn

[B16] 卫语句：不满足条件提前返回
来源：http://rf.shxzukj.cn

Py:   if not data: return
来源：http://wc.gzmigu.cn

PHP:  if (!$data) { return; }
来源：http://st.shxzskj.cn

JS:   if (!data) return;
来源：http://oi.lnxyls.cn

TS:   if (!data) return;
来源：http://aa.jctech888.com.cn

Java: if (data == null) return;
来源：http://gc.szxytkj.cn

Go:   if data == nil { return }
来源：http://qv.muxihuayi.cn

Ruby: return if data.nil?
来源：http://wd.gzmigu.cn

C#:   if (data == null) return;
来源：http://pq.yuntaijiaju.cn

================================================================================
来源：http://at.huixinmuqiang.cn

C. 函数与作用域
来源：http://dk.gzmigu.cn

================================================================================
来源：http://qe.jctech888.com.cn

[C01] 定义函数
来源：http://io.colortex.cn

Py:   def add(a, b): return a + b
来源：http://kr.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qn.wgjwhj.cn

JS:   function add(a, b) { return a + b; }
来源：http://jr.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ia.wgjwhj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://du.newstarts.cn

Go:   func add(a, b int) int { return a + b }
来源：http://yy.521024.cn

Ruby: def add(a, b); a + b; end
来源：http://xj.huixinmuqiang.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://io.lnxyls.cn

[C02] 默认参数
来源：http://yb.shtwfgs.cn

Py:   def greet(name="World"): return name
来源：http://yt.521024.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://oh.hahajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://cn.huixinmuqiang.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gs.shxzskj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://uf.huixiangedu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ak.gzmigu.cn

Ruby: def greet(name = "World") = name
来源：http://kv.nszjky.cn

C#:   string Greet(string name = "World") => name;
来源：http://kn.521024.cn

[C03] 可变参数
来源：http://us.bookmarksfly.cn

Py:   def total(*args): return sum(args)
来源：http://cv.hnjuh.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wg.huixiangedu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tm.wgjwhj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zg.shxzukj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zy.wgjwhj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hs.jctech888.com.cn

Ruby: def total(*nums); nums.sum; end
来源：http://op.szxytkj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cd.asd995.cn

[C04] 命名参数 / 关键字参数
来源：http://bx.shxzskj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ii.9csxet.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ns.nszjky.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tx.yuexingan06.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ux.muxihuayi.cn

Java: // 无：用 Builder 模式或 record
来源：http://yn.9csxet.cn

Go:   // 无：用配置结构体参数
来源：http://pw.yuexingan06.cn

Ruby: f(a: 1, b: 2)
来源：http://ho.bookmarksfly.cn

C#:   f(a: 1, b: 2)
来源：http://sx.bjjhwx.cn

[C05] 返回多个值
来源：http://gn.nicolike.cn

Py:   return a, b
来源：http://nq.jctech888.com.cn

PHP:  return [$a, $b];
来源：http://xd.haigaiapp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wx.shxzukj.cn

TS:   return { a, b };
来源：http://va.haigaiapp.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jo.chemitech.net.cn

Go:   return a, b
来源：http://py.newstarts.cn

Ruby: return a, b
来源：http://ws.shxzskj.cn

C#:   return (a, b);              // ValueTuple
来源：http://kt.szxytkj.cn

[C06] 匿名函数 / lambda
来源：http://ee.yuntaijiaju.cn

Py:   square = lambda x: x * x
来源：http://hb.colortex.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ig.nszjky.cn

JS:   const square = x => x * x;
来源：http://nn.chemitech.net.cn

TS:   const square = (x: number): number => x * x;
来源：http://qk.muxihuayi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zk.huixiangedu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ty.9csxet.cn

Ruby: square = ->(x) { x * x }
来源：http://og.colortex.cn

C#:   Func<int, int> square = x => x * x;
来源：http://pt.521024.cn

[C07] 把函数作为参数传入
来源：http://iz.bjjhwx.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wo.gzmigu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wh.hnjuh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cp.huixinmuqiang.cn

TS:   arr.map(String)
来源：http://gu.muxihuayi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zi.newstarts.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://em.muxihuayi.cn

Ruby: arr.map(&:upcase)
来源：http://rz.yuntaijiaju.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://eo.szxytkj.cn

[C08] 闭包
来源：http://fe.yuexingan06.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gd.muxihuayi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://va.haigaiapp.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://es.haigaiapp.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://oc.newstarts.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://od.panjiajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ok.huixinmuqiang.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pv.521024.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yr.yuexingan06.cn

[C09] 递归
来源：http://qv.yuntaijiaju.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lf.huixinmuqiang.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vg.hahajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nq.wgjwhj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://my.wgjwhj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ys.bjjhwx.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://oh.szxytkj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ii.newstarts.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fn.shtwfgs.cn

[C10] 变量作用域
来源：http://zd.yuntaijiaju.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ch.szxytkj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jr.bookmarksfly.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://av.jctech888.com.cn

TS:   同 JS
来源：http://xi.jctech888.com.cn

Java: 方法内为块级作用域
来源：http://qj.nicolike.cn

Go:   花括号块级作用域
来源：http://yk.yuexingan06.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zj.hahajie.cn

C#:   块级作用域
来源：http://oa.huixiangedu.cn

[C11] 模块导入与导出
来源：http://nj.huanxung.cn

Py:   from module import func
来源：http://jj.huanxung.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pr.chemitech.net.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://aw.colortex.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jc.gzmigu.cn

Java: import java.util.List;
来源：http://ck.shtwfgs.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://li.shxzskj.cn

Ruby: require "json"; require_relative "./util"
来源：http://pb.nicolike.cn

C#:   using System.Text;
来源：http://th.shtwfgs.cn

[C12] 立即执行函数 IIFE
来源：http://ab.shxzskj.cn

Py:   (lambda: print("run"))()
来源：http://qs.szsharing.cn

PHP:  (function () { echo "run"; })();
来源：http://rg.9csxet.cn

JS:   (() => { console.log("run"); })();
来源：http://si.hahajie.cn

TS:   (() => { console.log("run"); })();
来源：http://qf.haigaiapp.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ab.bjjhwx.cn

Go:   func() { fmt.Println("run") }()
来源：http://ob.lnxyls.cn

Ruby: -> { puts "run" }.call
来源：http://ni.huanxung.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ha.shxzskj.cn

[C13] 类型声明 / 类型注解
来源：http://rx.9csxet.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zc.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nx.asd995.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cj.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ym.bjjhwx.cn

Java: int add(int a, int b) { return a + b; }
来源：http://lo.muxihuayi.cn

Go:   func add(a, b int) int
来源：http://up.9csxet.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ip.gzmigu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wr.bookmarksfly.cn

[C14] 泛型函数
来源：http://nu.yuexingan06.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ul.yuexingan06.cn

PHP:  // 无泛型
来源：http://eu.jctech888.com.cn

JS:   // 无泛型
来源：http://ro.yuntaijiaju.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uv.wgjwhj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rz.colortex.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tu.hnjuh.cn

Ruby: # 无泛型
来源：http://us.nicolike.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zq.newstarts.cn

[C15] 解构 / 展开参数
来源：http://sf.panjiajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zt.nszjky.cn

PHP:  [$a, $b] = $pair;
来源：http://he.nszjky.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rq.jctech888.com.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dr.huixinmuqiang.cn

Java: // 无解构
来源：http://dx.muxihuayi.cn

Go:   // 无解构
来源：http://ze.huixiangedu.cn

Ruby: a, b = pair
来源：http://ga.huixinmuqiang.cn

C#:   var (a, b) = pair;
来源：http://pl.gzmigu.cn

[C16] 函数 / 方法重载
来源：http://xw.szxytkj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kp.colortex.cn

PHP:  // 无重载
来源：http://sx.newstarts.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ui.szsharing.cn

TS:   // 用联合类型或重载签名声明
来源：http://ub.muxihuayi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://vl.wgjwhj.cn


<!-- 参考信息 -->