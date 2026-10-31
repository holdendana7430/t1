代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ko.huixiangedu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dv.szsharing.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://jw.yuexingan06.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mv.nszjky.cn

[A26] 类型转换总览
来源：http://ve.szxytkj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://nk.chemitech.net.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ew.yuexingan06.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sp.hnjuh.cn

TS:   Number() String() Boolean() x as number
来源：http://mw.szxytkj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ua.szxytkj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yf.newstarts.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://fj.haigaiapp.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zn.huanxung.cn

================================================================================
来源：http://kd.shtwfgs.cn

B. 流程控制
来源：http://tw.bookmarksfly.cn

================================================================================
来源：http://ch.jctech888.com.cn

[B01] 条件判断 if / else
来源：http://to.huixiangedu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://fw.szxytkj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xg.muxihuayi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fl.szsharing.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dk.huixinmuqiang.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bt.shtwfgs.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qq.muxihuayi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://eq.bookmarksfly.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sp.chemitech.net.cn

[B02] 多分支 else if / elif
来源：http://ob.jianghongdianzi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://iq.nicolike.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rb.asd995.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vb.nszjky.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gm.newstarts.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zn.hahajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uq.lnxyls.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uc.521024.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gr.shxzukj.cn

[B03] switch / match / case
来源：http://fm.muxihuayi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lo.muxihuayi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://da.9csxet.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://no.nicolike.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fz.nszjky.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kh.shtwfgs.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fy.jctech888.com.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ha.shxzukj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nc.panjiajie.cn

[B04] for 计数循环
来源：http://hb.jianghongdianzi.cn

Py:   for i in range(10): print(i)
来源：http://zi.wgjwhj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://oz.521024.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hx.wgjwhj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tb.asd995.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kg.shxzukj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kr.muxihuayi.cn

Ruby: 10.times { |i| puts i }
来源：http://tv.wgjwhj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ow.jianghongdianzi.cn

[B05] 遍历数组 / 列表
来源：http://my.bookmarksfly.cn

Py:   for item in arr: print(item)
来源：http://jy.shtwfgs.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://to.lnxyls.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://xd.asd995.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://to.hnjuh.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qp.nszjky.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ol.yuexingan06.cn

Ruby: arr.each { |item| puts item }
来源：http://wr.chemitech.net.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gj.521024.cn

[B06] 遍历字典 / 对象
来源：http://cg.szxytkj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://rx.bookmarksfly.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qp.panjiajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rf.wgjwhj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rj.bookmarksfly.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mr.nicolike.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ld.asd995.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kw.bjjhwx.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xk.colortex.cn

[B07] while 循环
来源：http://ns.haigaiapp.cn

Py:   while i < 10: i += 1
来源：http://dp.chemitech.net.cn

PHP:  while ($i < 10) { $i++; }
来源：http://pv.huixinmuqiang.cn

JS:   while (i < 10) { i++; }
来源：http://ft.muxihuayi.cn

TS:   while (i < 10) { i++; }
来源：http://hv.wgjwhj.cn

Java: while (i < 10) { i++; }
来源：http://rg.szxytkj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dk.colortex.cn

Ruby: while i < 10; i += 1; end
来源：http://gh.haigaiapp.cn

C#:   while (i < 10) { i++; }
来源：http://ad.colortex.cn

[B08] do-while（至少执行一次）
来源：http://qu.nicolike.cn

Py:   # 无 do-while：用 while True + break
来源：http://ge.szxytkj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cs.gzmigu.cn

JS:   do { i++; } while (i < 10);
来源：http://lv.szsharing.cn

TS:   do { i++; } while (i < 10);
来源：http://vh.asd995.cn

Java: do { i++; } while (i < 10);
来源：http://oc.hahajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://hr.jctech888.com.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hw.shxzukj.cn

C#:   do { i++; } while (i < 10);
来源：http://zs.nicolike.cn

[B09] break 与 continue
来源：http://dw.haigaiapp.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pn.szxytkj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gt.newstarts.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yz.huanxung.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xw.9csxet.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ra.chemitech.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yp.huixinmuqiang.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zk.asd995.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bc.wgjwhj.cn

[B10] 遍历同时拿索引
来源：http://nf.muxihuayi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vw.bookmarksfly.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fi.bookmarksfly.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fj.521024.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wy.lnxyls.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qn.bookmarksfly.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bw.szsharing.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xj.huanxung.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sr.521024.cn

[B11] 生成数字序列 / 区间
来源：http://qv.panjiajie.cn

Py:   list(range(0, 10, 2))
来源：http://ow.shxzukj.cn

PHP:  range(0, 10, 2);
来源：http://xu.gzmigu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jl.szxytkj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ea.521024.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ax.shxzskj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cu.9csxet.cn

