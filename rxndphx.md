代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://dt.bjjhwx.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vd.nszjky.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tv.haigaiapp.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lw.bookmarksfly.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ga.bjjhwx.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ew.huixiangedu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ag.hahajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://eo.shtwfgs.cn

[A26] 类型转换总览
来源：http://ir.nicolike.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dn.shxzskj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mt.jianghongdianzi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ud.yuexingan06.cn

TS:   Number() String() Boolean() x as number
来源：http://am.chemitech.net.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://et.muxihuayi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dn.newstarts.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ai.nicolike.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nw.chemitech.net.cn

================================================================================
来源：http://oh.huanxung.cn

B. 流程控制
来源：http://sn.bjjhwx.cn

================================================================================
来源：http://io.jctech888.com.cn

[B01] 条件判断 if / else
来源：http://jk.huixiangedu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ni.gzmigu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tn.shxzukj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://iy.wgjwhj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vq.huanxung.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ue.gzmigu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tc.yuntaijiaju.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sn.huanxung.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cj.shxzukj.cn

[B02] 多分支 else if / elif
来源：http://jg.haigaiapp.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ei.bookmarksfly.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pz.muxihuayi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ln.shxzukj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hj.bjjhwx.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tq.bookmarksfly.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fy.yuntaijiaju.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://eo.nicolike.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jv.yuntaijiaju.cn

[B03] switch / match / case
来源：http://kh.newstarts.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ld.nicolike.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cm.yuexingan06.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ms.huixinmuqiang.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://im.yuexingan06.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jj.hahajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gp.bookmarksfly.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pf.521024.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qu.jianghongdianzi.cn

[B04] for 计数循环
来源：http://ip.huixinmuqiang.cn

Py:   for i in range(10): print(i)
来源：http://dv.jctech888.com.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ir.chemitech.net.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qw.bjjhwx.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gp.hnjuh.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kw.9csxet.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rb.jianghongdianzi.cn

Ruby: 10.times { |i| puts i }
来源：http://cj.chemitech.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sa.bjjhwx.cn

[B05] 遍历数组 / 列表
来源：http://eo.szxytkj.cn

Py:   for item in arr: print(item)
来源：http://pd.521024.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ut.shtwfgs.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://bx.szsharing.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yo.colortex.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://tj.huanxung.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kk.asd995.cn

Ruby: arr.each { |item| puts item }
来源：http://dx.shxzskj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ux.jianghongdianzi.cn

[B06] 遍历字典 / 对象
来源：http://ae.shtwfgs.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://js.521024.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mw.szxytkj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wr.nszjky.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ie.hnjuh.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://op.yuntaijiaju.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nc.lnxyls.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qd.gzmigu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ry.huixinmuqiang.cn

[B07] while 循环
来源：http://zm.gzmigu.cn

Py:   while i < 10: i += 1
来源：http://or.wgjwhj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://dg.shxzskj.cn

JS:   while (i < 10) { i++; }
来源：http://aq.haigaiapp.cn

TS:   while (i < 10) { i++; }
来源：http://nx.szsharing.cn

Java: while (i < 10) { i++; }
来源：http://ze.jctech888.com.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kk.shxzskj.cn

Ruby: while i < 10; i += 1; end
来源：http://vh.bookmarksfly.cn

C#:   while (i < 10) { i++; }
来源：http://jk.shxzskj.cn

[B08] do-while（至少执行一次）
来源：http://uz.chemitech.net.cn

Py:   # 无 do-while：用 while True + break
来源：http://xh.jianghongdianzi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vu.shxzukj.cn

JS:   do { i++; } while (i < 10);
来源：http://tq.asd995.cn

TS:   do { i++; } while (i < 10);
来源：http://cj.hnjuh.cn

Java: do { i++; } while (i < 10);
来源：http://dc.hnjuh.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://tk.521024.cn

Ruby: begin; i += 1; end while i < 10
来源：http://bl.shxzskj.cn

C#:   do { i++; } while (i < 10);
来源：http://sj.haigaiapp.cn

[B09] break 与 continue
来源：http://yb.lnxyls.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://uq.colortex.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ux.hahajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nd.shtwfgs.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pd.gzmigu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yi.newstarts.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kv.newstarts.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kw.panjiajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sp.521024.cn

[B10] 遍历同时拿索引
来源：http://uw.asd995.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ti.szxytkj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lz.huanxung.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vh.newstarts.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gv.gzmigu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yc.yuntaijiaju.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yo.colortex.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://id.colortex.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cl.wgjwhj.cn

[B11] 生成数字序列 / 区间
来源：http://bu.lnxyls.cn

Py:   list(range(0, 10, 2))
来源：http://yn.lnxyls.cn

