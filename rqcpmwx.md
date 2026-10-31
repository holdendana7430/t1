代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://uw.colortex.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zo.nszjky.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kq.panjiajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jr.szsharing.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://da.chemitech.net.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lj.9csxet.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://oc.lnxyls.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://un.asd995.cn

[A26] 类型转换总览
来源：http://lt.wgjwhj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://td.9csxet.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rt.yuexingan06.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sa.newstarts.cn

TS:   Number() String() Boolean() x as number
来源：http://hq.szsharing.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qu.nszjky.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://la.shtwfgs.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://bo.shxzukj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pd.yuexingan06.cn

================================================================================
来源：http://oj.newstarts.cn

B. 流程控制
来源：http://bp.hahajie.cn

================================================================================
来源：http://fc.521024.cn

[B01] 条件判断 if / else
来源：http://dv.nicolike.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://of.lnxyls.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ab.colortex.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zk.chemitech.net.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vb.9csxet.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xc.bjjhwx.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://sy.hahajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dr.yuexingan06.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://we.nicolike.cn

[B02] 多分支 else if / elif
来源：http://gz.wgjwhj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ne.asd995.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sb.wgjwhj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tu.bjjhwx.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mm.haigaiapp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qu.yuexingan06.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wg.lnxyls.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fz.szsharing.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pj.lnxyls.cn

[B03] switch / match / case
来源：http://ns.521024.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zy.wgjwhj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vi.huixiangedu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qd.huixinmuqiang.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zt.bjjhwx.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wd.bookmarksfly.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jk.nszjky.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zy.huixinmuqiang.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://aq.asd995.cn

[B04] for 计数循环
来源：http://ek.hahajie.cn

Py:   for i in range(10): print(i)
来源：http://bk.colortex.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vc.bjjhwx.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yz.9csxet.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ij.szsharing.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hu.szsharing.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mi.jctech888.com.cn

Ruby: 10.times { |i| puts i }
来源：http://ov.huanxung.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://io.jianghongdianzi.cn

[B05] 遍历数组 / 列表
来源：http://gx.bookmarksfly.cn

Py:   for item in arr: print(item)
来源：http://ki.yuexingan06.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dm.huixinmuqiang.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ct.shxzukj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bj.newstarts.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://rk.jianghongdianzi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jc.huixinmuqiang.cn

Ruby: arr.each { |item| puts item }
来源：http://qi.huanxung.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mu.newstarts.cn

[B06] 遍历字典 / 对象
来源：http://ue.lnxyls.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fg.shtwfgs.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ls.haigaiapp.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mq.haigaiapp.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://es.gzmigu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qv.wgjwhj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://et.asd995.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://is.bjjhwx.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qd.nicolike.cn

[B07] while 循环
来源：http://et.haigaiapp.cn

Py:   while i < 10: i += 1
来源：http://hi.newstarts.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qf.colortex.cn

JS:   while (i < 10) { i++; }
来源：http://ah.521024.cn

TS:   while (i < 10) { i++; }
来源：http://sf.nszjky.cn

Java: while (i < 10) { i++; }
来源：http://eh.huixiangedu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://my.szsharing.cn

Ruby: while i < 10; i += 1; end
来源：http://sr.hnjuh.cn

C#:   while (i < 10) { i++; }
来源：http://zs.9csxet.cn

[B08] do-while（至少执行一次）
来源：http://ik.chemitech.net.cn

Py:   # 无 do-while：用 while True + break
来源：http://xf.wgjwhj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://nd.shtwfgs.cn

JS:   do { i++; } while (i < 10);
来源：http://gf.shxzukj.cn

TS:   do { i++; } while (i < 10);
来源：http://gb.shxzskj.cn

Java: do { i++; } while (i < 10);
来源：http://fy.jctech888.com.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sh.chemitech.net.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ry.asd995.cn

C#:   do { i++; } while (i < 10);
来源：http://ux.huixiangedu.cn

[B09] break 与 continue
来源：http://os.huixinmuqiang.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tc.chemitech.net.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ro.asd995.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mw.jctech888.com.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lb.wgjwhj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ow.lnxyls.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://el.wgjwhj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://op.nicolike.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yl.huixinmuqiang.cn

[B10] 遍历同时拿索引
来源：http://ay.9csxet.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pj.yuexingan06.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qx.huanxung.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ze.shxzukj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nb.nicolike.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vj.huixiangedu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xs.colortex.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ct.yuexingan06.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lb.wgjwhj.cn

[B11] 生成数字序列 / 区间
来源：http://ke.szxytkj.cn

Py:   list(range(0, 10, 2))
来源：http://sj.gzmigu.cn

PHP:  range(0, 10, 2);
来源：http://hr.panjiajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ru.jctech888.com.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://of.asd995.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://iv.panjiajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cd.gzmigu.cn

