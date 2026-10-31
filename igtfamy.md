代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://sb.chemitech.net.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ar.hahajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rq.yuexingan06.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://wq.haigaiapp.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://od.panjiajie.cn

================================================================================
来源：http://wc.hnjuh.cn

B. 流程控制
来源：http://cx.bookmarksfly.cn

================================================================================
来源：http://cf.huixiangedu.cn

[B01] 条件判断 if / else
来源：http://aw.huanxung.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://qk.huixiangedu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://my.huanxung.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ix.gzmigu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bi.yuntaijiaju.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://pk.newstarts.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ff.gzmigu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cl.colortex.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hp.jianghongdianzi.cn

[B02] 多分支 else if / elif
来源：http://oh.bjjhwx.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lk.yuntaijiaju.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vy.gzmigu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jl.huanxung.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mb.wgjwhj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pk.wgjwhj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yg.shtwfgs.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://my.muxihuayi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uw.huanxung.cn

[B03] switch / match / case
来源：http://rd.wgjwhj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yl.haigaiapp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://er.szsharing.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lz.shxzukj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oq.521024.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nb.huixiangedu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ss.huanxung.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yj.haigaiapp.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ps.bookmarksfly.cn

[B04] for 计数循环
来源：http://us.muxihuayi.cn

Py:   for i in range(10): print(i)
来源：http://jp.nicolike.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ju.nicolike.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cx.lnxyls.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qb.huanxung.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ig.shxzukj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ev.muxihuayi.cn

Ruby: 10.times { |i| puts i }
来源：http://td.shtwfgs.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wx.szxytkj.cn

[B05] 遍历数组 / 列表
来源：http://rg.nicolike.cn

Py:   for item in arr: print(item)
来源：http://lk.haigaiapp.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rg.newstarts.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ir.shxzskj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://in.9csxet.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yf.nicolike.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vw.shxzskj.cn

Ruby: arr.each { |item| puts item }
来源：http://gi.nszjky.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jt.bjjhwx.cn

[B06] 遍历字典 / 对象
来源：http://ul.newstarts.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xi.colortex.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ue.asd995.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yl.muxihuayi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uj.panjiajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://to.yuexingan06.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nl.yuntaijiaju.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hn.521024.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ty.9csxet.cn

[B07] while 循环
来源：http://xq.szsharing.cn

Py:   while i < 10: i += 1
来源：http://an.szxytkj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bs.jctech888.com.cn

JS:   while (i < 10) { i++; }
来源：http://og.szsharing.cn

TS:   while (i < 10) { i++; }
来源：http://dh.yuntaijiaju.cn

Java: while (i < 10) { i++; }
来源：http://uw.shxzukj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yo.huixiangedu.cn

Ruby: while i < 10; i += 1; end
来源：http://vt.shxzskj.cn

C#:   while (i < 10) { i++; }
来源：http://sy.lnxyls.cn

[B08] do-while（至少执行一次）
来源：http://qm.colortex.cn

Py:   # 无 do-while：用 while True + break
来源：http://er.jctech888.com.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pi.asd995.cn

JS:   do { i++; } while (i < 10);
来源：http://ar.asd995.cn

TS:   do { i++; } while (i < 10);
来源：http://am.521024.cn

Java: do { i++; } while (i < 10);
来源：http://ru.colortex.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ge.jianghongdianzi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ax.jctech888.com.cn

C#:   do { i++; } while (i < 10);
来源：http://pr.yuexingan06.cn

[B09] break 与 continue
来源：http://bs.nszjky.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pk.huixiangedu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hp.gzmigu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pj.wgjwhj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tt.szxytkj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fw.newstarts.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tc.nszjky.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yq.nicolike.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cd.hnjuh.cn

[B10] 遍历同时拿索引
来源：http://gn.jctech888.com.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tw.panjiajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yf.wgjwhj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://we.gzmigu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yq.yuexingan06.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xv.haigaiapp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zu.gzmigu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ae.newstarts.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ui.szxytkj.cn

[B11] 生成数字序列 / 区间
来源：http://wl.panjiajie.cn

Py:   list(range(0, 10, 2))
来源：http://wu.jianghongdianzi.cn

PHP:  range(0, 10, 2);
来源：http://wz.nicolike.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cp.yuexingan06.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://az.yuexingan06.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jt.jctech888.com.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://al.nicolike.cn

Ruby: (0...10).step(2).to_a
来源：http://kt.521024.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ap.9csxet.cn

[B12] 跳出多层循环
来源：http://cq.colortex.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://mv.lnxyls.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fb.huixinmuqiang.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kj.asd995.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ws.huixinmuqiang.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wl.huanxung.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://at.shxzskj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xx.gzmigu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hc.asd995.cn

[B13] 判断是否为数字
来源：http://uc.jctech888.com.cn

