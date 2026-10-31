代发 wailian999

[B01] 条件判断 if / else
来源：http://bj.szxytkj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bw.shxzskj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jn.huixinmuqiang.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bn.hnjuh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://no.panjiajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://jt.shxzskj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://px.panjiajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cj.chemitech.net.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qy.jctech888.com.cn

[B02] 多分支 else if / elif
来源：http://ce.9csxet.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tt.yuntaijiaju.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gc.muxihuayi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nr.bjjhwx.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jp.gzmigu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gs.9csxet.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cg.yuntaijiaju.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zy.newstarts.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yi.nszjky.cn

[B03] switch / match / case
来源：http://jd.jianghongdianzi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kn.yuexingan06.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pu.9csxet.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dm.newstarts.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qn.bookmarksfly.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ao.newstarts.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ri.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://no.wgjwhj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dm.lnxyls.cn

[B04] for 计数循环
来源：http://ua.muxihuayi.cn

Py:   for i in range(10): print(i)
来源：http://yz.asd995.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://oh.newstarts.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fz.521024.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gw.bookmarksfly.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kr.colortex.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://km.9csxet.cn

Ruby: 10.times { |i| puts i }
来源：http://kg.gzmigu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ay.bookmarksfly.cn

[B05] 遍历数组 / 列表
来源：http://op.521024.cn

Py:   for item in arr: print(item)
来源：http://de.shxzukj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ma.shtwfgs.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://bo.huixinmuqiang.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://px.shxzskj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://kn.chemitech.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zh.521024.cn

Ruby: arr.each { |item| puts item }
来源：http://fx.hnjuh.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://li.chemitech.net.cn

[B06] 遍历字典 / 对象
来源：http://mg.newstarts.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sl.shtwfgs.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bj.hnjuh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oa.shxzskj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zo.colortex.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://au.9csxet.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zv.huixinmuqiang.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qi.bjjhwx.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jm.lnxyls.cn

[B07] while 循环
来源：http://qp.panjiajie.cn

Py:   while i < 10: i += 1
来源：http://ky.nszjky.cn

PHP:  while ($i < 10) { $i++; }
来源：http://rv.szxytkj.cn

JS:   while (i < 10) { i++; }
来源：http://zx.bjjhwx.cn

TS:   while (i < 10) { i++; }
来源：http://in.huixiangedu.cn

Java: while (i < 10) { i++; }
来源：http://gb.panjiajie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mq.hnjuh.cn

Ruby: while i < 10; i += 1; end
来源：http://pk.bjjhwx.cn

C#:   while (i < 10) { i++; }
来源：http://bn.521024.cn

[B08] do-while（至少执行一次）
来源：http://wp.gzmigu.cn

Py:   # 无 do-while：用 while True + break
来源：http://hz.shxzukj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://tf.gzmigu.cn

JS:   do { i++; } while (i < 10);
来源：http://zf.gzmigu.cn

TS:   do { i++; } while (i < 10);
来源：http://mw.nszjky.cn

Java: do { i++; } while (i < 10);
来源：http://jh.szsharing.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://za.newstarts.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mx.colortex.cn

C#:   do { i++; } while (i < 10);
来源：http://ov.panjiajie.cn

[B09] break 与 continue
来源：http://pa.colortex.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ld.wgjwhj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://np.shxzskj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kd.shtwfgs.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hn.gzmigu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uv.huixiangedu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ce.szxytkj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sm.gzmigu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dr.gzmigu.cn

[B10] 遍历同时拿索引
来源：http://wo.szsharing.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://go.haigaiapp.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rp.jianghongdianzi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yo.nicolike.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ac.lnxyls.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sl.521024.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bd.huixinmuqiang.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zq.huanxung.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zu.shxzukj.cn

[B11] 生成数字序列 / 区间
来源：http://nc.szsharing.cn

Py:   list(range(0, 10, 2))
来源：http://ua.lnxyls.cn

PHP:  range(0, 10, 2);
来源：http://bj.shxzukj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ze.bookmarksfly.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fl.newstarts.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kb.shxzukj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lp.shxzskj.cn

Ruby: (0...10).step(2).to_a
来源：http://we.shxzukj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ml.huixiangedu.cn

[B12] 跳出多层循环
来源：http://xg.huanxung.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hu.chemitech.net.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wy.panjiajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bj.panjiajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mr.shxzskj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://df.asd995.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://eg.bjjhwx.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yp.bookmarksfly.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qb.szxytkj.cn

[B13] 判断是否为数字
来源：http://nk.521024.cn

Py:   isinstance(x, (int, float))
来源：http://or.nicolike.cn

PHP:  is_numeric($x)
来源：http://qm.nszjky.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ih.nszjky.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ow.colortex.cn

Java: x instanceof Number
来源：http://wn.huixinmuqiang.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://re.jianghongdianzi.cn

Ruby: x.is_a?(Numeric)
来源：http://oj.newstarts.cn