Ruby: (0...10).step(2).to_a
来源：http://et.shxzukj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zm.hahajie.cn

[B12] 跳出多层循环
来源：http://pp.huanxung.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://el.szxytkj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://au.szxytkj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rh.asd995.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tg.bjjhwx.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ko.huixinmuqiang.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cv.nszjky.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wi.shxzskj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wv.gzmigu.cn

[B13] 判断是否为数字
来源：http://or.jianghongdianzi.cn

Py:   isinstance(x, (int, float))
来源：http://vh.huanxung.cn

PHP:  is_numeric($x)
来源：http://xp.huixinmuqiang.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://is.muxihuayi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gh.nicolike.cn

Java: x instanceof Number
来源：http://bb.shxzukj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qn.yuntaijiaju.cn

Ruby: x.is_a?(Numeric)
来源：http://ic.shxzukj.cn

C#:   x is int or double or decimal
来源：http://jb.hnjuh.cn

[B14] 判断值是否在集合内
来源：http://xz.szsharing.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nj.szsharing.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lc.nszjky.cn

JS:   [1, 2, 3].includes(x)
来源：http://wz.shtwfgs.cn

TS:   [1, 2, 3].includes(x)
来源：http://in.panjiajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://il.521024.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jt.shtwfgs.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gt.jianghongdianzi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://eb.jctech888.com.cn

[B15] 布尔运算与取反
来源：http://vn.huixinmuqiang.cn

Py:   a and b or not c
来源：http://gx.jianghongdianzi.cn

PHP:  $a && $b || !$c
来源：http://fe.521024.cn

JS:   a && b || !c
来源：http://gw.shxzskj.cn

TS:   a && b || !c
来源：http://zm.newstarts.cn

Java: a && b || !c
来源：http://xq.nszjky.cn

Go:   a && b || !c
来源：http://xm.nszjky.cn

Ruby: a && b || !c
来源：http://gu.bjjhwx.cn

C#:   a && b || !c
来源：http://vw.newstarts.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vn.nszjky.cn

Py:   if not data: return
来源：http://vq.szxytkj.cn

PHP:  if (!$data) { return; }
来源：http://kv.newstarts.cn

JS:   if (!data) return;
来源：http://ju.newstarts.cn

TS:   if (!data) return;
来源：http://sk.szsharing.cn

Java: if (data == null) return;
来源：http://eg.wgjwhj.cn

Go:   if data == nil { return }
来源：http://os.gzmigu.cn

Ruby: return if data.nil?
来源：http://fi.9csxet.cn

C#:   if (data == null) return;
来源：http://le.jianghongdianzi.cn

================================================================================
来源：http://ky.huixinmuqiang.cn

C. 函数与作用域
来源：http://at.bookmarksfly.cn

================================================================================
来源：http://dl.huixinmuqiang.cn

[C01] 定义函数
来源：http://xk.shtwfgs.cn

Py:   def add(a, b): return a + b
来源：http://nd.hahajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dm.nicolike.cn

JS:   function add(a, b) { return a + b; }
来源：http://dj.szxytkj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://su.muxihuayi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://iy.chemitech.net.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hq.shxzukj.cn

Ruby: def add(a, b); a + b; end
来源：http://dy.chemitech.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://py.newstarts.cn

[C02] 默认参数
来源：http://xk.bjjhwx.cn

Py:   def greet(name="World"): return name
来源：http://pm.haigaiapp.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://sa.haigaiapp.cn

JS:   function greet(name = "World") { return name; }
来源：http://xr.yuntaijiaju.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lv.panjiajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://eg.jctech888.com.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ql.bjjhwx.cn

Ruby: def greet(name = "World") = name
来源：http://fx.521024.cn

C#:   string Greet(string name = "World") => name;
来源：http://rc.9csxet.cn

[C03] 可变参数
来源：http://db.jctech888.com.cn

Py:   def total(*args): return sum(args)
来源：http://et.jianghongdianzi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ko.jianghongdianzi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://uw.huixinmuqiang.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xt.panjiajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://oc.wgjwhj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yr.muxihuayi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yd.asd995.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mf.yuexingan06.cn

[C04] 命名参数 / 关键字参数
来源：http://sn.gzmigu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jo.szxytkj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qa.haigaiapp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zv.muxihuayi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ii.yuntaijiaju.cn

Java: // 无：用 Builder 模式或 record
来源：http://kl.9csxet.cn

Go:   // 无：用配置结构体参数
来源：http://lu.nicolike.cn

Ruby: f(a: 1, b: 2)
来源：http://jh.shxzukj.cn

C#:   f(a: 1, b: 2)
来源：http://zn.bjjhwx.cn

[C05] 返回多个值
来源：http://aj.shxzskj.cn

