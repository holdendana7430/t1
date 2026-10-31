代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fq.jctech888.com.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ar.nicolike.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://xm.yuexingan06.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://oa.huixiangedu.cn

[A26] 类型转换总览
来源：http://ye.szsharing.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://af.hnjuh.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qu.jianghongdianzi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xm.yuexingan06.cn

TS:   Number() String() Boolean() x as number
来源：http://jw.nicolike.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vi.jianghongdianzi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vd.nicolike.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://if.nszjky.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xs.szxytkj.cn

================================================================================
来源：http://if.chemitech.net.cn

B. 流程控制
来源：http://fe.szsharing.cn

================================================================================
来源：http://xs.muxihuayi.cn

[B01] 条件判断 if / else
来源：http://vy.muxihuayi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://rs.nszjky.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ab.yuexingan06.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gz.huanxung.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://uz.panjiajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://tx.jianghongdianzi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bq.bookmarksfly.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rp.yuntaijiaju.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wi.haigaiapp.cn

[B02] 多分支 else if / elif
来源：http://rw.hahajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pg.muxihuayi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qz.bjjhwx.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vj.521024.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ir.bookmarksfly.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://di.jctech888.com.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qp.newstarts.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uu.huanxung.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gp.szxytkj.cn

[B03] switch / match / case
来源：http://fe.panjiajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://re.nszjky.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bi.huanxung.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lx.nicolike.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ek.chemitech.net.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ll.nszjky.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dt.gzmigu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gb.9csxet.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gz.gzmigu.cn

[B04] for 计数循环
来源：http://el.colortex.cn

Py:   for i in range(10): print(i)
来源：http://rg.nicolike.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xb.huixinmuqiang.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eo.jctech888.com.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://aj.nszjky.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://np.shtwfgs.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://oy.newstarts.cn

Ruby: 10.times { |i| puts i }
来源：http://en.yuntaijiaju.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tb.nszjky.cn

[B05] 遍历数组 / 列表
来源：http://mw.newstarts.cn

Py:   for item in arr: print(item)
来源：http://pf.nszjky.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sj.szsharing.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yk.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://zr.muxihuayi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zu.gzmigu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lu.szsharing.cn

Ruby: arr.each { |item| puts item }
来源：http://tx.nicolike.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wb.huixinmuqiang.cn

[B06] 遍历字典 / 对象
来源：http://tf.huixiangedu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xn.chemitech.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vo.hnjuh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vi.shxzukj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yl.huixinmuqiang.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yn.szxytkj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fu.bookmarksfly.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://el.szsharing.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vp.nicolike.cn

[B07] while 循环
来源：http://ji.yuntaijiaju.cn

Py:   while i < 10: i += 1
来源：http://un.wgjwhj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://du.hahajie.cn

JS:   while (i < 10) { i++; }
来源：http://bu.hnjuh.cn

TS:   while (i < 10) { i++; }
来源：http://aa.hnjuh.cn

Java: while (i < 10) { i++; }
来源：http://mx.gzmigu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nf.jctech888.com.cn

Ruby: while i < 10; i += 1; end
来源：http://av.haigaiapp.cn

C#:   while (i < 10) { i++; }
来源：http://lj.jianghongdianzi.cn

[B08] do-while（至少执行一次）
来源：http://vj.shxzskj.cn

Py:   # 无 do-while：用 while True + break
来源：http://of.panjiajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mo.9csxet.cn

JS:   do { i++; } while (i < 10);
来源：http://xj.colortex.cn

TS:   do { i++; } while (i < 10);
来源：http://nw.muxihuayi.cn

Java: do { i++; } while (i < 10);
来源：http://zt.huanxung.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://kz.muxihuayi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rw.newstarts.cn

C#:   do { i++; } while (i < 10);
来源：http://dc.huixiangedu.cn

[B09] break 与 continue
来源：http://qs.huixiangedu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qk.shxzukj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://an.chemitech.net.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ux.9csxet.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vl.bjjhwx.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lz.jianghongdianzi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ku.huixinmuqiang.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bv.szxytkj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wa.wgjwhj.cn

[B10] 遍历同时拿索引
来源：http://ho.panjiajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ae.jianghongdianzi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rt.huixiangedu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fm.9csxet.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qm.shxzukj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://km.asd995.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ge.panjiajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ny.nszjky.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mf.lnxyls.cn

[B11] 生成数字序列 / 区间
来源：http://tk.chemitech.net.cn

Py:   list(range(0, 10, 2))
来源：http://ki.hahajie.cn

PHP:  range(0, 10, 2);
来源：http://ql.muxihuayi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ah.nicolike.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uj.jctech888.com.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://eg.shxzukj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://eq.colortex.cn

Ruby: (0...10).step(2).to_a
来源：http://zg.shtwfgs.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mq.newstarts.cn

