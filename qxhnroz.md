代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://yo.yuexingan06.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ap.haigaiapp.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mn.huixinmuqiang.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wn.wgjwhj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nz.shtwfgs.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jm.bjjhwx.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://gv.wgjwhj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bg.shtwfgs.cn

[A26] 类型转换总览
来源：http://mw.huanxung.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://js.asd995.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sy.yuntaijiaju.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gx.lnxyls.cn

TS:   Number() String() Boolean() x as number
来源：http://sc.nicolike.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tt.asd995.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sz.szsharing.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://bj.panjiajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hn.jctech888.com.cn

================================================================================
来源：http://ek.jctech888.com.cn

B. 流程控制
来源：http://oh.chemitech.net.cn

================================================================================
来源：http://vg.yuexingan06.cn

[B01] 条件判断 if / else
来源：http://yo.gzmigu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://sq.521024.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://iw.gzmigu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dp.huixiangedu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kw.bookmarksfly.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ow.jianghongdianzi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://em.bookmarksfly.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ym.bookmarksfly.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yq.huanxung.cn

[B02] 多分支 else if / elif
来源：http://xp.chemitech.net.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ca.huixinmuqiang.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fo.bookmarksfly.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fa.asd995.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ht.newstarts.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xe.bjjhwx.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wc.panjiajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://iv.huixiangedu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ia.shxzukj.cn

[B03] switch / match / case
来源：http://ii.huixinmuqiang.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://px.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fc.gzmigu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://iy.shxzskj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hn.521024.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nu.szxytkj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fo.asd995.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tk.shtwfgs.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ar.haigaiapp.cn

[B04] for 计数循环
来源：http://js.hnjuh.cn

Py:   for i in range(10): print(i)
来源：http://qa.9csxet.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ld.newstarts.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yl.shtwfgs.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gf.lnxyls.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dw.gzmigu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bs.521024.cn

Ruby: 10.times { |i| puts i }
来源：http://uu.jctech888.com.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zt.jctech888.com.cn

[B05] 遍历数组 / 列表
来源：http://ho.szsharing.cn

Py:   for item in arr: print(item)
来源：http://tp.nicolike.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://el.colortex.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wu.szsharing.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ww.colortex.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://is.nszjky.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xz.bjjhwx.cn

Ruby: arr.each { |item| puts item }
来源：http://zx.bjjhwx.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://to.yuexingan06.cn

[B06] 遍历字典 / 对象
来源：http://su.colortex.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://az.lnxyls.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kl.panjiajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vg.szxytkj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tm.shtwfgs.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gv.521024.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lt.haigaiapp.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://he.szxytkj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qy.bjjhwx.cn

[B07] while 循环
来源：http://xs.asd995.cn

Py:   while i < 10: i += 1
来源：http://qd.chemitech.net.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mz.jianghongdianzi.cn

JS:   while (i < 10) { i++; }
来源：http://lu.shxzukj.cn

TS:   while (i < 10) { i++; }
来源：http://tp.bookmarksfly.cn

Java: while (i < 10) { i++; }
来源：http://xu.hnjuh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ze.hahajie.cn

Ruby: while i < 10; i += 1; end
来源：http://cn.bookmarksfly.cn

C#:   while (i < 10) { i++; }
来源：http://fk.hahajie.cn

[B08] do-while（至少执行一次）
来源：http://hl.521024.cn

Py:   # 无 do-while：用 while True + break
来源：http://tb.wgjwhj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://fm.hnjuh.cn

JS:   do { i++; } while (i < 10);
来源：http://ss.szxytkj.cn

TS:   do { i++; } while (i < 10);
来源：http://oc.newstarts.cn

Java: do { i++; } while (i < 10);
来源：http://ms.lnxyls.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://kj.bookmarksfly.cn

Ruby: begin; i += 1; end while i < 10
来源：http://nt.muxihuayi.cn

C#:   do { i++; } while (i < 10);
来源：http://xc.yuexingan06.cn

[B09] break 与 continue
来源：http://zg.jctech888.com.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gk.nszjky.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sh.wgjwhj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pz.nicolike.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zn.bjjhwx.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sn.huanxung.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fn.nicolike.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ol.huixiangedu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yb.huixinmuqiang.cn

[B10] 遍历同时拿索引
来源：http://uw.muxihuayi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ky.yuexingan06.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fx.colortex.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cd.szxytkj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ti.panjiajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jd.wgjwhj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jo.lnxyls.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ny.nszjky.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://eb.nicolike.cn

[B11] 生成数字序列 / 区间
来源：http://mw.newstarts.cn

Py:   list(range(0, 10, 2))
来源：http://tv.gzmigu.cn

PHP:  range(0, 10, 2);
来源：http://ku.huixiangedu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://js.newstarts.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://or.szxytkj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uv.nicolike.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ev.hnjuh.cn

