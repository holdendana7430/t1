代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://eu.chemitech.net.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xi.huanxung.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rp.colortex.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://xu.chemitech.net.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ta.jianghongdianzi.cn

================================================================================
来源：http://rh.huixiangedu.cn

B. 流程控制
来源：http://jo.shxzskj.cn

================================================================================
来源：http://wk.wgjwhj.cn

[B01] 条件判断 if / else
来源：http://vs.shxzskj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://fx.nszjky.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ni.bookmarksfly.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gq.jianghongdianzi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ql.jianghongdianzi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://cv.bookmarksfly.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ws.panjiajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fn.bjjhwx.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jj.wgjwhj.cn

[B02] 多分支 else if / elif
来源：http://xr.colortex.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://so.gzmigu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://aa.nszjky.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nt.yuexingan06.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vm.newstarts.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ej.hnjuh.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wr.huixinmuqiang.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xh.bookmarksfly.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rf.bookmarksfly.cn

[B03] switch / match / case
来源：http://vl.wgjwhj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zc.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gu.bjjhwx.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bi.521024.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dy.521024.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mc.panjiajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ww.chemitech.net.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ib.szsharing.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://af.szxytkj.cn

[B04] for 计数循环
来源：http://sk.hahajie.cn

Py:   for i in range(10): print(i)
来源：http://mk.muxihuayi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bk.wgjwhj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lm.nszjky.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hn.nicolike.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://um.newstarts.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vi.bjjhwx.cn

Ruby: 10.times { |i| puts i }
来源：http://bq.jctech888.com.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sw.shxzskj.cn

[B05] 遍历数组 / 列表
来源：http://ak.szsharing.cn

Py:   for item in arr: print(item)
来源：http://mz.muxihuayi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xa.hahajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gl.521024.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tt.muxihuayi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://cz.newstarts.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nf.huixiangedu.cn

Ruby: arr.each { |item| puts item }
来源：http://ao.asd995.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xi.521024.cn

[B06] 遍历字典 / 对象
来源：http://rh.wgjwhj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://kt.shxzskj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uh.gzmigu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ea.nicolike.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jo.shtwfgs.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qm.panjiajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vm.huanxung.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vq.huixiangedu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://oi.panjiajie.cn

[B07] while 循环
来源：http://qw.szxytkj.cn

Py:   while i < 10: i += 1
来源：http://ug.szxytkj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ux.szsharing.cn

JS:   while (i < 10) { i++; }
来源：http://tp.bjjhwx.cn

TS:   while (i < 10) { i++; }
来源：http://mg.shxzukj.cn

Java: while (i < 10) { i++; }
来源：http://bk.yuexingan06.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gl.huixinmuqiang.cn

Ruby: while i < 10; i += 1; end
来源：http://mm.huixiangedu.cn

C#:   while (i < 10) { i++; }
来源：http://rx.panjiajie.cn

[B08] do-while（至少执行一次）
来源：http://xm.muxihuayi.cn

Py:   # 无 do-while：用 while True + break
来源：http://ob.shtwfgs.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://dz.szxytkj.cn

JS:   do { i++; } while (i < 10);
来源：http://tp.chemitech.net.cn

TS:   do { i++; } while (i < 10);
来源：http://xc.wgjwhj.cn

Java: do { i++; } while (i < 10);
来源：http://qb.hahajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vy.huixiangedu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://tu.9csxet.cn

C#:   do { i++; } while (i < 10);
来源：http://zd.wgjwhj.cn

[B09] break 与 continue
来源：http://yr.hnjuh.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zv.yuntaijiaju.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uo.yuexingan06.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ht.521024.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jf.hahajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fc.huixiangedu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fd.wgjwhj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://si.nszjky.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yi.gzmigu.cn

[B10] 遍历同时拿索引
来源：http://cx.nicolike.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hy.huanxung.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ap.hnjuh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://le.lnxyls.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ro.hahajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zx.panjiajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kj.chemitech.net.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tu.shxzukj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ae.wgjwhj.cn

[B11] 生成数字序列 / 区间
来源：http://zy.shxzukj.cn

Py:   list(range(0, 10, 2))
来源：http://ru.huixinmuqiang.cn

PHP:  range(0, 10, 2);
来源：http://ze.bookmarksfly.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wg.nszjky.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uk.jctech888.com.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ya.shxzskj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://up.panjiajie.cn

Ruby: (0...10).step(2).to_a
来源：http://ux.yuexingan06.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wb.shxzskj.cn

[B12] 跳出多层循环
来源：http://vq.yuexingan06.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ag.lnxyls.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://yh.colortex.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yr.colortex.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://aj.haigaiapp.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zy.huixinmuqiang.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ko.yuntaijiaju.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://iq.szsharing.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://et.wgjwhj.cn

[B13] 判断是否为数字
来源：http://pk.yuntaijiaju.cn