[B12] 跳出多层循环
来源：http://hb.hahajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ey.yuntaijiaju.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://tr.bjjhwx.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wl.szsharing.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yt.jianghongdianzi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qh.lnxyls.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://aa.9csxet.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://be.huixinmuqiang.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pr.jctech888.com.cn

[B13] 判断是否为数字
来源：http://zk.chemitech.net.cn

Py:   isinstance(x, (int, float))
来源：http://xx.asd995.cn

PHP:  is_numeric($x)
来源：http://jg.jianghongdianzi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sj.shtwfgs.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://my.nicolike.cn

Java: x instanceof Number
来源：http://pk.colortex.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qq.newstarts.cn

Ruby: x.is_a?(Numeric)
来源：http://lr.shtwfgs.cn

C#:   x is int or double or decimal
来源：http://ae.nicolike.cn

[B14] 判断值是否在集合内
来源：http://sd.newstarts.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://go.521024.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pl.shxzukj.cn

JS:   [1, 2, 3].includes(x)
来源：http://ym.chemitech.net.cn

TS:   [1, 2, 3].includes(x)
来源：http://mb.gzmigu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rm.huanxung.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lk.9csxet.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jm.yuexingan06.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qm.nicolike.cn

[B15] 布尔运算与取反
来源：http://hc.haigaiapp.cn

Py:   a and b or not c
来源：http://ye.yuexingan06.cn

PHP:  $a && $b || !$c
来源：http://el.asd995.cn

JS:   a && b || !c
来源：http://dx.521024.cn

TS:   a && b || !c
来源：http://cy.lnxyls.cn

Java: a && b || !c
来源：http://ga.panjiajie.cn

Go:   a && b || !c
来源：http://nm.nszjky.cn

Ruby: a && b || !c
来源：http://xx.521024.cn

C#:   a && b || !c
来源：http://py.gzmigu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://rg.chemitech.net.cn

Py:   if not data: return
来源：http://nd.521024.cn

PHP:  if (!$data) { return; }
来源：http://ab.huanxung.cn

JS:   if (!data) return;
来源：http://rr.yuntaijiaju.cn

TS:   if (!data) return;
来源：http://yh.nicolike.cn

Java: if (data == null) return;
来源：http://mi.shtwfgs.cn

Go:   if data == nil { return }
来源：http://mr.haigaiapp.cn

Ruby: return if data.nil?
来源：http://co.jianghongdianzi.cn

C#:   if (data == null) return;
来源：http://ks.yuexingan06.cn

================================================================================
来源：http://rc.szsharing.cn

C. 函数与作用域
来源：http://lw.muxihuayi.cn

================================================================================
来源：http://is.asd995.cn

[C01] 定义函数
来源：http://ri.9csxet.cn

Py:   def add(a, b): return a + b
来源：http://tp.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cd.shxzukj.cn

JS:   function add(a, b) { return a + b; }
来源：http://xk.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://we.newstarts.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://sm.huixiangedu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://lz.hnjuh.cn

Ruby: def add(a, b); a + b; end
来源：http://bp.huixiangedu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ns.bjjhwx.cn

[C02] 默认参数
来源：http://ay.shtwfgs.cn

Py:   def greet(name="World"): return name
来源：http://mp.huixiangedu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://es.shtwfgs.cn

JS:   function greet(name = "World") { return name; }
来源：http://mr.haigaiapp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bk.lnxyls.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wm.haigaiapp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vp.hahajie.cn

Ruby: def greet(name = "World") = name
来源：http://zo.gzmigu.cn

C#:   string Greet(string name = "World") => name;
来源：http://hv.shxzukj.cn

[C03] 可变参数
来源：http://xg.yuntaijiaju.cn

Py:   def total(*args): return sum(args)
来源：http://wq.wgjwhj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ez.bjjhwx.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://uy.shxzukj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ty.yuexingan06.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gt.szsharing.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pl.muxihuayi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zz.shxzukj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jz.bjjhwx.cn

[C04] 命名参数 / 关键字参数
来源：http://pf.jianghongdianzi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sy.huixinmuqiang.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yv.yuexingan06.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hj.521024.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dj.bjjhwx.cn

Java: // 无：用 Builder 模式或 record
来源：http://ax.colortex.cn

Go:   // 无：用配置结构体参数
来源：http://zh.bjjhwx.cn

Ruby: f(a: 1, b: 2)
来源：http://vt.bookmarksfly.cn

C#:   f(a: 1, b: 2)
来源：http://zb.yuexingan06.cn

[C05] 返回多个值
来源：http://un.521024.cn

Py:   return a, b
来源：http://hp.bookmarksfly.cn

PHP:  return [$a, $b];
来源：http://jf.hnjuh.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://rr.9csxet.cn

TS:   return { a, b };
来源：http://lr.asd995.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kj.szsharing.cn

