代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ne.hnjuh.cn

================================================================================
来源：http://ll.chemitech.net.cn

B. 流程控制
来源：http://ld.shxzukj.cn

================================================================================
来源：http://pc.nicolike.cn

[B01] 条件判断 if / else
来源：http://ua.szsharing.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://tq.chemitech.net.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nf.shxzukj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xw.huanxung.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://if.bjjhwx.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bn.jianghongdianzi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yk.yuntaijiaju.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rq.yuntaijiaju.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fp.newstarts.cn

[B02] 多分支 else if / elif
来源：http://ys.hnjuh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nu.hnjuh.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kl.yuexingan06.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ho.jctech888.com.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lh.hnjuh.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fw.shtwfgs.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://eq.shtwfgs.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ob.bjjhwx.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kx.szsharing.cn

[B03] switch / match / case
来源：http://sm.hahajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tp.wgjwhj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gu.huixiangedu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://si.bjjhwx.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ei.521024.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qa.521024.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zn.yuntaijiaju.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://te.521024.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gg.9csxet.cn

[B04] for 计数循环
来源：http://it.bjjhwx.cn

Py:   for i in range(10): print(i)
来源：http://hs.huixinmuqiang.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mj.szxytkj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lp.asd995.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dl.huanxung.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ud.jianghongdianzi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ar.colortex.cn

Ruby: 10.times { |i| puts i }
来源：http://ou.huanxung.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://la.521024.cn

[B05] 遍历数组 / 列表
来源：http://sx.colortex.cn

Py:   for item in arr: print(item)
来源：http://gj.szsharing.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://oi.huixinmuqiang.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qr.szsharing.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tp.jianghongdianzi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://et.panjiajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ku.shxzukj.cn

Ruby: arr.each { |item| puts item }
来源：http://mu.szsharing.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://be.hnjuh.cn

[B06] 遍历字典 / 对象
来源：http://zh.panjiajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ju.szxytkj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tc.huixinmuqiang.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yx.bookmarksfly.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vu.shtwfgs.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fm.bookmarksfly.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://za.asd995.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://oe.nicolike.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rz.jianghongdianzi.cn

[B07] while 循环
来源：http://md.lnxyls.cn

Py:   while i < 10: i += 1
来源：http://mw.9csxet.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wu.chemitech.net.cn

JS:   while (i < 10) { i++; }
来源：http://rw.chemitech.net.cn

TS:   while (i < 10) { i++; }
来源：http://gf.newstarts.cn

Java: while (i < 10) { i++; }
来源：http://wk.shxzskj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zf.gzmigu.cn

Ruby: while i < 10; i += 1; end
来源：http://jk.haigaiapp.cn

C#:   while (i < 10) { i++; }
来源：http://fe.bjjhwx.cn

[B08] do-while（至少执行一次）
来源：http://yq.newstarts.cn

Py:   # 无 do-while：用 while True + break
来源：http://qz.wgjwhj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://sm.lnxyls.cn

JS:   do { i++; } while (i < 10);
来源：http://uu.lnxyls.cn

TS:   do { i++; } while (i < 10);
来源：http://nt.gzmigu.cn

Java: do { i++; } while (i < 10);
来源：http://sf.haigaiapp.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://pv.asd995.cn

Ruby: begin; i += 1; end while i < 10
来源：http://yp.hnjuh.cn

C#:   do { i++; } while (i < 10);
来源：http://la.bjjhwx.cn

[B09] break 与 continue
来源：http://rs.muxihuayi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://re.szsharing.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rq.jctech888.com.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ao.gzmigu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tb.gzmigu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://an.9csxet.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wu.nszjky.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qz.nszjky.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cv.asd995.cn

[B10] 遍历同时拿索引
来源：http://zb.panjiajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sb.panjiajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dv.bjjhwx.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qm.shxzukj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tt.bookmarksfly.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bq.jctech888.com.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rn.yuntaijiaju.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xm.shxzukj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fj.szxytkj.cn

[B11] 生成数字序列 / 区间
来源：http://ej.yuexingan06.cn

Py:   list(range(0, 10, 2))
来源：http://ie.hnjuh.cn

PHP:  range(0, 10, 2);
来源：http://ry.wgjwhj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qr.jctech888.com.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zy.shxzskj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fy.nicolike.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cx.shtwfgs.cn

Ruby: (0...10).step(2).to_a
来源：http://rq.bjjhwx.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ht.521024.cn

[B12] 跳出多层循环
来源：http://ok.bookmarksfly.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zh.hahajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ss.hahajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tb.yuexingan06.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qn.newstarts.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zf.lnxyls.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://so.asd995.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://iz.panjiajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rf.panjiajie.cn

[B13] 判断是否为数字
来源：http://ad.nszjky.cn

Py:   isinstance(x, (int, float))
来源：http://yn.newstarts.cn

