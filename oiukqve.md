代发 wailian999

[A26] 类型转换总览
来源：http://yc.hahajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sk.gzmigu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ka.newstarts.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://re.asd995.cn

TS:   Number() String() Boolean() x as number
来源：http://ya.9csxet.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wl.yuexingan06.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hd.nicolike.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://eu.shxzukj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tp.yuntaijiaju.cn

================================================================================
来源：http://ex.szsharing.cn

B. 流程控制
来源：http://vc.wgjwhj.cn

================================================================================
来源：http://fa.huixiangedu.cn

[B01] 条件判断 if / else
来源：http://et.newstarts.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://nq.huanxung.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sg.shxzskj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rn.9csxet.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sl.muxihuayi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://kw.nicolike.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xi.gzmigu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nh.shxzukj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gs.yuexingan06.cn

[B02] 多分支 else if / elif
来源：http://ke.nicolike.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vm.shxzukj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lk.haigaiapp.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ko.hnjuh.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ok.huanxung.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fo.muxihuayi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://go.jianghongdianzi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ou.521024.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cy.yuntaijiaju.cn

[B03] switch / match / case
来源：http://fd.hahajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mv.chemitech.net.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zn.shtwfgs.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jr.chemitech.net.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vw.chemitech.net.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wb.asd995.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://im.shtwfgs.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ay.yuexingan06.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wd.hnjuh.cn

[B04] for 计数循环
来源：http://mx.shxzukj.cn

Py:   for i in range(10): print(i)
来源：http://cr.yuexingan06.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ob.jctech888.com.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gc.szsharing.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ij.nszjky.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://al.lnxyls.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jy.haigaiapp.cn

Ruby: 10.times { |i| puts i }
来源：http://gd.haigaiapp.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://uz.shtwfgs.cn

[B05] 遍历数组 / 列表
来源：http://yv.chemitech.net.cn

Py:   for item in arr: print(item)
来源：http://vo.bookmarksfly.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ig.lnxyls.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://no.hnjuh.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yk.bookmarksfly.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pb.huixiangedu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gu.szsharing.cn

Ruby: arr.each { |item| puts item }
来源：http://xy.bjjhwx.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zx.hahajie.cn

[B06] 遍历字典 / 对象
来源：http://vz.hahajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://es.lnxyls.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bx.szsharing.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wt.shxzskj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bc.yuexingan06.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gb.nszjky.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zz.huixiangedu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ik.hahajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nr.huixiangedu.cn

[B07] while 循环
来源：http://fy.jctech888.com.cn

Py:   while i < 10: i += 1
来源：http://zs.wgjwhj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hi.jctech888.com.cn

JS:   while (i < 10) { i++; }
来源：http://wm.asd995.cn

TS:   while (i < 10) { i++; }
来源：http://be.lnxyls.cn

Java: while (i < 10) { i++; }
来源：http://to.asd995.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pk.yuexingan06.cn

Ruby: while i < 10; i += 1; end
来源：http://rq.jianghongdianzi.cn

C#:   while (i < 10) { i++; }
来源：http://mk.hnjuh.cn

[B08] do-while（至少执行一次）
来源：http://rr.yuexingan06.cn

Py:   # 无 do-while：用 while True + break
来源：http://tq.wgjwhj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ve.shtwfgs.cn

JS:   do { i++; } while (i < 10);
来源：http://ph.szsharing.cn

TS:   do { i++; } while (i < 10);
来源：http://vk.asd995.cn

Java: do { i++; } while (i < 10);
来源：http://cb.yuntaijiaju.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://qx.yuexingan06.cn

Ruby: begin; i += 1; end while i < 10
来源：http://uz.nszjky.cn

C#:   do { i++; } while (i < 10);
来源：http://gj.huanxung.cn

[B09] break 与 continue
来源：http://mx.521024.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ch.szxytkj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ni.521024.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lv.9csxet.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wl.chemitech.net.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yo.bjjhwx.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vf.colortex.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mu.shxzukj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xk.nszjky.cn

[B10] 遍历同时拿索引
来源：http://yq.newstarts.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nu.521024.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ky.panjiajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tn.hnjuh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://su.jctech888.com.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vc.wgjwhj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gz.szsharing.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pf.jianghongdianzi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://em.nszjky.cn

[B11] 生成数字序列 / 区间
来源：http://ml.yuexingan06.cn

Py:   list(range(0, 10, 2))
来源：http://tj.yuntaijiaju.cn

PHP:  range(0, 10, 2);
来源：http://ao.huixinmuqiang.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pt.huixiangedu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cf.9csxet.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ky.lnxyls.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pw.panjiajie.cn

Ruby: (0...10).step(2).to_a
来源：http://vl.hahajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mx.hahajie.cn

[B12] 跳出多层循环
来源：http://uz.yuexingan06.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wq.jianghongdianzi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://cn.lnxyls.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tg.bookmarksfly.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wl.jianghongdianzi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ck.nicolike.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ox.chemitech.net.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hd.chemitech.net.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ri.nicolike.cn

