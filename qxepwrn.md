代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://zt.9csxet.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kr.huixiangedu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cu.wgjwhj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://cg.chemitech.net.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://du.shtwfgs.cn

================================================================================
来源：http://zn.shtwfgs.cn

B. 流程控制
来源：http://fe.asd995.cn

================================================================================
来源：http://tr.9csxet.cn

[B01] 条件判断 if / else
来源：http://qy.shxzskj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://at.bookmarksfly.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sq.yuntaijiaju.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ha.panjiajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://id.jctech888.com.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://sp.jctech888.com.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://uc.szxytkj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zs.asd995.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://eh.newstarts.cn

[B02] 多分支 else if / elif
来源：http://jp.shxzskj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kj.nszjky.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ih.jctech888.com.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ma.chemitech.net.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wf.521024.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gh.shtwfgs.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nk.hnjuh.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ay.bookmarksfly.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rk.shtwfgs.cn

[B03] switch / match / case
来源：http://cm.shtwfgs.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wb.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zz.shtwfgs.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lt.nicolike.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gg.jctech888.com.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ej.huixiangedu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mh.muxihuayi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ml.shxzskj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vl.521024.cn

[B04] for 计数循环
来源：http://jg.colortex.cn

Py:   for i in range(10): print(i)
来源：http://wc.shxzukj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ck.muxihuayi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ni.yuntaijiaju.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uz.wgjwhj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hm.huanxung.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jr.yuntaijiaju.cn

Ruby: 10.times { |i| puts i }
来源：http://mm.muxihuayi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pk.huixinmuqiang.cn

[B05] 遍历数组 / 列表
来源：http://bg.jianghongdianzi.cn

Py:   for item in arr: print(item)
来源：http://zh.shtwfgs.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sm.nszjky.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://xt.shxzukj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ms.shxzskj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://dv.shxzskj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pt.haigaiapp.cn

Ruby: arr.each { |item| puts item }
来源：http://wt.bjjhwx.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://io.hnjuh.cn

[B06] 遍历字典 / 对象
来源：http://be.huanxung.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://de.szxytkj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sr.hnjuh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ph.huanxung.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bb.chemitech.net.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qu.szsharing.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qn.shxzukj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ut.yuntaijiaju.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xd.9csxet.cn

[B07] while 循环
来源：http://xb.colortex.cn

Py:   while i < 10: i += 1
来源：http://qb.shxzskj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xq.bjjhwx.cn

JS:   while (i < 10) { i++; }
来源：http://zo.bjjhwx.cn

TS:   while (i < 10) { i++; }
来源：http://rg.521024.cn

Java: while (i < 10) { i++; }
来源：http://be.9csxet.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zf.9csxet.cn

Ruby: while i < 10; i += 1; end
来源：http://cq.huixinmuqiang.cn

C#:   while (i < 10) { i++; }
来源：http://za.jianghongdianzi.cn

[B08] do-while（至少执行一次）
来源：http://ja.shtwfgs.cn

Py:   # 无 do-while：用 while True + break
来源：http://qc.szxytkj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zh.szxytkj.cn

JS:   do { i++; } while (i < 10);
来源：http://si.shtwfgs.cn

TS:   do { i++; } while (i < 10);
来源：http://be.jctech888.com.cn

Java: do { i++; } while (i < 10);
来源：http://yp.hnjuh.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://at.colortex.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qp.jctech888.com.cn

C#:   do { i++; } while (i < 10);
来源：http://ex.nicolike.cn

[B09] break 与 continue
来源：http://kk.9csxet.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vv.jianghongdianzi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ky.yuexingan06.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ne.nicolike.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tb.huixinmuqiang.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dm.bjjhwx.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tx.hahajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://px.bookmarksfly.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ft.haigaiapp.cn

[B10] 遍历同时拿索引
来源：http://rw.szxytkj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qc.bjjhwx.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xd.gzmigu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jg.asd995.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wc.lnxyls.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wy.shxzskj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vb.9csxet.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rj.nszjky.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qd.huanxung.cn

[B11] 生成数字序列 / 区间
来源：http://ec.shxzskj.cn

Py:   list(range(0, 10, 2))
来源：http://kw.newstarts.cn

PHP:  range(0, 10, 2);
来源：http://du.huixinmuqiang.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ot.chemitech.net.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sl.colortex.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://or.9csxet.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kv.szxytkj.cn

Ruby: (0...10).step(2).to_a
来源：http://yu.bjjhwx.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://un.shxzskj.cn

[B12] 跳出多层循环
来源：http://rh.9csxet.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wr.bookmarksfly.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vs.haigaiapp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ft.huixiangedu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://uq.haigaiapp.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wu.chemitech.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://db.szsharing.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kg.huixiangedu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sp.bjjhwx.cn

[B13] 判断是否为数字
来源：http://ms.shxzukj.cn