Ruby: (0...10).step(2).to_a
来源：http://vl.nszjky.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vk.chemitech.net.cn

[B12] 跳出多层循环
来源：http://jy.huanxung.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://um.521024.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://iu.lnxyls.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pc.wgjwhj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dl.shxzukj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rx.szxytkj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qp.haigaiapp.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ww.muxihuayi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ya.huixiangedu.cn

[B13] 判断是否为数字
来源：http://tx.hnjuh.cn

Py:   isinstance(x, (int, float))
来源：http://jh.shtwfgs.cn

PHP:  is_numeric($x)
来源：http://em.hnjuh.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wm.yuntaijiaju.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hx.colortex.cn

Java: x instanceof Number
来源：http://zw.wgjwhj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pc.szsharing.cn

Ruby: x.is_a?(Numeric)
来源：http://mk.huanxung.cn

C#:   x is int or double or decimal
来源：http://tv.wgjwhj.cn

[B14] 判断值是否在集合内
来源：http://ux.newstarts.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cu.gzmigu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ci.asd995.cn

JS:   [1, 2, 3].includes(x)
来源：http://qs.chemitech.net.cn

TS:   [1, 2, 3].includes(x)
来源：http://qz.shxzskj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ej.chemitech.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yx.lnxyls.cn

Ruby: [1, 2, 3].include?(x)
来源：http://um.chemitech.net.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hm.gzmigu.cn

[B15] 布尔运算与取反
来源：http://lp.huanxung.cn

Py:   a and b or not c
来源：http://hj.asd995.cn

PHP:  $a && $b || !$c
来源：http://ya.hahajie.cn

JS:   a && b || !c
来源：http://ms.huanxung.cn

TS:   a && b || !c
来源：http://bl.chemitech.net.cn

Java: a && b || !c
来源：http://kb.nicolike.cn

Go:   a && b || !c
来源：http://tc.hnjuh.cn

Ruby: a && b || !c
来源：http://tb.bookmarksfly.cn

C#:   a && b || !c
来源：http://wv.hahajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://et.521024.cn

Py:   if not data: return
来源：http://te.nicolike.cn

PHP:  if (!$data) { return; }
来源：http://hj.bjjhwx.cn

JS:   if (!data) return;
来源：http://es.9csxet.cn

TS:   if (!data) return;
来源：http://tb.jctech888.com.cn

Java: if (data == null) return;
来源：http://uq.bookmarksfly.cn

Go:   if data == nil { return }
来源：http://ol.yuexingan06.cn

Ruby: return if data.nil?
来源：http://da.521024.cn

C#:   if (data == null) return;
来源：http://wa.hnjuh.cn

================================================================================
来源：http://zq.shtwfgs.cn

C. 函数与作用域
来源：http://eq.9csxet.cn

================================================================================
来源：http://ww.colortex.cn

[C01] 定义函数
来源：http://zi.haigaiapp.cn

Py:   def add(a, b): return a + b
来源：http://sa.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ru.chemitech.net.cn

JS:   function add(a, b) { return a + b; }
来源：http://vs.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hj.bookmarksfly.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://nh.chemitech.net.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vu.gzmigu.cn

Ruby: def add(a, b); a + b; end
来源：http://nb.hahajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ps.9csxet.cn

[C02] 默认参数
来源：http://ch.bjjhwx.cn

Py:   def greet(name="World"): return name
来源：http://ro.bjjhwx.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ky.yuntaijiaju.cn

JS:   function greet(name = "World") { return name; }
来源：http://os.lnxyls.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ke.haigaiapp.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zm.lnxyls.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://me.hahajie.cn

Ruby: def greet(name = "World") = name
来源：http://lb.521024.cn

C#:   string Greet(string name = "World") => name;
来源：http://bj.muxihuayi.cn

[C03] 可变参数
来源：http://ba.colortex.cn

Py:   def total(*args): return sum(args)
来源：http://pg.9csxet.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rh.hnjuh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ud.panjiajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ly.shxzukj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ma.gzmigu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qg.jctech888.com.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gv.bjjhwx.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rh.yuntaijiaju.cn

[C04] 命名参数 / 关键字参数
来源：http://am.9csxet.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uq.hahajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mz.9csxet.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://an.gzmigu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://na.panjiajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://hg.yuntaijiaju.cn

Go:   // 无：用配置结构体参数
来源：http://jj.bookmarksfly.cn

Ruby: f(a: 1, b: 2)
来源：http://ei.9csxet.cn

C#:   f(a: 1, b: 2)
来源：http://gs.yuexingan06.cn

[C05] 返回多个值
来源：http://sz.bookmarksfly.cn

