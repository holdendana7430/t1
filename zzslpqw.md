代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qo.szxytkj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://rz.muxihuayi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gw.huixiangedu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pl.shtwfgs.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hi.bookmarksfly.cn

[B02] 多分支 else if / elif
来源：http://na.gzmigu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sa.chemitech.net.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jb.colortex.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://to.gzmigu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://np.9csxet.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gk.bjjhwx.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yn.chemitech.net.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uf.yuexingan06.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pv.521024.cn

[B03] switch / match / case
来源：http://jb.jctech888.com.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://by.muxihuayi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gd.lnxyls.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wr.nszjky.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wi.521024.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://me.muxihuayi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vd.huixiangedu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wy.521024.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yf.jctech888.com.cn

[B04] for 计数循环
来源：http://kl.huixinmuqiang.cn

Py:   for i in range(10): print(i)
来源：http://sm.gzmigu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://im.szsharing.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://me.yuntaijiaju.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lr.jctech888.com.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gz.haigaiapp.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lp.szxytkj.cn

Ruby: 10.times { |i| puts i }
来源：http://bn.nicolike.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sz.jctech888.com.cn

[B05] 遍历数组 / 列表
来源：http://ye.shxzskj.cn

Py:   for item in arr: print(item)
来源：http://zv.newstarts.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ws.gzmigu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ag.muxihuayi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://wr.muxihuayi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xb.gzmigu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gx.yuexingan06.cn

Ruby: arr.each { |item| puts item }
来源：http://vt.lnxyls.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hw.nszjky.cn

[B06] 遍历字典 / 对象
来源：http://cd.haigaiapp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hi.jianghongdianzi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pd.jianghongdianzi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cj.shxzskj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mt.shxzukj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ga.jctech888.com.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://at.huanxung.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xn.shxzskj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cn.panjiajie.cn

[B07] while 循环
来源：http://zh.newstarts.cn

Py:   while i < 10: i += 1
来源：http://wz.huixinmuqiang.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zf.hahajie.cn

JS:   while (i < 10) { i++; }
来源：http://tt.jctech888.com.cn

TS:   while (i < 10) { i++; }
来源：http://ik.lnxyls.cn

Java: while (i < 10) { i++; }
来源：http://uz.szxytkj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://at.gzmigu.cn

Ruby: while i < 10; i += 1; end
来源：http://az.shxzskj.cn

C#:   while (i < 10) { i++; }
来源：http://ff.huanxung.cn

[B08] do-while（至少执行一次）
来源：http://oi.shtwfgs.cn

Py:   # 无 do-while：用 while True + break
来源：http://lh.shxzskj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://lo.nszjky.cn

JS:   do { i++; } while (i < 10);
来源：http://dr.szxytkj.cn

TS:   do { i++; } while (i < 10);
来源：http://fx.jianghongdianzi.cn

Java: do { i++; } while (i < 10);
来源：http://gn.gzmigu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://za.jctech888.com.cn

Ruby: begin; i += 1; end while i < 10
来源：http://kk.newstarts.cn

C#:   do { i++; } while (i < 10);
来源：http://ua.hnjuh.cn

[B09] break 与 continue
来源：http://or.gzmigu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qb.nicolike.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dh.jianghongdianzi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lf.colortex.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://so.muxihuayi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mr.chemitech.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vl.wgjwhj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ph.newstarts.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fj.bookmarksfly.cn

[B10] 遍历同时拿索引
来源：http://sr.wgjwhj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wh.shxzukj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gn.9csxet.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xx.shxzskj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lo.521024.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lr.muxihuayi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tv.shtwfgs.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nx.colortex.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://iq.9csxet.cn

[B11] 生成数字序列 / 区间
来源：http://uy.hnjuh.cn

Py:   list(range(0, 10, 2))
来源：http://an.colortex.cn

PHP:  range(0, 10, 2);
来源：http://da.yuntaijiaju.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eo.panjiajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oo.yuntaijiaju.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qz.gzmigu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ny.shxzukj.cn

Ruby: (0...10).step(2).to_a
来源：http://pl.bookmarksfly.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ah.huixinmuqiang.cn

[B12] 跳出多层循环
来源：http://rq.jctech888.com.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://cb.shxzukj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://tb.bookmarksfly.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lk.lnxyls.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nb.yuntaijiaju.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dq.hnjuh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bo.colortex.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ex.colortex.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hy.asd995.cn

[B13] 判断是否为数字
来源：http://mg.lnxyls.cn

Py:   isinstance(x, (int, float))
来源：http://nq.huixiangedu.cn

PHP:  is_numeric($x)
来源：http://pr.jctech888.com.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wx.huanxung.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://er.jctech888.com.cn

Java: x instanceof Number
来源：http://gt.yuexingan06.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zb.haigaiapp.cn

Ruby: x.is_a?(Numeric)
来源：http://sv.521024.cn

