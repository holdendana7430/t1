代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://pa.haigaiapp.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nl.chemitech.net.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ti.yuexingan06.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ao.9csxet.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gz.huanxung.cn

================================================================================
来源：http://ej.newstarts.cn

B. 流程控制
来源：http://ya.jianghongdianzi.cn

================================================================================
来源：http://ss.muxihuayi.cn

[B01] 条件判断 if / else
来源：http://wc.chemitech.net.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://gj.bjjhwx.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kg.huixinmuqiang.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ey.hnjuh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wz.wgjwhj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ie.hahajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cw.nszjky.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ek.haigaiapp.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://we.wgjwhj.cn

[B02] 多分支 else if / elif
来源：http://gl.colortex.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hq.bookmarksfly.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ct.9csxet.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mo.nszjky.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://su.haigaiapp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qj.colortex.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qa.panjiajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://sc.szsharing.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wv.lnxyls.cn

[B03] switch / match / case
来源：http://vs.huixinmuqiang.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://er.szsharing.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qw.newstarts.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nq.lnxyls.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nm.gzmigu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lo.muxihuayi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://oe.asd995.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zj.bjjhwx.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fx.shxzukj.cn

[B04] for 计数循环
来源：http://jb.shxzskj.cn

Py:   for i in range(10): print(i)
来源：http://wt.521024.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jc.shxzskj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xd.szxytkj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qu.szxytkj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qg.asd995.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lk.gzmigu.cn

Ruby: 10.times { |i| puts i }
来源：http://su.panjiajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://re.bjjhwx.cn

[B05] 遍历数组 / 列表
来源：http://jh.shtwfgs.cn

Py:   for item in arr: print(item)
来源：http://kw.asd995.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cg.bookmarksfly.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://my.bjjhwx.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://nn.muxihuayi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://av.newstarts.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wh.newstarts.cn

Ruby: arr.each { |item| puts item }
来源：http://gp.521024.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qk.huanxung.cn

[B06] 遍历字典 / 对象
来源：http://cy.jctech888.com.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pd.bookmarksfly.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hg.nszjky.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://py.gzmigu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ci.haigaiapp.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ek.huixiangedu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lo.huixinmuqiang.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dq.gzmigu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cg.nszjky.cn

[B07] while 循环
来源：http://bg.9csxet.cn

Py:   while i < 10: i += 1
来源：http://oc.9csxet.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wb.hnjuh.cn

JS:   while (i < 10) { i++; }
来源：http://tt.nicolike.cn

TS:   while (i < 10) { i++; }
来源：http://ts.521024.cn

Java: while (i < 10) { i++; }
来源：http://yj.9csxet.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tt.9csxet.cn

Ruby: while i < 10; i += 1; end
来源：http://er.521024.cn

C#:   while (i < 10) { i++; }
来源：http://ri.colortex.cn

[B08] do-while（至少执行一次）
来源：http://rc.yuntaijiaju.cn

Py:   # 无 do-while：用 while True + break
来源：http://cd.haigaiapp.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://yt.gzmigu.cn

JS:   do { i++; } while (i < 10);
来源：http://qq.wgjwhj.cn

TS:   do { i++; } while (i < 10);
来源：http://jp.haigaiapp.cn

Java: do { i++; } while (i < 10);
来源：http://yd.shtwfgs.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ve.huixiangedu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://tk.muxihuayi.cn

C#:   do { i++; } while (i < 10);
来源：http://tq.panjiajie.cn

[B09] break 与 continue
来源：http://cv.jctech888.com.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ri.hahajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ju.asd995.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lh.shxzskj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bq.szsharing.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ia.jianghongdianzi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://oj.shtwfgs.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bu.shxzukj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eo.hahajie.cn

[B10] 遍历同时拿索引
来源：http://ui.wgjwhj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.shxzskj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dl.panjiajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://oq.chemitech.net.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mc.gzmigu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xv.jctech888.com.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xf.yuexingan06.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://la.yuntaijiaju.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mz.szsharing.cn

[B11] 生成数字序列 / 区间
来源：http://ue.muxihuayi.cn

Py:   list(range(0, 10, 2))
来源：http://lt.shxzukj.cn

PHP:  range(0, 10, 2);
来源：http://xj.bookmarksfly.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ma.bjjhwx.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jb.huixinmuqiang.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zm.9csxet.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://om.wgjwhj.cn

Ruby: (0...10).step(2).to_a
来源：http://tv.colortex.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mz.haigaiapp.cn

[B12] 跳出多层循环
来源：http://gt.jianghongdianzi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ze.jianghongdianzi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://yb.bjjhwx.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fl.szxytkj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fx.bjjhwx.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ub.haigaiapp.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wj.lnxyls.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xf.shxzskj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cw.wgjwhj.cn

[B13] 判断是否为数字
来源：http://nw.szsharing.cn

Py:   isinstance(x, (int, float))
来源：http://nh.hahajie.cn

