代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://xt.szsharing.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://at.hahajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ct.bjjhwx.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rq.yuexingan06.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xz.huixinmuqiang.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xx.lnxyls.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hv.huanxung.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wk.wgjwhj.cn

[A26] 类型转换总览
来源：http://dm.wgjwhj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://di.nszjky.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tm.chemitech.net.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pe.szsharing.cn

TS:   Number() String() Boolean() x as number
来源：http://ln.haigaiapp.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nc.szsharing.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://uc.yuexingan06.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zy.panjiajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wk.bookmarksfly.cn

================================================================================
来源：http://vm.nszjky.cn

B. 流程控制
来源：http://fs.asd995.cn

================================================================================
来源：http://eg.shxzskj.cn

[B01] 条件判断 if / else
来源：http://yt.yuexingan06.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://tn.huixiangedu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mh.panjiajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ay.muxihuayi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lo.yuntaijiaju.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://fs.yuexingan06.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wz.shxzukj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://iv.nicolike.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fu.wgjwhj.cn

[B02] 多分支 else if / elif
来源：http://cz.chemitech.net.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jp.hahajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hs.wgjwhj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ik.shxzskj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nr.9csxet.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lv.shxzukj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qy.szsharing.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wh.lnxyls.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xe.9csxet.cn

[B03] switch / match / case
来源：http://hh.bookmarksfly.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://aw.521024.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://if.jctech888.com.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nu.yuntaijiaju.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ja.jianghongdianzi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dw.yuntaijiaju.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xk.jctech888.com.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zi.newstarts.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mh.shxzskj.cn

[B04] for 计数循环
来源：http://ea.haigaiapp.cn

Py:   for i in range(10): print(i)
来源：http://oj.huixiangedu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://va.panjiajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bi.nicolike.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bk.wgjwhj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kx.panjiajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fc.yuntaijiaju.cn

Ruby: 10.times { |i| puts i }
来源：http://ua.haigaiapp.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vm.gzmigu.cn

[B05] 遍历数组 / 列表
来源：http://zg.szxytkj.cn

Py:   for item in arr: print(item)
来源：http://nf.szsharing.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jr.bookmarksfly.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yi.nicolike.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://hm.jianghongdianzi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pj.colortex.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gj.huanxung.cn

Ruby: arr.each { |item| puts item }
来源：http://eb.huixiangedu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gy.bookmarksfly.cn

[B06] 遍历字典 / 对象
来源：http://dw.bookmarksfly.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://lt.muxihuayi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vf.chemitech.net.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pc.panjiajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wi.huixiangedu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tb.newstarts.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ys.lnxyls.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yt.szsharing.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://du.lnxyls.cn

[B07] while 循环
来源：http://gx.bookmarksfly.cn

Py:   while i < 10: i += 1
来源：http://xp.gzmigu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://jk.nicolike.cn

JS:   while (i < 10) { i++; }
来源：http://xh.shxzskj.cn

TS:   while (i < 10) { i++; }
来源：http://ki.muxihuayi.cn

Java: while (i < 10) { i++; }
来源：http://vu.huixiangedu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bz.gzmigu.cn

Ruby: while i < 10; i += 1; end
来源：http://yq.asd995.cn

C#:   while (i < 10) { i++; }
来源：http://rr.lnxyls.cn

[B08] do-while（至少执行一次）
来源：http://kp.bjjhwx.cn

Py:   # 无 do-while：用 while True + break
来源：http://ub.huixinmuqiang.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xi.bookmarksfly.cn

JS:   do { i++; } while (i < 10);
来源：http://kd.nszjky.cn

TS:   do { i++; } while (i < 10);
来源：http://hx.bjjhwx.cn

Java: do { i++; } while (i < 10);
来源：http://ms.yuntaijiaju.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://we.asd995.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jr.wgjwhj.cn

C#:   do { i++; } while (i < 10);
来源：http://ke.bookmarksfly.cn

[B09] break 与 continue
来源：http://mz.bjjhwx.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://be.gzmigu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vt.shxzukj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://np.jctech888.com.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://du.wgjwhj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pc.9csxet.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bc.shxzskj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lb.yuntaijiaju.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dq.chemitech.net.cn

[B10] 遍历同时拿索引
来源：http://vz.newstarts.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sj.shxzskj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sx.shxzskj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rn.panjiajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jb.chemitech.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wt.chemitech.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wi.shxzukj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qo.newstarts.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kg.shtwfgs.cn

[B11] 生成数字序列 / 区间
来源：http://gh.muxihuayi.cn

Py:   list(range(0, 10, 2))
来源：http://rc.chemitech.net.cn

PHP:  range(0, 10, 2);
来源：http://dr.bjjhwx.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nx.huixinmuqiang.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sw.colortex.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ho.shtwfgs.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wm.yuexingan06.cn

