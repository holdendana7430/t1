代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rr.huixinmuqiang.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://hh.wgjwhj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nf.szsharing.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lq.chemitech.net.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ng.hnjuh.cn

[B02] 多分支 else if / elif
来源：http://jz.521024.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://al.newstarts.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bm.haigaiapp.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://an.9csxet.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tj.jctech888.com.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zv.asd995.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ce.asd995.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uz.haigaiapp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ir.huanxung.cn

[B03] switch / match / case
来源：http://kn.hnjuh.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bn.shtwfgs.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qx.newstarts.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xl.colortex.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tz.521024.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bm.521024.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ev.9csxet.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ii.jianghongdianzi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://op.asd995.cn

[B04] for 计数循环
来源：http://gu.jctech888.com.cn

Py:   for i in range(10): print(i)
来源：http://ls.chemitech.net.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xi.yuntaijiaju.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cm.huixinmuqiang.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yh.panjiajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pm.chemitech.net.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qj.gzmigu.cn

Ruby: 10.times { |i| puts i }
来源：http://he.jianghongdianzi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yi.panjiajie.cn

[B05] 遍历数组 / 列表
来源：http://pu.muxihuayi.cn

Py:   for item in arr: print(item)
来源：http://us.shtwfgs.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://uk.shxzukj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://rl.haigaiapp.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ow.huanxung.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://aw.nicolike.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kj.nicolike.cn

Ruby: arr.each { |item| puts item }
来源：http://lz.newstarts.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tn.szxytkj.cn

[B06] 遍历字典 / 对象
来源：http://rf.haigaiapp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://yg.jctech888.com.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://br.haigaiapp.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bj.bookmarksfly.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lc.gzmigu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://my.muxihuayi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://on.asd995.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wa.szsharing.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zk.521024.cn

[B07] while 循环
来源：http://xc.bookmarksfly.cn

Py:   while i < 10: i += 1
来源：http://gt.colortex.cn

PHP:  while ($i < 10) { $i++; }
来源：http://tt.bjjhwx.cn

JS:   while (i < 10) { i++; }
来源：http://gj.lnxyls.cn

TS:   while (i < 10) { i++; }
来源：http://eo.9csxet.cn

Java: while (i < 10) { i++; }
来源：http://lf.huixiangedu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lf.chemitech.net.cn

Ruby: while i < 10; i += 1; end
来源：http://zv.shxzskj.cn

C#:   while (i < 10) { i++; }
来源：http://zc.muxihuayi.cn

[B08] do-while（至少执行一次）
来源：http://hj.nicolike.cn

Py:   # 无 do-while：用 while True + break
来源：http://pn.wgjwhj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pa.hahajie.cn

JS:   do { i++; } while (i < 10);
来源：http://ph.lnxyls.cn

TS:   do { i++; } while (i < 10);
来源：http://lf.hnjuh.cn

Java: do { i++; } while (i < 10);
来源：http://qc.gzmigu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mq.yuexingan06.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jz.yuntaijiaju.cn

C#:   do { i++; } while (i < 10);
来源：http://rc.nicolike.cn

[B09] break 与 continue
来源：http://sa.wgjwhj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jh.yuexingan06.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jb.huixinmuqiang.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gx.shxzskj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bj.huixiangedu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vk.huixiangedu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ah.shxzukj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lx.huixinmuqiang.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://co.muxihuayi.cn

[B10] 遍历同时拿索引
来源：http://zt.bjjhwx.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cz.panjiajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wx.shxzukj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sw.hnjuh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nc.bjjhwx.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ep.chemitech.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tn.szxytkj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nk.yuexingan06.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cq.shxzskj.cn

[B11] 生成数字序列 / 区间
来源：http://mp.bookmarksfly.cn

Py:   list(range(0, 10, 2))
来源：http://em.haigaiapp.cn

PHP:  range(0, 10, 2);
来源：http://lc.nicolike.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wc.haigaiapp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cd.jctech888.com.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jc.huixinmuqiang.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bs.jianghongdianzi.cn

Ruby: (0...10).step(2).to_a
来源：http://nt.newstarts.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://oj.huanxung.cn

[B12] 跳出多层循环
来源：http://no.wgjwhj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tu.asd995.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://oo.muxihuayi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://um.szxytkj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qs.newstarts.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://el.bookmarksfly.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ik.nszjky.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vn.9csxet.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gg.colortex.cn

[B13] 判断是否为数字
来源：http://pt.shxzukj.cn

Py:   isinstance(x, (int, float))
来源：http://yr.lnxyls.cn

PHP:  is_numeric($x)
来源：http://uy.wgjwhj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pw.nicolike.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://je.shtwfgs.cn

Java: x instanceof Number
来源：http://kj.newstarts.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qz.shtwfgs.cn

Ruby: x.is_a?(Numeric)
来源：http://sp.shxzskj.cn

C#:   x is int or double or decimal
来源：http://rf.szxytkj.cn

