代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uu.9csxet.cn

================================================================================
来源：http://mu.newstarts.cn

B. 流程控制
来源：http://ur.gzmigu.cn

================================================================================
来源：http://ua.lnxyls.cn

[B01] 条件判断 if / else
来源：http://ny.jianghongdianzi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ft.bookmarksfly.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://no.521024.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xt.521024.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yx.nicolike.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://dn.lnxyls.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yi.521024.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yk.huanxung.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lz.yuexingan06.cn

[B02] 多分支 else if / elif
来源：http://ok.szxytkj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yr.hahajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yt.nicolike.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wn.hahajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gq.gzmigu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mm.yuexingan06.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mb.asd995.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://sm.bjjhwx.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yj.hnjuh.cn

[B03] switch / match / case
来源：http://cx.shxzskj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://im.chemitech.net.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://us.nszjky.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wy.muxihuayi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nq.bookmarksfly.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gz.panjiajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hp.huixinmuqiang.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rl.huixiangedu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xl.bjjhwx.cn

[B04] for 计数循环
来源：http://sq.huanxung.cn

Py:   for i in range(10): print(i)
来源：http://dx.hahajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kt.shxzukj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vu.panjiajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rn.shxzukj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://di.huanxung.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lu.shxzukj.cn

Ruby: 10.times { |i| puts i }
来源：http://zp.bookmarksfly.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zp.nszjky.cn

[B05] 遍历数组 / 列表
来源：http://tp.huixiangedu.cn

Py:   for item in arr: print(item)
来源：http://dj.yuexingan06.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sb.shxzukj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hq.hnjuh.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tw.yuexingan06.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://mz.panjiajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tj.newstarts.cn

Ruby: arr.each { |item| puts item }
来源：http://ks.521024.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sn.lnxyls.cn

[B06] 遍历字典 / 对象
来源：http://xb.hahajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://bn.huanxung.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lq.521024.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ds.muxihuayi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qw.haigaiapp.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pw.gzmigu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sm.bookmarksfly.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://am.chemitech.net.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ss.bookmarksfly.cn

[B07] while 循环
来源：http://gp.chemitech.net.cn

Py:   while i < 10: i += 1
来源：http://lo.szxytkj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xo.panjiajie.cn

JS:   while (i < 10) { i++; }
来源：http://am.jianghongdianzi.cn

TS:   while (i < 10) { i++; }
来源：http://bn.newstarts.cn

Java: while (i < 10) { i++; }
来源：http://ml.shxzukj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dq.shtwfgs.cn

Ruby: while i < 10; i += 1; end
来源：http://cs.521024.cn

C#:   while (i < 10) { i++; }
来源：http://vs.yuntaijiaju.cn

[B08] do-while（至少执行一次）
来源：http://vj.yuntaijiaju.cn

Py:   # 无 do-while：用 while True + break
来源：http://kf.haigaiapp.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://np.9csxet.cn

JS:   do { i++; } while (i < 10);
来源：http://xb.hnjuh.cn

TS:   do { i++; } while (i < 10);
来源：http://iy.nszjky.cn

Java: do { i++; } while (i < 10);
来源：http://ig.lnxyls.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ph.gzmigu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://tz.colortex.cn

C#:   do { i++; } while (i < 10);
来源：http://ny.yuexingan06.cn

[B09] break 与 continue
来源：http://mm.hahajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zv.jctech888.com.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fj.huixinmuqiang.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gu.asd995.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ac.bjjhwx.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ku.huixinmuqiang.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cw.wgjwhj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vu.panjiajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vc.chemitech.net.cn

[B10] 遍历同时拿索引
来源：http://gb.bookmarksfly.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://st.jctech888.com.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uz.szsharing.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pt.nicolike.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://up.huixinmuqiang.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tq.bjjhwx.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gb.chemitech.net.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vv.lnxyls.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://li.9csxet.cn

[B11] 生成数字序列 / 区间
来源：http://vw.szsharing.cn

Py:   list(range(0, 10, 2))
来源：http://hv.shxzukj.cn

PHP:  range(0, 10, 2);
来源：http://yn.yuntaijiaju.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nj.huanxung.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vx.jianghongdianzi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ld.gzmigu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wh.muxihuayi.cn

Ruby: (0...10).step(2).to_a
来源：http://mh.jianghongdianzi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qc.bjjhwx.cn

[B12] 跳出多层循环
来源：http://fo.yuntaijiaju.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://uj.huixinmuqiang.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://nd.nicolike.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hf.jianghongdianzi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ba.jianghongdianzi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gg.szxytkj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://og.szsharing.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gq.muxihuayi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gn.panjiajie.cn

[B13] 判断是否为数字
来源：http://hz.shtwfgs.cn

Py:   isinstance(x, (int, float))
来源：http://xt.nicolike.cn

