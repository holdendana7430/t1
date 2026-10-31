代发 wailian999

[B01] 条件判断 if / else
来源：http://xg.gzmigu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dg.huixinmuqiang.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dg.yuntaijiaju.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rz.yuexingan06.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mm.gzmigu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://hy.hahajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hk.521024.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wc.bjjhwx.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mz.hnjuh.cn

[B02] 多分支 else if / elif
来源：http://zu.wgjwhj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ui.bookmarksfly.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fc.yuexingan06.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ip.szsharing.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wj.yuexingan06.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yk.hahajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ds.yuexingan06.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bg.colortex.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mg.chemitech.net.cn

[B03] switch / match / case
来源：http://ux.nszjky.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wn.yuntaijiaju.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jw.huanxung.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://no.gzmigu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ng.bjjhwx.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tn.chemitech.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ww.huixiangedu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://om.yuexingan06.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hd.chemitech.net.cn

[B04] for 计数循环
来源：http://dy.szxytkj.cn

Py:   for i in range(10): print(i)
来源：http://if.haigaiapp.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://di.521024.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jo.lnxyls.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://an.chemitech.net.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pw.huanxung.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xg.szsharing.cn

Ruby: 10.times { |i| puts i }
来源：http://do.haigaiapp.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ig.muxihuayi.cn

[B05] 遍历数组 / 列表
来源：http://ij.nicolike.cn

Py:   for item in arr: print(item)
来源：http://gn.colortex.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ln.haigaiapp.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://eh.wgjwhj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://pa.szsharing.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://bu.shtwfgs.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cs.chemitech.net.cn

Ruby: arr.each { |item| puts item }
来源：http://wa.521024.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zw.wgjwhj.cn

[B06] 遍历字典 / 对象
来源：http://os.huixiangedu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://bg.panjiajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ev.nszjky.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jb.nszjky.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nf.chemitech.net.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bu.jianghongdianzi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://it.shxzskj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ji.huixinmuqiang.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ji.jianghongdianzi.cn

[B07] while 循环
来源：http://re.panjiajie.cn

Py:   while i < 10: i += 1
来源：http://oc.muxihuayi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://dg.bjjhwx.cn

JS:   while (i < 10) { i++; }
来源：http://vv.huixinmuqiang.cn

TS:   while (i < 10) { i++; }
来源：http://gi.bookmarksfly.cn

Java: while (i < 10) { i++; }
来源：http://rv.yuntaijiaju.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://th.yuexingan06.cn

Ruby: while i < 10; i += 1; end
来源：http://wm.yuntaijiaju.cn

C#:   while (i < 10) { i++; }
来源：http://cz.jctech888.com.cn

[B08] do-while（至少执行一次）
来源：http://dv.newstarts.cn

Py:   # 无 do-while：用 while True + break
来源：http://rz.wgjwhj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mk.yuexingan06.cn

JS:   do { i++; } while (i < 10);
来源：http://pw.newstarts.cn

TS:   do { i++; } while (i < 10);
来源：http://dg.huixinmuqiang.cn

Java: do { i++; } while (i < 10);
来源：http://rn.panjiajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jp.nicolike.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ov.hnjuh.cn

C#:   do { i++; } while (i < 10);
来源：http://ow.chemitech.net.cn

[B09] break 与 continue
来源：http://lg.yuntaijiaju.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bp.shxzskj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gk.nszjky.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yk.haigaiapp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fq.gzmigu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://le.muxihuayi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lr.muxihuayi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pd.jctech888.com.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wo.nszjky.cn

[B10] 遍历同时拿索引
来源：http://cj.haigaiapp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jh.shxzskj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pf.shxzskj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cc.jctech888.com.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://of.szxytkj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://oc.wgjwhj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://er.asd995.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jk.bookmarksfly.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kr.huanxung.cn

[B11] 生成数字序列 / 区间
来源：http://ix.gzmigu.cn

Py:   list(range(0, 10, 2))
来源：http://je.wgjwhj.cn

PHP:  range(0, 10, 2);
来源：http://jz.szsharing.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ck.jctech888.com.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ot.bjjhwx.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rr.yuntaijiaju.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wn.huanxung.cn

Ruby: (0...10).step(2).to_a
来源：http://nn.nicolike.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://iy.shtwfgs.cn

[B12] 跳出多层循环
来源：http://tv.hahajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://st.muxihuayi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://yo.haigaiapp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kz.huixiangedu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sz.wgjwhj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hi.hnjuh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nh.asd995.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pg.nicolike.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://og.jianghongdianzi.cn

[B13] 判断是否为数字
来源：http://dk.yuexingan06.cn

Py:   isinstance(x, (int, float))
来源：http://mi.jctech888.com.cn

PHP:  is_numeric($x)
来源：http://yj.wgjwhj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vv.newstarts.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zz.huixiangedu.cn

