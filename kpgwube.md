代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zx.nicolike.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ou.huixinmuqiang.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://oy.newstarts.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wh.asd995.cn

[A26] 类型转换总览
来源：http://ys.asd995.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mu.nszjky.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yh.wgjwhj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hi.panjiajie.cn

TS:   Number() String() Boolean() x as number
来源：http://kt.9csxet.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dz.bjjhwx.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rs.yuntaijiaju.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://hd.huanxung.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ut.asd995.cn

================================================================================
来源：http://bo.9csxet.cn

B. 流程控制
来源：http://mm.haigaiapp.cn

================================================================================
来源：http://be.szxytkj.cn

[B01] 条件判断 if / else
来源：http://op.panjiajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://zy.huixinmuqiang.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cm.lnxyls.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ns.asd995.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rd.asd995.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://by.lnxyls.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rt.nicolike.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qm.chemitech.net.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cs.nszjky.cn

[B02] 多分支 else if / elif
来源：http://px.haigaiapp.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qu.bjjhwx.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://aj.newstarts.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nm.muxihuayi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ko.521024.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pq.nicolike.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://iz.bookmarksfly.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zp.muxihuayi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jz.wgjwhj.cn

[B03] switch / match / case
来源：http://jh.521024.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wb.shtwfgs.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gg.lnxyls.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://om.shtwfgs.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vz.bjjhwx.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ru.gzmigu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jc.asd995.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wg.newstarts.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ds.9csxet.cn

[B04] for 计数循环
来源：http://oq.jctech888.com.cn

Py:   for i in range(10): print(i)
来源：http://za.bookmarksfly.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yf.gzmigu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vk.shxzukj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dc.wgjwhj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bm.shxzskj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lu.wgjwhj.cn

Ruby: 10.times { |i| puts i }
来源：http://td.szsharing.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://eg.bjjhwx.cn

[B05] 遍历数组 / 列表
来源：http://mq.newstarts.cn

Py:   for item in arr: print(item)
来源：http://ww.huanxung.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zt.nicolike.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://vw.nszjky.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ng.panjiajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jm.shxzskj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ar.wgjwhj.cn

Ruby: arr.each { |item| puts item }
来源：http://ib.panjiajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hc.bookmarksfly.cn

[B06] 遍历字典 / 对象
来源：http://wn.panjiajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://uu.muxihuayi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bc.521024.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sr.nicolike.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zt.hahajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jv.521024.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ue.yuexingan06.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ec.asd995.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fh.nicolike.cn

[B07] while 循环
来源：http://vl.bookmarksfly.cn

Py:   while i < 10: i += 1
来源：http://yc.hahajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bu.shtwfgs.cn

JS:   while (i < 10) { i++; }
来源：http://hv.hahajie.cn

TS:   while (i < 10) { i++; }
来源：http://nu.521024.cn

Java: while (i < 10) { i++; }
来源：http://ij.szsharing.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zv.yuexingan06.cn

Ruby: while i < 10; i += 1; end
来源：http://vv.jctech888.com.cn

C#:   while (i < 10) { i++; }
来源：http://nb.shxzskj.cn

[B08] do-while（至少执行一次）
来源：http://sf.muxihuayi.cn

Py:   # 无 do-while：用 while True + break
来源：http://hg.nicolike.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://hy.haigaiapp.cn

JS:   do { i++; } while (i < 10);
来源：http://oe.lnxyls.cn

TS:   do { i++; } while (i < 10);
来源：http://un.gzmigu.cn

Java: do { i++; } while (i < 10);
来源：http://ac.yuntaijiaju.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gq.nicolike.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rw.jctech888.com.cn

C#:   do { i++; } while (i < 10);
来源：http://ga.huanxung.cn

[B09] break 与 continue
来源：http://dh.colortex.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nr.bookmarksfly.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wb.bjjhwx.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ke.jianghongdianzi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pf.hnjuh.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xm.9csxet.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zm.shxzskj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ff.chemitech.net.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rc.lnxyls.cn

[B10] 遍历同时拿索引
来源：http://rv.muxihuayi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ty.shxzukj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xw.hahajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fd.wgjwhj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ov.hahajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://iy.bookmarksfly.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yd.asd995.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kc.haigaiapp.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://no.haigaiapp.cn

[B11] 生成数字序列 / 区间
来源：http://sn.panjiajie.cn

Py:   list(range(0, 10, 2))
来源：http://xs.yuntaijiaju.cn

PHP:  range(0, 10, 2);
来源：http://km.lnxyls.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://je.9csxet.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sh.shtwfgs.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://iv.wgjwhj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gk.yuntaijiaju.cn

Ruby: (0...10).step(2).to_a
来源：http://hp.huanxung.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://iq.huixinmuqiang.cn