Py:   isinstance(x, (int, float))
来源：http://ta.huixinmuqiang.cn

PHP:  is_numeric($x)
来源：http://hz.hahajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qh.lnxyls.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ck.bjjhwx.cn

Java: x instanceof Number
来源：http://kq.gzmigu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mo.huixinmuqiang.cn

Ruby: x.is_a?(Numeric)
来源：http://uy.nicolike.cn

C#:   x is int or double or decimal
来源：http://zz.hnjuh.cn

[B14] 判断值是否在集合内
来源：http://sf.szxytkj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ih.colortex.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://he.huanxung.cn

JS:   [1, 2, 3].includes(x)
来源：http://gm.bjjhwx.cn

TS:   [1, 2, 3].includes(x)
来源：http://mp.nszjky.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ir.9csxet.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zq.521024.cn

Ruby: [1, 2, 3].include?(x)
来源：http://sy.bjjhwx.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://oj.huixinmuqiang.cn

[B15] 布尔运算与取反
来源：http://vs.yuexingan06.cn

Py:   a and b or not c
来源：http://cj.shxzskj.cn

PHP:  $a && $b || !$c
来源：http://hx.huixinmuqiang.cn

JS:   a && b || !c
来源：http://qe.hahajie.cn

TS:   a && b || !c
来源：http://wx.gzmigu.cn

Java: a && b || !c
来源：http://bo.yuexingan06.cn

Go:   a && b || !c
来源：http://cf.jctech888.com.cn

Ruby: a && b || !c
来源：http://di.wgjwhj.cn

C#:   a && b || !c
来源：http://lc.huixinmuqiang.cn

[B16] 卫语句：不满足条件提前返回
来源：http://yz.yuexingan06.cn

Py:   if not data: return
来源：http://ak.muxihuayi.cn

PHP:  if (!$data) { return; }
来源：http://zl.szsharing.cn

JS:   if (!data) return;
来源：http://fk.newstarts.cn

TS:   if (!data) return;
来源：http://ca.lnxyls.cn

Java: if (data == null) return;
来源：http://nd.colortex.cn

Go:   if data == nil { return }
来源：http://zl.huixiangedu.cn

Ruby: return if data.nil?
来源：http://wo.nszjky.cn

C#:   if (data == null) return;
来源：http://fx.chemitech.net.cn

================================================================================
来源：http://kk.shtwfgs.cn

C. 函数与作用域
来源：http://dm.yuntaijiaju.cn

================================================================================
来源：http://fg.asd995.cn

[C01] 定义函数
来源：http://ws.huixiangedu.cn

Py:   def add(a, b): return a + b
来源：http://wt.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kd.bjjhwx.cn

JS:   function add(a, b) { return a + b; }
来源：http://uu.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kw.nicolike.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://pj.jianghongdianzi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jv.newstarts.cn

Ruby: def add(a, b); a + b; end
来源：http://ih.nicolike.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qd.muxihuayi.cn

[C02] 默认参数
来源：http://uq.521024.cn

Py:   def greet(name="World"): return name
来源：http://th.bjjhwx.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zi.yuexingan06.cn

JS:   function greet(name = "World") { return name; }
来源：http://cn.asd995.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://jj.nszjky.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cy.jctech888.com.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vl.gzmigu.cn

Ruby: def greet(name = "World") = name
来源：http://tb.gzmigu.cn

C#:   string Greet(string name = "World") => name;
来源：http://un.yuexingan06.cn

[C03] 可变参数
来源：http://jw.jctech888.com.cn

Py:   def total(*args): return sum(args)
来源：http://ua.521024.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ll.bjjhwx.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xd.huixiangedu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uo.huixinmuqiang.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xd.yuexingan06.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sk.newstarts.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xf.nszjky.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ux.hahajie.cn

[C04] 命名参数 / 关键字参数
来源：http://aj.huixiangedu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xk.9csxet.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vl.haigaiapp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ab.shxzskj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yf.huanxung.cn

Java: // 无：用 Builder 模式或 record
来源：http://gg.nszjky.cn

Go:   // 无：用配置结构体参数
来源：http://aa.jctech888.com.cn

Ruby: f(a: 1, b: 2)
来源：http://zk.9csxet.cn

C#:   f(a: 1, b: 2)
来源：http://yl.huixiangedu.cn

[C05] 返回多个值
来源：http://hv.huanxung.cn

Py:   return a, b
来源：http://wk.521024.cn

PHP:  return [$a, $b];
来源：http://mq.szsharing.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://cg.shtwfgs.cn

TS:   return { a, b };
来源：http://tj.shxzukj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fd.panjiajie.cn

Go:   return a, b
来源：http://ix.bookmarksfly.cn

Ruby: return a, b
来源：http://gp.shxzskj.cn

C#:   return (a, b);              // ValueTuple
来源：http://is.muxihuayi.cn