Ruby: (0...10).step(2).to_a
来源：http://rj.panjiajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xa.nicolike.cn

[B12] 跳出多层循环
来源：http://az.panjiajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ee.hahajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ye.9csxet.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wi.huixinmuqiang.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ps.shxzskj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ai.muxihuayi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ix.shxzskj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kg.nicolike.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zp.yuexingan06.cn

[B13] 判断是否为数字
来源：http://mb.hahajie.cn

Py:   isinstance(x, (int, float))
来源：http://ya.nicolike.cn

PHP:  is_numeric($x)
来源：http://zk.huixiangedu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hy.9csxet.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jk.wgjwhj.cn

Java: x instanceof Number
来源：http://xd.521024.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gq.521024.cn

Ruby: x.is_a?(Numeric)
来源：http://do.bjjhwx.cn

C#:   x is int or double or decimal
来源：http://zh.huixiangedu.cn

[B14] 判断值是否在集合内
来源：http://cu.panjiajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dz.bjjhwx.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ha.colortex.cn

JS:   [1, 2, 3].includes(x)
来源：http://ww.asd995.cn

TS:   [1, 2, 3].includes(x)
来源：http://jv.wgjwhj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ts.muxihuayi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pl.jianghongdianzi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rz.shxzskj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sw.bjjhwx.cn

[B15] 布尔运算与取反
来源：http://om.newstarts.cn

Py:   a and b or not c
来源：http://no.shtwfgs.cn

PHP:  $a && $b || !$c
来源：http://fb.chemitech.net.cn

JS:   a && b || !c
来源：http://hy.chemitech.net.cn

TS:   a && b || !c
来源：http://ag.huixinmuqiang.cn

Java: a && b || !c
来源：http://qn.bookmarksfly.cn

Go:   a && b || !c
来源：http://qr.newstarts.cn

Ruby: a && b || !c
来源：http://xg.panjiajie.cn

C#:   a && b || !c
来源：http://se.newstarts.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xj.szsharing.cn

Py:   if not data: return
来源：http://vq.9csxet.cn

PHP:  if (!$data) { return; }
来源：http://ea.szxytkj.cn

JS:   if (!data) return;
来源：http://ra.yuexingan06.cn

TS:   if (!data) return;
来源：http://nh.bjjhwx.cn

Java: if (data == null) return;
来源：http://eq.gzmigu.cn

Go:   if data == nil { return }
来源：http://rl.yuexingan06.cn

Ruby: return if data.nil?
来源：http://px.9csxet.cn

C#:   if (data == null) return;
来源：http://yz.huixiangedu.cn

================================================================================
来源：http://vb.bookmarksfly.cn

C. 函数与作用域
来源：http://on.jctech888.com.cn

================================================================================
来源：http://xq.muxihuayi.cn

[C01] 定义函数
来源：http://vc.521024.cn

Py:   def add(a, b): return a + b
来源：http://cf.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ds.nszjky.cn

JS:   function add(a, b) { return a + b; }
来源：http://pg.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lk.chemitech.net.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://kb.bjjhwx.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zc.shxzukj.cn

Ruby: def add(a, b); a + b; end
来源：http://vl.lnxyls.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rk.521024.cn

[C02] 默认参数
来源：http://pi.asd995.cn

Py:   def greet(name="World"): return name
来源：http://vq.nicolike.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yz.huixiangedu.cn

JS:   function greet(name = "World") { return name; }
来源：http://nj.nszjky.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ok.521024.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zn.asd995.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dc.nicolike.cn

Ruby: def greet(name = "World") = name
来源：http://lr.yuexingan06.cn

C#:   string Greet(string name = "World") => name;
来源：http://oa.huixinmuqiang.cn

[C03] 可变参数
来源：http://xu.shtwfgs.cn

Py:   def total(*args): return sum(args)
来源：http://ir.bookmarksfly.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sv.bjjhwx.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://uc.yuntaijiaju.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pw.newstarts.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wj.bookmarksfly.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nv.gzmigu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://id.newstarts.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tw.huanxung.cn

[C04] 命名参数 / 关键字参数
来源：http://ei.panjiajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qb.wgjwhj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://je.yuexingan06.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cf.yuexingan06.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yx.shtwfgs.cn

Java: // 无：用 Builder 模式或 record
来源：http://fc.hahajie.cn

Go:   // 无：用配置结构体参数
来源：http://ih.jianghongdianzi.cn

Ruby: f(a: 1, b: 2)
来源：http://cf.521024.cn

C#:   f(a: 1, b: 2)
来源：http://pg.wgjwhj.cn

[C05] 返回多个值
来源：http://oh.jianghongdianzi.cn

Py:   return a, b
来源：http://oj.shxzskj.cn

PHP:  return [$a, $b];
来源：http://dh.wgjwhj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xg.jianghongdianzi.cn