C#:   x is int or double or decimal
来源：http://nc.jctech888.com.cn

[B14] 判断值是否在集合内
来源：http://qp.shxzskj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ng.huanxung.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oi.lnxyls.cn

JS:   [1, 2, 3].includes(x)
来源：http://mq.9csxet.cn

TS:   [1, 2, 3].includes(x)
来源：http://wc.haigaiapp.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xv.panjiajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rv.panjiajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qo.yuexingan06.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nk.nicolike.cn

[B15] 布尔运算与取反
来源：http://fm.nszjky.cn

Py:   a and b or not c
来源：http://mk.szsharing.cn

PHP:  $a && $b || !$c
来源：http://oo.colortex.cn

JS:   a && b || !c
来源：http://uc.jianghongdianzi.cn

TS:   a && b || !c
来源：http://oa.jctech888.com.cn

Java: a && b || !c
来源：http://bo.yuntaijiaju.cn

Go:   a && b || !c
来源：http://ti.newstarts.cn

Ruby: a && b || !c
来源：http://nv.colortex.cn

C#:   a && b || !c
来源：http://lv.huixiangedu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://es.shtwfgs.cn

Py:   if not data: return
来源：http://fd.hahajie.cn

PHP:  if (!$data) { return; }
来源：http://wf.huixiangedu.cn

JS:   if (!data) return;
来源：http://pn.9csxet.cn

TS:   if (!data) return;
来源：http://fq.muxihuayi.cn

Java: if (data == null) return;
来源：http://rg.nicolike.cn

Go:   if data == nil { return }
来源：http://ys.shxzskj.cn

Ruby: return if data.nil?
来源：http://ib.yuexingan06.cn

C#:   if (data == null) return;
来源：http://sn.yuntaijiaju.cn

================================================================================
来源：http://yl.muxihuayi.cn

C. 函数与作用域
来源：http://to.shxzukj.cn

================================================================================
来源：http://aq.huixinmuqiang.cn

[C01] 定义函数
来源：http://gd.shxzskj.cn

Py:   def add(a, b): return a + b
来源：http://px.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rj.hnjuh.cn

JS:   function add(a, b) { return a + b; }
来源：http://pm.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yf.hnjuh.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ay.bjjhwx.cn

Go:   func add(a, b int) int { return a + b }
来源：http://bu.nszjky.cn

Ruby: def add(a, b); a + b; end
来源：http://nl.huixiangedu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ec.newstarts.cn

[C02] 默认参数
来源：http://ke.nicolike.cn

Py:   def greet(name="World"): return name
来源：http://oy.huixiangedu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qo.hnjuh.cn

JS:   function greet(name = "World") { return name; }
来源：http://vb.wgjwhj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wd.chemitech.net.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dy.huixiangedu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ti.521024.cn

Ruby: def greet(name = "World") = name
来源：http://rj.shtwfgs.cn

C#:   string Greet(string name = "World") => name;
来源：http://ck.bjjhwx.cn

[C03] 可变参数
来源：http://mv.jctech888.com.cn

Py:   def total(*args): return sum(args)
来源：http://rd.lnxyls.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vi.wgjwhj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hl.bookmarksfly.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hs.huanxung.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jp.nicolike.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lt.bjjhwx.cn

Ruby: def total(*nums); nums.sum; end
来源：http://le.panjiajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pt.bjjhwx.cn

[C04] 命名参数 / 关键字参数
来源：http://xn.wgjwhj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://le.szsharing.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vw.haigaiapp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cp.colortex.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vj.huanxung.cn

Java: // 无：用 Builder 模式或 record
来源：http://id.haigaiapp.cn

Go:   // 无：用配置结构体参数
来源：http://av.huixinmuqiang.cn

Ruby: f(a: 1, b: 2)
来源：http://dq.huanxung.cn

C#:   f(a: 1, b: 2)
来源：http://aq.yuexingan06.cn

[C05] 返回多个值
来源：http://sg.shxzskj.cn

Py:   return a, b
来源：http://jv.shxzukj.cn

PHP:  return [$a, $b];
来源：http://mi.9csxet.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jq.colortex.cn

TS:   return { a, b };
来源：http://qz.szxytkj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ic.lnxyls.cn

Go:   return a, b
来源：http://va.haigaiapp.cn

Ruby: return a, b
来源：http://je.lnxyls.cn

C#:   return (a, b);              // ValueTuple
来源：http://jz.wgjwhj.cn

[C06] 匿名函数 / lambda
来源：http://zj.huixinmuqiang.cn

Py:   square = lambda x: x * x
来源：http://vv.lnxyls.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://cv.shxzskj.cn

JS:   const square = x => x * x;
来源：http://fy.nszjky.cn

TS:   const square = (x: number): number => x * x;
来源：http://iw.nicolike.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rv.jianghongdianzi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jz.521024.cn