Ruby: (0...10).step(2).to_a
来源：http://sl.521024.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pu.szsharing.cn

[B12] 跳出多层循环
来源：http://in.panjiajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bb.muxihuayi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://im.colortex.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lo.gzmigu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gt.bookmarksfly.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://al.panjiajie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gc.hnjuh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qn.huixiangedu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://oq.521024.cn

[B13] 判断是否为数字
来源：http://nr.hnjuh.cn

Py:   isinstance(x, (int, float))
来源：http://tl.huixiangedu.cn

PHP:  is_numeric($x)
来源：http://ru.bookmarksfly.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iy.muxihuayi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cm.jctech888.com.cn

Java: x instanceof Number
来源：http://ma.huanxung.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://md.szxytkj.cn

Ruby: x.is_a?(Numeric)
来源：http://cq.colortex.cn

C#:   x is int or double or decimal
来源：http://qa.colortex.cn

[B14] 判断值是否在集合内
来源：http://dn.yuntaijiaju.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yx.shxzukj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://so.huixiangedu.cn

JS:   [1, 2, 3].includes(x)
来源：http://lq.szsharing.cn

TS:   [1, 2, 3].includes(x)
来源：http://cc.szxytkj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://au.hahajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jn.jctech888.com.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jd.shxzskj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gv.wgjwhj.cn

[B15] 布尔运算与取反
来源：http://de.muxihuayi.cn

Py:   a and b or not c
来源：http://qv.shtwfgs.cn

PHP:  $a && $b || !$c
来源：http://at.huixiangedu.cn

JS:   a && b || !c
来源：http://ew.huanxung.cn

TS:   a && b || !c
来源：http://gj.jianghongdianzi.cn

Java: a && b || !c
来源：http://un.huixiangedu.cn

Go:   a && b || !c
来源：http://pm.newstarts.cn

Ruby: a && b || !c
来源：http://rm.asd995.cn

C#:   a && b || !c
来源：http://gi.huixinmuqiang.cn

[B16] 卫语句：不满足条件提前返回
来源：http://an.asd995.cn

Py:   if not data: return
来源：http://hf.huixiangedu.cn

PHP:  if (!$data) { return; }
来源：http://cu.chemitech.net.cn

JS:   if (!data) return;
来源：http://jv.jianghongdianzi.cn

TS:   if (!data) return;
来源：http://uc.jianghongdianzi.cn

Java: if (data == null) return;
来源：http://zs.9csxet.cn

Go:   if data == nil { return }
来源：http://yx.gzmigu.cn

Ruby: return if data.nil?
来源：http://dv.chemitech.net.cn

C#:   if (data == null) return;
来源：http://og.szxytkj.cn

================================================================================
来源：http://nx.haigaiapp.cn

C. 函数与作用域
来源：http://wm.nicolike.cn

================================================================================
来源：http://gq.asd995.cn

[C01] 定义函数
来源：http://qf.nszjky.cn

Py:   def add(a, b): return a + b
来源：http://vn.hahajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zc.gzmigu.cn

JS:   function add(a, b) { return a + b; }
来源：http://jb.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bp.9csxet.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://np.newstarts.cn

Go:   func add(a, b int) int { return a + b }
来源：http://nf.nicolike.cn

Ruby: def add(a, b); a + b; end
来源：http://px.shtwfgs.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lp.shxzukj.cn

[C02] 默认参数
来源：http://pq.521024.cn

Py:   def greet(name="World"): return name
来源：http://xx.wgjwhj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qd.panjiajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://xq.szxytkj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xr.521024.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ow.szxytkj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://oq.huixinmuqiang.cn

Ruby: def greet(name = "World") = name
来源：http://hq.hnjuh.cn

C#:   string Greet(string name = "World") => name;
来源：http://sj.lnxyls.cn

[C03] 可变参数
来源：http://jv.shxzukj.cn

Py:   def total(*args): return sum(args)
来源：http://yx.muxihuayi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xp.panjiajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mz.newstarts.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://oa.huixiangedu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qa.panjiajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tk.shtwfgs.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tr.yuexingan06.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ax.shtwfgs.cn

[C04] 命名参数 / 关键字参数
来源：http://jh.szsharing.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yg.huixiangedu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hb.chemitech.net.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kf.huanxung.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yp.gzmigu.cn

Java: // 无：用 Builder 模式或 record
来源：http://qg.yuntaijiaju.cn

Go:   // 无：用配置结构体参数
来源：http://zd.yuexingan06.cn

Ruby: f(a: 1, b: 2)
来源：http://ec.shxzskj.cn

C#:   f(a: 1, b: 2)
来源：http://ff.bjjhwx.cn

[C05] 返回多个值
来源：http://gs.nszjky.cn

