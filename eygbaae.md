代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ai.colortex.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://yf.yuntaijiaju.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://on.colortex.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bi.9csxet.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ld.jianghongdianzi.cn

[B02] 多分支 else if / elif
来源：http://et.yuntaijiaju.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://po.szxytkj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xh.bjjhwx.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dc.szxytkj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://us.muxihuayi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dn.panjiajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jv.yuntaijiaju.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pd.huanxung.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yp.wgjwhj.cn

[B03] switch / match / case
来源：http://uf.shtwfgs.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hi.shxzskj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://em.521024.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ka.chemitech.net.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dy.jianghongdianzi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://in.shtwfgs.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ux.hnjuh.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://af.bookmarksfly.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kq.bookmarksfly.cn

[B04] for 计数循环
来源：http://of.hnjuh.cn

Py:   for i in range(10): print(i)
来源：http://ov.wgjwhj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tn.panjiajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pm.hahajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pz.shxzskj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ry.yuntaijiaju.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gr.nicolike.cn

Ruby: 10.times { |i| puts i }
来源：http://gp.gzmigu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ed.huixinmuqiang.cn

[B05] 遍历数组 / 列表
来源：http://kf.asd995.cn

Py:   for item in arr: print(item)
来源：http://he.shxzukj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://km.hnjuh.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wc.szsharing.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://jv.szxytkj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yv.nszjky.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://af.nszjky.cn

Ruby: arr.each { |item| puts item }
来源：http://iz.yuexingan06.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qf.nicolike.cn

[B06] 遍历字典 / 对象
来源：http://yt.haigaiapp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zq.wgjwhj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mh.shtwfgs.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wc.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://am.huanxung.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ac.shxzukj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://py.huixiangedu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xr.jctech888.com.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mb.szsharing.cn

[B07] while 循环
来源：http://fw.bjjhwx.cn

Py:   while i < 10: i += 1
来源：http://cu.nicolike.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wl.9csxet.cn

JS:   while (i < 10) { i++; }
来源：http://fn.asd995.cn

TS:   while (i < 10) { i++; }
来源：http://en.nicolike.cn

Java: while (i < 10) { i++; }
来源：http://wq.yuntaijiaju.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vw.huanxung.cn

Ruby: while i < 10; i += 1; end
来源：http://ld.huixiangedu.cn

C#:   while (i < 10) { i++; }
来源：http://lk.colortex.cn

[B08] do-while（至少执行一次）
来源：http://ve.huanxung.cn

Py:   # 无 do-while：用 while True + break
来源：http://xi.huanxung.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ji.newstarts.cn

JS:   do { i++; } while (i < 10);
来源：http://xw.nicolike.cn

TS:   do { i++; } while (i < 10);
来源：http://hm.nicolike.cn

Java: do { i++; } while (i < 10);
来源：http://wi.haigaiapp.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ia.colortex.cn

Ruby: begin; i += 1; end while i < 10
来源：http://gg.muxihuayi.cn

C#:   do { i++; } while (i < 10);
来源：http://iv.haigaiapp.cn

[B09] break 与 continue
来源：http://sz.huixiangedu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://uw.yuntaijiaju.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dg.huanxung.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vh.wgjwhj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rn.huixinmuqiang.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rh.shxzukj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nl.szxytkj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gx.asd995.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dw.hahajie.cn

[B10] 遍历同时拿索引
来源：http://ne.szsharing.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://av.hahajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yf.jctech888.com.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ns.bookmarksfly.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bz.shxzskj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gb.huixiangedu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uv.muxihuayi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://th.jctech888.com.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://up.nicolike.cn

[B11] 生成数字序列 / 区间
来源：http://jr.jianghongdianzi.cn

Py:   list(range(0, 10, 2))
来源：http://nk.huanxung.cn

PHP:  range(0, 10, 2);
来源：http://zl.szsharing.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ol.panjiajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pf.huixiangedu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gc.hahajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ms.wgjwhj.cn

Ruby: (0...10).step(2).to_a
来源：http://az.szxytkj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zy.muxihuayi.cn

[B12] 跳出多层循环
来源：http://wb.lnxyls.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ki.chemitech.net.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fp.asd995.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gu.521024.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rq.haigaiapp.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ip.hahajie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mh.newstarts.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hd.shxzskj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xw.huanxung.cn

[B13] 判断是否为数字
来源：http://qp.gzmigu.cn

Py:   isinstance(x, (int, float))
来源：http://dv.bookmarksfly.cn

PHP:  is_numeric($x)
来源：http://oc.colortex.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xu.yuexingan06.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cr.colortex.cn

Java: x instanceof Number
来源：http://gb.panjiajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://un.yuntaijiaju.cn

Ruby: x.is_a?(Numeric)
来源：http://oc.chemitech.net.cn

C#:   x is int or double or decimal
来源：http://xh.panjiajie.cn

[B14] 判断值是否在集合内
来源：http://de.lnxyls.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://du.colortex.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://eu.haigaiapp.cn