Ruby: square = ->(x) { x * x }
来源：http://aj.jctech888.com.cn

C#:   Func<int, int> square = x => x * x;
来源：http://na.gzmigu.cn

[C07] 把函数作为参数传入
来源：http://oy.nszjky.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yf.huanxung.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xn.hnjuh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ws.hnjuh.cn

TS:   arr.map(String)
来源：http://pb.nicolike.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kb.huixiangedu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ps.colortex.cn

Ruby: arr.map(&:upcase)
来源：http://em.haigaiapp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mi.colortex.cn

[C08] 闭包
来源：http://aw.wgjwhj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nu.yuntaijiaju.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yo.shtwfgs.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vb.nszjky.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://oo.huixiangedu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kq.wgjwhj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ti.shxzskj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ms.jianghongdianzi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rd.gzmigu.cn

[C09] 递归
来源：http://as.hahajie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://es.szxytkj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sm.chemitech.net.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hi.shxzskj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wj.wgjwhj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zu.wgjwhj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://iw.nicolike.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qm.szsharing.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://au.jctech888.com.cn

[C10] 变量作用域
来源：http://ly.panjiajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://oi.asd995.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yx.newstarts.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ko.bookmarksfly.cn

TS:   同 JS
来源：http://oh.lnxyls.cn

Java: 方法内为块级作用域
来源：http://st.szsharing.cn

Go:   花括号块级作用域
来源：http://qq.9csxet.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ki.shxzskj.cn

C#:   块级作用域
来源：http://co.bjjhwx.cn

[C11] 模块导入与导出
来源：http://gy.yuexingan06.cn

Py:   from module import func
来源：http://zq.yuexingan06.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://yg.nszjky.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gm.asd995.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fh.bookmarksfly.cn

Java: import java.util.List;
来源：http://kb.gzmigu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://el.jctech888.com.cn

Ruby: require "json"; require_relative "./util"
来源：http://sp.gzmigu.cn

C#:   using System.Text;
来源：http://oj.hahajie.cn

[C12] 立即执行函数 IIFE
来源：http://ud.hahajie.cn

Py:   (lambda: print("run"))()
来源：http://fr.huanxung.cn

PHP:  (function () { echo "run"; })();
来源：http://mm.szxytkj.cn

JS:   (() => { console.log("run"); })();
来源：http://yc.haigaiapp.cn

TS:   (() => { console.log("run"); })();
来源：http://ug.huixiangedu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rs.yuexingan06.cn

Go:   func() { fmt.Println("run") }()
来源：http://ns.yuexingan06.cn

Ruby: -> { puts "run" }.call
来源：http://gs.shxzukj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://sm.huixiangedu.cn

[C13] 类型声明 / 类型注解
来源：http://mo.muxihuayi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://oo.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ux.huixinmuqiang.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sw.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wx.bjjhwx.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ic.9csxet.cn

Go:   func add(a, b int) int
来源：http://zj.newstarts.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://oz.asd995.cn

C#:   int Add(int a, int b) => a + b;
来源：http://uz.hahajie.cn

[C14] 泛型函数
来源：http://vy.panjiajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yj.panjiajie.cn

PHP:  // 无泛型
来源：http://vu.lnxyls.cn

JS:   // 无泛型
来源：http://ub.bookmarksfly.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zi.nszjky.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://av.nicolike.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ag.nicolike.cn

Ruby: # 无泛型
来源：http://om.521024.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ta.9csxet.cn

[C15] 解构 / 展开参数
来源：http://kp.9csxet.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vx.bookmarksfly.cn

PHP:  [$a, $b] = $pair;
来源：http://hb.lnxyls.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ac.nszjky.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jv.hahajie.cn

Java: // 无解构
来源：http://nc.521024.cn

Go:   // 无解构
来源：http://tw.hahajie.cn

Ruby: a, b = pair
来源：http://cx.bjjhwx.cn

C#:   var (a, b) = pair;
来源：http://ju.shtwfgs.cn

[C16] 函数 / 方法重载
来源：http://co.nicolike.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mr.hnjuh.cn

PHP:  // 无重载
来源：http://sb.jianghongdianzi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zo.haigaiapp.cn

TS:   // 用联合类型或重载签名声明
来源：http://fk.9csxet.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ga.asd995.cn

Go:   // 无重载：用不同函数名
来源：http://aw.huanxung.cn

Ruby: # 无重载：靠动态参数
来源：http://al.asd995.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zj.szsharing.cn

================================================================================
来源：http://xs.gzmigu.cn

D. 数组 / 列表 / 集合
来源：http://dg.shtwfgs.cn

================================================================================
来源：http://ui.jianghongdianzi.cn

[D01] 创建数组 / 列表
来源：http://pl.huanxung.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://uv.nszjky.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ba.shtwfgs.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ur.huanxung.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://rv.gzmigu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lc.szsharing.cn


<!-- 参考信息 -->