[C06] 匿名函数 / lambda
来源：http://mh.shtwfgs.cn

Py:   square = lambda x: x * x
来源：http://do.shxzukj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pd.bjjhwx.cn

JS:   const square = x => x * x;
来源：http://ie.huixiangedu.cn

TS:   const square = (x: number): number => x * x;
来源：http://mq.bookmarksfly.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jh.newstarts.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ju.bookmarksfly.cn

Ruby: square = ->(x) { x * x }
来源：http://az.szsharing.cn

C#:   Func<int, int> square = x => x * x;
来源：http://rh.huanxung.cn

[C07] 把函数作为参数传入
来源：http://eb.lnxyls.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xu.hnjuh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://mx.gzmigu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gb.szxytkj.cn

TS:   arr.map(String)
来源：http://th.chemitech.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xt.wgjwhj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qd.yuexingan06.cn

Ruby: arr.map(&:upcase)
来源：http://ua.szsharing.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://af.lnxyls.cn

[C08] 闭包
来源：http://ma.shxzskj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yg.shtwfgs.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hb.lnxyls.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qu.shxzukj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://px.nszjky.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://aw.panjiajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tn.gzmigu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://if.yuexingan06.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fh.wgjwhj.cn

[C09] 递归
来源：http://cl.newstarts.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fs.hahajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sv.shxzskj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zs.muxihuayi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://js.bookmarksfly.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sh.521024.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ya.yuexingan06.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://az.huixinmuqiang.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://oh.chemitech.net.cn

[C10] 变量作用域
来源：http://dz.bjjhwx.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zr.newstarts.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hp.bjjhwx.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jx.gzmigu.cn

TS:   同 JS
来源：http://yg.szsharing.cn

Java: 方法内为块级作用域
来源：http://ml.bookmarksfly.cn

Go:   花括号块级作用域
来源：http://io.gzmigu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wh.jianghongdianzi.cn

C#:   块级作用域
来源：http://bh.szxytkj.cn

[C11] 模块导入与导出
来源：http://an.szxytkj.cn

Py:   from module import func
来源：http://eu.bjjhwx.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://cc.gzmigu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://wx.shxzskj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nx.bjjhwx.cn

Java: import java.util.List;
来源：http://pw.szsharing.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xc.521024.cn

Ruby: require "json"; require_relative "./util"
来源：http://xb.jianghongdianzi.cn

C#:   using System.Text;
来源：http://ne.jctech888.com.cn

[C12] 立即执行函数 IIFE
来源：http://ba.bookmarksfly.cn

Py:   (lambda: print("run"))()
来源：http://pi.huixinmuqiang.cn

PHP:  (function () { echo "run"; })();
来源：http://ie.colortex.cn

JS:   (() => { console.log("run"); })();
来源：http://ym.bookmarksfly.cn

TS:   (() => { console.log("run"); })();
来源：http://fi.9csxet.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vq.shtwfgs.cn

Go:   func() { fmt.Println("run") }()
来源：http://fd.yuexingan06.cn

Ruby: -> { puts "run" }.call
来源：http://wp.hahajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://vu.gzmigu.cn

[C13] 类型声明 / 类型注解
来源：http://vo.colortex.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hv.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zw.shtwfgs.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zx.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rh.szxytkj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ep.bookmarksfly.cn

Go:   func add(a, b int) int
来源：http://wu.nicolike.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://la.szxytkj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fc.nicolike.cn

[C14] 泛型函数
来源：http://ng.bjjhwx.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://iy.chemitech.net.cn

PHP:  // 无泛型
来源：http://py.shxzskj.cn

JS:   // 无泛型
来源：http://jk.jianghongdianzi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://px.asd995.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nn.muxihuayi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yc.chemitech.net.cn

Ruby: # 无泛型
来源：http://td.huanxung.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nx.colortex.cn

[C15] 解构 / 展开参数
来源：http://cy.yuexingan06.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ey.huixinmuqiang.cn

PHP:  [$a, $b] = $pair;
来源：http://up.gzmigu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qc.nicolike.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bt.jianghongdianzi.cn

Java: // 无解构
来源：http://ye.lnxyls.cn

Go:   // 无解构
来源：http://ux.shtwfgs.cn

Ruby: a, b = pair
来源：http://yv.panjiajie.cn

C#:   var (a, b) = pair;
来源：http://dw.9csxet.cn

[C16] 函数 / 方法重载
来源：http://bx.newstarts.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tm.nicolike.cn

PHP:  // 无重载
来源：http://mj.asd995.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zr.panjiajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://ob.lnxyls.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://lz.huixiangedu.cn

Go:   // 无重载：用不同函数名
来源：http://tx.colortex.cn

Ruby: # 无重载：靠动态参数
来源：http://pu.newstarts.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zl.shxzskj.cn

================================================================================
来源：http://bc.shxzskj.cn


<!-- 参考信息 -->