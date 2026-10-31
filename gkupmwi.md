代发 wailian999

[B01] 条件判断 if / else
来源：http://cz.shxzskj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wv.hahajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hk.gzmigu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wa.lnxyls.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tk.gzmigu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qg.hahajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cc.huixinmuqiang.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ak.bookmarksfly.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pq.shxzskj.cn

[B02] 多分支 else if / elif
来源：http://ba.jianghongdianzi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://le.bjjhwx.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qz.shtwfgs.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qr.hahajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.szxytkj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mr.shxzskj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kh.bjjhwx.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rq.panjiajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://st.muxihuayi.cn

[B03] switch / match / case
来源：http://kj.521024.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hy.huixinmuqiang.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zv.nicolike.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zf.wgjwhj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ud.521024.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vc.hnjuh.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lb.bjjhwx.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://iy.bookmarksfly.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kq.yuntaijiaju.cn

[B04] for 计数循环
来源：http://az.wgjwhj.cn

Py:   for i in range(10): print(i)
来源：http://aa.haigaiapp.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ot.shxzukj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xw.nicolike.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yq.huixinmuqiang.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ky.jctech888.com.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tt.haigaiapp.cn

Ruby: 10.times { |i| puts i }
来源：http://xx.chemitech.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sr.jctech888.com.cn

[B05] 遍历数组 / 列表
来源：http://fw.9csxet.cn

Py:   for item in arr: print(item)
来源：http://sn.huanxung.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ab.wgjwhj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yh.jctech888.com.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mn.colortex.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://co.nicolike.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lt.hnjuh.cn

Ruby: arr.each { |item| puts item }
来源：http://lv.szxytkj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ud.szsharing.cn

[B06] 遍历字典 / 对象
来源：http://jb.gzmigu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://kg.yuntaijiaju.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nv.huixiangedu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dc.panjiajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vd.gzmigu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ah.newstarts.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ji.9csxet.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://py.colortex.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://iy.9csxet.cn

[B07] while 循环
来源：http://cs.gzmigu.cn

Py:   while i < 10: i += 1
来源：http://er.shxzskj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://oh.asd995.cn

JS:   while (i < 10) { i++; }
来源：http://qt.szsharing.cn

TS:   while (i < 10) { i++; }
来源：http://by.bookmarksfly.cn

Java: while (i < 10) { i++; }
来源：http://za.huanxung.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ew.szsharing.cn

Ruby: while i < 10; i += 1; end
来源：http://iu.newstarts.cn

C#:   while (i < 10) { i++; }
来源：http://of.szxytkj.cn

[B08] do-while（至少执行一次）
来源：http://jx.wgjwhj.cn

Py:   # 无 do-while：用 while True + break
来源：http://zv.szxytkj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pv.hnjuh.cn

JS:   do { i++; } while (i < 10);
来源：http://ea.jianghongdianzi.cn

TS:   do { i++; } while (i < 10);
来源：http://gc.nicolike.cn

Java: do { i++; } while (i < 10);
来源：http://hi.newstarts.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wc.haigaiapp.cn

Ruby: begin; i += 1; end while i < 10
来源：http://go.bookmarksfly.cn

C#:   do { i++; } while (i < 10);
来源：http://cm.huanxung.cn

[B09] break 与 continue
来源：http://al.newstarts.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vw.hnjuh.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zz.colortex.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://es.hahajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://az.muxihuayi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gv.bjjhwx.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dy.muxihuayi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zq.shxzukj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nz.wgjwhj.cn

[B10] 遍历同时拿索引
来源：http://yo.521024.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wy.shxzukj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://se.gzmigu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ew.gzmigu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ds.muxihuayi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rl.huixiangedu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mx.yuntaijiaju.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wm.9csxet.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dv.huixinmuqiang.cn

[B11] 生成数字序列 / 区间
来源：http://qu.yuexingan06.cn

Py:   list(range(0, 10, 2))
来源：http://ws.colortex.cn

PHP:  range(0, 10, 2);
来源：http://mf.shxzskj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hd.panjiajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rv.bjjhwx.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ik.jctech888.com.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ls.lnxyls.cn

Ruby: (0...10).step(2).to_a
来源：http://pt.shtwfgs.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pz.panjiajie.cn

[B12] 跳出多层循环
来源：http://nb.shxzskj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://vp.yuntaijiaju.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wk.nicolike.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tc.521024.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://en.bjjhwx.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rj.szsharing.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mx.panjiajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://se.hahajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://of.szsharing.cn

[B13] 判断是否为数字
来源：http://uh.yuntaijiaju.cn

Py:   isinstance(x, (int, float))
来源：http://ve.bookmarksfly.cn

PHP:  is_numeric($x)
来源：http://ni.yuntaijiaju.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bq.haigaiapp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dw.lnxyls.cn

Java: x instanceof Number
来源：http://ip.newstarts.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uf.szxytkj.cn

