代发 wailian999

[A26] 类型转换总览
来源：http://kj.bjjhwx.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mk.wgjwhj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yk.shxzukj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ex.wgjwhj.cn

TS:   Number() String() Boolean() x as number
来源：http://au.shxzukj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hq.gzmigu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pl.yuexingan06.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lo.wgjwhj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vc.shxzukj.cn

================================================================================
来源：http://br.asd995.cn

B. 流程控制
来源：http://dy.yuexingan06.cn

================================================================================
来源：http://jl.hahajie.cn

[B01] 条件判断 if / else
来源：http://bt.jianghongdianzi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://rz.huixinmuqiang.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ub.nszjky.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pz.bjjhwx.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://op.jianghongdianzi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ij.huanxung.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wa.nszjky.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hd.huixiangedu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hg.huixinmuqiang.cn

[B02] 多分支 else if / elif
来源：http://kr.huixiangedu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fh.nszjky.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pf.521024.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tv.shxzskj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cd.asd995.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sz.newstarts.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wb.bookmarksfly.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ph.lnxyls.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ic.shxzukj.cn

[B03] switch / match / case
来源：http://pu.chemitech.net.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fr.bjjhwx.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fb.chemitech.net.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zl.bjjhwx.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vi.jctech888.com.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kr.yuntaijiaju.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gi.shtwfgs.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bo.muxihuayi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mi.lnxyls.cn

[B04] for 计数循环
来源：http://if.huixinmuqiang.cn

Py:   for i in range(10): print(i)
来源：http://kd.hnjuh.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ec.jctech888.com.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gy.9csxet.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uh.jctech888.com.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wg.shtwfgs.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wo.hahajie.cn

Ruby: 10.times { |i| puts i }
来源：http://hz.bookmarksfly.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ga.muxihuayi.cn

[B05] 遍历数组 / 列表
来源：http://rn.hnjuh.cn

Py:   for item in arr: print(item)
来源：http://ik.gzmigu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qm.jianghongdianzi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wk.szxytkj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mw.bjjhwx.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vt.yuexingan06.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ul.shxzskj.cn

Ruby: arr.each { |item| puts item }
来源：http://xu.panjiajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xn.yuexingan06.cn

[B06] 遍历字典 / 对象
来源：http://uw.szsharing.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sg.hahajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zs.asd995.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jh.huixiangedu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ff.nicolike.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yx.bookmarksfly.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bt.yuntaijiaju.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jq.bjjhwx.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zs.lnxyls.cn

[B07] while 循环
来源：http://ln.hnjuh.cn

Py:   while i < 10: i += 1
来源：http://kr.chemitech.net.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ww.szxytkj.cn

JS:   while (i < 10) { i++; }
来源：http://vf.hahajie.cn

TS:   while (i < 10) { i++; }
来源：http://rs.szxytkj.cn

Java: while (i < 10) { i++; }
来源：http://qp.yuntaijiaju.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qw.huixiangedu.cn

Ruby: while i < 10; i += 1; end
来源：http://sn.521024.cn

C#:   while (i < 10) { i++; }
来源：http://am.huixinmuqiang.cn

[B08] do-while（至少执行一次）
来源：http://al.colortex.cn

Py:   # 无 do-while：用 while True + break
来源：http://zz.9csxet.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pj.muxihuayi.cn

JS:   do { i++; } while (i < 10);
来源：http://zg.521024.cn

TS:   do { i++; } while (i < 10);
来源：http://ns.colortex.cn

Java: do { i++; } while (i < 10);
来源：http://hn.jianghongdianzi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mo.chemitech.net.cn

Ruby: begin; i += 1; end while i < 10
来源：http://st.nszjky.cn

C#:   do { i++; } while (i < 10);
来源：http://mz.shtwfgs.cn

[B09] break 与 continue
来源：http://zt.shtwfgs.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cr.nszjky.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://va.lnxyls.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vw.yuexingan06.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tt.colortex.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kw.lnxyls.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bd.jctech888.com.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pl.shtwfgs.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lz.lnxyls.cn

[B10] 遍历同时拿索引
来源：http://uv.muxihuayi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://my.nszjky.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wb.lnxyls.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zg.nicolike.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hl.szxytkj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ar.shxzskj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jg.hahajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vn.szsharing.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ro.yuexingan06.cn

[B11] 生成数字序列 / 区间
来源：http://fm.yuexingan06.cn

Py:   list(range(0, 10, 2))
来源：http://sn.9csxet.cn

PHP:  range(0, 10, 2);
来源：http://tr.521024.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pv.huixinmuqiang.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fc.yuexingan06.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ma.haigaiapp.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wg.bookmarksfly.cn

Ruby: (0...10).step(2).to_a
来源：http://zx.shxzukj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rp.9csxet.cn