Py:   return a, b
来源：http://af.jctech888.com.cn

PHP:  return [$a, $b];
来源：http://dk.jianghongdianzi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://hj.hnjuh.cn

TS:   return { a, b };
来源：http://sf.colortex.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jx.yuntaijiaju.cn

Go:   return a, b
来源：http://bv.hahajie.cn

Ruby: return a, b
来源：http://ms.bookmarksfly.cn

C#:   return (a, b);              // ValueTuple
来源：http://dx.wgjwhj.cn

[C06] 匿名函数 / lambda
来源：http://if.nicolike.cn

Py:   square = lambda x: x * x
来源：http://od.bookmarksfly.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://th.jianghongdianzi.cn

JS:   const square = x => x * x;
来源：http://cx.521024.cn

TS:   const square = (x: number): number => x * x;
来源：http://tr.jianghongdianzi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ul.shtwfgs.cn

Go:   sq := func(x int) int { return x * x }
来源：http://en.newstarts.cn

Ruby: square = ->(x) { x * x }
来源：http://qd.huanxung.cn

C#:   Func<int, int> square = x => x * x;
来源：http://vy.asd995.cn

[C07] 把函数作为参数传入
来源：http://wf.jctech888.com.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://po.521024.cn

PHP:  array_map("strtoupper", $arr);
来源：http://dn.9csxet.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lz.haigaiapp.cn

TS:   arr.map(String)
来源：http://wj.huixiangedu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ej.nszjky.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rp.lnxyls.cn

Ruby: arr.map(&:upcase)
来源：http://pa.jianghongdianzi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://dr.bookmarksfly.cn

[C08] 闭包
来源：http://gc.bookmarksfly.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kt.shxzskj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kb.shxzskj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zx.panjiajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qb.huanxung.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lo.nszjky.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zf.szxytkj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nk.yuexingan06.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ab.9csxet.cn

[C09] 递归
来源：http://he.colortex.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fp.jianghongdianzi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ok.shxzskj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bz.521024.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hu.lnxyls.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://if.shxzukj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://oz.bookmarksfly.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://to.muxihuayi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ao.yuntaijiaju.cn

[C10] 变量作用域
来源：http://pi.panjiajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lh.huixiangedu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nd.haigaiapp.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mt.hahajie.cn

TS:   同 JS
来源：http://uf.huixinmuqiang.cn

Java: 方法内为块级作用域
来源：http://ns.bookmarksfly.cn

Go:   花括号块级作用域
来源：http://de.panjiajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://il.521024.cn

C#:   块级作用域
来源：http://fs.muxihuayi.cn

[C11] 模块导入与导出
来源：http://hy.haigaiapp.cn

Py:   from module import func
来源：http://sp.newstarts.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://jp.panjiajie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://en.shxzskj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://es.haigaiapp.cn

Java: import java.util.List;
来源：http://sm.szxytkj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://er.hahajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://sl.jctech888.com.cn

C#:   using System.Text;
来源：http://qk.521024.cn

[C12] 立即执行函数 IIFE
来源：http://wi.jctech888.com.cn

Py:   (lambda: print("run"))()
来源：http://ga.huanxung.cn

PHP:  (function () { echo "run"; })();
来源：http://mr.newstarts.cn

JS:   (() => { console.log("run"); })();
来源：http://kn.huixiangedu.cn

TS:   (() => { console.log("run"); })();
来源：http://xc.huanxung.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qx.yuntaijiaju.cn

Go:   func() { fmt.Println("run") }()
来源：http://dc.shxzskj.cn

Ruby: -> { puts "run" }.call
来源：http://aw.jctech888.com.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://vq.gzmigu.cn

[C13] 类型声明 / 类型注解
来源：http://ho.jctech888.com.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mw.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dr.muxihuayi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pj.hahajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gn.yuntaijiaju.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xt.huixinmuqiang.cn

Go:   func add(a, b int) int
来源：http://et.asd995.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ls.bjjhwx.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vh.shtwfgs.cn

[C14] 泛型函数
来源：http://tq.newstarts.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yf.hnjuh.cn

PHP:  // 无泛型
来源：http://bm.bookmarksfly.cn

JS:   // 无泛型
来源：http://rf.huixinmuqiang.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mf.shtwfgs.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://al.huixinmuqiang.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://sr.colortex.cn

Ruby: # 无泛型
来源：http://qd.muxihuayi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://op.bjjhwx.cn

[C15] 解构 / 展开参数
来源：http://dm.nicolike.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jl.lnxyls.cn

PHP:  [$a, $b] = $pair;
来源：http://cj.gzmigu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dl.yuexingan06.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://oq.newstarts.cn

Java: // 无解构
来源：http://jd.newstarts.cn

Go:   // 无解构
来源：http://gi.bjjhwx.cn


<!-- 参考信息 -->