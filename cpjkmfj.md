代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fp.huanxung.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zo.hnjuh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://nr.asd995.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://so.jianghongdianzi.cn

[A26] 类型转换总览
来源：http://ro.huixiangedu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ck.nicolike.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hu.muxihuayi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wl.shxzukj.cn

TS:   Number() String() Boolean() x as number
来源：http://cl.521024.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kk.wgjwhj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ro.chemitech.net.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://bl.hnjuh.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xm.yuexingan06.cn

================================================================================
来源：http://nu.nszjky.cn

B. 流程控制
来源：http://cr.shtwfgs.cn

================================================================================
来源：http://zh.nicolike.cn

[B01] 条件判断 if / else
来源：http://jy.hnjuh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ve.lnxyls.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://my.bookmarksfly.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://iu.szxytkj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zo.yuexingan06.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://kn.yuntaijiaju.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://sp.yuntaijiaju.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://os.lnxyls.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://en.huanxung.cn

[B02] 多分支 else if / elif
来源：http://dl.bookmarksfly.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nm.hahajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dj.asd995.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://of.nszjky.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ei.szxytkj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://in.nicolike.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ye.colortex.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://og.jianghongdianzi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.huanxung.cn

[B03] switch / match / case
来源：http://xc.panjiajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ra.bookmarksfly.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yp.shxzskj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cj.gzmigu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fx.colortex.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ln.521024.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xt.hahajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zf.nicolike.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dy.nszjky.cn

[B04] for 计数循环
来源：http://vj.szxytkj.cn

Py:   for i in range(10): print(i)
来源：http://ol.szxytkj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dr.muxihuayi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dq.jctech888.com.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://aw.szxytkj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mt.bjjhwx.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qk.szsharing.cn

Ruby: 10.times { |i| puts i }
来源：http://bo.panjiajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yx.szsharing.cn

[B05] 遍历数组 / 列表
来源：http://tm.szsharing.cn

Py:   for item in arr: print(item)
来源：http://cr.wgjwhj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wg.shxzskj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://sc.521024.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://nz.muxihuayi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ln.jianghongdianzi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pn.yuntaijiaju.cn

Ruby: arr.each { |item| puts item }
来源：http://vj.muxihuayi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ae.bookmarksfly.cn

[B06] 遍历字典 / 对象
来源：http://ft.9csxet.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ld.panjiajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://la.newstarts.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gq.shtwfgs.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bh.shxzukj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://en.colortex.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ms.hahajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nt.szxytkj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xx.yuexingan06.cn

[B07] while 循环
来源：http://jw.muxihuayi.cn

Py:   while i < 10: i += 1
来源：http://mx.jctech888.com.cn

PHP:  while ($i < 10) { $i++; }
来源：http://am.huixinmuqiang.cn

JS:   while (i < 10) { i++; }
来源：http://rw.huixiangedu.cn

TS:   while (i < 10) { i++; }
来源：http://ki.panjiajie.cn

Java: while (i < 10) { i++; }
来源：http://cg.huixiangedu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gp.yuexingan06.cn

Ruby: while i < 10; i += 1; end
来源：http://ga.hnjuh.cn

C#:   while (i < 10) { i++; }
来源：http://wz.muxihuayi.cn

[B08] do-while（至少执行一次）
来源：http://pc.nszjky.cn

Py:   # 无 do-while：用 while True + break
来源：http://bt.yuexingan06.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://am.huixinmuqiang.cn

JS:   do { i++; } while (i < 10);
来源：http://do.chemitech.net.cn

TS:   do { i++; } while (i < 10);
来源：http://xa.szxytkj.cn

Java: do { i++; } while (i < 10);
来源：http://vn.huixinmuqiang.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://is.hahajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cx.gzmigu.cn

C#:   do { i++; } while (i < 10);
来源：http://ok.shxzskj.cn

[B09] break 与 continue
来源：http://ep.bjjhwx.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sp.nicolike.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://my.lnxyls.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://la.szsharing.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ue.jianghongdianzi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ac.muxihuayi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gf.huanxung.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xr.521024.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lt.huixiangedu.cn

[B10] 遍历同时拿索引
来源：http://st.colortex.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dh.yuexingan06.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://id.asd995.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lc.huixinmuqiang.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vi.colortex.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ll.haigaiapp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://oh.gzmigu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zu.huixinmuqiang.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lc.muxihuayi.cn

[B11] 生成数字序列 / 区间
来源：http://js.hnjuh.cn

Py:   list(range(0, 10, 2))
来源：http://tn.asd995.cn

PHP:  range(0, 10, 2);
来源：http://qg.newstarts.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sa.haigaiapp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nb.bookmarksfly.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sn.newstarts.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jf.hahajie.cn

Ruby: (0...10).step(2).to_a
来源：http://ah.haigaiapp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mj.wgjwhj.cn