[B12] 跳出多层循环
来源：http://ub.szsharing.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://nz.huixiangedu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://oa.nszjky.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pb.9csxet.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dq.bookmarksfly.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://er.huanxung.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kw.shxzukj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ji.huixinmuqiang.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://na.shtwfgs.cn

[B13] 判断是否为数字
来源：http://ln.shxzskj.cn

Py:   isinstance(x, (int, float))
来源：http://uk.lnxyls.cn

PHP:  is_numeric($x)
来源：http://ep.huixiangedu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dy.huixinmuqiang.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yi.muxihuayi.cn

Java: x instanceof Number
来源：http://py.hnjuh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ob.nszjky.cn

Ruby: x.is_a?(Numeric)
来源：http://yy.muxihuayi.cn

C#:   x is int or double or decimal
来源：http://vl.colortex.cn

[B14] 判断值是否在集合内
来源：http://vq.shxzukj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yt.wgjwhj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ju.hnjuh.cn

JS:   [1, 2, 3].includes(x)
来源：http://yy.hnjuh.cn

TS:   [1, 2, 3].includes(x)
来源：http://yp.gzmigu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://zr.shtwfgs.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dj.panjiajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://yy.szxytkj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fz.jctech888.com.cn

[B15] 布尔运算与取反
来源：http://ls.521024.cn

Py:   a and b or not c
来源：http://ay.bjjhwx.cn

PHP:  $a && $b || !$c
来源：http://vm.hahajie.cn

JS:   a && b || !c
来源：http://xi.shxzskj.cn

TS:   a && b || !c
来源：http://ew.bookmarksfly.cn

Java: a && b || !c
来源：http://tt.nicolike.cn

Go:   a && b || !c
来源：http://jw.huanxung.cn

Ruby: a && b || !c
来源：http://ri.521024.cn

C#:   a && b || !c
来源：http://ua.gzmigu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://du.gzmigu.cn

Py:   if not data: return
来源：http://xs.szxytkj.cn

PHP:  if (!$data) { return; }
来源：http://kg.colortex.cn

JS:   if (!data) return;
来源：http://xy.jctech888.com.cn

TS:   if (!data) return;
来源：http://cq.szxytkj.cn

Java: if (data == null) return;
来源：http://bu.haigaiapp.cn

Go:   if data == nil { return }
来源：http://dg.hnjuh.cn

Ruby: return if data.nil?
来源：http://ol.newstarts.cn

C#:   if (data == null) return;
来源：http://pu.huanxung.cn

================================================================================
来源：http://jv.szsharing.cn

C. 函数与作用域
来源：http://ei.gzmigu.cn

================================================================================
来源：http://qt.muxihuayi.cn

[C01] 定义函数
来源：http://bs.muxihuayi.cn

Py:   def add(a, b): return a + b
来源：http://cj.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dv.bookmarksfly.cn

JS:   function add(a, b) { return a + b; }
来源：http://xx.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fg.9csxet.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ju.gzmigu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://gs.huixiangedu.cn

Ruby: def add(a, b); a + b; end
来源：http://to.muxihuayi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gn.nszjky.cn

[C02] 默认参数
来源：http://dl.nszjky.cn

Py:   def greet(name="World"): return name
来源：http://si.shtwfgs.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://oo.jctech888.com.cn

JS:   function greet(name = "World") { return name; }
来源：http://zt.colortex.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ob.panjiajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cj.colortex.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yo.521024.cn

Ruby: def greet(name = "World") = name
来源：http://ac.jctech888.com.cn

C#:   string Greet(string name = "World") => name;
来源：http://uv.panjiajie.cn

[C03] 可变参数
来源：http://pe.bjjhwx.cn

Py:   def total(*args): return sum(args)
来源：http://lb.shxzskj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qf.huixiangedu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://se.bookmarksfly.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uh.panjiajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nj.yuexingan06.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vg.wgjwhj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ky.newstarts.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sr.jctech888.com.cn

[C04] 命名参数 / 关键字参数
来源：http://my.bjjhwx.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://df.jctech888.com.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dm.asd995.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qw.gzmigu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hy.muxihuayi.cn

Java: // 无：用 Builder 模式或 record
来源：http://ki.szsharing.cn

Go:   // 无：用配置结构体参数
来源：http://lq.szsharing.cn

Ruby: f(a: 1, b: 2)
来源：http://ey.nicolike.cn

C#:   f(a: 1, b: 2)
来源：http://cw.hahajie.cn

[C05] 返回多个值
来源：http://pd.huixinmuqiang.cn

Py:   return a, b
来源：http://ki.nicolike.cn

PHP:  return [$a, $b];
来源：http://cn.shxzskj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://rt.asd995.cn

TS:   return { a, b };
来源：http://hb.bjjhwx.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xj.newstarts.cn

Go:   return a, b
来源：http://mu.hnjuh.cn

Ruby: return a, b
来源：http://ju.haigaiapp.cn