PHP:  range(0, 10, 2);
来源：http://vi.huanxung.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zi.huanxung.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rs.jianghongdianzi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ed.colortex.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ab.jianghongdianzi.cn

Ruby: (0...10).step(2).to_a
来源：http://ke.521024.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xd.bookmarksfly.cn

[B12] 跳出多层循环
来源：http://an.nicolike.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xk.szxytkj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mg.huanxung.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cv.huixinmuqiang.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kz.hnjuh.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yb.bjjhwx.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uw.huixiangedu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zy.jctech888.com.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nf.shxzskj.cn

[B13] 判断是否为数字
来源：http://mf.nszjky.cn

Py:   isinstance(x, (int, float))
来源：http://py.szsharing.cn

PHP:  is_numeric($x)
来源：http://lf.shtwfgs.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xq.jctech888.com.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fk.bjjhwx.cn

Java: x instanceof Number
来源：http://gu.colortex.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gu.nicolike.cn

Ruby: x.is_a?(Numeric)
来源：http://vo.huanxung.cn

C#:   x is int or double or decimal
来源：http://sk.nicolike.cn

[B14] 判断值是否在集合内
来源：http://is.huanxung.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://iz.haigaiapp.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ow.szsharing.cn

JS:   [1, 2, 3].includes(x)
来源：http://pe.huixinmuqiang.cn

TS:   [1, 2, 3].includes(x)
来源：http://ag.hahajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://pv.lnxyls.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jp.hahajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xk.hnjuh.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mo.nicolike.cn

[B15] 布尔运算与取反
来源：http://kz.jctech888.com.cn

Py:   a and b or not c
来源：http://jy.shtwfgs.cn

PHP:  $a && $b || !$c
来源：http://fa.nicolike.cn

JS:   a && b || !c
来源：http://mn.huixiangedu.cn

TS:   a && b || !c
来源：http://ea.bookmarksfly.cn

Java: a && b || !c
来源：http://ki.newstarts.cn

Go:   a && b || !c
来源：http://zp.hahajie.cn

Ruby: a && b || !c
来源：http://eb.colortex.cn

C#:   a && b || !c
来源：http://ua.jianghongdianzi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://nv.yuntaijiaju.cn

Py:   if not data: return
来源：http://az.hahajie.cn

PHP:  if (!$data) { return; }
来源：http://br.hahajie.cn

JS:   if (!data) return;
来源：http://yk.huixiangedu.cn

TS:   if (!data) return;
来源：http://zo.haigaiapp.cn

Java: if (data == null) return;
来源：http://ld.nszjky.cn

Go:   if data == nil { return }
来源：http://qm.yuexingan06.cn

Ruby: return if data.nil?
来源：http://gk.9csxet.cn

C#:   if (data == null) return;
来源：http://mv.hahajie.cn

================================================================================
来源：http://qh.nicolike.cn

C. 函数与作用域
来源：http://sy.jctech888.com.cn

================================================================================
来源：http://ib.lnxyls.cn

[C01] 定义函数
来源：http://ts.huixinmuqiang.cn

Py:   def add(a, b): return a + b
来源：http://ix.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ix.haigaiapp.cn

JS:   function add(a, b) { return a + b; }
来源：http://gq.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yr.hnjuh.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://nc.hnjuh.cn

Go:   func add(a, b int) int { return a + b }
来源：http://cv.hahajie.cn

Ruby: def add(a, b); a + b; end
来源：http://et.colortex.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://va.521024.cn

[C02] 默认参数
来源：http://os.shtwfgs.cn

Py:   def greet(name="World"): return name
来源：http://yh.shxzskj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hu.shxzukj.cn

JS:   function greet(name = "World") { return name; }
来源：http://dg.yuntaijiaju.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hn.nszjky.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://de.shtwfgs.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ku.asd995.cn

Ruby: def greet(name = "World") = name
来源：http://ph.shtwfgs.cn

C#:   string Greet(string name = "World") => name;
来源：http://oy.szsharing.cn

[C03] 可变参数
来源：http://rn.jianghongdianzi.cn

Py:   def total(*args): return sum(args)
来源：http://iw.nszjky.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://iw.shtwfgs.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dx.szsharing.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ow.newstarts.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://os.shtwfgs.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xa.huixiangedu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://mp.asd995.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://td.gzmigu.cn

[C04] 命名参数 / 关键字参数
来源：http://od.hnjuh.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zx.gzmigu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://us.jctech888.com.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kw.hnjuh.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zf.asd995.cn

Java: // 无：用 Builder 模式或 record
来源：http://gb.chemitech.net.cn

Go:   // 无：用配置结构体参数
来源：http://bz.shtwfgs.cn

Ruby: f(a: 1, b: 2)
来源：http://dg.szxytkj.cn

C#:   f(a: 1, b: 2)
来源：http://se.9csxet.cn