[B12] 跳出多层循环
来源：http://qb.yuexingan06.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zx.wgjwhj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fa.szxytkj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rb.colortex.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vx.asd995.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hc.chemitech.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mu.bjjhwx.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wi.gzmigu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uj.haigaiapp.cn

[B13] 判断是否为数字
来源：http://dm.asd995.cn

Py:   isinstance(x, (int, float))
来源：http://jp.colortex.cn

PHP:  is_numeric($x)
来源：http://gp.haigaiapp.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lr.yuexingan06.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zp.9csxet.cn

Java: x instanceof Number
来源：http://pp.wgjwhj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fh.newstarts.cn

Ruby: x.is_a?(Numeric)
来源：http://uv.hahajie.cn

C#:   x is int or double or decimal
来源：http://wm.newstarts.cn

[B14] 判断值是否在集合内
来源：http://mz.bookmarksfly.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yo.shxzukj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ey.gzmigu.cn

JS:   [1, 2, 3].includes(x)
来源：http://ji.asd995.cn

TS:   [1, 2, 3].includes(x)
来源：http://cn.521024.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hn.jctech888.com.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kj.shxzskj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fs.szxytkj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ns.nszjky.cn

[B15] 布尔运算与取反
来源：http://wz.huixinmuqiang.cn

Py:   a and b or not c
来源：http://ss.bookmarksfly.cn

PHP:  $a && $b || !$c
来源：http://ht.huanxung.cn

JS:   a && b || !c
来源：http://do.chemitech.net.cn

TS:   a && b || !c
来源：http://fz.lnxyls.cn

Java: a && b || !c
来源：http://nq.nszjky.cn

Go:   a && b || !c
来源：http://rs.shxzukj.cn

Ruby: a && b || !c
来源：http://gu.hahajie.cn

C#:   a && b || !c
来源：http://au.hahajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ik.shxzukj.cn

Py:   if not data: return
来源：http://od.bjjhwx.cn

PHP:  if (!$data) { return; }
来源：http://pn.asd995.cn

JS:   if (!data) return;
来源：http://kk.wgjwhj.cn

TS:   if (!data) return;
来源：http://pm.shxzskj.cn

Java: if (data == null) return;
来源：http://rz.jctech888.com.cn

Go:   if data == nil { return }
来源：http://tk.szxytkj.cn

Ruby: return if data.nil?
来源：http://hs.nicolike.cn

C#:   if (data == null) return;
来源：http://ro.shxzskj.cn

================================================================================
来源：http://gh.chemitech.net.cn

C. 函数与作用域
来源：http://qp.jctech888.com.cn

================================================================================
来源：http://uu.shxzskj.cn

[C01] 定义函数
来源：http://os.521024.cn

Py:   def add(a, b): return a + b
来源：http://uf.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yk.huixiangedu.cn

JS:   function add(a, b) { return a + b; }
来源：http://ql.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ja.bookmarksfly.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://aq.lnxyls.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dj.jianghongdianzi.cn

Ruby: def add(a, b); a + b; end
来源：http://yq.chemitech.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jd.panjiajie.cn

[C02] 默认参数
来源：http://so.shxzukj.cn

Py:   def greet(name="World"): return name
来源：http://lf.jctech888.com.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lj.bookmarksfly.cn

JS:   function greet(name = "World") { return name; }
来源：http://bk.newstarts.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ph.huixiangedu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://mw.newstarts.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dp.haigaiapp.cn

Ruby: def greet(name = "World") = name
来源：http://ro.haigaiapp.cn

C#:   string Greet(string name = "World") => name;
来源：http://gq.panjiajie.cn

[C03] 可变参数
来源：http://es.gzmigu.cn

Py:   def total(*args): return sum(args)
来源：http://fg.colortex.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yp.hahajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ba.lnxyls.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bb.huixiangedu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://og.bjjhwx.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bh.hahajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://by.muxihuayi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bf.wgjwhj.cn

[C04] 命名参数 / 关键字参数
来源：http://kb.521024.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qv.huixiangedu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hj.gzmigu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rb.yuexingan06.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://no.yuexingan06.cn

Java: // 无：用 Builder 模式或 record
来源：http://hw.huanxung.cn

Go:   // 无：用配置结构体参数
来源：http://mr.shxzukj.cn

Ruby: f(a: 1, b: 2)
来源：http://mh.huanxung.cn

C#:   f(a: 1, b: 2)
来源：http://ru.asd995.cn

[C05] 返回多个值
来源：http://cs.jctech888.com.cn

Py:   return a, b
来源：http://qs.muxihuayi.cn

PHP:  return [$a, $b];
来源：http://da.gzmigu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ao.yuntaijiaju.cn

TS:   return { a, b };
来源：http://fc.gzmigu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mt.nszjky.cn