C#:   return (a, b);              // ValueTuple
来源：http://xq.huanxung.cn

[C06] 匿名函数 / lambda
来源：http://ov.szxytkj.cn

Py:   square = lambda x: x * x
来源：http://mg.yuexingan06.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://yr.szsharing.cn

JS:   const square = x => x * x;
来源：http://zu.szxytkj.cn

TS:   const square = (x: number): number => x * x;
来源：http://sr.haigaiapp.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wp.jianghongdianzi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fc.huixiangedu.cn

Ruby: square = ->(x) { x * x }
来源：http://sl.huanxung.cn

C#:   Func<int, int> square = x => x * x;
来源：http://yg.wgjwhj.cn

[C07] 把函数作为参数传入
来源：http://ll.muxihuayi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fi.szsharing.cn

PHP:  array_map("strtoupper", $arr);
来源：http://sl.bookmarksfly.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hr.yuexingan06.cn

TS:   arr.map(String)
来源：http://kz.gzmigu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cg.yuexingan06.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kq.jianghongdianzi.cn

Ruby: arr.map(&:upcase)
来源：http://wh.hahajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hm.hahajie.cn

[C08] 闭包
来源：http://jp.asd995.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yx.gzmigu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zy.szxytkj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bl.newstarts.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://iz.hnjuh.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yn.bookmarksfly.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lj.nicolike.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cz.huixiangedu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xd.haigaiapp.cn

[C09] 递归
来源：http://qz.gzmigu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sr.huanxung.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fe.huixiangedu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gu.jctech888.com.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bb.huixiangedu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yo.shxzukj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cd.gzmigu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ul.shtwfgs.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rp.yuexingan06.cn

[C10] 变量作用域
来源：http://kv.9csxet.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fl.newstarts.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rf.jctech888.com.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bh.newstarts.cn

TS:   同 JS
来源：http://go.haigaiapp.cn

Java: 方法内为块级作用域
来源：http://dl.hahajie.cn

Go:   花括号块级作用域
来源：http://qj.bookmarksfly.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wz.nicolike.cn

C#:   块级作用域
来源：http://ab.huixinmuqiang.cn

[C11] 模块导入与导出
来源：http://qs.lnxyls.cn

Py:   from module import func
来源：http://my.muxihuayi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pd.bjjhwx.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://me.hnjuh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kx.hnjuh.cn

Java: import java.util.List;
来源：http://fe.jctech888.com.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rj.muxihuayi.cn

Ruby: require "json"; require_relative "./util"
来源：http://ht.newstarts.cn

C#:   using System.Text;
来源：http://ny.muxihuayi.cn

[C12] 立即执行函数 IIFE
来源：http://yd.asd995.cn

Py:   (lambda: print("run"))()
来源：http://kv.panjiajie.cn

PHP:  (function () { echo "run"; })();
来源：http://ar.jctech888.com.cn

JS:   (() => { console.log("run"); })();
来源：http://ev.chemitech.net.cn

TS:   (() => { console.log("run"); })();
来源：http://zs.yuexingan06.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lm.colortex.cn

Go:   func() { fmt.Println("run") }()
来源：http://lf.yuntaijiaju.cn

Ruby: -> { puts "run" }.call
来源：http://wg.hahajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qm.bjjhwx.cn

[C13] 类型声明 / 类型注解
来源：http://mx.hnjuh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nt.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pd.nszjky.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hs.szxytkj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bo.nicolike.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tw.chemitech.net.cn

Go:   func add(a, b int) int
来源：http://ed.hnjuh.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jw.asd995.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ra.panjiajie.cn

[C14] 泛型函数
来源：http://jn.chemitech.net.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://aq.colortex.cn

PHP:  // 无泛型
来源：http://uq.gzmigu.cn

JS:   // 无泛型
来源：http://do.yuexingan06.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ft.hahajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lx.hahajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ch.shxzukj.cn

Ruby: # 无泛型
来源：http://yb.shxzukj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wl.gzmigu.cn

[C15] 解构 / 展开参数
来源：http://zi.shxzskj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qi.nicolike.cn

PHP:  [$a, $b] = $pair;
来源：http://pq.bookmarksfly.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yw.muxihuayi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ny.bookmarksfly.cn

Java: // 无解构
来源：http://ei.lnxyls.cn

Go:   // 无解构
来源：http://vz.huixiangedu.cn

Ruby: a, b = pair
来源：http://ed.shxzskj.cn

C#:   var (a, b) = pair;
来源：http://qx.wgjwhj.cn

[C16] 函数 / 方法重载
来源：http://cr.wgjwhj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ob.asd995.cn

PHP:  // 无重载
来源：http://ld.gzmigu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://oc.wgjwhj.cn

TS:   // 用联合类型或重载签名声明
来源：http://bb.huixiangedu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ld.yuntaijiaju.cn


<!-- 参考信息 -->