JS:   [1, 2, 3].includes(x)
来源：http://ph.colortex.cn

TS:   [1, 2, 3].includes(x)
来源：http://tf.huixinmuqiang.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://yn.lnxyls.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ol.hahajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zx.asd995.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vi.huixinmuqiang.cn

[B15] 布尔运算与取反
来源：http://bp.huixinmuqiang.cn

Py:   a and b or not c
来源：http://xd.hnjuh.cn

PHP:  $a && $b || !$c
来源：http://ht.haigaiapp.cn

JS:   a && b || !c
来源：http://wj.huixiangedu.cn

TS:   a && b || !c
来源：http://lc.shxzukj.cn

Java: a && b || !c
来源：http://tr.nicolike.cn

Go:   a && b || !c
来源：http://si.muxihuayi.cn

Ruby: a && b || !c
来源：http://gb.shxzukj.cn

C#:   a && b || !c
来源：http://ju.newstarts.cn

[B16] 卫语句：不满足条件提前返回
来源：http://us.hahajie.cn

Py:   if not data: return
来源：http://tq.wgjwhj.cn

PHP:  if (!$data) { return; }
来源：http://gd.nicolike.cn

JS:   if (!data) return;
来源：http://mi.huixiangedu.cn

TS:   if (!data) return;
来源：http://is.jctech888.com.cn

Java: if (data == null) return;
来源：http://ox.9csxet.cn

Go:   if data == nil { return }
来源：http://zp.lnxyls.cn

Ruby: return if data.nil?
来源：http://cj.shxzskj.cn

C#:   if (data == null) return;
来源：http://wj.yuexingan06.cn

================================================================================
来源：http://gc.szsharing.cn

C. 函数与作用域
来源：http://ma.muxihuayi.cn

================================================================================
来源：http://dv.shxzukj.cn

[C01] 定义函数
来源：http://yl.nszjky.cn

Py:   def add(a, b): return a + b
来源：http://bd.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ej.wgjwhj.cn

JS:   function add(a, b) { return a + b; }
来源：http://ya.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jp.huanxung.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ub.gzmigu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qj.huanxung.cn

Ruby: def add(a, b); a + b; end
来源：http://vk.asd995.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yi.shxzukj.cn

[C02] 默认参数
来源：http://qe.yuntaijiaju.cn

Py:   def greet(name="World"): return name
来源：http://mi.bookmarksfly.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wh.shxzskj.cn

JS:   function greet(name = "World") { return name; }
来源：http://lp.9csxet.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://jn.shxzskj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fb.colortex.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://se.gzmigu.cn

Ruby: def greet(name = "World") = name
来源：http://gv.huanxung.cn

C#:   string Greet(string name = "World") => name;
来源：http://ox.hnjuh.cn

[C03] 可变参数
来源：http://ji.jianghongdianzi.cn

Py:   def total(*args): return sum(args)
来源：http://zb.szsharing.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fc.huanxung.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sb.jctech888.com.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pg.jianghongdianzi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rm.nicolike.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://is.colortex.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yk.shxzskj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ts.colortex.cn

[C04] 命名参数 / 关键字参数
来源：http://zp.asd995.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ov.521024.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dz.shxzskj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bf.shxzskj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://oy.colortex.cn

Java: // 无：用 Builder 模式或 record
来源：http://ev.yuntaijiaju.cn

Go:   // 无：用配置结构体参数
来源：http://na.asd995.cn

Ruby: f(a: 1, b: 2)
来源：http://eh.chemitech.net.cn

C#:   f(a: 1, b: 2)
来源：http://ml.yuntaijiaju.cn

[C05] 返回多个值
来源：http://tz.panjiajie.cn

Py:   return a, b
来源：http://vh.haigaiapp.cn

PHP:  return [$a, $b];
来源：http://ut.yuntaijiaju.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://su.colortex.cn

TS:   return { a, b };
来源：http://xv.huixinmuqiang.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zo.chemitech.net.cn

Go:   return a, b
来源：http://ks.colortex.cn

Ruby: return a, b
来源：http://xz.huixiangedu.cn

C#:   return (a, b);              // ValueTuple
来源：http://wg.jctech888.com.cn

[C06] 匿名函数 / lambda
来源：http://xk.szsharing.cn

Py:   square = lambda x: x * x
来源：http://er.nszjky.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ie.huixiangedu.cn

JS:   const square = x => x * x;
来源：http://np.muxihuayi.cn

TS:   const square = (x: number): number => x * x;
来源：http://hx.gzmigu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://me.szsharing.cn

Go:   sq := func(x int) int { return x * x }
来源：http://sr.huanxung.cn

Ruby: square = ->(x) { x * x }
来源：http://ma.shtwfgs.cn

C#:   Func<int, int> square = x => x * x;
来源：http://yh.huixinmuqiang.cn

[C07] 把函数作为参数传入
来源：http://qa.chemitech.net.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wu.szsharing.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vh.colortex.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://su.bookmarksfly.cn