Py:   isinstance(x, (int, float))
来源：http://wc.jctech888.com.cn

PHP:  is_numeric($x)
来源：http://aj.nszjky.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wg.newstarts.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gn.huixinmuqiang.cn

Java: x instanceof Number
来源：http://am.jianghongdianzi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yh.jctech888.com.cn

Ruby: x.is_a?(Numeric)
来源：http://rd.9csxet.cn

C#:   x is int or double or decimal
来源：http://mj.bookmarksfly.cn

[B14] 判断值是否在集合内
来源：http://gz.wgjwhj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ql.521024.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://do.9csxet.cn

JS:   [1, 2, 3].includes(x)
来源：http://vz.gzmigu.cn

TS:   [1, 2, 3].includes(x)
来源：http://fz.haigaiapp.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dx.haigaiapp.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jj.lnxyls.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jj.newstarts.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lg.nszjky.cn

[B15] 布尔运算与取反
来源：http://ov.gzmigu.cn

Py:   a and b or not c
来源：http://xx.huixinmuqiang.cn

PHP:  $a && $b || !$c
来源：http://mi.asd995.cn

JS:   a && b || !c
来源：http://tg.huixinmuqiang.cn

TS:   a && b || !c
来源：http://tz.colortex.cn

Java: a && b || !c
来源：http://xa.9csxet.cn

Go:   a && b || !c
来源：http://uq.lnxyls.cn

Ruby: a && b || !c
来源：http://go.gzmigu.cn

C#:   a && b || !c
来源：http://sj.nszjky.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zi.shxzukj.cn

Py:   if not data: return
来源：http://uy.jctech888.com.cn

PHP:  if (!$data) { return; }
来源：http://ta.colortex.cn

JS:   if (!data) return;
来源：http://hc.szxytkj.cn

TS:   if (!data) return;
来源：http://ik.shxzskj.cn

Java: if (data == null) return;
来源：http://ek.9csxet.cn

Go:   if data == nil { return }
来源：http://ec.chemitech.net.cn

Ruby: return if data.nil?
来源：http://xj.shtwfgs.cn

C#:   if (data == null) return;
来源：http://lj.lnxyls.cn

================================================================================
来源：http://bv.nszjky.cn

C. 函数与作用域
来源：http://vd.hahajie.cn

================================================================================
来源：http://by.wgjwhj.cn

[C01] 定义函数
来源：http://pw.lnxyls.cn

Py:   def add(a, b): return a + b
来源：http://gi.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://az.shtwfgs.cn

JS:   function add(a, b) { return a + b; }
来源：http://he.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zf.huixinmuqiang.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zr.newstarts.cn

Go:   func add(a, b int) int { return a + b }
来源：http://gf.bookmarksfly.cn

Ruby: def add(a, b); a + b; end
来源：http://dl.hnjuh.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vy.asd995.cn

[C02] 默认参数
来源：http://zt.nszjky.cn

Py:   def greet(name="World"): return name
来源：http://un.yuntaijiaju.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lm.szsharing.cn

JS:   function greet(name = "World") { return name; }
来源：http://bh.bjjhwx.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://tr.521024.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://gi.huanxung.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://my.szsharing.cn

Ruby: def greet(name = "World") = name
来源：http://wu.yuexingan06.cn

C#:   string Greet(string name = "World") => name;
来源：http://kp.9csxet.cn

[C03] 可变参数
来源：http://ur.asd995.cn

Py:   def total(*args): return sum(args)
来源：http://ka.huixinmuqiang.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nr.panjiajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fc.colortex.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mo.shtwfgs.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bb.shtwfgs.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hr.hahajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tp.hahajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gz.hahajie.cn

[C04] 命名参数 / 关键字参数
来源：http://uu.shxzskj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qn.colortex.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yz.nszjky.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kk.jctech888.com.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ir.nicolike.cn

Java: // 无：用 Builder 模式或 record
来源：http://wn.colortex.cn

Go:   // 无：用配置结构体参数
来源：http://hs.9csxet.cn

Ruby: f(a: 1, b: 2)
来源：http://wy.shxzukj.cn

C#:   f(a: 1, b: 2)
来源：http://lf.chemitech.net.cn

[C05] 返回多个值
来源：http://us.shtwfgs.cn

Py:   return a, b
来源：http://bs.huixinmuqiang.cn

PHP:  return [$a, $b];
来源：http://cq.jianghongdianzi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wp.huixinmuqiang.cn

TS:   return { a, b };
来源：http://jd.chemitech.net.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nc.bookmarksfly.cn

Go:   return a, b
来源：http://is.panjiajie.cn

Ruby: return a, b
来源：http://ii.muxihuayi.cn

C#:   return (a, b);              // ValueTuple
来源：http://lz.nicolike.cn

[C06] 匿名函数 / lambda
来源：http://zq.bjjhwx.cn