Java: x instanceof Number
来源：http://xf.nicolike.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uw.haigaiapp.cn

Ruby: x.is_a?(Numeric)
来源：http://xb.huanxung.cn

C#:   x is int or double or decimal
来源：http://ea.asd995.cn

[B14] 判断值是否在集合内
来源：http://qb.asd995.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://np.haigaiapp.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ry.shtwfgs.cn

JS:   [1, 2, 3].includes(x)
来源：http://zi.asd995.cn

TS:   [1, 2, 3].includes(x)
来源：http://zj.shxzskj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ju.huanxung.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sp.szxytkj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jn.jctech888.com.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://se.521024.cn

[B15] 布尔运算与取反
来源：http://oq.jctech888.com.cn

Py:   a and b or not c
来源：http://vz.lnxyls.cn

PHP:  $a && $b || !$c
来源：http://mm.nszjky.cn

JS:   a && b || !c
来源：http://fq.shxzukj.cn

TS:   a && b || !c
来源：http://hx.bookmarksfly.cn

Java: a && b || !c
来源：http://by.shxzskj.cn

Go:   a && b || !c
来源：http://fd.szsharing.cn

Ruby: a && b || !c
来源：http://il.huanxung.cn

C#:   a && b || !c
来源：http://hp.hnjuh.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ct.colortex.cn

Py:   if not data: return
来源：http://uu.chemitech.net.cn

PHP:  if (!$data) { return; }
来源：http://gh.shtwfgs.cn

JS:   if (!data) return;
来源：http://rf.haigaiapp.cn

TS:   if (!data) return;
来源：http://an.shtwfgs.cn

Java: if (data == null) return;
来源：http://fe.nszjky.cn

Go:   if data == nil { return }
来源：http://eu.panjiajie.cn

Ruby: return if data.nil?
来源：http://nc.shxzukj.cn

C#:   if (data == null) return;
来源：http://uy.yuntaijiaju.cn

================================================================================
来源：http://dy.lnxyls.cn

C. 函数与作用域
来源：http://ud.bjjhwx.cn

================================================================================
来源：http://ny.colortex.cn

[C01] 定义函数
来源：http://kw.haigaiapp.cn

Py:   def add(a, b): return a + b
来源：http://np.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vz.newstarts.cn

JS:   function add(a, b) { return a + b; }
来源：http://ml.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pf.chemitech.net.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vd.gzmigu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ui.shtwfgs.cn

Ruby: def add(a, b); a + b; end
来源：http://ku.asd995.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://co.9csxet.cn

[C02] 默认参数
来源：http://qy.shtwfgs.cn

Py:   def greet(name="World"): return name
来源：http://uw.huanxung.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://aq.jianghongdianzi.cn

JS:   function greet(name = "World") { return name; }
来源：http://tk.bjjhwx.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ac.lnxyls.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://al.bjjhwx.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wt.nicolike.cn

Ruby: def greet(name = "World") = name
来源：http://lt.lnxyls.cn

C#:   string Greet(string name = "World") => name;
来源：http://ki.nszjky.cn

[C03] 可变参数
来源：http://yk.9csxet.cn

Py:   def total(*args): return sum(args)
来源：http://jc.lnxyls.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ci.jianghongdianzi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://px.521024.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cm.521024.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vf.huixiangedu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wn.shtwfgs.cn

Ruby: def total(*nums); nums.sum; end
来源：http://kb.yuntaijiaju.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zy.huanxung.cn

[C04] 命名参数 / 关键字参数
来源：http://ov.panjiajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dl.gzmigu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fj.colortex.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tn.panjiajie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mq.bookmarksfly.cn

Java: // 无：用 Builder 模式或 record
来源：http://vq.chemitech.net.cn

Go:   // 无：用配置结构体参数
来源：http://se.gzmigu.cn

Ruby: f(a: 1, b: 2)
来源：http://lc.shxzskj.cn

C#:   f(a: 1, b: 2)
来源：http://wy.yuexingan06.cn

[C05] 返回多个值
来源：http://zg.bjjhwx.cn

Py:   return a, b
来源：http://vv.panjiajie.cn

PHP:  return [$a, $b];
来源：http://hu.521024.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ew.hnjuh.cn

TS:   return { a, b };
来源：http://oh.jianghongdianzi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mh.hahajie.cn

Go:   return a, b
来源：http://fd.gzmigu.cn

Ruby: return a, b
来源：http://ti.bookmarksfly.cn

C#:   return (a, b);              // ValueTuple
来源：http://ja.chemitech.net.cn

[C06] 匿名函数 / lambda
来源：http://zv.shxzskj.cn

Py:   square = lambda x: x * x
来源：http://cs.yuntaijiaju.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://nf.yuexingan06.cn

JS:   const square = x => x * x;
来源：http://jn.chemitech.net.cn

TS:   const square = (x: number): number => x * x;
来源：http://he.szxytkj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kz.yuexingan06.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ra.yuntaijiaju.cn

