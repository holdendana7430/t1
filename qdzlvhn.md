代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rq.hahajie.cn

================================================================================
来源：http://nh.521024.cn

B. 流程控制
来源：http://qj.bookmarksfly.cn

================================================================================
来源：http://fp.panjiajie.cn

[B01] 条件判断 if / else
来源：http://ob.panjiajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hs.yuexingan06.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kh.shtwfgs.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hu.huixiangedu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://of.colortex.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://mb.chemitech.net.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bu.huanxung.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rq.nicolike.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ph.yuexingan06.cn

[B02] 多分支 else if / elif
来源：http://qv.shxzskj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bk.huanxung.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hx.chemitech.net.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sv.huanxung.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rw.haigaiapp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cl.bjjhwx.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tj.jctech888.com.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://iz.bookmarksfly.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zs.9csxet.cn

[B03] switch / match / case
来源：http://ak.szsharing.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ch.bookmarksfly.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xe.wgjwhj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bn.jctech888.com.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vf.gzmigu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zi.panjiajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hi.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qa.huanxung.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vj.hnjuh.cn

[B04] for 计数循环
来源：http://tr.shtwfgs.cn

Py:   for i in range(10): print(i)
来源：http://wh.hahajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vm.hahajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lp.bookmarksfly.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zk.szsharing.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ym.huixiangedu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hs.newstarts.cn

Ruby: 10.times { |i| puts i }
来源：http://tz.newstarts.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xf.jianghongdianzi.cn

[B05] 遍历数组 / 列表
来源：http://ac.bookmarksfly.cn

Py:   for item in arr: print(item)
来源：http://xp.lnxyls.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://su.haigaiapp.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://bl.gzmigu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://os.asd995.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jc.wgjwhj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hh.shxzskj.cn

Ruby: arr.each { |item| puts item }
来源：http://ph.chemitech.net.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pe.yuntaijiaju.cn

[B06] 遍历字典 / 对象
来源：http://qd.wgjwhj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mv.bookmarksfly.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://se.chemitech.net.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dv.shtwfgs.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pb.yuntaijiaju.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jt.newstarts.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zo.shtwfgs.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://su.wgjwhj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ll.gzmigu.cn

[B07] while 循环
来源：http://xe.colortex.cn

Py:   while i < 10: i += 1
来源：http://wq.hahajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://uf.newstarts.cn

JS:   while (i < 10) { i++; }
来源：http://gr.jctech888.com.cn

TS:   while (i < 10) { i++; }
来源：http://gh.521024.cn

Java: while (i < 10) { i++; }
来源：http://dz.jctech888.com.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gl.yuexingan06.cn

Ruby: while i < 10; i += 1; end
来源：http://pd.bjjhwx.cn

C#:   while (i < 10) { i++; }
来源：http://js.huixiangedu.cn

[B08] do-while（至少执行一次）
来源：http://an.haigaiapp.cn

Py:   # 无 do-while：用 while True + break
来源：http://tx.nicolike.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ku.panjiajie.cn

JS:   do { i++; } while (i < 10);
来源：http://sg.asd995.cn

TS:   do { i++; } while (i < 10);
来源：http://dd.lnxyls.cn

Java: do { i++; } while (i < 10);
来源：http://wv.hnjuh.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://lc.gzmigu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mx.colortex.cn

C#:   do { i++; } while (i < 10);
来源：http://zz.szxytkj.cn

[B09] break 与 continue
来源：http://ex.shtwfgs.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://an.newstarts.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ts.yuntaijiaju.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oy.wgjwhj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zl.newstarts.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cc.haigaiapp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dy.yuexingan06.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://md.lnxyls.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ci.huanxung.cn

[B10] 遍历同时拿索引
来源：http://pz.muxihuayi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ks.hahajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ed.shtwfgs.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yj.gzmigu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ml.haigaiapp.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jv.nicolike.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xr.shxzskj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://te.yuntaijiaju.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zl.asd995.cn

[B11] 生成数字序列 / 区间
来源：http://er.szsharing.cn

Py:   list(range(0, 10, 2))
来源：http://at.gzmigu.cn

PHP:  range(0, 10, 2);
来源：http://ud.panjiajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kb.jctech888.com.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://us.nicolike.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gs.huixinmuqiang.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://we.huanxung.cn

Ruby: (0...10).step(2).to_a
来源：http://di.huixinmuqiang.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ya.jctech888.com.cn

[B12] 跳出多层循环
来源：http://mq.gzmigu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yz.yuntaijiaju.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://rb.chemitech.net.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://to.szxytkj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wx.huanxung.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hp.jctech888.com.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nm.wgjwhj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gm.wgjwhj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ez.muxihuayi.cn

[B13] 判断是否为数字
来源：http://kn.shxzskj.cn

Py:   isinstance(x, (int, float))
来源：http://du.shtwfgs.cn

PHP:  is_numeric($x)
来源：http://xh.szxytkj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zw.huanxung.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hp.shxzskj.cn