C#:   x is int or double or decimal
来源：http://wt.haigaiapp.cn

[B14] 判断值是否在集合内
来源：http://bv.jianghongdianzi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://di.asd995.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ij.shxzukj.cn

JS:   [1, 2, 3].includes(x)
来源：http://yu.haigaiapp.cn

TS:   [1, 2, 3].includes(x)
来源：http://iz.colortex.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hu.shxzukj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ht.szsharing.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rj.jctech888.com.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pi.yuexingan06.cn

[B15] 布尔运算与取反
来源：http://jf.hahajie.cn

Py:   a and b or not c
来源：http://fl.muxihuayi.cn

PHP:  $a && $b || !$c
来源：http://uo.huixiangedu.cn

JS:   a && b || !c
来源：http://rp.huanxung.cn

TS:   a && b || !c
来源：http://hy.9csxet.cn

Java: a && b || !c
来源：http://ng.yuntaijiaju.cn

Go:   a && b || !c
来源：http://sp.9csxet.cn

Ruby: a && b || !c
来源：http://gm.bjjhwx.cn

C#:   a && b || !c
来源：http://rn.huixinmuqiang.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jp.521024.cn

Py:   if not data: return
来源：http://nq.huanxung.cn

PHP:  if (!$data) { return; }
来源：http://aa.panjiajie.cn

JS:   if (!data) return;
来源：http://sy.colortex.cn

TS:   if (!data) return;
来源：http://vu.wgjwhj.cn

Java: if (data == null) return;
来源：http://rp.chemitech.net.cn

Go:   if data == nil { return }
来源：http://gs.panjiajie.cn

Ruby: return if data.nil?
来源：http://dd.shxzukj.cn

C#:   if (data == null) return;
来源：http://sr.panjiajie.cn

================================================================================
来源：http://km.colortex.cn

C. 函数与作用域
来源：http://gd.hnjuh.cn

================================================================================
来源：http://mq.lnxyls.cn

[C01] 定义函数
来源：http://rw.521024.cn

Py:   def add(a, b): return a + b
来源：http://cw.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rc.lnxyls.cn

JS:   function add(a, b) { return a + b; }
来源：http://np.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://no.panjiajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gs.huanxung.cn

Go:   func add(a, b int) int { return a + b }
来源：http://il.bjjhwx.cn

Ruby: def add(a, b); a + b; end
来源：http://zg.shxzukj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dy.chemitech.net.cn

[C02] 默认参数
来源：http://ng.muxihuayi.cn

Py:   def greet(name="World"): return name
来源：http://wg.asd995.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qd.panjiajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://gf.bookmarksfly.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://he.nszjky.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ab.huixiangedu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pr.bjjhwx.cn

Ruby: def greet(name = "World") = name
来源：http://wu.colortex.cn

C#:   string Greet(string name = "World") => name;
来源：http://gw.muxihuayi.cn

[C03] 可变参数
来源：http://cy.hnjuh.cn

Py:   def total(*args): return sum(args)
来源：http://ft.yuntaijiaju.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fb.9csxet.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wr.bjjhwx.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ip.jctech888.com.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mi.asd995.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fr.shxzukj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fl.colortex.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://le.huanxung.cn

[C04] 命名参数 / 关键字参数
来源：http://xs.newstarts.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://od.asd995.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nk.chemitech.net.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ld.hahajie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rv.huanxung.cn

Java: // 无：用 Builder 模式或 record
来源：http://uv.shtwfgs.cn

Go:   // 无：用配置结构体参数
来源：http://td.nicolike.cn

Ruby: f(a: 1, b: 2)
来源：http://dy.jianghongdianzi.cn

C#:   f(a: 1, b: 2)
来源：http://zt.hnjuh.cn

[C05] 返回多个值
来源：http://fb.bookmarksfly.cn

Py:   return a, b
来源：http://aa.9csxet.cn

PHP:  return [$a, $b];
来源：http://fj.9csxet.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://na.huanxung.cn

TS:   return { a, b };
来源：http://yi.yuntaijiaju.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ka.chemitech.net.cn

Go:   return a, b
来源：http://eg.colortex.cn

Ruby: return a, b
来源：http://fo.gzmigu.cn

C#:   return (a, b);              // ValueTuple
来源：http://dy.huanxung.cn

[C06] 匿名函数 / lambda
来源：http://dy.bjjhwx.cn

Py:   square = lambda x: x * x
来源：http://aj.gzmigu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ze.9csxet.cn

JS:   const square = x => x * x;
来源：http://qt.panjiajie.cn

TS:   const square = (x: number): number => x * x;
来源：http://xi.newstarts.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mc.bookmarksfly.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qs.szxytkj.cn

Ruby: square = ->(x) { x * x }
来源：http://ct.szxytkj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ve.panjiajie.cn

[C07] 把函数作为参数传入
来源：http://sh.nszjky.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dw.shxzskj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://aq.colortex.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yi.shxzukj.cn