Ruby: x.is_a?(Numeric)
来源：http://nd.huixinmuqiang.cn

C#:   x is int or double or decimal
来源：http://zv.hnjuh.cn

[B14] 判断值是否在集合内
来源：http://nd.huixinmuqiang.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mh.lnxyls.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fw.lnxyls.cn

JS:   [1, 2, 3].includes(x)
来源：http://oe.jianghongdianzi.cn

TS:   [1, 2, 3].includes(x)
来源：http://lh.bjjhwx.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://bm.hahajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nv.asd995.cn

Ruby: [1, 2, 3].include?(x)
来源：http://sa.lnxyls.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kt.hahajie.cn

[B15] 布尔运算与取反
来源：http://rz.huanxung.cn

Py:   a and b or not c
来源：http://ol.shxzukj.cn

PHP:  $a && $b || !$c
来源：http://jq.shxzskj.cn

JS:   a && b || !c
来源：http://ju.shxzskj.cn

TS:   a && b || !c
来源：http://jt.hnjuh.cn

Java: a && b || !c
来源：http://vk.yuntaijiaju.cn

Go:   a && b || !c
来源：http://fy.newstarts.cn

Ruby: a && b || !c
来源：http://ou.huixinmuqiang.cn

C#:   a && b || !c
来源：http://mi.huanxung.cn

[B16] 卫语句：不满足条件提前返回
来源：http://nk.panjiajie.cn

Py:   if not data: return
来源：http://bb.nszjky.cn

PHP:  if (!$data) { return; }
来源：http://cj.panjiajie.cn

JS:   if (!data) return;
来源：http://lf.shtwfgs.cn

TS:   if (!data) return;
来源：http://iz.nicolike.cn

Java: if (data == null) return;
来源：http://dl.huanxung.cn

Go:   if data == nil { return }
来源：http://cf.hahajie.cn

Ruby: return if data.nil?
来源：http://pn.lnxyls.cn

C#:   if (data == null) return;
来源：http://cm.lnxyls.cn

================================================================================
来源：http://ua.hahajie.cn

C. 函数与作用域
来源：http://sp.bjjhwx.cn

================================================================================
来源：http://iv.jianghongdianzi.cn

[C01] 定义函数
来源：http://gp.huixiangedu.cn

Py:   def add(a, b): return a + b
来源：http://hm.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wq.muxihuayi.cn

JS:   function add(a, b) { return a + b; }
来源：http://wu.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vh.nicolike.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ts.newstarts.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vz.shtwfgs.cn

Ruby: def add(a, b); a + b; end
来源：http://qb.521024.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fi.colortex.cn

[C02] 默认参数
来源：http://sc.huanxung.cn

Py:   def greet(name="World"): return name
来源：http://st.szsharing.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hg.521024.cn

JS:   function greet(name = "World") { return name; }
来源：http://sm.bjjhwx.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ry.szsharing.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cp.9csxet.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vn.haigaiapp.cn

Ruby: def greet(name = "World") = name
来源：http://gl.9csxet.cn

C#:   string Greet(string name = "World") => name;
来源：http://ef.wgjwhj.cn

[C03] 可变参数
来源：http://sz.szsharing.cn

Py:   def total(*args): return sum(args)
来源：http://mw.shtwfgs.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wg.lnxyls.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hx.huanxung.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dt.gzmigu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jx.521024.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gd.haigaiapp.cn

Ruby: def total(*nums); nums.sum; end
来源：http://oc.huixinmuqiang.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qe.newstarts.cn

[C04] 命名参数 / 关键字参数
来源：http://hm.szsharing.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ke.nszjky.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kc.lnxyls.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pm.shxzukj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pw.gzmigu.cn

Java: // 无：用 Builder 模式或 record
来源：http://zc.shxzskj.cn

Go:   // 无：用配置结构体参数
来源：http://me.muxihuayi.cn

Ruby: f(a: 1, b: 2)
来源：http://se.newstarts.cn

C#:   f(a: 1, b: 2)
来源：http://op.huanxung.cn

[C05] 返回多个值
来源：http://oh.muxihuayi.cn

Py:   return a, b
来源：http://gq.asd995.cn

PHP:  return [$a, $b];
来源：http://gz.521024.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://kp.hnjuh.cn

TS:   return { a, b };
来源：http://gz.521024.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://uw.huanxung.cn

Go:   return a, b
来源：http://kr.shtwfgs.cn

Ruby: return a, b
来源：http://ms.haigaiapp.cn

C#:   return (a, b);              // ValueTuple
来源：http://zh.nszjky.cn

[C06] 匿名函数 / lambda
来源：http://ej.bjjhwx.cn

Py:   square = lambda x: x * x
来源：http://ez.nicolike.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://sa.panjiajie.cn

JS:   const square = x => x * x;
来源：http://oi.nicolike.cn

TS:   const square = (x: number): number => x * x;
来源：http://ka.gzmigu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://we.shxzukj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ko.shtwfgs.cn