[B12] 跳出多层循环
来源：http://mt.bjjhwx.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://cm.chemitech.net.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fe.yuntaijiaju.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zo.nszjky.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lu.huanxung.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ow.9csxet.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yf.huanxung.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jk.szsharing.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.szxytkj.cn

[B13] 判断是否为数字
来源：http://lp.huixinmuqiang.cn

Py:   isinstance(x, (int, float))
来源：http://rf.bjjhwx.cn

PHP:  is_numeric($x)
来源：http://lh.colortex.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yb.jctech888.com.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oh.szsharing.cn

Java: x instanceof Number
来源：http://ve.lnxyls.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kj.huixinmuqiang.cn

Ruby: x.is_a?(Numeric)
来源：http://gp.huanxung.cn

C#:   x is int or double or decimal
来源：http://dc.gzmigu.cn

[B14] 判断值是否在集合内
来源：http://vo.shxzskj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qd.asd995.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gi.shxzskj.cn

JS:   [1, 2, 3].includes(x)
来源：http://tq.asd995.cn

TS:   [1, 2, 3].includes(x)
来源：http://ac.lnxyls.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ik.bookmarksfly.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dn.muxihuayi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gm.jctech888.com.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://eo.nicolike.cn

[B15] 布尔运算与取反
来源：http://cw.nszjky.cn

Py:   a and b or not c
来源：http://fs.bjjhwx.cn

PHP:  $a && $b || !$c
来源：http://sn.chemitech.net.cn

JS:   a && b || !c
来源：http://rl.9csxet.cn

TS:   a && b || !c
来源：http://cw.jctech888.com.cn

Java: a && b || !c
来源：http://pk.asd995.cn

Go:   a && b || !c
来源：http://fg.shxzskj.cn

Ruby: a && b || !c
来源：http://sm.panjiajie.cn

C#:   a && b || !c
来源：http://xg.lnxyls.cn

[B16] 卫语句：不满足条件提前返回
来源：http://da.521024.cn

Py:   if not data: return
来源：http://tw.haigaiapp.cn

PHP:  if (!$data) { return; }
来源：http://ko.9csxet.cn

JS:   if (!data) return;
来源：http://am.yuexingan06.cn

TS:   if (!data) return;
来源：http://xq.lnxyls.cn

Java: if (data == null) return;
来源：http://yf.asd995.cn

Go:   if data == nil { return }
来源：http://zn.muxihuayi.cn

Ruby: return if data.nil?
来源：http://hs.huixiangedu.cn

C#:   if (data == null) return;
来源：http://iu.lnxyls.cn

================================================================================
来源：http://ny.lnxyls.cn

C. 函数与作用域
来源：http://mj.yuntaijiaju.cn

================================================================================
来源：http://qu.521024.cn

[C01] 定义函数
来源：http://oq.szxytkj.cn

Py:   def add(a, b): return a + b
来源：http://na.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yf.jianghongdianzi.cn

JS:   function add(a, b) { return a + b; }
来源：http://nt.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yk.hnjuh.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://kh.9csxet.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jx.jctech888.com.cn

Ruby: def add(a, b); a + b; end
来源：http://mt.bjjhwx.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tz.muxihuayi.cn

[C02] 默认参数
来源：http://zz.huixiangedu.cn

Py:   def greet(name="World"): return name
来源：http://sc.nszjky.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tt.9csxet.cn

JS:   function greet(name = "World") { return name; }
来源：http://qi.nszjky.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://jt.hnjuh.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dd.newstarts.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jc.asd995.cn

Ruby: def greet(name = "World") = name
来源：http://xa.colortex.cn

C#:   string Greet(string name = "World") => name;
来源：http://yg.muxihuayi.cn

[C03] 可变参数
来源：http://xq.huixiangedu.cn

Py:   def total(*args): return sum(args)
来源：http://sn.haigaiapp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ta.asd995.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nt.hahajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cu.bookmarksfly.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ob.hnjuh.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gj.hnjuh.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yt.hnjuh.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://us.muxihuayi.cn

[C04] 命名参数 / 关键字参数
来源：http://ue.yuexingan06.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xj.shxzukj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fd.shxzukj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pd.521024.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sv.chemitech.net.cn

Java: // 无：用 Builder 模式或 record
来源：http://nq.newstarts.cn

Go:   // 无：用配置结构体参数
来源：http://wx.lnxyls.cn

Ruby: f(a: 1, b: 2)
来源：http://di.hnjuh.cn

C#:   f(a: 1, b: 2)
来源：http://yk.shtwfgs.cn

[C05] 返回多个值
来源：http://mr.yuntaijiaju.cn

Py:   return a, b
来源：http://sr.bookmarksfly.cn

PHP:  return [$a, $b];
来源：http://yc.jianghongdianzi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://gk.521024.cn

TS:   return { a, b };
来源：http://jx.asd995.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zx.colortex.cn