Py:   return a, b
来源：http://zk.bookmarksfly.cn

PHP:  return [$a, $b];
来源：http://qw.chemitech.net.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://uz.shtwfgs.cn

TS:   return { a, b };
来源：http://jq.shxzskj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nl.szsharing.cn

Go:   return a, b
来源：http://gn.panjiajie.cn

Ruby: return a, b
来源：http://lp.huixiangedu.cn

C#:   return (a, b);              // ValueTuple
来源：http://ug.nszjky.cn

[C06] 匿名函数 / lambda
来源：http://mc.jctech888.com.cn

Py:   square = lambda x: x * x
来源：http://zi.9csxet.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wa.panjiajie.cn

JS:   const square = x => x * x;
来源：http://pt.newstarts.cn

TS:   const square = (x: number): number => x * x;
来源：http://xm.gzmigu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://oj.jianghongdianzi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zi.shtwfgs.cn

Ruby: square = ->(x) { x * x }
来源：http://nc.huixinmuqiang.cn

C#:   Func<int, int> square = x => x * x;
来源：http://oi.asd995.cn

[C07] 把函数作为参数传入
来源：http://ji.bjjhwx.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jr.asd995.cn

PHP:  array_map("strtoupper", $arr);
来源：http://tv.yuexingan06.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://oq.huixinmuqiang.cn

TS:   arr.map(String)
来源：http://mj.huanxung.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vc.asd995.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mr.szxytkj.cn

Ruby: arr.map(&:upcase)
来源：http://ba.muxihuayi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ng.panjiajie.cn

[C08] 闭包
来源：http://sz.gzmigu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mk.shxzukj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qx.asd995.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hv.huanxung.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gl.nicolike.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tm.chemitech.net.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wk.gzmigu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cl.chemitech.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tl.yuntaijiaju.cn

[C09] 递归
来源：http://yn.9csxet.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://to.9csxet.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ae.muxihuayi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cb.colortex.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kk.szxytkj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ib.asd995.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zo.gzmigu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rv.newstarts.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://aj.shtwfgs.cn

[C10] 变量作用域
来源：http://yc.colortex.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wd.muxihuayi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dv.jianghongdianzi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yg.bjjhwx.cn

TS:   同 JS
来源：http://yf.lnxyls.cn

Java: 方法内为块级作用域
来源：http://kz.szsharing.cn

Go:   花括号块级作用域
来源：http://zl.bookmarksfly.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ee.jianghongdianzi.cn

C#:   块级作用域
来源：http://so.bookmarksfly.cn

[C11] 模块导入与导出
来源：http://qp.szxytkj.cn

Py:   from module import func
来源：http://fk.gzmigu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vu.hnjuh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://dl.haigaiapp.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nq.panjiajie.cn

Java: import java.util.List;
来源：http://hf.shxzskj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mo.shxzskj.cn

Ruby: require "json"; require_relative "./util"
来源：http://kx.nicolike.cn

C#:   using System.Text;
来源：http://oi.chemitech.net.cn

[C12] 立即执行函数 IIFE
来源：http://iw.hnjuh.cn

Py:   (lambda: print("run"))()
来源：http://dl.shxzukj.cn

PHP:  (function () { echo "run"; })();
来源：http://gd.colortex.cn

JS:   (() => { console.log("run"); })();
来源：http://pn.chemitech.net.cn

TS:   (() => { console.log("run"); })();
来源：http://ty.nicolike.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rr.shtwfgs.cn

Go:   func() { fmt.Println("run") }()
来源：http://lv.colortex.cn

Ruby: -> { puts "run" }.call
来源：http://fz.huixiangedu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mu.nicolike.cn

[C13] 类型声明 / 类型注解
来源：http://dy.muxihuayi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zn.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cn.jctech888.com.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tg.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lp.shxzskj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://pt.asd995.cn

Go:   func add(a, b int) int
来源：http://dn.9csxet.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dn.haigaiapp.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qb.lnxyls.cn

[C14] 泛型函数
来源：http://ya.gzmigu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cy.szsharing.cn

PHP:  // 无泛型
来源：http://jq.bjjhwx.cn

JS:   // 无泛型
来源：http://dv.asd995.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ki.huanxung.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zg.haigaiapp.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lp.chemitech.net.cn

Ruby: # 无泛型
来源：http://ks.chemitech.net.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dw.colortex.cn

[C15] 解构 / 展开参数
来源：http://hx.wgjwhj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tl.nszjky.cn

PHP:  [$a, $b] = $pair;
来源：http://qb.huixiangedu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://oq.huixinmuqiang.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qx.jctech888.com.cn

Java: // 无解构
来源：http://cn.bookmarksfly.cn

Go:   // 无解构
来源：http://fo.szsharing.cn


<!-- 参考信息 -->