Java: x instanceof Number
来源：http://xr.yuexingan06.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cg.nszjky.cn

Ruby: x.is_a?(Numeric)
来源：http://nu.asd995.cn

C#:   x is int or double or decimal
来源：http://in.bjjhwx.cn

[B14] 判断值是否在集合内
来源：http://ec.hnjuh.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xt.muxihuayi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gt.yuntaijiaju.cn

JS:   [1, 2, 3].includes(x)
来源：http://jz.9csxet.cn

TS:   [1, 2, 3].includes(x)
来源：http://sg.nicolike.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rn.521024.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fk.bjjhwx.cn

Ruby: [1, 2, 3].include?(x)
来源：http://od.huixiangedu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kt.asd995.cn

[B15] 布尔运算与取反
来源：http://nq.nicolike.cn

Py:   a and b or not c
来源：http://dz.chemitech.net.cn

PHP:  $a && $b || !$c
来源：http://mm.huixinmuqiang.cn

JS:   a && b || !c
来源：http://tt.hahajie.cn

TS:   a && b || !c
来源：http://dx.jianghongdianzi.cn

Java: a && b || !c
来源：http://nl.panjiajie.cn

Go:   a && b || !c
来源：http://nj.9csxet.cn

Ruby: a && b || !c
来源：http://ep.hahajie.cn

C#:   a && b || !c
来源：http://yc.szxytkj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bd.shxzskj.cn

Py:   if not data: return
来源：http://qh.lnxyls.cn

PHP:  if (!$data) { return; }
来源：http://rm.huanxung.cn

JS:   if (!data) return;
来源：http://yo.9csxet.cn

TS:   if (!data) return;
来源：http://mf.bookmarksfly.cn

Java: if (data == null) return;
来源：http://ph.jctech888.com.cn

Go:   if data == nil { return }
来源：http://nv.lnxyls.cn

Ruby: return if data.nil?
来源：http://ro.nszjky.cn

C#:   if (data == null) return;
来源：http://hg.shxzukj.cn

================================================================================
来源：http://lm.hahajie.cn

C. 函数与作用域
来源：http://te.nszjky.cn

================================================================================
来源：http://ix.hnjuh.cn

[C01] 定义函数
来源：http://qy.yuntaijiaju.cn

Py:   def add(a, b): return a + b
来源：http://in.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wb.gzmigu.cn

JS:   function add(a, b) { return a + b; }
来源：http://kp.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zm.newstarts.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://me.muxihuayi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rx.szsharing.cn

Ruby: def add(a, b); a + b; end
来源：http://eu.shtwfgs.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://om.muxihuayi.cn

[C02] 默认参数
来源：http://ez.asd995.cn

Py:   def greet(name="World"): return name
来源：http://pl.muxihuayi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://so.521024.cn

JS:   function greet(name = "World") { return name; }
来源：http://dh.yuntaijiaju.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vr.jctech888.com.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://pm.nszjky.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vb.colortex.cn

Ruby: def greet(name = "World") = name
来源：http://wd.yuntaijiaju.cn

C#:   string Greet(string name = "World") => name;
来源：http://vh.bjjhwx.cn

[C03] 可变参数
来源：http://mz.colortex.cn

Py:   def total(*args): return sum(args)
来源：http://uc.wgjwhj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hr.asd995.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jo.huixinmuqiang.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://oa.9csxet.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kg.jianghongdianzi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://my.szsharing.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tj.jctech888.com.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://si.hnjuh.cn

[C04] 命名参数 / 关键字参数
来源：http://fc.521024.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sr.huixinmuqiang.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vd.szxytkj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://en.shtwfgs.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ui.bjjhwx.cn

Java: // 无：用 Builder 模式或 record
来源：http://kl.hnjuh.cn

Go:   // 无：用配置结构体参数
来源：http://mj.gzmigu.cn

Ruby: f(a: 1, b: 2)
来源：http://qy.chemitech.net.cn

C#:   f(a: 1, b: 2)
来源：http://uu.yuexingan06.cn

[C05] 返回多个值
来源：http://rv.hahajie.cn

Py:   return a, b
来源：http://yv.panjiajie.cn

PHP:  return [$a, $b];
来源：http://cz.colortex.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://tq.chemitech.net.cn

TS:   return { a, b };
来源：http://qo.jctech888.com.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ik.hahajie.cn

Go:   return a, b
来源：http://nv.hnjuh.cn

Ruby: return a, b
来源：http://fw.shxzskj.cn

C#:   return (a, b);              // ValueTuple
来源：http://xd.huanxung.cn

[C06] 匿名函数 / lambda
来源：http://ec.szsharing.cn

Py:   square = lambda x: x * x
来源：http://hh.hnjuh.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ri.bjjhwx.cn

JS:   const square = x => x * x;
来源：http://hd.nszjky.cn

TS:   const square = (x: number): number => x * x;
来源：http://ao.szxytkj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gn.wgjwhj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://bw.chemitech.net.cn