[B13] 判断是否为数字
来源：http://de.shxzskj.cn

Py:   isinstance(x, (int, float))
来源：http://iu.huanxung.cn

PHP:  is_numeric($x)
来源：http://lq.nszjky.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wd.shxzukj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pc.huixiangedu.cn

Java: x instanceof Number
来源：http://he.nszjky.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://st.521024.cn

Ruby: x.is_a?(Numeric)
来源：http://nz.hahajie.cn

C#:   x is int or double or decimal
来源：http://ul.huixinmuqiang.cn

[B14] 判断值是否在集合内
来源：http://eb.szxytkj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zk.szsharing.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kl.newstarts.cn

JS:   [1, 2, 3].includes(x)
来源：http://so.nszjky.cn

TS:   [1, 2, 3].includes(x)
来源：http://ql.nicolike.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://sw.9csxet.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ow.muxihuayi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://nn.521024.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fe.huixiangedu.cn

[B15] 布尔运算与取反
来源：http://bf.wgjwhj.cn

Py:   a and b or not c
来源：http://yr.bjjhwx.cn

PHP:  $a && $b || !$c
来源：http://lh.nszjky.cn

JS:   a && b || !c
来源：http://nq.szsharing.cn

TS:   a && b || !c
来源：http://ip.colortex.cn

Java: a && b || !c
来源：http://fg.hahajie.cn

Go:   a && b || !c
来源：http://ns.gzmigu.cn

Ruby: a && b || !c
来源：http://ry.nszjky.cn

C#:   a && b || !c
来源：http://gp.hnjuh.cn

[B16] 卫语句：不满足条件提前返回
来源：http://in.chemitech.net.cn

Py:   if not data: return
来源：http://cw.shxzskj.cn

PHP:  if (!$data) { return; }
来源：http://an.shxzskj.cn

JS:   if (!data) return;
来源：http://lo.shxzukj.cn

TS:   if (!data) return;
来源：http://ts.jctech888.com.cn

Java: if (data == null) return;
来源：http://ef.hnjuh.cn

Go:   if data == nil { return }
来源：http://tw.jctech888.com.cn

Ruby: return if data.nil?
来源：http://le.9csxet.cn

C#:   if (data == null) return;
来源：http://mu.jianghongdianzi.cn

================================================================================
来源：http://uh.huixiangedu.cn

C. 函数与作用域
来源：http://wl.huanxung.cn

================================================================================
来源：http://kg.wgjwhj.cn

[C01] 定义函数
来源：http://bq.newstarts.cn

Py:   def add(a, b): return a + b
来源：http://xi.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jr.lnxyls.cn

JS:   function add(a, b) { return a + b; }
来源：http://dw.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gl.bookmarksfly.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ao.asd995.cn

Go:   func add(a, b int) int { return a + b }
来源：http://tq.huanxung.cn

Ruby: def add(a, b); a + b; end
来源：http://jj.nszjky.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://om.panjiajie.cn

[C02] 默认参数
来源：http://cd.panjiajie.cn

Py:   def greet(name="World"): return name
来源：http://xd.bookmarksfly.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vj.szxytkj.cn

JS:   function greet(name = "World") { return name; }
来源：http://yw.haigaiapp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://uk.szxytkj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zw.shxzskj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://su.shxzskj.cn

Ruby: def greet(name = "World") = name
来源：http://ms.nicolike.cn

C#:   string Greet(string name = "World") => name;
来源：http://dq.szsharing.cn

[C03] 可变参数
来源：http://gc.szxytkj.cn

Py:   def total(*args): return sum(args)
来源：http://cj.muxihuayi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wp.jianghongdianzi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pi.newstarts.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xa.521024.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://aw.bjjhwx.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bm.huixiangedu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://mg.bjjhwx.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bm.huanxung.cn

[C04] 命名参数 / 关键字参数
来源：http://tq.nicolike.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cf.wgjwhj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://eb.lnxyls.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pv.jianghongdianzi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xl.huixiangedu.cn

Java: // 无：用 Builder 模式或 record
来源：http://un.hnjuh.cn

Go:   // 无：用配置结构体参数
来源：http://ux.bookmarksfly.cn

Ruby: f(a: 1, b: 2)
来源：http://sb.jianghongdianzi.cn

C#:   f(a: 1, b: 2)
来源：http://le.shxzukj.cn

[C05] 返回多个值
来源：http://fi.asd995.cn

Py:   return a, b
来源：http://wb.szxytkj.cn

PHP:  return [$a, $b];
来源：http://sh.nicolike.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fu.szsharing.cn

TS:   return { a, b };
来源：http://gi.szsharing.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xd.szsharing.cn

Go:   return a, b
来源：http://xj.hnjuh.cn

Ruby: return a, b
来源：http://as.huanxung.cn