Go:   return a, b
来源：http://cs.lnxyls.cn

Ruby: return a, b
来源：http://xu.chemitech.net.cn

C#:   return (a, b);              // ValueTuple
来源：http://gd.huixinmuqiang.cn

[C06] 匿名函数 / lambda
来源：http://cl.huixiangedu.cn

Py:   square = lambda x: x * x
来源：http://kg.nicolike.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://tg.newstarts.cn

JS:   const square = x => x * x;
来源：http://rg.gzmigu.cn

TS:   const square = (x: number): number => x * x;
来源：http://pw.bookmarksfly.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ki.jianghongdianzi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ks.9csxet.cn

Ruby: square = ->(x) { x * x }
来源：http://tf.colortex.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wp.wgjwhj.cn

[C07] 把函数作为参数传入
来源：http://sd.hahajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ny.szxytkj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xh.asd995.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://we.haigaiapp.cn

TS:   arr.map(String)
来源：http://ea.shtwfgs.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ty.jctech888.com.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tm.colortex.cn

Ruby: arr.map(&:upcase)
来源：http://rx.shxzukj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://om.wgjwhj.cn

[C08] 闭包
来源：http://vk.colortex.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://so.huixinmuqiang.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tf.muxihuayi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ye.shxzukj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ot.huixiangedu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wa.shxzskj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://we.yuntaijiaju.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vq.lnxyls.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ak.shxzukj.cn

[C09] 递归
来源：http://gc.muxihuayi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hn.jianghongdianzi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://un.muxihuayi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mz.jctech888.com.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vy.hnjuh.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fr.gzmigu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qm.szxytkj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xw.yuexingan06.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wd.asd995.cn

[C10] 变量作用域
来源：http://wy.colortex.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yy.yuntaijiaju.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bl.yuexingan06.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pu.yuexingan06.cn

TS:   同 JS
来源：http://hh.huixinmuqiang.cn

Java: 方法内为块级作用域
来源：http://zx.huixinmuqiang.cn

Go:   花括号块级作用域
来源：http://eo.colortex.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tr.lnxyls.cn

C#:   块级作用域
来源：http://rd.bookmarksfly.cn

[C11] 模块导入与导出
来源：http://hn.wgjwhj.cn

Py:   from module import func
来源：http://bh.colortex.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://jq.chemitech.net.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://dh.panjiajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ak.shtwfgs.cn

Java: import java.util.List;
来源：http://qm.bookmarksfly.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://eu.szsharing.cn

Ruby: require "json"; require_relative "./util"
来源：http://zw.jianghongdianzi.cn

C#:   using System.Text;
来源：http://nn.newstarts.cn

[C12] 立即执行函数 IIFE
来源：http://xp.yuntaijiaju.cn

Py:   (lambda: print("run"))()
来源：http://em.haigaiapp.cn

PHP:  (function () { echo "run"; })();
来源：http://bg.wgjwhj.cn

JS:   (() => { console.log("run"); })();
来源：http://xy.shtwfgs.cn

TS:   (() => { console.log("run"); })();
来源：http://ul.haigaiapp.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yr.nicolike.cn

Go:   func() { fmt.Println("run") }()
来源：http://op.hahajie.cn

Ruby: -> { puts "run" }.call
来源：http://ci.huixiangedu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xu.wgjwhj.cn

[C13] 类型声明 / 类型注解
来源：http://kr.jianghongdianzi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vb.haigaiapp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sk.jctech888.com.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ga.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ye.huixinmuqiang.cn

Java: int add(int a, int b) { return a + b; }
来源：http://of.muxihuayi.cn

Go:   func add(a, b int) int
来源：http://lb.521024.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://py.lnxyls.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tx.shxzskj.cn

[C14] 泛型函数
来源：http://nd.colortex.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qq.haigaiapp.cn

PHP:  // 无泛型
来源：http://hg.nszjky.cn

JS:   // 无泛型
来源：http://xk.shxzskj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ua.shxzukj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qe.newstarts.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ep.hahajie.cn

Ruby: # 无泛型
来源：http://rt.yuntaijiaju.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pj.szxytkj.cn

[C15] 解构 / 展开参数
来源：http://qo.jctech888.com.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tn.colortex.cn

PHP:  [$a, $b] = $pair;
来源：http://jr.newstarts.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bp.nicolike.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://iy.9csxet.cn

Java: // 无解构
来源：http://uf.hahajie.cn

Go:   // 无解构
来源：http://ol.gzmigu.cn

Ruby: a, b = pair
来源：http://yr.asd995.cn

C#:   var (a, b) = pair;
来源：http://rv.gzmigu.cn

[C16] 函数 / 方法重载
来源：http://vc.jctech888.com.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dd.nicolike.cn


<!-- 参考信息 -->