Ruby: square = ->(x) { x * x }
来源：http://af.szsharing.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ix.hahajie.cn

[C07] 把函数作为参数传入
来源：http://jo.9csxet.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://if.chemitech.net.cn

PHP:  array_map("strtoupper", $arr);
来源：http://nc.nszjky.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vv.521024.cn

TS:   arr.map(String)
来源：http://ch.yuexingan06.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vy.jctech888.com.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ha.shxzukj.cn

Ruby: arr.map(&:upcase)
来源：http://tt.szsharing.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://kt.panjiajie.cn

[C08] 闭包
来源：http://lv.nicolike.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fa.asd995.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hc.shxzskj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ry.hnjuh.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://oe.hahajie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vq.chemitech.net.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zx.bookmarksfly.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://iq.huixinmuqiang.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xo.newstarts.cn

[C09] 递归
来源：http://tm.jctech888.com.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ab.huixinmuqiang.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hl.gzmigu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ws.asd995.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jz.lnxyls.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nj.wgjwhj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xa.shxzskj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mc.shtwfgs.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zy.nszjky.cn

[C10] 变量作用域
来源：http://al.hahajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gf.haigaiapp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nj.szxytkj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ku.shtwfgs.cn

TS:   同 JS
来源：http://la.shxzskj.cn

Java: 方法内为块级作用域
来源：http://hf.szsharing.cn

Go:   花括号块级作用域
来源：http://ay.jianghongdianzi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ip.bjjhwx.cn

C#:   块级作用域
来源：http://pg.nicolike.cn

[C11] 模块导入与导出
来源：http://rx.panjiajie.cn

Py:   from module import func
来源：http://nh.lnxyls.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kl.chemitech.net.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ta.szxytkj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fo.muxihuayi.cn

Java: import java.util.List;
来源：http://ks.szxytkj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cc.bjjhwx.cn

Ruby: require "json"; require_relative "./util"
来源：http://da.shxzskj.cn

C#:   using System.Text;
来源：http://gt.shtwfgs.cn

[C12] 立即执行函数 IIFE
来源：http://jd.nszjky.cn

Py:   (lambda: print("run"))()
来源：http://ww.panjiajie.cn

PHP:  (function () { echo "run"; })();
来源：http://vy.huanxung.cn

JS:   (() => { console.log("run"); })();
来源：http://yh.bjjhwx.cn

TS:   (() => { console.log("run"); })();
来源：http://ib.asd995.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ww.muxihuayi.cn

Go:   func() { fmt.Println("run") }()
来源：http://dh.hahajie.cn

Ruby: -> { puts "run" }.call
来源：http://bb.jianghongdianzi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://st.521024.cn

[C13] 类型声明 / 类型注解
来源：http://jq.bjjhwx.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://va.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ol.huixinmuqiang.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://od.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vx.lnxyls.cn

Java: int add(int a, int b) { return a + b; }
来源：http://un.hnjuh.cn

Go:   func add(a, b int) int
来源：http://hr.newstarts.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uz.nicolike.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tp.lnxyls.cn

[C14] 泛型函数
来源：http://li.nicolike.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://as.jianghongdianzi.cn

PHP:  // 无泛型
来源：http://eh.muxihuayi.cn

JS:   // 无泛型
来源：http://li.521024.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mz.yuexingan06.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zx.szsharing.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://en.shtwfgs.cn

Ruby: # 无泛型
来源：http://lq.bjjhwx.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zs.jctech888.com.cn

[C15] 解构 / 展开参数
来源：http://jx.jctech888.com.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kv.nszjky.cn

PHP:  [$a, $b] = $pair;
来源：http://ee.shxzskj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xa.yuntaijiaju.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vl.9csxet.cn

Java: // 无解构
来源：http://ts.asd995.cn

Go:   // 无解构
来源：http://wk.yuntaijiaju.cn

Ruby: a, b = pair
来源：http://gx.521024.cn

C#:   var (a, b) = pair;
来源：http://oz.szxytkj.cn

[C16] 函数 / 方法重载
来源：http://tr.chemitech.net.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ex.yuntaijiaju.cn

PHP:  // 无重载
来源：http://pm.shxzukj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ee.hahajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://wk.huixiangedu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wj.asd995.cn

Go:   // 无重载：用不同函数名
来源：http://dx.shxzukj.cn

Ruby: # 无重载：靠动态参数
来源：http://rt.shtwfgs.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://sx.bjjhwx.cn

================================================================================
来源：http://eb.521024.cn

D. 数组 / 列表 / 集合
来源：http://jh.asd995.cn

================================================================================
来源：http://ka.nszjky.cn

[D01] 创建数组 / 列表
来源：http://hi.jctech888.com.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hc.chemitech.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ry.shxzukj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cx.shtwfgs.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dt.yuexingan06.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://it.bjjhwx.cn


<!-- 参考信息 -->