PHP:  is_numeric($x)
来源：http://dw.szsharing.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xx.lnxyls.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hi.yuntaijiaju.cn

Java: x instanceof Number
来源：http://sp.panjiajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wb.jianghongdianzi.cn

Ruby: x.is_a?(Numeric)
来源：http://xu.chemitech.net.cn

C#:   x is int or double or decimal
来源：http://lr.yuexingan06.cn

[B14] 判断值是否在集合内
来源：http://gz.nszjky.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jw.nszjky.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yn.huixinmuqiang.cn

JS:   [1, 2, 3].includes(x)
来源：http://ok.hahajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://vo.newstarts.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://bz.wgjwhj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mk.szsharing.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ft.gzmigu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qy.huanxung.cn

[B15] 布尔运算与取反
来源：http://rz.bjjhwx.cn

Py:   a and b or not c
来源：http://xn.huixiangedu.cn

PHP:  $a && $b || !$c
来源：http://md.szsharing.cn

JS:   a && b || !c
来源：http://os.colortex.cn

TS:   a && b || !c
来源：http://al.haigaiapp.cn

Java: a && b || !c
来源：http://zc.hahajie.cn

Go:   a && b || !c
来源：http://ij.panjiajie.cn

Ruby: a && b || !c
来源：http://og.newstarts.cn

C#:   a && b || !c
来源：http://cm.jctech888.com.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fn.521024.cn

Py:   if not data: return
来源：http://kz.muxihuayi.cn

PHP:  if (!$data) { return; }
来源：http://nw.521024.cn

JS:   if (!data) return;
来源：http://yp.nicolike.cn

TS:   if (!data) return;
来源：http://da.bookmarksfly.cn

Java: if (data == null) return;
来源：http://ky.wgjwhj.cn

Go:   if data == nil { return }
来源：http://zm.huixinmuqiang.cn

Ruby: return if data.nil?
来源：http://hp.shxzskj.cn

C#:   if (data == null) return;
来源：http://uc.huixinmuqiang.cn

================================================================================
来源：http://um.muxihuayi.cn

C. 函数与作用域
来源：http://bj.bookmarksfly.cn

================================================================================
来源：http://uz.shxzskj.cn

[C01] 定义函数
来源：http://ap.huixiangedu.cn

Py:   def add(a, b): return a + b
来源：http://rq.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ki.asd995.cn

JS:   function add(a, b) { return a + b; }
来源：http://yf.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pc.jianghongdianzi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vl.nicolike.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hv.shtwfgs.cn

Ruby: def add(a, b); a + b; end
来源：http://ku.panjiajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xg.wgjwhj.cn

[C02] 默认参数
来源：http://ge.huixiangedu.cn

Py:   def greet(name="World"): return name
来源：http://fq.colortex.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ia.huixinmuqiang.cn

JS:   function greet(name = "World") { return name; }
来源：http://xe.shtwfgs.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hh.jianghongdianzi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ew.bjjhwx.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://br.hahajie.cn

Ruby: def greet(name = "World") = name
来源：http://ni.yuntaijiaju.cn

C#:   string Greet(string name = "World") => name;
来源：http://jq.asd995.cn

[C03] 可变参数
来源：http://uw.shxzukj.cn

Py:   def total(*args): return sum(args)
来源：http://bp.bjjhwx.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mx.gzmigu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xf.huanxung.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fd.shxzukj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ek.hahajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://my.haigaiapp.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gv.asd995.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://li.colortex.cn

[C04] 命名参数 / 关键字参数
来源：http://af.colortex.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ld.gzmigu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://at.yuexingan06.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tu.yuntaijiaju.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kj.hnjuh.cn

Java: // 无：用 Builder 模式或 record
来源：http://mf.panjiajie.cn

Go:   // 无：用配置结构体参数
来源：http://xz.muxihuayi.cn

Ruby: f(a: 1, b: 2)
来源：http://js.jctech888.com.cn

C#:   f(a: 1, b: 2)
来源：http://xa.huanxung.cn

[C05] 返回多个值
来源：http://ka.hnjuh.cn

Py:   return a, b
来源：http://mo.jianghongdianzi.cn

PHP:  return [$a, $b];
来源：http://ic.9csxet.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://lm.bookmarksfly.cn

TS:   return { a, b };
来源：http://yk.huixinmuqiang.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zi.panjiajie.cn

Go:   return a, b
来源：http://ex.bjjhwx.cn

Ruby: return a, b
来源：http://ud.haigaiapp.cn

C#:   return (a, b);              // ValueTuple
来源：http://dc.nszjky.cn

[C06] 匿名函数 / lambda
来源：http://cn.jianghongdianzi.cn

Py:   square = lambda x: x * x
来源：http://bx.szxytkj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://px.panjiajie.cn

JS:   const square = x => x * x;
来源：http://gs.lnxyls.cn

