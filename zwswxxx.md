代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://kb.szsharing.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pa.bookmarksfly.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kg.yuntaijiaju.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vn.yuntaijiaju.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jt.colortex.cn

================================================================================
来源：http://wc.muxihuayi.cn

B. 流程控制
来源：http://rj.yuexingan06.cn

================================================================================
来源：http://lb.nszjky.cn

[B01] 条件判断 if / else
来源：http://ek.gzmigu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://uy.hahajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ra.lnxyls.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tf.shtwfgs.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ly.huixinmuqiang.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ay.bookmarksfly.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hq.shxzukj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bc.hahajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qf.huixiangedu.cn

[B02] 多分支 else if / elif
来源：http://st.hnjuh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ov.hahajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ba.yuntaijiaju.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vw.hnjuh.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vf.hahajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ne.yuexingan06.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tc.gzmigu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dt.gzmigu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qr.nszjky.cn

[B03] switch / match / case
来源：http://no.wgjwhj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yb.huixinmuqiang.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tu.yuexingan06.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://de.jianghongdianzi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mf.huixiangedu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bp.panjiajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://go.yuntaijiaju.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nb.jctech888.com.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fa.panjiajie.cn

[B04] for 计数循环
来源：http://te.bookmarksfly.cn

Py:   for i in range(10): print(i)
来源：http://xu.hahajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://oa.muxihuayi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lp.gzmigu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rd.shxzskj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cu.shxzukj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cz.jianghongdianzi.cn

Ruby: 10.times { |i| puts i }
来源：http://zk.yuntaijiaju.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ks.shxzskj.cn

[B05] 遍历数组 / 列表
来源：http://vc.shxzukj.cn

Py:   for item in arr: print(item)
来源：http://mn.haigaiapp.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yg.521024.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dc.521024.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://uf.9csxet.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://rg.asd995.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://iz.nszjky.cn

Ruby: arr.each { |item| puts item }
来源：http://zt.bjjhwx.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vv.yuntaijiaju.cn

[B06] 遍历字典 / 对象
来源：http://cm.bookmarksfly.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://jf.newstarts.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lj.jianghongdianzi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fs.panjiajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qt.521024.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ge.huixinmuqiang.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ci.wgjwhj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ca.huixiangedu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gh.huanxung.cn

[B07] while 循环
来源：http://bd.panjiajie.cn

Py:   while i < 10: i += 1
来源：http://tk.shxzukj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xb.lnxyls.cn

JS:   while (i < 10) { i++; }
来源：http://in.asd995.cn

TS:   while (i < 10) { i++; }
来源：http://sj.szsharing.cn

Java: while (i < 10) { i++; }
来源：http://ql.bjjhwx.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://oh.asd995.cn

Ruby: while i < 10; i += 1; end
来源：http://kt.hnjuh.cn

C#:   while (i < 10) { i++; }
来源：http://dg.gzmigu.cn

[B08] do-while（至少执行一次）
来源：http://bi.huanxung.cn

Py:   # 无 do-while：用 while True + break
来源：http://qj.bookmarksfly.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://td.colortex.cn

JS:   do { i++; } while (i < 10);
来源：http://yq.shxzskj.cn

TS:   do { i++; } while (i < 10);
来源：http://na.nszjky.cn

Java: do { i++; } while (i < 10);
来源：http://em.szxytkj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ao.jctech888.com.cn

Ruby: begin; i += 1; end while i < 10
来源：http://aq.521024.cn

C#:   do { i++; } while (i < 10);
来源：http://vm.muxihuayi.cn

[B09] break 与 continue
来源：http://lm.jctech888.com.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://te.szsharing.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://is.yuexingan06.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://np.asd995.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://le.shtwfgs.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sg.szsharing.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vk.hahajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ka.nszjky.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ce.shxzskj.cn

[B10] 遍历同时拿索引
来源：http://gx.haigaiapp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ya.jctech888.com.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dp.hnjuh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sp.bjjhwx.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ik.panjiajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uo.hahajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vb.9csxet.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qk.lnxyls.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cj.wgjwhj.cn

[B11] 生成数字序列 / 区间
来源：http://fg.lnxyls.cn

Py:   list(range(0, 10, 2))
来源：http://rx.muxihuayi.cn

PHP:  range(0, 10, 2);
来源：http://ww.hahajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pm.newstarts.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dm.jianghongdianzi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ac.jctech888.com.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hv.shxzukj.cn

Ruby: (0...10).step(2).to_a
来源：http://hg.hahajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ow.shxzskj.cn

[B12] 跳出多层循环
来源：http://xt.szsharing.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://nt.bjjhwx.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://xu.gzmigu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ek.chemitech.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wf.yuexingan06.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mt.shxzskj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yf.asd995.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jw.lnxyls.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lb.jctech888.com.cn