Py:   return a, b
来源：http://bp.chemitech.net.cn

PHP:  return [$a, $b];
来源：http://hb.huixinmuqiang.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ol.chemitech.net.cn

TS:   return { a, b };
来源：http://mu.gzmigu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nk.asd995.cn

Go:   return a, b
来源：http://zs.huanxung.cn

Ruby: return a, b
来源：http://yh.yuntaijiaju.cn

C#:   return (a, b);              // ValueTuple
来源：http://ds.lnxyls.cn

[C06] 匿名函数 / lambda
来源：http://fq.huixiangedu.cn

Py:   square = lambda x: x * x
来源：http://lz.hahajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fk.9csxet.cn

JS:   const square = x => x * x;
来源：http://qu.huixiangedu.cn

TS:   const square = (x: number): number => x * x;
来源：http://ik.shxzskj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gb.haigaiapp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ti.haigaiapp.cn

Ruby: square = ->(x) { x * x }
来源：http://ac.bjjhwx.cn

C#:   Func<int, int> square = x => x * x;
来源：http://yf.shxzskj.cn

[C07] 把函数作为参数传入
来源：http://bv.shtwfgs.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ai.lnxyls.cn

PHP:  array_map("strtoupper", $arr);
来源：http://fm.lnxyls.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yk.nszjky.cn

TS:   arr.map(String)
来源：http://jg.yuexingan06.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qg.bookmarksfly.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bx.colortex.cn

Ruby: arr.map(&:upcase)
来源：http://yj.haigaiapp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hx.newstarts.cn

[C08] 闭包
来源：http://xe.haigaiapp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qs.nicolike.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ya.hahajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vs.hahajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://oa.huixiangedu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sq.haigaiapp.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://at.jctech888.com.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wd.huixinmuqiang.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dv.hahajie.cn

[C09] 递归
来源：http://ht.9csxet.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://az.lnxyls.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://za.haigaiapp.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tt.nicolike.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tz.shxzukj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qe.colortex.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uh.szsharing.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ps.lnxyls.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rl.muxihuayi.cn

[C10] 变量作用域
来源：http://rn.panjiajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pv.nicolike.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://aa.chemitech.net.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wr.wgjwhj.cn

TS:   同 JS
来源：http://df.shtwfgs.cn

Java: 方法内为块级作用域
来源：http://yf.hahajie.cn

Go:   花括号块级作用域
来源：http://ag.hnjuh.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ys.chemitech.net.cn

C#:   块级作用域
来源：http://fx.haigaiapp.cn

[C11] 模块导入与导出
来源：http://qc.chemitech.net.cn

Py:   from module import func
来源：http://aw.asd995.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://jd.huanxung.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://pt.haigaiapp.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dj.hnjuh.cn

Java: import java.util.List;
来源：http://cu.bjjhwx.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hm.hnjuh.cn

Ruby: require "json"; require_relative "./util"
来源：http://ng.nicolike.cn

C#:   using System.Text;
来源：http://ai.colortex.cn

[C12] 立即执行函数 IIFE
来源：http://yx.521024.cn

Py:   (lambda: print("run"))()
来源：http://eg.shtwfgs.cn

PHP:  (function () { echo "run"; })();
来源：http://yi.muxihuayi.cn

JS:   (() => { console.log("run"); })();
来源：http://nc.chemitech.net.cn

TS:   (() => { console.log("run"); })();
来源：http://cy.yuexingan06.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yi.521024.cn

Go:   func() { fmt.Println("run") }()
来源：http://xp.jctech888.com.cn

Ruby: -> { puts "run" }.call
来源：http://uv.bookmarksfly.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://je.bookmarksfly.cn

[C13] 类型声明 / 类型注解
来源：http://vu.haigaiapp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bh.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ud.yuntaijiaju.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ue.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hr.nszjky.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ph.hahajie.cn

Go:   func add(a, b int) int
来源：http://le.gzmigu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jl.yuexingan06.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vl.jctech888.com.cn

[C14] 泛型函数
来源：http://ic.panjiajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://la.haigaiapp.cn

PHP:  // 无泛型
来源：http://nw.huanxung.cn

JS:   // 无泛型
来源：http://je.shtwfgs.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://br.hnjuh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xr.lnxyls.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hp.shtwfgs.cn

Ruby: # 无泛型
来源：http://qb.yuexingan06.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xh.9csxet.cn

[C15] 解构 / 展开参数
来源：http://hy.521024.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xa.szxytkj.cn

PHP:  [$a, $b] = $pair;
来源：http://dw.szxytkj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ff.bookmarksfly.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mm.9csxet.cn

Java: // 无解构
来源：http://pk.panjiajie.cn

Go:   // 无解构
来源：http://ur.huixinmuqiang.cn


<!-- 参考信息 -->