PHP:  is_numeric($x)
来源：http://co.szsharing.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fe.szxytkj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://he.colortex.cn

Java: x instanceof Number
来源：http://rh.colortex.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xu.shxzskj.cn

Ruby: x.is_a?(Numeric)
来源：http://ip.wgjwhj.cn

C#:   x is int or double or decimal
来源：http://vr.521024.cn

[B14] 判断值是否在集合内
来源：http://nl.muxihuayi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://we.szsharing.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hx.shxzukj.cn

JS:   [1, 2, 3].includes(x)
来源：http://hr.panjiajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://td.huixiangedu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dn.haigaiapp.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wl.bjjhwx.cn

Ruby: [1, 2, 3].include?(x)
来源：http://go.jctech888.com.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ay.newstarts.cn

[B15] 布尔运算与取反
来源：http://uz.bookmarksfly.cn

Py:   a and b or not c
来源：http://ms.huixiangedu.cn

PHP:  $a && $b || !$c
来源：http://hs.hahajie.cn

JS:   a && b || !c
来源：http://ul.9csxet.cn

TS:   a && b || !c
来源：http://ea.huixinmuqiang.cn

Java: a && b || !c
来源：http://vs.hahajie.cn

Go:   a && b || !c
来源：http://hs.nicolike.cn

Ruby: a && b || !c
来源：http://pr.chemitech.net.cn

C#:   a && b || !c
来源：http://br.yuntaijiaju.cn

[B16] 卫语句：不满足条件提前返回
来源：http://mw.shxzukj.cn

Py:   if not data: return
来源：http://qd.haigaiapp.cn

PHP:  if (!$data) { return; }
来源：http://pd.shxzskj.cn

JS:   if (!data) return;
来源：http://be.bjjhwx.cn

TS:   if (!data) return;
来源：http://yq.panjiajie.cn

Java: if (data == null) return;
来源：http://wi.bookmarksfly.cn

Go:   if data == nil { return }
来源：http://rc.colortex.cn

Ruby: return if data.nil?
来源：http://yh.yuexingan06.cn

C#:   if (data == null) return;
来源：http://xq.nszjky.cn

================================================================================
来源：http://wq.haigaiapp.cn

C. 函数与作用域
来源：http://af.gzmigu.cn

================================================================================
来源：http://fs.panjiajie.cn

[C01] 定义函数
来源：http://nc.huixiangedu.cn

Py:   def add(a, b): return a + b
来源：http://sm.muxihuayi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ew.bookmarksfly.cn

JS:   function add(a, b) { return a + b; }
来源：http://oe.panjiajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wb.hnjuh.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ik.jianghongdianzi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://oa.newstarts.cn

Ruby: def add(a, b); a + b; end
来源：http://wt.nicolike.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://go.lnxyls.cn

[C02] 默认参数
来源：http://it.bjjhwx.cn

Py:   def greet(name="World"): return name
来源：http://bz.wgjwhj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://mv.panjiajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://me.szxytkj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://tz.huixinmuqiang.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://xf.hahajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yt.chemitech.net.cn

Ruby: def greet(name = "World") = name
来源：http://af.jctech888.com.cn

C#:   string Greet(string name = "World") => name;
来源：http://yz.chemitech.net.cn

[C03] 可变参数
来源：http://ce.huanxung.cn

Py:   def total(*args): return sum(args)
来源：http://dz.wgjwhj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fz.muxihuayi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lh.colortex.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yc.colortex.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xj.colortex.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ul.bookmarksfly.cn

Ruby: def total(*nums); nums.sum; end
来源：http://cx.bookmarksfly.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://uf.hahajie.cn

[C04] 命名参数 / 关键字参数
来源：http://tn.haigaiapp.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://eh.shtwfgs.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xh.newstarts.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rg.wgjwhj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bk.521024.cn

Java: // 无：用 Builder 模式或 record
来源：http://pc.chemitech.net.cn

Go:   // 无：用配置结构体参数
来源：http://my.huanxung.cn

Ruby: f(a: 1, b: 2)
来源：http://su.lnxyls.cn

C#:   f(a: 1, b: 2)
来源：http://nq.lnxyls.cn

[C05] 返回多个值
来源：http://ht.huixiangedu.cn

Py:   return a, b
来源：http://iq.jctech888.com.cn

PHP:  return [$a, $b];
来源：http://id.szsharing.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qe.521024.cn

TS:   return { a, b };
来源：http://ef.muxihuayi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ku.huixinmuqiang.cn

Go:   return a, b
来源：http://hs.huixiangedu.cn

Ruby: return a, b
来源：http://lk.nicolike.cn

C#:   return (a, b);              // ValueTuple
来源：http://vl.jianghongdianzi.cn

[C06] 匿名函数 / lambda
来源：http://mu.colortex.cn

Py:   square = lambda x: x * x
来源：http://gx.haigaiapp.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pu.yuntaijiaju.cn