PHP:  is_numeric($x)
来源：http://sh.lnxyls.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://eq.szsharing.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lg.chemitech.net.cn

Java: x instanceof Number
来源：http://qd.panjiajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vi.huanxung.cn

Ruby: x.is_a?(Numeric)
来源：http://si.muxihuayi.cn

C#:   x is int or double or decimal
来源：http://qr.newstarts.cn

[B14] 判断值是否在集合内
来源：http://ny.bookmarksfly.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hw.nszjky.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wl.bjjhwx.cn

JS:   [1, 2, 3].includes(x)
来源：http://lt.shxzskj.cn

TS:   [1, 2, 3].includes(x)
来源：http://rm.szxytkj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://py.bookmarksfly.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zc.shxzukj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vi.szsharing.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ko.9csxet.cn

[B15] 布尔运算与取反
来源：http://yi.colortex.cn

Py:   a and b or not c
来源：http://hw.lnxyls.cn

PHP:  $a && $b || !$c
来源：http://lj.lnxyls.cn

JS:   a && b || !c
来源：http://wv.nicolike.cn

TS:   a && b || !c
来源：http://oq.yuexingan06.cn

Java: a && b || !c
来源：http://ws.shxzskj.cn

Go:   a && b || !c
来源：http://hj.shxzukj.cn

Ruby: a && b || !c
来源：http://ed.jctech888.com.cn

C#:   a && b || !c
来源：http://ek.huixiangedu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://pt.lnxyls.cn

Py:   if not data: return
来源：http://uy.nicolike.cn

PHP:  if (!$data) { return; }
来源：http://br.muxihuayi.cn

JS:   if (!data) return;
来源：http://uk.hahajie.cn

TS:   if (!data) return;
来源：http://ev.haigaiapp.cn

Java: if (data == null) return;
来源：http://wb.521024.cn

Go:   if data == nil { return }
来源：http://yy.gzmigu.cn

Ruby: return if data.nil?
来源：http://cu.yuexingan06.cn

C#:   if (data == null) return;
来源：http://cb.shxzukj.cn

================================================================================
来源：http://yw.newstarts.cn

C. 函数与作用域
来源：http://ff.muxihuayi.cn

================================================================================
来源：http://te.szxytkj.cn

[C01] 定义函数
来源：http://wk.shxzukj.cn

Py:   def add(a, b): return a + b
来源：http://hx.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vn.bookmarksfly.cn

JS:   function add(a, b) { return a + b; }
来源：http://ck.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ee.jianghongdianzi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ze.yuexingan06.cn

Go:   func add(a, b int) int { return a + b }
来源：http://pe.yuexingan06.cn

Ruby: def add(a, b); a + b; end
来源：http://mb.shxzukj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ey.jianghongdianzi.cn

[C02] 默认参数
来源：http://eb.bjjhwx.cn

Py:   def greet(name="World"): return name
来源：http://hn.yuexingan06.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://is.szsharing.cn

JS:   function greet(name = "World") { return name; }
来源：http://qb.bjjhwx.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://es.bookmarksfly.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wx.hnjuh.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tz.huixiangedu.cn

Ruby: def greet(name = "World") = name
来源：http://yj.szsharing.cn

C#:   string Greet(string name = "World") => name;
来源：http://xg.shxzukj.cn

[C03] 可变参数
来源：http://ej.lnxyls.cn

Py:   def total(*args): return sum(args)
来源：http://ln.huixinmuqiang.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://se.bookmarksfly.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xv.nicolike.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yc.muxihuayi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://oc.szsharing.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://px.huanxung.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ge.huixiangedu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://oo.szxytkj.cn

[C04] 命名参数 / 关键字参数
来源：http://ny.yuexingan06.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ld.huixinmuqiang.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rg.bjjhwx.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tr.szsharing.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zp.wgjwhj.cn

Java: // 无：用 Builder 模式或 record
来源：http://dd.shtwfgs.cn

Go:   // 无：用配置结构体参数
来源：http://wl.huixiangedu.cn

Ruby: f(a: 1, b: 2)
来源：http://iy.yuexingan06.cn

C#:   f(a: 1, b: 2)
来源：http://pz.nszjky.cn

[C05] 返回多个值
来源：http://pf.huanxung.cn

Py:   return a, b
来源：http://jr.nicolike.cn

PHP:  return [$a, $b];
来源：http://du.nicolike.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://tl.jctech888.com.cn

TS:   return { a, b };
来源：http://qp.haigaiapp.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zz.jctech888.com.cn

Go:   return a, b
来源：http://tj.yuntaijiaju.cn

Ruby: return a, b
来源：http://px.haigaiapp.cn

C#:   return (a, b);              // ValueTuple
来源：http://jb.asd995.cn

[C06] 匿名函数 / lambda
来源：http://pr.yuntaijiaju.cn

Py:   square = lambda x: x * x
来源：http://rj.szsharing.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://kz.huanxung.cn

