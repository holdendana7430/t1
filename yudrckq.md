代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://cl.newstarts.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tj.shtwfgs.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vy.szxytkj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://tx.huixiangedu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yb.newstarts.cn

================================================================================
来源：http://cv.haigaiapp.cn

B. 流程控制
来源：http://us.521024.cn

================================================================================
来源：http://qz.chemitech.net.cn

[B01] 条件判断 if / else
来源：http://bx.huanxung.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dr.bjjhwx.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cc.newstarts.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rg.yuntaijiaju.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://le.shxzskj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xr.521024.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qa.jctech888.com.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ly.wgjwhj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cu.asd995.cn

[B02] 多分支 else if / elif
来源：http://ud.szsharing.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xh.huanxung.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ki.wgjwhj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hh.jctech888.com.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://au.haigaiapp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wp.nszjky.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bk.newstarts.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rr.szsharing.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yh.nszjky.cn

[B03] switch / match / case
来源：http://ac.panjiajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fe.szsharing.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wq.wgjwhj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://if.yuexingan06.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ui.panjiajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dq.yuntaijiaju.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tb.521024.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zg.gzmigu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://to.chemitech.net.cn

[B04] for 计数循环
来源：http://li.muxihuayi.cn

Py:   for i in range(10): print(i)
来源：http://ix.bjjhwx.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dg.colortex.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vk.asd995.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ll.wgjwhj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ss.yuexingan06.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://as.asd995.cn

Ruby: 10.times { |i| puts i }
来源：http://zb.colortex.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xw.szxytkj.cn

[B05] 遍历数组 / 列表
来源：http://yb.haigaiapp.cn

Py:   for item in arr: print(item)
来源：http://yc.muxihuayi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nh.nicolike.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ge.bookmarksfly.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ml.newstarts.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://oo.huixinmuqiang.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ph.huixiangedu.cn

Ruby: arr.each { |item| puts item }
来源：http://xc.muxihuayi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://us.haigaiapp.cn

[B06] 遍历字典 / 对象
来源：http://ce.lnxyls.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://nc.9csxet.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gw.hnjuh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eh.muxihuayi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tl.asd995.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ya.panjiajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nq.shxzukj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fz.jctech888.com.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pd.szxytkj.cn

[B07] while 循环
来源：http://qa.jianghongdianzi.cn

Py:   while i < 10: i += 1
来源：http://rj.yuntaijiaju.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vy.colortex.cn

JS:   while (i < 10) { i++; }
来源：http://ey.newstarts.cn

TS:   while (i < 10) { i++; }
来源：http://vi.hnjuh.cn

Java: while (i < 10) { i++; }
来源：http://bb.shxzukj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nm.panjiajie.cn

Ruby: while i < 10; i += 1; end
来源：http://ot.yuntaijiaju.cn

C#:   while (i < 10) { i++; }
来源：http://pu.yuexingan06.cn

[B08] do-while（至少执行一次）
来源：http://rf.bookmarksfly.cn

Py:   # 无 do-while：用 while True + break
来源：http://cd.hnjuh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://la.yuexingan06.cn

JS:   do { i++; } while (i < 10);
来源：http://tt.yuexingan06.cn

TS:   do { i++; } while (i < 10);
来源：http://mx.bjjhwx.cn

Java: do { i++; } while (i < 10);
来源：http://tx.panjiajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://qj.huixiangedu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jf.colortex.cn

C#:   do { i++; } while (i < 10);
来源：http://ww.yuexingan06.cn

[B09] break 与 continue
来源：http://yj.hnjuh.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://br.lnxyls.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jn.panjiajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dr.shtwfgs.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fq.asd995.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bi.bookmarksfly.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xe.shxzukj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lz.nszjky.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qw.bjjhwx.cn

[B10] 遍历同时拿索引
来源：http://mi.muxihuayi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ym.chemitech.net.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ky.shxzukj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ip.jctech888.com.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ud.huixiangedu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vt.chemitech.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yb.nszjky.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wb.jctech888.com.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sv.shtwfgs.cn

[B11] 生成数字序列 / 区间
来源：http://wo.huixinmuqiang.cn

Py:   list(range(0, 10, 2))
来源：http://ba.huixiangedu.cn

PHP:  range(0, 10, 2);
来源：http://hy.521024.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ax.9csxet.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cw.hnjuh.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lz.shxzskj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rm.nszjky.cn

Ruby: (0...10).step(2).to_a
来源：http://tj.gzmigu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ex.szsharing.cn

[B12] 跳出多层循环
来源：http://jq.9csxet.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ky.newstarts.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://sa.lnxyls.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rt.jianghongdianzi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hk.yuntaijiaju.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://oo.muxihuayi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ur.hnjuh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jn.haigaiapp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yk.hahajie.cn

[B13] 判断是否为数字
来源：http://wv.huanxung.cn

Py:   isinstance(x, (int, float))
来源：http://wz.yuntaijiaju.cn