TS:   arr.map(String)
来源：http://ex.gzmigu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wa.nicolike.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zf.bjjhwx.cn

Ruby: arr.map(&:upcase)
来源：http://qc.nicolike.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://or.gzmigu.cn

[C08] 闭包
来源：http://ga.jctech888.com.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ed.szsharing.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ln.9csxet.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zu.lnxyls.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://et.huixiangedu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gh.muxihuayi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zg.yuntaijiaju.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ox.jctech888.com.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gc.huanxung.cn

[C09] 递归
来源：http://bd.muxihuayi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yc.shtwfgs.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zc.szxytkj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kc.yuntaijiaju.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://id.shxzukj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uk.szxytkj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ru.521024.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fg.panjiajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xh.asd995.cn

[C10] 变量作用域
来源：http://jz.jctech888.com.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zo.jianghongdianzi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lm.wgjwhj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://oo.shtwfgs.cn

TS:   同 JS
来源：http://zf.shxzukj.cn

Java: 方法内为块级作用域
来源：http://cs.panjiajie.cn

Go:   花括号块级作用域
来源：http://dh.huixinmuqiang.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ei.colortex.cn

C#:   块级作用域
来源：http://qw.asd995.cn

[C11] 模块导入与导出
来源：http://ao.shtwfgs.cn

Py:   from module import func
来源：http://wb.szxytkj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://oi.shxzukj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://wl.yuntaijiaju.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lb.nszjky.cn

Java: import java.util.List;
来源：http://cd.lnxyls.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xb.9csxet.cn

Ruby: require "json"; require_relative "./util"
来源：http://lw.521024.cn

C#:   using System.Text;
来源：http://mq.bookmarksfly.cn

[C12] 立即执行函数 IIFE
来源：http://wg.szxytkj.cn

Py:   (lambda: print("run"))()
来源：http://qd.jianghongdianzi.cn

PHP:  (function () { echo "run"; })();
来源：http://xn.szxytkj.cn

JS:   (() => { console.log("run"); })();
来源：http://tx.shxzskj.cn

TS:   (() => { console.log("run"); })();
来源：http://wc.szxytkj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dh.shxzukj.cn

Go:   func() { fmt.Println("run") }()
来源：http://rs.szsharing.cn

Ruby: -> { puts "run" }.call
来源：http://wg.9csxet.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pl.wgjwhj.cn

[C13] 类型声明 / 类型注解
来源：http://to.huanxung.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ua.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tp.panjiajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ir.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rp.nicolike.cn

Java: int add(int a, int b) { return a + b; }
来源：http://pc.huixiangedu.cn

Go:   func add(a, b int) int
来源：http://we.colortex.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xn.nicolike.cn

C#:   int Add(int a, int b) => a + b;
来源：http://hs.muxihuayi.cn

[C14] 泛型函数
来源：http://ig.panjiajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dh.nicolike.cn

PHP:  // 无泛型
来源：http://um.chemitech.net.cn

JS:   // 无泛型
来源：http://ui.jctech888.com.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gw.haigaiapp.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://od.huixiangedu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ui.nszjky.cn

Ruby: # 无泛型
来源：http://ax.huixiangedu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yh.hahajie.cn

[C15] 解构 / 展开参数
来源：http://aj.newstarts.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wq.newstarts.cn

PHP:  [$a, $b] = $pair;
来源：http://vl.521024.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://et.newstarts.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vm.shxzukj.cn

Java: // 无解构
来源：http://dt.chemitech.net.cn

Go:   // 无解构
来源：http://hz.gzmigu.cn

Ruby: a, b = pair
来源：http://bt.huixiangedu.cn

C#:   var (a, b) = pair;
来源：http://oq.nicolike.cn

[C16] 函数 / 方法重载
来源：http://ow.9csxet.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xw.panjiajie.cn

PHP:  // 无重载
来源：http://ec.muxihuayi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://tc.wgjwhj.cn

TS:   // 用联合类型或重载签名声明
来源：http://hj.huanxung.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jx.hahajie.cn

Go:   // 无重载：用不同函数名
来源：http://hk.jctech888.com.cn

Ruby: # 无重载：靠动态参数
来源：http://wb.bjjhwx.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fb.panjiajie.cn

================================================================================
来源：http://na.shxzskj.cn

D. 数组 / 列表 / 集合
来源：http://kp.jctech888.com.cn

================================================================================
来源：http://no.huixinmuqiang.cn

[D01] 创建数组 / 列表
来源：http://tj.szsharing.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://az.jctech888.com.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tz.hnjuh.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ut.panjiajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://nz.newstarts.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://py.colortex.cn

Go:   arr := []int{1, 2, 3}
来源：http://ye.haigaiapp.cn

Ruby: arr = [1, 2, 3]
来源：http://it.haigaiapp.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rl.shxzukj.cn

[D02] 追加元素到末尾
来源：http://ud.gzmigu.cn


<!-- 参考信息 -->