[B13] 判断是否为数字
来源：http://dt.shtwfgs.cn

Py:   isinstance(x, (int, float))
来源：http://pl.521024.cn

PHP:  is_numeric($x)
来源：http://ie.wgjwhj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ze.wgjwhj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ny.bookmarksfly.cn

Java: x instanceof Number
来源：http://wf.hahajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zy.wgjwhj.cn

Ruby: x.is_a?(Numeric)
来源：http://rm.muxihuayi.cn

C#:   x is int or double or decimal
来源：http://nw.yuexingan06.cn

[B14] 判断值是否在集合内
来源：http://wh.haigaiapp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tf.bjjhwx.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://od.nszjky.cn

JS:   [1, 2, 3].includes(x)
来源：http://yz.shxzukj.cn

TS:   [1, 2, 3].includes(x)
来源：http://lu.huixiangedu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://oj.szsharing.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fc.hahajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ac.shxzskj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fb.lnxyls.cn

[B15] 布尔运算与取反
来源：http://dg.shxzukj.cn

Py:   a and b or not c
来源：http://rk.lnxyls.cn

PHP:  $a && $b || !$c
来源：http://nf.9csxet.cn

JS:   a && b || !c
来源：http://vs.szsharing.cn

TS:   a && b || !c
来源：http://uw.hnjuh.cn

Java: a && b || !c
来源：http://zc.panjiajie.cn

Go:   a && b || !c
来源：http://cj.szxytkj.cn

Ruby: a && b || !c
来源：http://fd.bjjhwx.cn

C#:   a && b || !c
来源：http://ar.panjiajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zw.lnxyls.cn

Py:   if not data: return
来源：http://dp.colortex.cn

PHP:  if (!$data) { return; }
来源：http://rz.jctech888.com.cn

JS:   if (!data) return;
来源：http://id.asd995.cn

TS:   if (!data) return;
来源：http://tx.bjjhwx.cn

Java: if (data == null) return;
来源：http://og.colortex.cn

Go:   if data == nil { return }
来源：http://me.shxzskj.cn

Ruby: return if data.nil?
来源：http://xk.szxytkj.cn

C#:   if (data == null) return;
来源：http://zq.huixiangedu.cn

================================================================================
来源：http://pz.yuexingan06.cn

C. 函数与作用域
来源：http://jf.szxytkj.cn

================================================================================
来源：http://wj.hahajie.cn

[C01] 定义函数
来源：http://yx.asd995.cn

Py:   def add(a, b): return a + b
来源：http://uo.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ua.hahajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://gx.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sp.nicolike.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://sk.shtwfgs.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xk.haigaiapp.cn

Ruby: def add(a, b); a + b; end
来源：http://lx.szxytkj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://np.bjjhwx.cn

[C02] 默认参数
来源：http://zu.gzmigu.cn

Py:   def greet(name="World"): return name
来源：http://go.shxzskj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://br.shxzskj.cn

JS:   function greet(name = "World") { return name; }
来源：http://gb.asd995.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://do.colortex.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://al.bjjhwx.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ib.yuexingan06.cn

Ruby: def greet(name = "World") = name
来源：http://cg.szsharing.cn

C#:   string Greet(string name = "World") => name;
来源：http://eq.huixiangedu.cn

[C03] 可变参数
来源：http://nx.nszjky.cn

Py:   def total(*args): return sum(args)
来源：http://wa.szxytkj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uj.huanxung.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://et.huixinmuqiang.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wi.hahajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://au.haigaiapp.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xj.gzmigu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://sz.shxzskj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://aw.9csxet.cn

[C04] 命名参数 / 关键字参数
来源：http://lo.521024.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fd.hnjuh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zf.hahajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kt.asd995.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://iw.szsharing.cn

Java: // 无：用 Builder 模式或 record
来源：http://gt.huixiangedu.cn

Go:   // 无：用配置结构体参数
来源：http://qt.hahajie.cn

Ruby: f(a: 1, b: 2)
来源：http://vj.huixinmuqiang.cn

C#:   f(a: 1, b: 2)
来源：http://sk.yuexingan06.cn

[C05] 返回多个值
来源：http://sh.chemitech.net.cn

Py:   return a, b
来源：http://ct.asd995.cn

PHP:  return [$a, $b];
来源：http://du.haigaiapp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xg.szsharing.cn

TS:   return { a, b };
来源：http://dz.huixinmuqiang.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yy.521024.cn

Go:   return a, b
来源：http://vb.colortex.cn

Ruby: return a, b
来源：http://db.nszjky.cn

C#:   return (a, b);              // ValueTuple
来源：http://gy.huixinmuqiang.cn

[C06] 匿名函数 / lambda
来源：http://pe.yuexingan06.cn