Ruby: square = ->(x) { x * x }
来源：http://ck.bookmarksfly.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ho.chemitech.net.cn

[C07] 把函数作为参数传入
来源：http://pg.hahajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://el.szsharing.cn

PHP:  array_map("strtoupper", $arr);
来源：http://gn.newstarts.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rq.jctech888.com.cn

TS:   arr.map(String)
来源：http://br.panjiajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fs.huanxung.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ah.yuntaijiaju.cn

Ruby: arr.map(&:upcase)
来源：http://ne.muxihuayi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fp.szsharing.cn

[C08] 闭包
来源：http://px.gzmigu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://sy.bjjhwx.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zq.shxzukj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://un.jctech888.com.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rw.shtwfgs.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qj.shxzskj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://va.yuntaijiaju.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uu.jctech888.com.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tl.newstarts.cn

[C09] 递归
来源：http://zn.yuntaijiaju.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yq.shtwfgs.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bt.szxytkj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ct.asd995.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oq.shxzukj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jd.wgjwhj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ds.haigaiapp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lo.nicolike.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wc.haigaiapp.cn

[C10] 变量作用域
来源：http://tp.shxzskj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ru.szxytkj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fa.shxzskj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rt.huixiangedu.cn

TS:   同 JS
来源：http://cl.huixinmuqiang.cn

Java: 方法内为块级作用域
来源：http://ko.jianghongdianzi.cn

Go:   花括号块级作用域
来源：http://vy.9csxet.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://si.newstarts.cn

C#:   块级作用域
来源：http://bh.hnjuh.cn

[C11] 模块导入与导出
来源：http://ol.shtwfgs.cn

Py:   from module import func
来源：http://yx.yuntaijiaju.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xf.newstarts.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://lc.jctech888.com.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rm.haigaiapp.cn

Java: import java.util.List;
来源：http://hp.bookmarksfly.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bc.huixinmuqiang.cn

Ruby: require "json"; require_relative "./util"
来源：http://pf.shxzukj.cn

C#:   using System.Text;
来源：http://mq.newstarts.cn

[C12] 立即执行函数 IIFE
来源：http://kt.shtwfgs.cn

Py:   (lambda: print("run"))()
来源：http://ee.bjjhwx.cn

PHP:  (function () { echo "run"; })();
来源：http://pq.521024.cn

JS:   (() => { console.log("run"); })();
来源：http://ma.panjiajie.cn

TS:   (() => { console.log("run"); })();
来源：http://ml.chemitech.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xs.huanxung.cn

Go:   func() { fmt.Println("run") }()
来源：http://fx.chemitech.net.cn

Ruby: -> { puts "run" }.call
来源：http://vl.muxihuayi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ji.yuexingan06.cn

[C13] 类型声明 / 类型注解
来源：http://vp.huanxung.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cn.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ac.hahajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dr.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bh.9csxet.cn

Java: int add(int a, int b) { return a + b; }
来源：http://er.szsharing.cn

Go:   func add(a, b int) int
来源：http://ux.muxihuayi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pe.jctech888.com.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xb.521024.cn

[C14] 泛型函数
来源：http://ad.szxytkj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cx.521024.cn

PHP:  // 无泛型
来源：http://ra.lnxyls.cn

JS:   // 无泛型
来源：http://pj.panjiajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bu.asd995.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nm.huixinmuqiang.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mt.szsharing.cn

Ruby: # 无泛型
来源：http://sj.gzmigu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zv.nszjky.cn

[C15] 解构 / 展开参数
来源：http://ug.newstarts.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ct.huixinmuqiang.cn

PHP:  [$a, $b] = $pair;
来源：http://tt.colortex.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uj.chemitech.net.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kc.huixinmuqiang.cn

Java: // 无解构
来源：http://tw.yuntaijiaju.cn

Go:   // 无解构
来源：http://ur.szsharing.cn

Ruby: a, b = pair
来源：http://ff.bookmarksfly.cn

C#:   var (a, b) = pair;
来源：http://xq.shxzskj.cn

[C16] 函数 / 方法重载
来源：http://cq.szsharing.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rw.yuexingan06.cn

PHP:  // 无重载
来源：http://cg.nicolike.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://db.521024.cn

TS:   // 用联合类型或重载签名声明
来源：http://ho.panjiajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://mw.yuntaijiaju.cn

Go:   // 无重载：用不同函数名
来源：http://os.shxzskj.cn

Ruby: # 无重载：靠动态参数
来源：http://dy.nicolike.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mp.9csxet.cn

================================================================================
来源：http://sv.yuntaijiaju.cn

D. 数组 / 列表 / 集合
来源：http://vm.shxzukj.cn

================================================================================
来源：http://sg.nicolike.cn

[D01] 创建数组 / 列表
来源：http://sf.huixinmuqiang.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mx.9csxet.cn


<!-- 参考信息 -->