Go:   return a, b
来源：http://jk.yuexingan06.cn

Ruby: return a, b
来源：http://aj.shxzskj.cn

C#:   return (a, b);              // ValueTuple
来源：http://xo.szxytkj.cn

[C06] 匿名函数 / lambda
来源：http://ln.yuntaijiaju.cn

Py:   square = lambda x: x * x
来源：http://ei.lnxyls.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://lg.jianghongdianzi.cn

JS:   const square = x => x * x;
来源：http://ei.shtwfgs.cn

TS:   const square = (x: number): number => x * x;
来源：http://qm.chemitech.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kb.521024.cn

Go:   sq := func(x int) int { return x * x }
来源：http://tr.chemitech.net.cn

Ruby: square = ->(x) { x * x }
来源：http://ks.hnjuh.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ky.bookmarksfly.cn

[C07] 把函数作为参数传入
来源：http://hk.asd995.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dt.nicolike.cn

PHP:  array_map("strtoupper", $arr);
来源：http://qh.colortex.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://of.haigaiapp.cn

TS:   arr.map(String)
来源：http://zo.521024.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ha.huixinmuqiang.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vr.9csxet.cn

Ruby: arr.map(&:upcase)
来源：http://nz.gzmigu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://es.newstarts.cn

[C08] 闭包
来源：http://je.9csxet.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bd.shtwfgs.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xr.bjjhwx.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ur.huixiangedu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qn.szxytkj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bi.asd995.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ix.shxzukj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ef.shtwfgs.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xa.muxihuayi.cn

[C09] 递归
来源：http://hu.haigaiapp.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fd.wgjwhj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mw.yuexingan06.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ni.huixinmuqiang.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tc.colortex.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pi.asd995.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ot.newstarts.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://eg.muxihuayi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wi.521024.cn

[C10] 变量作用域
来源：http://wl.lnxyls.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kz.jctech888.com.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kj.lnxyls.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ok.jctech888.com.cn

TS:   同 JS
来源：http://qi.colortex.cn

Java: 方法内为块级作用域
来源：http://ar.521024.cn

Go:   花括号块级作用域
来源：http://yp.hnjuh.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bc.lnxyls.cn

C#:   块级作用域
来源：http://py.huixiangedu.cn

[C11] 模块导入与导出
来源：http://on.szsharing.cn

Py:   from module import func
来源：http://hz.nszjky.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://uh.haigaiapp.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ai.9csxet.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ys.shxzukj.cn

Java: import java.util.List;
来源：http://xy.muxihuayi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cx.szxytkj.cn

Ruby: require "json"; require_relative "./util"
来源：http://fm.asd995.cn

C#:   using System.Text;
来源：http://ql.panjiajie.cn

[C12] 立即执行函数 IIFE
来源：http://pm.nicolike.cn

Py:   (lambda: print("run"))()
来源：http://yf.yuexingan06.cn

PHP:  (function () { echo "run"; })();
来源：http://sq.shxzskj.cn

JS:   (() => { console.log("run"); })();
来源：http://rr.bookmarksfly.cn

TS:   (() => { console.log("run"); })();
来源：http://yd.nszjky.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vb.jianghongdianzi.cn

Go:   func() { fmt.Println("run") }()
来源：http://um.huixiangedu.cn

Ruby: -> { puts "run" }.call
来源：http://ib.panjiajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ll.hnjuh.cn

[C13] 类型声明 / 类型注解
来源：http://cc.jctech888.com.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bi.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yk.gzmigu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vd.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dj.hnjuh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://df.haigaiapp.cn

Go:   func add(a, b int) int
来源：http://au.yuexingan06.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://oi.colortex.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mz.colortex.cn

[C14] 泛型函数
来源：http://tx.huixiangedu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yt.huixiangedu.cn

PHP:  // 无泛型
来源：http://vi.9csxet.cn

JS:   // 无泛型
来源：http://zp.hahajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lr.yuntaijiaju.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qj.wgjwhj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ld.muxihuayi.cn

Ruby: # 无泛型
来源：http://cd.jianghongdianzi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yq.newstarts.cn

[C15] 解构 / 展开参数
来源：http://oa.yuntaijiaju.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mh.jianghongdianzi.cn

PHP:  [$a, $b] = $pair;
来源：http://gr.szxytkj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ep.shxzskj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hy.newstarts.cn

Java: // 无解构
来源：http://mj.shxzukj.cn

Go:   // 无解构
来源：http://qy.colortex.cn

Ruby: a, b = pair
来源：http://ie.gzmigu.cn

C#:   var (a, b) = pair;
来源：http://ww.nicolike.cn

[C16] 函数 / 方法重载
来源：http://ee.huixinmuqiang.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ig.bjjhwx.cn


<!-- 参考信息 -->