Py:   isinstance(x, (int, float))
来源：http://yf.asd995.cn

PHP:  is_numeric($x)
来源：http://dx.jianghongdianzi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nl.shxzukj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ng.shxzukj.cn

Java: x instanceof Number
来源：http://cr.nicolike.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wz.szsharing.cn

Ruby: x.is_a?(Numeric)
来源：http://vz.jianghongdianzi.cn

C#:   x is int or double or decimal
来源：http://pn.hahajie.cn

[B14] 判断值是否在集合内
来源：http://jh.nszjky.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wy.yuexingan06.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://af.chemitech.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://ba.jctech888.com.cn

TS:   [1, 2, 3].includes(x)
来源：http://bp.muxihuayi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://cu.newstarts.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dh.newstarts.cn

Ruby: [1, 2, 3].include?(x)
来源：http://od.huanxung.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ky.gzmigu.cn

[B15] 布尔运算与取反
来源：http://iw.asd995.cn

Py:   a and b or not c
来源：http://zr.hnjuh.cn

PHP:  $a && $b || !$c
来源：http://za.yuntaijiaju.cn

JS:   a && b || !c
来源：http://vj.shxzskj.cn

TS:   a && b || !c
来源：http://kp.hnjuh.cn

Java: a && b || !c
来源：http://zh.yuntaijiaju.cn

Go:   a && b || !c
来源：http://qt.huanxung.cn

Ruby: a && b || !c
来源：http://ow.huixinmuqiang.cn

C#:   a && b || !c
来源：http://aw.hahajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qv.huanxung.cn

Py:   if not data: return
来源：http://nl.shtwfgs.cn

PHP:  if (!$data) { return; }
来源：http://ks.521024.cn

JS:   if (!data) return;
来源：http://ew.haigaiapp.cn

TS:   if (!data) return;
来源：http://sr.yuntaijiaju.cn

Java: if (data == null) return;
来源：http://gl.shtwfgs.cn

Go:   if data == nil { return }
来源：http://ae.nszjky.cn

Ruby: return if data.nil?
来源：http://ow.asd995.cn

C#:   if (data == null) return;
来源：http://gr.521024.cn

================================================================================
来源：http://mh.shtwfgs.cn

C. 函数与作用域
来源：http://ch.gzmigu.cn

================================================================================
来源：http://xa.yuntaijiaju.cn

[C01] 定义函数
来源：http://up.521024.cn

Py:   def add(a, b): return a + b
来源：http://te.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yl.haigaiapp.cn

JS:   function add(a, b) { return a + b; }
来源：http://kh.yuexingan06.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wv.shxzskj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bx.asd995.cn

Go:   func add(a, b int) int { return a + b }
来源：http://bk.hnjuh.cn

Ruby: def add(a, b); a + b; end
来源：http://dx.huixiangedu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vu.bjjhwx.cn

[C02] 默认参数
来源：http://li.huanxung.cn

Py:   def greet(name="World"): return name
来源：http://bf.szsharing.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://px.jctech888.com.cn

JS:   function greet(name = "World") { return name; }
来源：http://ef.9csxet.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ip.panjiajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jq.jctech888.com.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rk.hahajie.cn

Ruby: def greet(name = "World") = name
来源：http://dd.hahajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://mp.9csxet.cn

[C03] 可变参数
来源：http://az.shxzukj.cn

Py:   def total(*args): return sum(args)
来源：http://bw.lnxyls.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ra.gzmigu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ho.panjiajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fg.nszjky.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wx.asd995.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://je.hnjuh.cn

Ruby: def total(*nums); nums.sum; end
来源：http://do.huanxung.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jo.asd995.cn

[C04] 命名参数 / 关键字参数
来源：http://wf.hnjuh.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ed.huixinmuqiang.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ve.jctech888.com.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wv.jctech888.com.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ds.lnxyls.cn

Java: // 无：用 Builder 模式或 record
来源：http://ff.haigaiapp.cn

Go:   // 无：用配置结构体参数
来源：http://hh.jianghongdianzi.cn

Ruby: f(a: 1, b: 2)
来源：http://xf.colortex.cn

C#:   f(a: 1, b: 2)
来源：http://jm.jianghongdianzi.cn

[C05] 返回多个值
来源：http://kn.huixinmuqiang.cn

Py:   return a, b
来源：http://om.lnxyls.cn

PHP:  return [$a, $b];
来源：http://mv.nicolike.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ko.huixiangedu.cn

TS:   return { a, b };
来源：http://mk.newstarts.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fu.colortex.cn

Go:   return a, b
来源：http://cf.haigaiapp.cn

Ruby: return a, b
来源：http://rx.yuexingan06.cn

C#:   return (a, b);              // ValueTuple
来源：http://ql.yuntaijiaju.cn

[C06] 匿名函数 / lambda
来源：http://up.9csxet.cn