[B14] 判断值是否在集合内
来源：http://yc.9csxet.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ix.panjiajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qk.haigaiapp.cn

JS:   [1, 2, 3].includes(x)
来源：http://kh.asd995.cn

TS:   [1, 2, 3].includes(x)
来源：http://jv.521024.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://so.szxytkj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fp.szsharing.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vy.wgjwhj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ka.shtwfgs.cn

[B15] 布尔运算与取反
来源：http://yp.bjjhwx.cn

Py:   a and b or not c
来源：http://fb.lnxyls.cn

PHP:  $a && $b || !$c
来源：http://vv.szxytkj.cn

JS:   a && b || !c
来源：http://eh.newstarts.cn

TS:   a && b || !c
来源：http://hl.gzmigu.cn

Java: a && b || !c
来源：http://uj.huixinmuqiang.cn

Go:   a && b || !c
来源：http://ht.shtwfgs.cn

Ruby: a && b || !c
来源：http://ys.huixiangedu.cn

C#:   a && b || !c
来源：http://jr.colortex.cn

[B16] 卫语句：不满足条件提前返回
来源：http://dg.bjjhwx.cn

Py:   if not data: return
来源：http://he.lnxyls.cn

PHP:  if (!$data) { return; }
来源：http://uh.huixiangedu.cn

JS:   if (!data) return;
来源：http://zo.panjiajie.cn

TS:   if (!data) return;
来源：http://tk.yuexingan06.cn

Java: if (data == null) return;
来源：http://zz.huixiangedu.cn

Go:   if data == nil { return }
来源：http://hi.hnjuh.cn

Ruby: return if data.nil?
来源：http://hk.shxzskj.cn

C#:   if (data == null) return;
来源：http://wc.szsharing.cn

================================================================================
来源：http://hg.wgjwhj.cn

C. 函数与作用域
来源：http://ua.shxzukj.cn

================================================================================
来源：http://ky.huixinmuqiang.cn

[C01] 定义函数
来源：http://zz.huixinmuqiang.cn

Py:   def add(a, b): return a + b
来源：http://lv.shxzskj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ob.haigaiapp.cn

JS:   function add(a, b) { return a + b; }
来源：http://ts.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cm.shxzukj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://yt.hnjuh.cn

Go:   func add(a, b int) int { return a + b }
来源：http://km.szxytkj.cn

Ruby: def add(a, b); a + b; end
来源：http://fn.shtwfgs.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://eu.shxzukj.cn

[C02] 默认参数
来源：http://rr.gzmigu.cn

Py:   def greet(name="World"): return name
来源：http://ge.hnjuh.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://oh.521024.cn

JS:   function greet(name = "World") { return name; }
来源：http://lo.yuntaijiaju.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hq.wgjwhj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dd.gzmigu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://of.yuntaijiaju.cn

Ruby: def greet(name = "World") = name
来源：http://hi.haigaiapp.cn

C#:   string Greet(string name = "World") => name;
来源：http://mw.hahajie.cn

[C03] 可变参数
来源：http://tt.hahajie.cn

Py:   def total(*args): return sum(args)
来源：http://dx.huanxung.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qt.huixinmuqiang.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wb.huixinmuqiang.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rm.huixinmuqiang.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lg.haigaiapp.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://th.jianghongdianzi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wh.yuntaijiaju.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hv.shtwfgs.cn

[C04] 命名参数 / 关键字参数
来源：http://gp.bookmarksfly.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ok.wgjwhj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rh.huixiangedu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vj.nszjky.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://us.huixiangedu.cn

Java: // 无：用 Builder 模式或 record
来源：http://xv.521024.cn

Go:   // 无：用配置结构体参数
来源：http://ht.huanxung.cn

Ruby: f(a: 1, b: 2)
来源：http://yh.szxytkj.cn

C#:   f(a: 1, b: 2)
来源：http://lo.panjiajie.cn

[C05] 返回多个值
来源：http://ip.huixiangedu.cn

Py:   return a, b
来源：http://cl.wgjwhj.cn

PHP:  return [$a, $b];
来源：http://ee.szxytkj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://em.521024.cn

TS:   return { a, b };
来源：http://jc.hnjuh.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vx.colortex.cn

Go:   return a, b
来源：http://pv.gzmigu.cn

Ruby: return a, b
来源：http://xy.hahajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://dx.shtwfgs.cn

[C06] 匿名函数 / lambda
来源：http://jv.hnjuh.cn

Py:   square = lambda x: x * x
来源：http://es.bookmarksfly.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ey.jianghongdianzi.cn

JS:   const square = x => x * x;
来源：http://dr.9csxet.cn

TS:   const square = (x: number): number => x * x;
来源：http://dh.lnxyls.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dv.lnxyls.cn

Go:   sq := func(x int) int { return x * x }
来源：http://cx.jctech888.com.cn

Ruby: square = ->(x) { x * x }
来源：http://ql.jctech888.com.cn

C#:   Func<int, int> square = x => x * x;
来源：http://mg.bookmarksfly.cn