TS:   arr.map(String)
来源：http://ey.jctech888.com.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ry.muxihuayi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://up.gzmigu.cn

Ruby: arr.map(&:upcase)
来源：http://bc.huixinmuqiang.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ng.newstarts.cn

[C08] 闭包
来源：http://ur.yuntaijiaju.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ng.nszjky.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jn.szsharing.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bn.newstarts.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pe.hahajie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bj.newstarts.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rj.9csxet.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sp.jctech888.com.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ac.jctech888.com.cn

[C09] 递归
来源：http://vl.yuexingan06.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pd.gzmigu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ef.szsharing.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://or.haigaiapp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://af.gzmigu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ij.yuexingan06.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pk.yuntaijiaju.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cy.szsharing.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zn.521024.cn

[C10] 变量作用域
来源：http://id.wgjwhj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ec.panjiajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ce.panjiajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ms.wgjwhj.cn

TS:   同 JS
来源：http://op.yuexingan06.cn

Java: 方法内为块级作用域
来源：http://ne.yuntaijiaju.cn

Go:   花括号块级作用域
来源：http://ch.asd995.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vp.hahajie.cn

C#:   块级作用域
来源：http://fu.shxzskj.cn

[C11] 模块导入与导出
来源：http://os.jianghongdianzi.cn

Py:   from module import func
来源：http://kv.jctech888.com.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qd.gzmigu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zq.huixiangedu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lr.colortex.cn

Java: import java.util.List;
来源：http://fn.jctech888.com.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lm.yuexingan06.cn

Ruby: require "json"; require_relative "./util"
来源：http://fu.jianghongdianzi.cn

C#:   using System.Text;
来源：http://pb.yuexingan06.cn

[C12] 立即执行函数 IIFE
来源：http://qv.panjiajie.cn

Py:   (lambda: print("run"))()
来源：http://rb.jianghongdianzi.cn

PHP:  (function () { echo "run"; })();
来源：http://oh.nszjky.cn

JS:   (() => { console.log("run"); })();
来源：http://bt.shxzskj.cn

TS:   (() => { console.log("run"); })();
来源：http://pi.szxytkj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xv.muxihuayi.cn

Go:   func() { fmt.Println("run") }()
来源：http://lx.nicolike.cn

Ruby: -> { puts "run" }.call
来源：http://tc.szxytkj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://uy.asd995.cn

[C13] 类型声明 / 类型注解
来源：http://ol.huixiangedu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://uc.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bb.bjjhwx.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://uo.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://eb.shxzukj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ud.wgjwhj.cn

Go:   func add(a, b int) int
来源：http://dk.521024.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gc.muxihuayi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vy.yuntaijiaju.cn

[C14] 泛型函数
来源：http://nl.colortex.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://oj.shtwfgs.cn

PHP:  // 无泛型
来源：http://lp.colortex.cn

JS:   // 无泛型
来源：http://az.jianghongdianzi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gb.gzmigu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ml.yuexingan06.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mw.nszjky.cn

Ruby: # 无泛型
来源：http://fp.huixinmuqiang.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wy.newstarts.cn

[C15] 解构 / 展开参数
来源：http://br.shxzukj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gk.jianghongdianzi.cn

PHP:  [$a, $b] = $pair;
来源：http://zr.shxzukj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bh.muxihuayi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://md.hnjuh.cn

Java: // 无解构
来源：http://rk.hnjuh.cn

Go:   // 无解构
来源：http://ju.jctech888.com.cn

Ruby: a, b = pair
来源：http://rq.chemitech.net.cn

C#:   var (a, b) = pair;
来源：http://qm.shtwfgs.cn

[C16] 函数 / 方法重载
来源：http://eq.szsharing.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sf.wgjwhj.cn

PHP:  // 无重载
来源：http://wv.gzmigu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://vj.szsharing.cn

TS:   // 用联合类型或重载签名声明
来源：http://bg.shtwfgs.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wy.hahajie.cn

Go:   // 无重载：用不同函数名
来源：http://rb.9csxet.cn

Ruby: # 无重载：靠动态参数
来源：http://si.gzmigu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yd.yuntaijiaju.cn

================================================================================
来源：http://hg.muxihuayi.cn

D. 数组 / 列表 / 集合
来源：http://st.asd995.cn

================================================================================
来源：http://ot.shxzukj.cn

[D01] 创建数组 / 列表
来源：http://sp.asd995.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ct.huixiangedu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xd.huixinmuqiang.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tk.jctech888.com.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ht.newstarts.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://us.huanxung.cn

Go:   arr := []int{1, 2, 3}
来源：http://gx.bjjhwx.cn

Ruby: arr = [1, 2, 3]
来源：http://bj.yuntaijiaju.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qk.shtwfgs.cn

[D02] 追加元素到末尾
来源：http://fw.9csxet.cn


<!-- 参考信息 -->