JS:   const square = x => x * x;
来源：http://wo.huixinmuqiang.cn

TS:   const square = (x: number): number => x * x;
来源：http://yf.newstarts.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lg.lnxyls.cn

Go:   sq := func(x int) int { return x * x }
来源：http://vn.panjiajie.cn

Ruby: square = ->(x) { x * x }
来源：http://qu.huixinmuqiang.cn

C#:   Func<int, int> square = x => x * x;
来源：http://vw.yuntaijiaju.cn

[C07] 把函数作为参数传入
来源：http://fd.nicolike.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lp.shtwfgs.cn

PHP:  array_map("strtoupper", $arr);
来源：http://dg.yuntaijiaju.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qw.jianghongdianzi.cn

TS:   arr.map(String)
来源：http://dr.nszjky.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dq.huixinmuqiang.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qk.lnxyls.cn

Ruby: arr.map(&:upcase)
来源：http://xl.panjiajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://st.panjiajie.cn

[C08] 闭包
来源：http://le.shxzskj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lz.colortex.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://da.shxzskj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fh.haigaiapp.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uv.chemitech.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://eh.colortex.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://uo.newstarts.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ku.huixinmuqiang.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://md.panjiajie.cn

[C09] 递归
来源：http://qf.lnxyls.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qx.hnjuh.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cu.haigaiapp.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://re.521024.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oa.huixiangedu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ye.panjiajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qe.hnjuh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://si.lnxyls.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gu.bookmarksfly.cn

[C10] 变量作用域
来源：http://fz.9csxet.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hk.chemitech.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vw.hnjuh.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ap.shxzskj.cn

TS:   同 JS
来源：http://hi.521024.cn

Java: 方法内为块级作用域
来源：http://oh.hnjuh.cn

Go:   花括号块级作用域
来源：http://qs.lnxyls.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nv.nicolike.cn

C#:   块级作用域
来源：http://kk.521024.cn

[C11] 模块导入与导出
来源：http://yh.yuexingan06.cn

Py:   from module import func
来源：http://fg.nszjky.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xr.nszjky.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ro.yuexingan06.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://te.szsharing.cn

Java: import java.util.List;
来源：http://sb.nicolike.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dc.jianghongdianzi.cn

Ruby: require "json"; require_relative "./util"
来源：http://mx.lnxyls.cn

C#:   using System.Text;
来源：http://ap.jianghongdianzi.cn

[C12] 立即执行函数 IIFE
来源：http://ud.yuntaijiaju.cn

Py:   (lambda: print("run"))()
来源：http://ae.szxytkj.cn

PHP:  (function () { echo "run"; })();
来源：http://hq.szsharing.cn

JS:   (() => { console.log("run"); })();
来源：http://au.shtwfgs.cn

TS:   (() => { console.log("run"); })();
来源：http://gv.shxzskj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://oe.yuexingan06.cn

Go:   func() { fmt.Println("run") }()
来源：http://gd.shxzukj.cn

Ruby: -> { puts "run" }.call
来源：http://ed.9csxet.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://by.shtwfgs.cn

[C13] 类型声明 / 类型注解
来源：http://ql.jianghongdianzi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jn.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mh.hahajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xh.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bs.wgjwhj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ux.shxzskj.cn

Go:   func add(a, b int) int
来源：http://da.gzmigu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jy.huixinmuqiang.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vo.huixinmuqiang.cn

[C14] 泛型函数
来源：http://xi.wgjwhj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gw.huixiangedu.cn

PHP:  // 无泛型
来源：http://ej.asd995.cn

JS:   // 无泛型
来源：http://os.huanxung.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pp.yuexingan06.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fq.newstarts.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ke.nicolike.cn

Ruby: # 无泛型
来源：http://jf.hahajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yx.yuntaijiaju.cn

[C15] 解构 / 展开参数
来源：http://nh.haigaiapp.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ly.asd995.cn

PHP:  [$a, $b] = $pair;
来源：http://qa.huixinmuqiang.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vr.9csxet.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://af.lnxyls.cn

Java: // 无解构
来源：http://ib.gzmigu.cn

Go:   // 无解构
来源：http://fw.chemitech.net.cn

Ruby: a, b = pair
来源：http://yb.nicolike.cn

C#:   var (a, b) = pair;
来源：http://tw.521024.cn

[C16] 函数 / 方法重载
来源：http://em.muxihuayi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ro.gzmigu.cn

PHP:  // 无重载
来源：http://hb.shxzskj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ox.szxytkj.cn

TS:   // 用联合类型或重载签名声明
来源：http://gz.szxytkj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ym.huixiangedu.cn

Go:   // 无重载：用不同函数名
来源：http://vf.nicolike.cn

Ruby: # 无重载：靠动态参数
来源：http://gj.wgjwhj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://em.huixinmuqiang.cn

================================================================================
来源：http://cp.9csxet.cn


<!-- 参考信息 -->