Py:   square = lambda x: x * x
来源：http://yt.huixiangedu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://en.huixiangedu.cn

JS:   const square = x => x * x;
来源：http://th.huixiangedu.cn

TS:   const square = (x: number): number => x * x;
来源：http://ck.shtwfgs.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pl.szsharing.cn

Go:   sq := func(x int) int { return x * x }
来源：http://re.hahajie.cn

Ruby: square = ->(x) { x * x }
来源：http://oy.shxzskj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://mf.huixiangedu.cn

[C07] 把函数作为参数传入
来源：http://oy.newstarts.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ar.szsharing.cn

PHP:  array_map("strtoupper", $arr);
来源：http://yc.wgjwhj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ax.521024.cn

TS:   arr.map(String)
来源：http://rr.colortex.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fv.haigaiapp.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hm.shtwfgs.cn

Ruby: arr.map(&:upcase)
来源：http://vh.yuntaijiaju.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://sv.szxytkj.cn

[C08] 闭包
来源：http://ax.haigaiapp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mp.huixinmuqiang.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zy.yuntaijiaju.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bc.yuntaijiaju.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ts.wgjwhj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bs.bjjhwx.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gx.szsharing.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tr.bookmarksfly.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gc.huanxung.cn

[C09] 递归
来源：http://ya.lnxyls.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hs.newstarts.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pq.521024.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mq.huixiangedu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dk.wgjwhj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kb.nicolike.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://la.haigaiapp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cd.lnxyls.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jh.asd995.cn

[C10] 变量作用域
来源：http://zv.szxytkj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zc.huanxung.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://af.huixinmuqiang.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://or.521024.cn

TS:   同 JS
来源：http://tp.huixinmuqiang.cn

Java: 方法内为块级作用域
来源：http://dp.shxzukj.cn

Go:   花括号块级作用域
来源：http://ku.hahajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lh.jianghongdianzi.cn

C#:   块级作用域
来源：http://cf.bjjhwx.cn

[C11] 模块导入与导出
来源：http://ts.huixinmuqiang.cn

Py:   from module import func
来源：http://fd.muxihuayi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://po.shxzukj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gs.chemitech.net.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://oe.nszjky.cn

Java: import java.util.List;
来源：http://ug.nicolike.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fr.hnjuh.cn

Ruby: require "json"; require_relative "./util"
来源：http://mk.nicolike.cn

C#:   using System.Text;
来源：http://gy.chemitech.net.cn

[C12] 立即执行函数 IIFE
来源：http://ng.shxzskj.cn

Py:   (lambda: print("run"))()
来源：http://hf.nszjky.cn

PHP:  (function () { echo "run"; })();
来源：http://sg.hahajie.cn

JS:   (() => { console.log("run"); })();
来源：http://tb.shxzukj.cn

TS:   (() => { console.log("run"); })();
来源：http://lv.nicolike.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lc.shxzskj.cn

Go:   func() { fmt.Println("run") }()
来源：http://xy.huanxung.cn

Ruby: -> { puts "run" }.call
来源：http://hp.newstarts.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xm.colortex.cn

[C13] 类型声明 / 类型注解
来源：http://pm.bookmarksfly.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://be.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xs.hahajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vy.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ut.szxytkj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jh.nicolike.cn

Go:   func add(a, b int) int
来源：http://wf.muxihuayi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xl.panjiajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nl.jianghongdianzi.cn

[C14] 泛型函数
来源：http://ls.bjjhwx.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qm.szsharing.cn

PHP:  // 无泛型
来源：http://no.newstarts.cn

JS:   // 无泛型
来源：http://ng.asd995.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gm.shxzskj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xn.jctech888.com.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ue.colortex.cn

Ruby: # 无泛型
来源：http://un.yuntaijiaju.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ts.gzmigu.cn

[C15] 解构 / 展开参数
来源：http://yh.haigaiapp.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xt.szsharing.cn

PHP:  [$a, $b] = $pair;
来源：http://nz.newstarts.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mn.nszjky.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wz.newstarts.cn

Java: // 无解构
来源：http://xh.521024.cn

Go:   // 无解构
来源：http://lo.szxytkj.cn

Ruby: a, b = pair
来源：http://jz.panjiajie.cn

C#:   var (a, b) = pair;
来源：http://nt.chemitech.net.cn

[C16] 函数 / 方法重载
来源：http://wk.muxihuayi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rg.yuexingan06.cn

PHP:  // 无重载
来源：http://xa.bjjhwx.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://tn.panjiajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://zi.nicolike.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qp.jctech888.com.cn

Go:   // 无重载：用不同函数名
来源：http://se.szsharing.cn

Ruby: # 无重载：靠动态参数
来源：http://un.hnjuh.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ng.yuntaijiaju.cn

================================================================================
来源：http://ie.wgjwhj.cn


<!-- 参考信息 -->