TS:   return { a, b };
来源：http://fd.521024.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dt.szsharing.cn

Go:   return a, b
来源：http://ig.jctech888.com.cn

Ruby: return a, b
来源：http://hi.hnjuh.cn

C#:   return (a, b);              // ValueTuple
来源：http://qn.shxzukj.cn

[C06] 匿名函数 / lambda
来源：http://rp.szxytkj.cn

Py:   square = lambda x: x * x
来源：http://sk.asd995.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qa.bookmarksfly.cn

JS:   const square = x => x * x;
来源：http://yj.yuntaijiaju.cn

TS:   const square = (x: number): number => x * x;
来源：http://ip.haigaiapp.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wx.asd995.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gb.hnjuh.cn

Ruby: square = ->(x) { x * x }
来源：http://ty.asd995.cn

C#:   Func<int, int> square = x => x * x;
来源：http://vi.hahajie.cn

[C07] 把函数作为参数传入
来源：http://sb.colortex.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ym.asd995.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ve.nicolike.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://iw.colortex.cn

TS:   arr.map(String)
来源：http://cw.hahajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rv.yuexingan06.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jc.huanxung.cn

Ruby: arr.map(&:upcase)
来源：http://yg.lnxyls.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://me.huanxung.cn

[C08] 闭包
来源：http://zd.gzmigu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vk.panjiajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://um.hnjuh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zo.haigaiapp.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xx.bjjhwx.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hj.huixiangedu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://md.colortex.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qn.panjiajie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://go.shxzukj.cn

[C09] 递归
来源：http://ib.521024.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sa.huanxung.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hj.lnxyls.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rz.hahajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sq.wgjwhj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bt.nicolike.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rx.wgjwhj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://do.nicolike.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ru.jctech888.com.cn

[C10] 变量作用域
来源：http://qb.gzmigu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gt.huanxung.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mw.panjiajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zv.nszjky.cn

TS:   同 JS
来源：http://mu.jctech888.com.cn

Java: 方法内为块级作用域
来源：http://ge.panjiajie.cn

Go:   花括号块级作用域
来源：http://ke.shtwfgs.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ul.szsharing.cn

C#:   块级作用域
来源：http://fd.szsharing.cn

[C11] 模块导入与导出
来源：http://vp.nicolike.cn

Py:   from module import func
来源：http://rt.bjjhwx.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://il.lnxyls.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://cd.wgjwhj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sd.yuntaijiaju.cn

Java: import java.util.List;
来源：http://io.nicolike.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ts.nszjky.cn

Ruby: require "json"; require_relative "./util"
来源：http://bp.jctech888.com.cn

C#:   using System.Text;
来源：http://go.szxytkj.cn

[C12] 立即执行函数 IIFE
来源：http://kc.huixiangedu.cn

Py:   (lambda: print("run"))()
来源：http://fe.shtwfgs.cn

PHP:  (function () { echo "run"; })();
来源：http://nt.muxihuayi.cn

JS:   (() => { console.log("run"); })();
来源：http://ts.nszjky.cn

TS:   (() => { console.log("run"); })();
来源：http://ry.hnjuh.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://al.yuntaijiaju.cn

Go:   func() { fmt.Println("run") }()
来源：http://ly.yuntaijiaju.cn

Ruby: -> { puts "run" }.call
来源：http://wj.bookmarksfly.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zw.bjjhwx.cn

[C13] 类型声明 / 类型注解
来源：http://uu.szxytkj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xk.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cg.szsharing.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rp.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tm.jctech888.com.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cu.jianghongdianzi.cn

Go:   func add(a, b int) int
来源：http://zf.huixiangedu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fj.hnjuh.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qu.hahajie.cn

[C14] 泛型函数
来源：http://ea.chemitech.net.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vt.newstarts.cn

PHP:  // 无泛型
来源：http://he.gzmigu.cn

JS:   // 无泛型
来源：http://gg.chemitech.net.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://la.9csxet.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cx.szsharing.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cf.yuexingan06.cn

Ruby: # 无泛型
来源：http://rg.muxihuayi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pf.yuntaijiaju.cn

[C15] 解构 / 展开参数
来源：http://he.newstarts.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tw.muxihuayi.cn

PHP:  [$a, $b] = $pair;
来源：http://wx.huixiangedu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bx.szsharing.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ac.szsharing.cn

Java: // 无解构
来源：http://it.hahajie.cn

Go:   // 无解构
来源：http://hv.huixiangedu.cn

Ruby: a, b = pair
来源：http://hn.nszjky.cn

C#:   var (a, b) = pair;
来源：http://cg.wgjwhj.cn

[C16] 函数 / 方法重载
来源：http://kr.gzmigu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://uf.9csxet.cn


<!-- 参考信息 -->