C#:   return (a, b);              // ValueTuple
来源：http://kn.muxihuayi.cn

[C06] 匿名函数 / lambda
来源：http://uo.bookmarksfly.cn

Py:   square = lambda x: x * x
来源：http://ke.9csxet.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fl.hahajie.cn

JS:   const square = x => x * x;
来源：http://xt.nicolike.cn

TS:   const square = (x: number): number => x * x;
来源：http://nz.colortex.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ch.newstarts.cn

Go:   sq := func(x int) int { return x * x }
来源：http://in.9csxet.cn

Ruby: square = ->(x) { x * x }
来源：http://pv.bookmarksfly.cn

C#:   Func<int, int> square = x => x * x;
来源：http://vn.hnjuh.cn

[C07] 把函数作为参数传入
来源：http://hj.huanxung.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bn.szsharing.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ki.shtwfgs.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://np.shtwfgs.cn

TS:   arr.map(String)
来源：http://yn.jctech888.com.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vm.nszjky.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xo.haigaiapp.cn

Ruby: arr.map(&:upcase)
来源：http://vz.wgjwhj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mx.nszjky.cn

[C08] 闭包
来源：http://bv.nicolike.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ni.nicolike.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tj.huixiangedu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jm.jctech888.com.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://in.hahajie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ht.panjiajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vf.chemitech.net.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ri.huanxung.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kc.muxihuayi.cn

[C09] 递归
来源：http://xi.shxzskj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://af.szsharing.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bt.muxihuayi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vw.nicolike.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rm.lnxyls.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xs.muxihuayi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pa.yuexingan06.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://oq.jianghongdianzi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lj.chemitech.net.cn

[C10] 变量作用域
来源：http://xg.newstarts.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vr.muxihuayi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rr.asd995.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://iy.shxzukj.cn

TS:   同 JS
来源：http://qy.gzmigu.cn

Java: 方法内为块级作用域
来源：http://te.gzmigu.cn

Go:   花括号块级作用域
来源：http://du.shxzukj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kt.huixinmuqiang.cn

C#:   块级作用域
来源：http://cb.shtwfgs.cn

[C11] 模块导入与导出
来源：http://zu.wgjwhj.cn

Py:   from module import func
来源：http://er.panjiajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kf.521024.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kz.haigaiapp.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://id.9csxet.cn

Java: import java.util.List;
来源：http://si.colortex.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ws.521024.cn

Ruby: require "json"; require_relative "./util"
来源：http://ov.colortex.cn

C#:   using System.Text;
来源：http://qj.shtwfgs.cn

[C12] 立即执行函数 IIFE
来源：http://sy.hnjuh.cn

Py:   (lambda: print("run"))()
来源：http://xc.hnjuh.cn

PHP:  (function () { echo "run"; })();
来源：http://fw.haigaiapp.cn

JS:   (() => { console.log("run"); })();
来源：http://ao.jianghongdianzi.cn

TS:   (() => { console.log("run"); })();
来源：http://pz.panjiajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://et.bookmarksfly.cn

Go:   func() { fmt.Println("run") }()
来源：http://xq.521024.cn

Ruby: -> { puts "run" }.call
来源：http://lj.nszjky.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://dg.hnjuh.cn

[C13] 类型声明 / 类型注解
来源：http://hf.wgjwhj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://az.muxihuayi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fi.shtwfgs.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vv.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ob.wgjwhj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://pv.asd995.cn

Go:   func add(a, b int) int
来源：http://wk.hnjuh.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://df.lnxyls.cn

C#:   int Add(int a, int b) => a + b;
来源：http://pk.shtwfgs.cn

[C14] 泛型函数
来源：http://wu.jctech888.com.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ek.yuntaijiaju.cn

PHP:  // 无泛型
来源：http://dt.521024.cn

JS:   // 无泛型
来源：http://ci.muxihuayi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yj.shxzskj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vl.huixinmuqiang.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vy.haigaiapp.cn

Ruby: # 无泛型
来源：http://mo.huixiangedu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ho.gzmigu.cn

[C15] 解构 / 展开参数
来源：http://lb.lnxyls.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fz.hahajie.cn

PHP:  [$a, $b] = $pair;
来源：http://zw.bjjhwx.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ph.shxzukj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tm.9csxet.cn

Java: // 无解构
来源：http://yr.nszjky.cn

Go:   // 无解构
来源：http://bp.muxihuayi.cn

Ruby: a, b = pair
来源：http://pr.huixiangedu.cn

C#:   var (a, b) = pair;
来源：http://hh.panjiajie.cn

[C16] 函数 / 方法重载
来源：http://bd.521024.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jh.haigaiapp.cn

PHP:  // 无重载
来源：http://wj.nicolike.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://we.huanxung.cn

TS:   // 用联合类型或重载签名声明
来源：http://ft.jctech888.com.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://mn.colortex.cn


<!-- 参考信息 -->