Py:   square = lambda x: x * x
来源：http://ym.muxihuayi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ur.lnxyls.cn

JS:   const square = x => x * x;
来源：http://fy.chemitech.net.cn

TS:   const square = (x: number): number => x * x;
来源：http://dr.wgjwhj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yh.chemitech.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ug.newstarts.cn

Ruby: square = ->(x) { x * x }
来源：http://st.huanxung.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ro.shxzukj.cn

[C07] 把函数作为参数传入
来源：http://qm.asd995.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cl.hnjuh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://py.bookmarksfly.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qa.nicolike.cn

TS:   arr.map(String)
来源：http://tu.chemitech.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qb.gzmigu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jq.jctech888.com.cn

Ruby: arr.map(&:upcase)
来源：http://dl.muxihuayi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ty.hahajie.cn

[C08] 闭包
来源：http://ej.jctech888.com.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://sc.newstarts.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pq.asd995.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qa.muxihuayi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uu.yuntaijiaju.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fb.szsharing.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dc.jianghongdianzi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ci.huanxung.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ot.yuntaijiaju.cn

[C09] 递归
来源：http://dw.asd995.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rv.bjjhwx.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vz.gzmigu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://si.muxihuayi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jc.hahajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ri.chemitech.net.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ji.nszjky.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kt.asd995.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vl.shxzukj.cn

[C10] 变量作用域
来源：http://cz.gzmigu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nx.szxytkj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ti.jianghongdianzi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://th.huixiangedu.cn

TS:   同 JS
来源：http://jb.muxihuayi.cn

Java: 方法内为块级作用域
来源：http://rw.521024.cn

Go:   花括号块级作用域
来源：http://xy.nszjky.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tz.huanxung.cn

C#:   块级作用域
来源：http://us.9csxet.cn

[C11] 模块导入与导出
来源：http://rp.asd995.cn

Py:   from module import func
来源：http://du.jctech888.com.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pi.lnxyls.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ws.yuexingan06.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lm.gzmigu.cn

Java: import java.util.List;
来源：http://mg.yuntaijiaju.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dk.colortex.cn

Ruby: require "json"; require_relative "./util"
来源：http://cc.colortex.cn

C#:   using System.Text;
来源：http://km.jianghongdianzi.cn

[C12] 立即执行函数 IIFE
来源：http://hj.muxihuayi.cn

Py:   (lambda: print("run"))()
来源：http://iu.wgjwhj.cn

PHP:  (function () { echo "run"; })();
来源：http://oz.9csxet.cn

JS:   (() => { console.log("run"); })();
来源：http://ab.bjjhwx.cn

TS:   (() => { console.log("run"); })();
来源：http://jr.lnxyls.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bm.jianghongdianzi.cn

Go:   func() { fmt.Println("run") }()
来源：http://av.lnxyls.cn

Ruby: -> { puts "run" }.call
来源：http://fb.yuntaijiaju.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pl.bjjhwx.cn

[C13] 类型声明 / 类型注解
来源：http://vr.huanxung.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pd.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zz.wgjwhj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://md.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kj.asd995.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fb.nszjky.cn

Go:   func add(a, b int) int
来源：http://sk.huixiangedu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dh.lnxyls.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qw.huanxung.cn

[C14] 泛型函数
来源：http://ng.huanxung.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://va.szxytkj.cn

PHP:  // 无泛型
来源：http://bt.szsharing.cn

JS:   // 无泛型
来源：http://mo.shtwfgs.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dj.bjjhwx.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dn.yuntaijiaju.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qy.huixinmuqiang.cn

Ruby: # 无泛型
来源：http://wk.nicolike.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://el.hahajie.cn

[C15] 解构 / 展开参数
来源：http://rt.gzmigu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ly.wgjwhj.cn

PHP:  [$a, $b] = $pair;
来源：http://ml.huixiangedu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://et.nicolike.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tw.yuexingan06.cn

Java: // 无解构
来源：http://jp.yuexingan06.cn

Go:   // 无解构
来源：http://tl.newstarts.cn

Ruby: a, b = pair
来源：http://eb.newstarts.cn

C#:   var (a, b) = pair;
来源：http://pk.huixinmuqiang.cn

[C16] 函数 / 方法重载
来源：http://kp.gzmigu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wm.jianghongdianzi.cn

PHP:  // 无重载
来源：http://zj.muxihuayi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lf.wgjwhj.cn

TS:   // 用联合类型或重载签名声明
来源：http://zf.shtwfgs.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://tm.colortex.cn

Go:   // 无重载：用不同函数名
来源：http://wt.hahajie.cn

Ruby: # 无重载：靠动态参数
来源：http://lb.huixinmuqiang.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://jb.shtwfgs.cn

================================================================================
来源：http://ru.huixinmuqiang.cn


<!-- 参考信息 -->