Go:   return a, b
来源：http://ze.muxihuayi.cn

Ruby: return a, b
来源：http://vf.haigaiapp.cn

C#:   return (a, b);              // ValueTuple
来源：http://ic.gzmigu.cn

[C06] 匿名函数 / lambda
来源：http://ef.yuexingan06.cn

Py:   square = lambda x: x * x
来源：http://as.szxytkj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://da.bookmarksfly.cn

JS:   const square = x => x * x;
来源：http://gi.asd995.cn

TS:   const square = (x: number): number => x * x;
来源：http://vk.hahajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ld.colortex.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rm.haigaiapp.cn

Ruby: square = ->(x) { x * x }
来源：http://qi.yuntaijiaju.cn

C#:   Func<int, int> square = x => x * x;
来源：http://mw.gzmigu.cn

[C07] 把函数作为参数传入
来源：http://an.9csxet.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tg.shtwfgs.cn

PHP:  array_map("strtoupper", $arr);
来源：http://fh.wgjwhj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uw.asd995.cn

TS:   arr.map(String)
来源：http://hk.lnxyls.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jf.hahajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qh.asd995.cn

Ruby: arr.map(&:upcase)
来源：http://er.shtwfgs.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://zv.huixinmuqiang.cn

[C08] 闭包
来源：http://em.newstarts.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://oy.nszjky.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ac.szxytkj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://io.gzmigu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mq.gzmigu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://se.gzmigu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yr.szsharing.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hj.bookmarksfly.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zf.haigaiapp.cn

[C09] 递归
来源：http://fb.bjjhwx.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vi.yuexingan06.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jq.gzmigu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wy.bjjhwx.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ev.521024.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yb.hahajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://av.chemitech.net.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ox.shtwfgs.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tp.muxihuayi.cn

[C10] 变量作用域
来源：http://sm.shtwfgs.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ij.jianghongdianzi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hn.shtwfgs.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ca.lnxyls.cn

TS:   同 JS
来源：http://zs.yuexingan06.cn

Java: 方法内为块级作用域
来源：http://jj.jianghongdianzi.cn

Go:   花括号块级作用域
来源：http://yl.nicolike.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://iw.hahajie.cn

C#:   块级作用域
来源：http://ao.gzmigu.cn

[C11] 模块导入与导出
来源：http://dy.jctech888.com.cn

Py:   from module import func
来源：http://ck.gzmigu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ry.szsharing.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://af.shxzukj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pt.wgjwhj.cn

Java: import java.util.List;
来源：http://xx.bookmarksfly.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fs.521024.cn

Ruby: require "json"; require_relative "./util"
来源：http://rt.chemitech.net.cn

C#:   using System.Text;
来源：http://cj.nicolike.cn

[C12] 立即执行函数 IIFE
来源：http://oz.gzmigu.cn

Py:   (lambda: print("run"))()
来源：http://qq.nicolike.cn

PHP:  (function () { echo "run"; })();
来源：http://tg.bookmarksfly.cn

JS:   (() => { console.log("run"); })();
来源：http://ij.9csxet.cn

TS:   (() => { console.log("run"); })();
来源：http://ts.yuntaijiaju.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rz.nszjky.cn

Go:   func() { fmt.Println("run") }()
来源：http://ei.yuntaijiaju.cn

Ruby: -> { puts "run" }.call
来源：http://ju.nicolike.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://bx.bookmarksfly.cn

[C13] 类型声明 / 类型注解
来源：http://ml.huixiangedu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://op.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://di.huanxung.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vs.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fm.huixiangedu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://yh.panjiajie.cn

Go:   func add(a, b int) int
来源：http://bp.shxzskj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ws.jianghongdianzi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nf.panjiajie.cn

[C14] 泛型函数
来源：http://tm.panjiajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ql.chemitech.net.cn

PHP:  // 无泛型
来源：http://pr.chemitech.net.cn

JS:   // 无泛型
来源：http://tp.shxzukj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ut.huixinmuqiang.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ka.muxihuayi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zf.szsharing.cn

Ruby: # 无泛型
来源：http://fu.9csxet.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zh.colortex.cn

[C15] 解构 / 展开参数
来源：http://ky.asd995.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nx.gzmigu.cn

PHP:  [$a, $b] = $pair;
来源：http://mh.huixiangedu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rt.haigaiapp.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qw.newstarts.cn

Java: // 无解构
来源：http://zz.shxzskj.cn

Go:   // 无解构
来源：http://me.huanxung.cn

Ruby: a, b = pair
来源：http://fi.haigaiapp.cn

C#:   var (a, b) = pair;
来源：http://zq.huixinmuqiang.cn

[C16] 函数 / 方法重载
来源：http://am.asd995.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rh.yuexingan06.cn


<!-- 参考信息 -->