[C07] 把函数作为参数传入
来源：http://zk.521024.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ls.wgjwhj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://rh.hnjuh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ht.shtwfgs.cn

TS:   arr.map(String)
来源：http://ki.hahajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pv.gzmigu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lu.shxzukj.cn

Ruby: arr.map(&:upcase)
来源：http://bk.huanxung.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jj.shxzukj.cn

[C08] 闭包
来源：http://fd.nszjky.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yd.huixinmuqiang.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yj.gzmigu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wc.hahajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zb.9csxet.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yt.yuntaijiaju.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://oq.9csxet.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://oe.bookmarksfly.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gx.shtwfgs.cn

[C09] 递归
来源：http://yx.chemitech.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yo.jianghongdianzi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://iz.gzmigu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ul.bookmarksfly.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xw.szxytkj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gx.wgjwhj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jd.lnxyls.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jy.jctech888.com.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wl.huixiangedu.cn

[C10] 变量作用域
来源：http://le.newstarts.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ij.yuexingan06.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vo.muxihuayi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ox.nszjky.cn

TS:   同 JS
来源：http://da.szxytkj.cn

Java: 方法内为块级作用域
来源：http://on.jianghongdianzi.cn

Go:   花括号块级作用域
来源：http://rh.gzmigu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ec.huixinmuqiang.cn

C#:   块级作用域
来源：http://zi.muxihuayi.cn

[C11] 模块导入与导出
来源：http://si.newstarts.cn

Py:   from module import func
来源：http://el.huixinmuqiang.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://eb.yuntaijiaju.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://tu.shxzskj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://be.panjiajie.cn

Java: import java.util.List;
来源：http://cf.hahajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qy.yuexingan06.cn

Ruby: require "json"; require_relative "./util"
来源：http://eo.bjjhwx.cn

C#:   using System.Text;
来源：http://sb.szxytkj.cn

[C12] 立即执行函数 IIFE
来源：http://ii.colortex.cn

Py:   (lambda: print("run"))()
来源：http://bh.shtwfgs.cn

PHP:  (function () { echo "run"; })();
来源：http://xs.hnjuh.cn

JS:   (() => { console.log("run"); })();
来源：http://ib.huanxung.cn

TS:   (() => { console.log("run"); })();
来源：http://qa.newstarts.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.shxzukj.cn

Go:   func() { fmt.Println("run") }()
来源：http://og.muxihuayi.cn

Ruby: -> { puts "run" }.call
来源：http://ik.521024.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://rl.hahajie.cn

[C13] 类型声明 / 类型注解
来源：http://bm.muxihuayi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nt.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lz.shtwfgs.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tk.hnjuh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://om.huixiangedu.cn

Go:   func add(a, b int) int
来源：http://hx.hnjuh.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dl.jianghongdianzi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tn.jianghongdianzi.cn

[C14] 泛型函数
来源：http://cy.lnxyls.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ax.gzmigu.cn

PHP:  // 无泛型
来源：http://tk.newstarts.cn

JS:   // 无泛型
来源：http://ph.muxihuayi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lg.shxzskj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://je.shxzskj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://sm.chemitech.net.cn

Ruby: # 无泛型
来源：http://cl.nicolike.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cz.colortex.cn

[C15] 解构 / 展开参数
来源：http://zc.yuntaijiaju.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nw.hnjuh.cn

PHP:  [$a, $b] = $pair;
来源：http://gm.chemitech.net.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vn.jianghongdianzi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ur.jianghongdianzi.cn

Java: // 无解构
来源：http://yk.nicolike.cn

Go:   // 无解构
来源：http://vy.521024.cn

Ruby: a, b = pair
来源：http://zp.asd995.cn

C#:   var (a, b) = pair;
来源：http://qn.hnjuh.cn

[C16] 函数 / 方法重载
来源：http://ed.szxytkj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ha.colortex.cn

PHP:  // 无重载
来源：http://zv.nszjky.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://al.shxzskj.cn

TS:   // 用联合类型或重载签名声明
来源：http://fv.nicolike.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://up.panjiajie.cn

Go:   // 无重载：用不同函数名
来源：http://th.521024.cn

Ruby: # 无重载：靠动态参数
来源：http://be.bjjhwx.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rn.hnjuh.cn

================================================================================
来源：http://nb.shxzskj.cn

D. 数组 / 列表 / 集合
来源：http://cs.shtwfgs.cn

================================================================================
来源：http://zl.szsharing.cn

[D01] 创建数组 / 列表
来源：http://jc.asd995.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rs.hahajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gz.hahajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qz.521024.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zh.asd995.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://me.lnxyls.cn

Go:   arr := []int{1, 2, 3}
来源：http://ht.nszjky.cn

Ruby: arr = [1, 2, 3]
来源：http://jd.shtwfgs.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pv.shxzskj.cn

[D02] 追加元素到末尾
来源：http://zg.jianghongdianzi.cn


<!-- 参考信息 -->