Py:   square = lambda x: x * x
来源：http://kk.9csxet.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zx.nicolike.cn

JS:   const square = x => x * x;
来源：http://on.yuntaijiaju.cn

TS:   const square = (x: number): number => x * x;
来源：http://jm.asd995.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://np.chemitech.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wv.huanxung.cn

Ruby: square = ->(x) { x * x }
来源：http://hi.huixiangedu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://de.nszjky.cn

[C07] 把函数作为参数传入
来源：http://un.szxytkj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://oj.colortex.cn

PHP:  array_map("strtoupper", $arr);
来源：http://rj.jianghongdianzi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jv.shxzskj.cn

TS:   arr.map(String)
来源：http://hx.asd995.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cj.yuexingan06.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wr.jianghongdianzi.cn

Ruby: arr.map(&:upcase)
来源：http://yr.yuntaijiaju.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ez.huixinmuqiang.cn

[C08] 闭包
来源：http://ss.wgjwhj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ht.9csxet.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bn.muxihuayi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://oa.szxytkj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dr.wgjwhj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yz.yuexingan06.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vk.yuexingan06.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tv.bjjhwx.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yr.hnjuh.cn

[C09] 递归
来源：http://tw.panjiajie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gb.shxzukj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://np.yuexingan06.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jn.bjjhwx.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bj.nicolike.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bv.yuexingan06.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mj.gzmigu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ks.huixinmuqiang.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xt.wgjwhj.cn

[C10] 变量作用域
来源：http://rq.asd995.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hl.wgjwhj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jl.lnxyls.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ds.panjiajie.cn

TS:   同 JS
来源：http://pg.gzmigu.cn

Java: 方法内为块级作用域
来源：http://uw.panjiajie.cn

Go:   花括号块级作用域
来源：http://fb.chemitech.net.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pq.shtwfgs.cn

C#:   块级作用域
来源：http://bk.hahajie.cn

[C11] 模块导入与导出
来源：http://dx.hahajie.cn

Py:   from module import func
来源：http://hv.muxihuayi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xs.asd995.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ps.wgjwhj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xy.asd995.cn

Java: import java.util.List;
来源：http://bs.colortex.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yb.szxytkj.cn

Ruby: require "json"; require_relative "./util"
来源：http://lc.huixinmuqiang.cn

C#:   using System.Text;
来源：http://ed.haigaiapp.cn

[C12] 立即执行函数 IIFE
来源：http://ll.szsharing.cn

Py:   (lambda: print("run"))()
来源：http://fe.shxzukj.cn

PHP:  (function () { echo "run"; })();
来源：http://eo.hahajie.cn

JS:   (() => { console.log("run"); })();
来源：http://rx.panjiajie.cn

TS:   (() => { console.log("run"); })();
来源：http://iu.hahajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://px.521024.cn

Go:   func() { fmt.Println("run") }()
来源：http://bv.nszjky.cn

Ruby: -> { puts "run" }.call
来源：http://yy.shtwfgs.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fh.nszjky.cn

[C13] 类型声明 / 类型注解
来源：http://zb.haigaiapp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xn.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bo.jctech888.com.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://co.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jt.yuexingan06.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tb.jctech888.com.cn

Go:   func add(a, b int) int
来源：http://bq.nszjky.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hu.huanxung.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qo.nszjky.cn

[C14] 泛型函数
来源：http://dq.panjiajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zl.huixinmuqiang.cn

PHP:  // 无泛型
来源：http://vg.521024.cn

JS:   // 无泛型
来源：http://yg.muxihuayi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nq.shxzskj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ic.newstarts.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wd.521024.cn

Ruby: # 无泛型
来源：http://th.szsharing.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zs.muxihuayi.cn

[C15] 解构 / 展开参数
来源：http://jq.muxihuayi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ii.colortex.cn

PHP:  [$a, $b] = $pair;
来源：http://qr.521024.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qr.jianghongdianzi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://om.haigaiapp.cn

Java: // 无解构
来源：http://df.lnxyls.cn

Go:   // 无解构
来源：http://le.521024.cn

Ruby: a, b = pair
来源：http://er.asd995.cn

C#:   var (a, b) = pair;
来源：http://qg.wgjwhj.cn

[C16] 函数 / 方法重载
来源：http://le.haigaiapp.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mv.shxzskj.cn

PHP:  // 无重载
来源：http://sb.jianghongdianzi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://da.lnxyls.cn

TS:   // 用联合类型或重载签名声明
来源：http://zs.wgjwhj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://iz.521024.cn

Go:   // 无重载：用不同函数名
来源：http://ko.shxzskj.cn

Ruby: # 无重载：靠动态参数
来源：http://ag.521024.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ck.szxytkj.cn

================================================================================
来源：http://gw.chemitech.net.cn


<!-- 参考信息 -->