TS:   const square = (x: number): number => x * x;
来源：http://ev.yuexingan06.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hn.panjiajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://em.lnxyls.cn

Ruby: square = ->(x) { x * x }
来源：http://ov.muxihuayi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fh.nszjky.cn

[C07] 把函数作为参数传入
来源：http://fn.chemitech.net.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://an.huixiangedu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://og.jianghongdianzi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tx.huanxung.cn

TS:   arr.map(String)
来源：http://yd.lnxyls.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yo.huixiangedu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zz.jctech888.com.cn

Ruby: arr.map(&:upcase)
来源：http://yp.bookmarksfly.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ui.9csxet.cn

[C08] 闭包
来源：http://md.shxzukj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ia.shxzskj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sh.asd995.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cj.huixiangedu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jn.gzmigu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://if.shxzskj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kg.hahajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dh.shxzukj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kj.huanxung.cn

[C09] 递归
来源：http://wb.chemitech.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dn.huixiangedu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ns.gzmigu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ac.bjjhwx.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wr.haigaiapp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ew.jctech888.com.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://oi.muxihuayi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gq.nicolike.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jj.haigaiapp.cn

[C10] 变量作用域
来源：http://gq.szxytkj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ef.shtwfgs.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xo.shtwfgs.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://so.jctech888.com.cn

TS:   同 JS
来源：http://bn.huixiangedu.cn

Java: 方法内为块级作用域
来源：http://vd.lnxyls.cn

Go:   花括号块级作用域
来源：http://po.shtwfgs.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ci.huixinmuqiang.cn

C#:   块级作用域
来源：http://bm.yuexingan06.cn

[C11] 模块导入与导出
来源：http://xk.jianghongdianzi.cn

Py:   from module import func
来源：http://ze.bjjhwx.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ij.huanxung.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://yc.yuntaijiaju.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cx.huixiangedu.cn

Java: import java.util.List;
来源：http://pz.yuexingan06.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ey.gzmigu.cn

Ruby: require "json"; require_relative "./util"
来源：http://cj.gzmigu.cn

C#:   using System.Text;
来源：http://vd.521024.cn

[C12] 立即执行函数 IIFE
来源：http://id.bjjhwx.cn

Py:   (lambda: print("run"))()
来源：http://pl.521024.cn

PHP:  (function () { echo "run"; })();
来源：http://lj.muxihuayi.cn

JS:   (() => { console.log("run"); })();
来源：http://zm.shxzukj.cn

TS:   (() => { console.log("run"); })();
来源：http://do.huanxung.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lb.huixiangedu.cn

Go:   func() { fmt.Println("run") }()
来源：http://tw.yuexingan06.cn

Ruby: -> { puts "run" }.call
来源：http://ub.yuexingan06.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://og.521024.cn

[C13] 类型声明 / 类型注解
来源：http://tn.shxzskj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dd.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kn.huixinmuqiang.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hu.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mt.521024.cn

Java: int add(int a, int b) { return a + b; }
来源：http://rp.huanxung.cn

Go:   func add(a, b int) int
来源：http://ni.hnjuh.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dg.asd995.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ti.huixiangedu.cn

[C14] 泛型函数
来源：http://fz.chemitech.net.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vu.szsharing.cn

PHP:  // 无泛型
来源：http://qr.bookmarksfly.cn

JS:   // 无泛型
来源：http://kx.lnxyls.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mr.haigaiapp.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tx.521024.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://re.asd995.cn

Ruby: # 无泛型
来源：http://jr.huixiangedu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mp.panjiajie.cn

[C15] 解构 / 展开参数
来源：http://cy.huixinmuqiang.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ad.bookmarksfly.cn

PHP:  [$a, $b] = $pair;
来源：http://xj.shxzskj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hj.colortex.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pa.shxzukj.cn

Java: // 无解构
来源：http://un.shxzskj.cn

Go:   // 无解构
来源：http://jj.huixiangedu.cn

Ruby: a, b = pair
来源：http://sg.521024.cn

C#:   var (a, b) = pair;
来源：http://qi.yuexingan06.cn

[C16] 函数 / 方法重载
来源：http://fo.shxzukj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hl.521024.cn

PHP:  // 无重载
来源：http://kt.jianghongdianzi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://px.huixinmuqiang.cn

TS:   // 用联合类型或重载签名声明
来源：http://hc.chemitech.net.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ge.huixiangedu.cn

Go:   // 无重载：用不同函数名
来源：http://oo.hahajie.cn

Ruby: # 无重载：靠动态参数
来源：http://hk.szxytkj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://id.lnxyls.cn

================================================================================
来源：http://ze.jctech888.com.cn

D. 数组 / 列表 / 集合
来源：http://ki.asd995.cn

================================================================================
来源：http://fy.nszjky.cn

[D01] 创建数组 / 列表
来源：http://tl.colortex.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pu.yuntaijiaju.cn


<!-- 参考信息 -->