JS:   const square = x => x * x;
来源：http://cg.shxzukj.cn

TS:   const square = (x: number): number => x * x;
来源：http://fm.huanxung.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fs.9csxet.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ri.haigaiapp.cn

Ruby: square = ->(x) { x * x }
来源：http://vt.muxihuayi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dr.521024.cn

[C07] 把函数作为参数传入
来源：http://lh.bjjhwx.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kr.hahajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jx.huixiangedu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bo.nszjky.cn

TS:   arr.map(String)
来源：http://bm.panjiajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sh.huixinmuqiang.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cu.shxzukj.cn

Ruby: arr.map(&:upcase)
来源：http://ua.hnjuh.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://lc.shxzskj.cn

[C08] 闭包
来源：http://ur.lnxyls.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qy.521024.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hr.hahajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gr.haigaiapp.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bm.newstarts.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rx.lnxyls.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vf.nicolike.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ye.panjiajie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hd.newstarts.cn

[C09] 递归
来源：http://dt.chemitech.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wv.szsharing.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fy.jianghongdianzi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dn.huixinmuqiang.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ft.hahajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fp.bjjhwx.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gb.jctech888.com.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ok.szsharing.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pp.nicolike.cn

[C10] 变量作用域
来源：http://vd.szxytkj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wf.lnxyls.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ge.nszjky.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://re.jianghongdianzi.cn

TS:   同 JS
来源：http://rp.szsharing.cn

Java: 方法内为块级作用域
来源：http://cj.haigaiapp.cn

Go:   花括号块级作用域
来源：http://iv.asd995.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yb.wgjwhj.cn

C#:   块级作用域
来源：http://gh.szxytkj.cn

[C11] 模块导入与导出
来源：http://ie.hahajie.cn

Py:   from module import func
来源：http://uu.panjiajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://re.huixiangedu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://mq.haigaiapp.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rt.jianghongdianzi.cn

Java: import java.util.List;
来源：http://gh.szsharing.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mi.521024.cn

Ruby: require "json"; require_relative "./util"
来源：http://gv.shxzskj.cn

C#:   using System.Text;
来源：http://xj.hnjuh.cn

[C12] 立即执行函数 IIFE
来源：http://qf.hahajie.cn

Py:   (lambda: print("run"))()
来源：http://iw.bjjhwx.cn

PHP:  (function () { echo "run"; })();
来源：http://or.bookmarksfly.cn

JS:   (() => { console.log("run"); })();
来源：http://ym.huixiangedu.cn

TS:   (() => { console.log("run"); })();
来源：http://ha.muxihuayi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ru.nszjky.cn

Go:   func() { fmt.Println("run") }()
来源：http://pn.jctech888.com.cn

Ruby: -> { puts "run" }.call
来源：http://vg.nszjky.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ul.szxytkj.cn

[C13] 类型声明 / 类型注解
来源：http://if.haigaiapp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ni.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vf.huanxung.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sv.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hn.jianghongdianzi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://iy.lnxyls.cn

Go:   func add(a, b int) int
来源：http://cf.jianghongdianzi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kw.szxytkj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://rq.yuntaijiaju.cn

[C14] 泛型函数
来源：http://ga.colortex.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://iz.nicolike.cn

PHP:  // 无泛型
来源：http://gv.chemitech.net.cn

JS:   // 无泛型
来源：http://hs.9csxet.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fm.huanxung.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lr.hnjuh.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jh.hahajie.cn

Ruby: # 无泛型
来源：http://kj.shxzskj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yz.szsharing.cn

[C15] 解构 / 展开参数
来源：http://eu.shxzskj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nz.shtwfgs.cn

PHP:  [$a, $b] = $pair;
来源：http://vc.yuntaijiaju.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://io.chemitech.net.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yk.asd995.cn

Java: // 无解构
来源：http://vy.haigaiapp.cn

Go:   // 无解构
来源：http://xf.yuexingan06.cn

Ruby: a, b = pair
来源：http://vs.haigaiapp.cn

C#:   var (a, b) = pair;
来源：http://nw.nszjky.cn

[C16] 函数 / 方法重载
来源：http://mh.yuntaijiaju.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jg.shtwfgs.cn

PHP:  // 无重载
来源：http://cy.hahajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://do.shxzskj.cn

TS:   // 用联合类型或重载签名声明
来源：http://ln.shtwfgs.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://sr.hahajie.cn

Go:   // 无重载：用不同函数名
来源：http://mm.asd995.cn

Ruby: # 无重载：靠动态参数
来源：http://gd.hahajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://bt.bjjhwx.cn

================================================================================
来源：http://bb.9csxet.cn

D. 数组 / 列表 / 集合
来源：http://cn.hahajie.cn

================================================================================
来源：http://gy.szsharing.cn

[D01] 创建数组 / 列表
来源：http://op.hnjuh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ty.9csxet.cn


<!-- 参考信息 -->