PHP:  is_numeric($x)
来源：http://fu.lnxyls.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ht.panjiajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ek.bjjhwx.cn

Java: x instanceof Number
来源：http://jn.colortex.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ej.huixinmuqiang.cn

Ruby: x.is_a?(Numeric)
来源：http://ib.szsharing.cn

C#:   x is int or double or decimal
来源：http://yc.huixinmuqiang.cn

[B14] 判断值是否在集合内
来源：http://dd.huanxung.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vh.szxytkj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wn.bjjhwx.cn

JS:   [1, 2, 3].includes(x)
来源：http://rm.gzmigu.cn

TS:   [1, 2, 3].includes(x)
来源：http://ii.shxzukj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rp.lnxyls.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gz.nszjky.cn

Ruby: [1, 2, 3].include?(x)
来源：http://yi.bjjhwx.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bf.lnxyls.cn

[B15] 布尔运算与取反
来源：http://ck.shxzskj.cn

Py:   a and b or not c
来源：http://uq.huixiangedu.cn

PHP:  $a && $b || !$c
来源：http://zt.asd995.cn

JS:   a && b || !c
来源：http://az.shxzskj.cn

TS:   a && b || !c
来源：http://ae.lnxyls.cn

Java: a && b || !c
来源：http://lg.yuexingan06.cn

Go:   a && b || !c
来源：http://kz.shxzskj.cn

Ruby: a && b || !c
来源：http://vk.nicolike.cn

C#:   a && b || !c
来源：http://nc.newstarts.cn

[B16] 卫语句：不满足条件提前返回
来源：http://rr.haigaiapp.cn

Py:   if not data: return
来源：http://nr.hnjuh.cn

PHP:  if (!$data) { return; }
来源：http://et.muxihuayi.cn

JS:   if (!data) return;
来源：http://kn.yuexingan06.cn

TS:   if (!data) return;
来源：http://ku.9csxet.cn

Java: if (data == null) return;
来源：http://ry.haigaiapp.cn

Go:   if data == nil { return }
来源：http://xw.muxihuayi.cn

Ruby: return if data.nil?
来源：http://ng.shxzskj.cn

C#:   if (data == null) return;
来源：http://fc.panjiajie.cn

================================================================================
来源：http://ed.521024.cn

C. 函数与作用域
来源：http://yg.bjjhwx.cn

================================================================================
来源：http://sy.9csxet.cn

[C01] 定义函数
来源：http://zd.gzmigu.cn

Py:   def add(a, b): return a + b
来源：http://kn.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://li.muxihuayi.cn

JS:   function add(a, b) { return a + b; }
来源：http://jl.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://um.jianghongdianzi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://sj.asd995.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ua.szxytkj.cn

Ruby: def add(a, b); a + b; end
来源：http://yo.szxytkj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ke.bjjhwx.cn

[C02] 默认参数
来源：http://zn.wgjwhj.cn

Py:   def greet(name="World"): return name
来源：http://ur.shxzukj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://pq.huixinmuqiang.cn

JS:   function greet(name = "World") { return name; }
来源：http://ee.hahajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://re.jctech888.com.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cu.nicolike.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gn.asd995.cn

Ruby: def greet(name = "World") = name
来源：http://ud.szxytkj.cn

C#:   string Greet(string name = "World") => name;
来源：http://xo.shtwfgs.cn

[C03] 可变参数
来源：http://to.bookmarksfly.cn

Py:   def total(*args): return sum(args)
来源：http://xk.nicolike.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jg.yuexingan06.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mz.hnjuh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pg.shtwfgs.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ys.newstarts.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://oo.newstarts.cn

Ruby: def total(*nums); nums.sum; end
来源：http://sr.521024.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cs.hnjuh.cn

[C04] 命名参数 / 关键字参数
来源：http://pi.hahajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cf.newstarts.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rq.nicolike.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ft.wgjwhj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://oj.bjjhwx.cn

Java: // 无：用 Builder 模式或 record
来源：http://my.panjiajie.cn

Go:   // 无：用配置结构体参数
来源：http://mc.yuexingan06.cn

Ruby: f(a: 1, b: 2)
来源：http://ym.yuexingan06.cn

C#:   f(a: 1, b: 2)
来源：http://sb.szxytkj.cn

[C05] 返回多个值
来源：http://id.colortex.cn

Py:   return a, b
来源：http://sg.yuntaijiaju.cn

PHP:  return [$a, $b];
来源：http://bu.muxihuayi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ng.chemitech.net.cn

TS:   return { a, b };
来源：http://hl.gzmigu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://og.panjiajie.cn

Go:   return a, b
来源：http://sa.yuexingan06.cn

Ruby: return a, b
来源：http://va.yuntaijiaju.cn

C#:   return (a, b);              // ValueTuple
来源：http://iz.bookmarksfly.cn