[C05] 返回多个值
来源：http://yr.colortex.cn

Py:   return a, b
来源：http://kl.panjiajie.cn

PHP:  return [$a, $b];
来源：http://zm.szsharing.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://uc.wgjwhj.cn

TS:   return { a, b };
来源：http://qy.szsharing.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hq.lnxyls.cn

Go:   return a, b
来源：http://bd.9csxet.cn

Ruby: return a, b
来源：http://au.nszjky.cn

C#:   return (a, b);              // ValueTuple
来源：http://iz.newstarts.cn

[C06] 匿名函数 / lambda
来源：http://vp.newstarts.cn

Py:   square = lambda x: x * x
来源：http://yv.nszjky.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://dk.521024.cn

JS:   const square = x => x * x;
来源：http://sk.gzmigu.cn

TS:   const square = (x: number): number => x * x;
来源：http://mh.panjiajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mw.lnxyls.cn

Go:   sq := func(x int) int { return x * x }
来源：http://sz.newstarts.cn

Ruby: square = ->(x) { x * x }
来源：http://vh.asd995.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ve.hahajie.cn

[C07] 把函数作为参数传入
来源：http://he.lnxyls.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gc.shxzskj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://go.nicolike.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lk.huixinmuqiang.cn

TS:   arr.map(String)
来源：http://jk.shtwfgs.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://go.bjjhwx.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://so.haigaiapp.cn

Ruby: arr.map(&:upcase)
来源：http://go.jctech888.com.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gt.yuntaijiaju.cn

[C08] 闭包
来源：http://fl.jianghongdianzi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ed.muxihuayi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jh.yuexingan06.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dv.muxihuayi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cm.yuntaijiaju.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://iv.jianghongdianzi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vu.lnxyls.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sp.lnxyls.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ys.huanxung.cn

[C09] 递归
来源：http://zy.shxzskj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cg.haigaiapp.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lw.asd995.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ay.nszjky.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kv.9csxet.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ti.lnxyls.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jw.yuntaijiaju.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pc.newstarts.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tk.9csxet.cn

[C10] 变量作用域
来源：http://fx.shtwfgs.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kp.shxzskj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mu.asd995.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xy.huixinmuqiang.cn

TS:   同 JS
来源：http://op.szxytkj.cn

Java: 方法内为块级作用域
来源：http://tl.gzmigu.cn

Go:   花括号块级作用域
来源：http://ye.szxytkj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tu.yuntaijiaju.cn

C#:   块级作用域
来源：http://xe.panjiajie.cn

[C11] 模块导入与导出
来源：http://gw.nszjky.cn

Py:   from module import func
来源：http://mb.huixinmuqiang.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pv.szsharing.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gb.huixinmuqiang.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xa.szsharing.cn

Java: import java.util.List;
来源：http://rc.colortex.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zr.lnxyls.cn

Ruby: require "json"; require_relative "./util"
来源：http://au.haigaiapp.cn

C#:   using System.Text;
来源：http://ze.nicolike.cn

[C12] 立即执行函数 IIFE
来源：http://uv.bookmarksfly.cn

Py:   (lambda: print("run"))()
来源：http://eq.521024.cn

PHP:  (function () { echo "run"; })();
来源：http://lw.shtwfgs.cn

JS:   (() => { console.log("run"); })();
来源：http://wi.huixiangedu.cn

TS:   (() => { console.log("run"); })();
来源：http://fz.hahajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wx.hahajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://wj.wgjwhj.cn

Ruby: -> { puts "run" }.call
来源：http://fr.gzmigu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fb.521024.cn

[C13] 类型声明 / 类型注解
来源：http://uo.huanxung.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qn.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ak.panjiajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yn.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://je.colortex.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jq.muxihuayi.cn

Go:   func add(a, b int) int
来源：http://xp.yuntaijiaju.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vc.yuntaijiaju.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wz.9csxet.cn

[C14] 泛型函数
来源：http://cn.jctech888.com.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fs.jianghongdianzi.cn

PHP:  // 无泛型
来源：http://jk.lnxyls.cn

JS:   // 无泛型
来源：http://tr.colortex.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ik.bjjhwx.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zg.yuntaijiaju.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bc.9csxet.cn

Ruby: # 无泛型
来源：http://ik.9csxet.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://uk.panjiajie.cn

[C15] 解构 / 展开参数
来源：http://fq.gzmigu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nd.huixinmuqiang.cn

PHP:  [$a, $b] = $pair;
来源：http://fm.jctech888.com.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ov.huixiangedu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ez.haigaiapp.cn

Java: // 无解构
来源：http://uc.shxzukj.cn

Go:   // 无解构
来源：http://bi.shxzukj.cn


<!-- 参考信息 -->