Ruby: square = ->(x) { x * x }
来源：http://in.521024.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ko.nszjky.cn

[C07] 把函数作为参数传入
来源：http://sn.521024.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xs.panjiajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://fz.nszjky.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bo.gzmigu.cn

TS:   arr.map(String)
来源：http://bb.huixiangedu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ts.colortex.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ri.shxzskj.cn

Ruby: arr.map(&:upcase)
来源：http://qq.szsharing.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ch.chemitech.net.cn

[C08] 闭包
来源：http://vy.shtwfgs.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://no.hnjuh.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wx.huanxung.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pk.hahajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rb.lnxyls.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ed.wgjwhj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tg.chemitech.net.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ep.nicolike.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zj.shxzskj.cn

[C09] 递归
来源：http://yc.gzmigu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sf.hahajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fk.bookmarksfly.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ps.shxzukj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mh.hnjuh.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ti.nicolike.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jp.haigaiapp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qm.haigaiapp.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xv.gzmigu.cn

[C10] 变量作用域
来源：http://hx.huixiangedu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pp.szsharing.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ar.nicolike.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://oz.shtwfgs.cn

TS:   同 JS
来源：http://py.jianghongdianzi.cn

Java: 方法内为块级作用域
来源：http://re.asd995.cn

Go:   花括号块级作用域
来源：http://dq.muxihuayi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jj.bookmarksfly.cn

C#:   块级作用域
来源：http://ry.521024.cn

[C11] 模块导入与导出
来源：http://eu.huixinmuqiang.cn

Py:   from module import func
来源：http://fu.gzmigu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ly.shxzukj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hs.shxzukj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nq.wgjwhj.cn

Java: import java.util.List;
来源：http://eh.colortex.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bm.bjjhwx.cn

Ruby: require "json"; require_relative "./util"
来源：http://hp.huixiangedu.cn

C#:   using System.Text;
来源：http://tp.shxzskj.cn

[C12] 立即执行函数 IIFE
来源：http://qn.newstarts.cn

Py:   (lambda: print("run"))()
来源：http://hj.gzmigu.cn

PHP:  (function () { echo "run"; })();
来源：http://qn.colortex.cn

JS:   (() => { console.log("run"); })();
来源：http://sg.shxzskj.cn

TS:   (() => { console.log("run"); })();
来源：http://pe.hahajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xw.colortex.cn

Go:   func() { fmt.Println("run") }()
来源：http://na.jianghongdianzi.cn

Ruby: -> { puts "run" }.call
来源：http://gy.yuexingan06.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ux.nicolike.cn

[C13] 类型声明 / 类型注解
来源：http://rr.wgjwhj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yt.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ve.bookmarksfly.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://eh.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tl.chemitech.net.cn

Java: int add(int a, int b) { return a + b; }
来源：http://om.hnjuh.cn

Go:   func add(a, b int) int
来源：http://gq.yuexingan06.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mx.521024.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ab.szxytkj.cn

[C14] 泛型函数
来源：http://xr.chemitech.net.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nz.9csxet.cn

PHP:  // 无泛型
来源：http://eb.shxzskj.cn

JS:   // 无泛型
来源：http://el.bookmarksfly.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zx.bjjhwx.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nl.newstarts.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://sy.gzmigu.cn

Ruby: # 无泛型
来源：http://ce.nicolike.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vt.colortex.cn

[C15] 解构 / 展开参数
来源：http://ad.muxihuayi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://je.yuexingan06.cn

PHP:  [$a, $b] = $pair;
来源：http://ee.521024.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qb.lnxyls.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ng.huixiangedu.cn

Java: // 无解构
来源：http://vo.muxihuayi.cn

Go:   // 无解构
来源：http://bl.jianghongdianzi.cn

Ruby: a, b = pair
来源：http://dj.gzmigu.cn

C#:   var (a, b) = pair;
来源：http://ry.colortex.cn

[C16] 函数 / 方法重载
来源：http://ba.hahajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ak.colortex.cn

PHP:  // 无重载
来源：http://lb.jianghongdianzi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://jq.jctech888.com.cn

TS:   // 用联合类型或重载签名声明
来源：http://bv.muxihuayi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://lx.newstarts.cn

Go:   // 无重载：用不同函数名
来源：http://ye.wgjwhj.cn

Ruby: # 无重载：靠动态参数
来源：http://jh.szxytkj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://tf.huixinmuqiang.cn

================================================================================
来源：http://hn.9csxet.cn

D. 数组 / 列表 / 集合
来源：http://zl.wgjwhj.cn

================================================================================
来源：http://zz.haigaiapp.cn

[D01] 创建数组 / 列表
来源：http://rr.9csxet.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://cj.haigaiapp.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nh.jctech888.com.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://av.521024.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://pa.haigaiapp.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zz.szxytkj.cn


<!-- 参考信息 -->