[C06] 匿名函数 / lambda
来源：http://nc.yuexingan06.cn

Py:   square = lambda x: x * x
来源：http://dz.yuexingan06.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fx.jianghongdianzi.cn

JS:   const square = x => x * x;
来源：http://vq.yuexingan06.cn

TS:   const square = (x: number): number => x * x;
来源：http://oa.huanxung.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gt.huanxung.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hx.huixiangedu.cn

Ruby: square = ->(x) { x * x }
来源：http://ru.nszjky.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ef.nicolike.cn

[C07] 把函数作为参数传入
来源：http://nz.newstarts.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://re.gzmigu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jv.nicolike.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ei.shxzskj.cn

TS:   arr.map(String)
来源：http://cx.asd995.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cd.shtwfgs.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ag.yuexingan06.cn

Ruby: arr.map(&:upcase)
来源：http://xy.chemitech.net.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pz.wgjwhj.cn

[C08] 闭包
来源：http://yn.panjiajie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mo.haigaiapp.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zb.wgjwhj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://au.shtwfgs.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ot.hahajie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cx.hnjuh.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vn.lnxyls.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://oa.nszjky.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ac.9csxet.cn

[C09] 递归
来源：http://pc.nicolike.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qg.asd995.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nx.yuntaijiaju.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fr.jctech888.com.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kj.yuntaijiaju.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://je.nicolike.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nu.yuexingan06.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ir.shxzukj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hu.bjjhwx.cn

[C10] 变量作用域
来源：http://fo.huanxung.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bu.hnjuh.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gz.haigaiapp.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xu.chemitech.net.cn

TS:   同 JS
来源：http://es.nszjky.cn

Java: 方法内为块级作用域
来源：http://hz.jianghongdianzi.cn

Go:   花括号块级作用域
来源：http://vu.colortex.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yr.gzmigu.cn

C#:   块级作用域
来源：http://kr.lnxyls.cn

[C11] 模块导入与导出
来源：http://gd.huixiangedu.cn

Py:   from module import func
来源：http://bi.colortex.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zz.newstarts.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://dd.lnxyls.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ww.newstarts.cn

Java: import java.util.List;
来源：http://se.hnjuh.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xf.gzmigu.cn

Ruby: require "json"; require_relative "./util"
来源：http://ku.yuntaijiaju.cn

C#:   using System.Text;
来源：http://lf.gzmigu.cn

[C12] 立即执行函数 IIFE
来源：http://yl.bookmarksfly.cn

Py:   (lambda: print("run"))()
来源：http://dg.jianghongdianzi.cn

PHP:  (function () { echo "run"; })();
来源：http://fd.nszjky.cn

JS:   (() => { console.log("run"); })();
来源：http://is.szsharing.cn

TS:   (() => { console.log("run"); })();
来源：http://ab.shxzukj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ux.jianghongdianzi.cn

Go:   func() { fmt.Println("run") }()
来源：http://ca.huanxung.cn

Ruby: -> { puts "run" }.call
来源：http://yl.jianghongdianzi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://sb.nszjky.cn

[C13] 类型声明 / 类型注解
来源：http://ki.hnjuh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xp.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vz.huanxung.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ly.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lp.shxzukj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ou.yuexingan06.cn

Go:   func add(a, b int) int
来源：http://ks.panjiajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hw.shxzskj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://yx.chemitech.net.cn

[C14] 泛型函数
来源：http://iu.haigaiapp.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hm.chemitech.net.cn

PHP:  // 无泛型
来源：http://kf.hahajie.cn

JS:   // 无泛型
来源：http://xg.huixinmuqiang.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qj.szsharing.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ks.nszjky.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ez.jctech888.com.cn

Ruby: # 无泛型
来源：http://yy.huixinmuqiang.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nc.521024.cn

[C15] 解构 / 展开参数
来源：http://nw.gzmigu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ty.asd995.cn

PHP:  [$a, $b] = $pair;
来源：http://vp.chemitech.net.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tm.bjjhwx.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pv.haigaiapp.cn

Java: // 无解构
来源：http://qd.gzmigu.cn

Go:   // 无解构
来源：http://xd.gzmigu.cn

Ruby: a, b = pair
来源：http://lv.colortex.cn

C#:   var (a, b) = pair;
来源：http://pg.chemitech.net.cn

[C16] 函数 / 方法重载
来源：http://dr.9csxet.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xm.jianghongdianzi.cn

PHP:  // 无重载
来源：http://hr.jianghongdianzi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bd.haigaiapp.cn

TS:   // 用联合类型或重载签名声明
来源：http://xd.gzmigu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pl.huixiangedu.cn

Go:   // 无重载：用不同函数名
来源：http://gs.muxihuayi.cn

Ruby: # 无重载：靠动态参数
来源：http://vv.nszjky.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://tq.bookmarksfly.cn

================================================================================
来源：http://vp.szxytkj.cn


<!-- 参考信息 -->