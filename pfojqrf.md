代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uv.521024.cn

================================================================================
来源：http://rd.shxzskj.cn

B. 流程控制
来源：http://gn.bjjhwx.cn

================================================================================
来源：http://iw.yuexingan06.cn

[B01] 条件判断 if / else
来源：http://hw.muxihuayi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://zq.shxzukj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tn.jianghongdianzi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fp.haigaiapp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sx.nicolike.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://iu.chemitech.net.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://as.gzmigu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jv.hnjuh.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lq.shxzskj.cn

[B02] 多分支 else if / elif
来源：http://ke.szxytkj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fb.shxzskj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zd.yuntaijiaju.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wi.yuexingan06.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ef.bjjhwx.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rs.chemitech.net.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bj.huixinmuqiang.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kp.newstarts.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://li.hahajie.cn

[B03] switch / match / case
来源：http://xi.gzmigu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://su.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://az.newstarts.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ye.nicolike.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ug.nszjky.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ki.szxytkj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://eo.panjiajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://na.wgjwhj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ub.newstarts.cn

[B04] for 计数循环
来源：http://ez.colortex.cn

Py:   for i in range(10): print(i)
来源：http://dp.shtwfgs.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sq.asd995.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xp.haigaiapp.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xq.huixiangedu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ok.hahajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zi.shxzukj.cn

Ruby: 10.times { |i| puts i }
来源：http://nb.huixiangedu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rv.haigaiapp.cn

[B05] 遍历数组 / 列表
来源：http://ag.hahajie.cn

Py:   for item in arr: print(item)
来源：http://vr.hahajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pu.shxzukj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zd.nszjky.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://oz.shtwfgs.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://bs.szsharing.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sk.huixiangedu.cn

Ruby: arr.each { |item| puts item }
来源：http://ip.bjjhwx.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nh.bookmarksfly.cn

[B06] 遍历字典 / 对象
来源：http://lt.yuntaijiaju.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vz.hnjuh.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vd.jctech888.com.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wi.shxzskj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iz.nicolike.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://te.yuexingan06.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://aw.bjjhwx.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bw.huixinmuqiang.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ln.jctech888.com.cn

[B07] while 循环
来源：http://nf.bookmarksfly.cn

Py:   while i < 10: i += 1
来源：http://hc.huixiangedu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://kc.huanxung.cn

JS:   while (i < 10) { i++; }
来源：http://ka.shxzukj.cn

TS:   while (i < 10) { i++; }
来源：http://cr.lnxyls.cn

Java: while (i < 10) { i++; }
来源：http://tx.yuntaijiaju.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tr.yuntaijiaju.cn

Ruby: while i < 10; i += 1; end
来源：http://nq.colortex.cn

C#:   while (i < 10) { i++; }
来源：http://ox.huixinmuqiang.cn

[B08] do-while（至少执行一次）
来源：http://rq.lnxyls.cn

Py:   # 无 do-while：用 while True + break
来源：http://wg.szsharing.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ne.szsharing.cn

JS:   do { i++; } while (i < 10);
来源：http://iy.gzmigu.cn

TS:   do { i++; } while (i < 10);
来源：http://eh.bookmarksfly.cn

Java: do { i++; } while (i < 10);
来源：http://zl.nszjky.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://rw.haigaiapp.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zz.wgjwhj.cn

C#:   do { i++; } while (i < 10);
来源：http://bx.wgjwhj.cn

[B09] break 与 continue
来源：http://qe.bjjhwx.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tp.521024.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ck.bjjhwx.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rn.shxzukj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yl.bjjhwx.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ox.huixiangedu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cs.wgjwhj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dq.shtwfgs.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zl.wgjwhj.cn

[B10] 遍历同时拿索引
来源：http://cx.shtwfgs.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://iy.shxzskj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tv.gzmigu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://eo.lnxyls.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dh.huanxung.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cd.gzmigu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://el.jianghongdianzi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ze.jianghongdianzi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zq.shxzukj.cn

[B11] 生成数字序列 / 区间
来源：http://ip.yuexingan06.cn

Py:   list(range(0, 10, 2))
来源：http://ih.9csxet.cn

PHP:  range(0, 10, 2);
来源：http://pm.jianghongdianzi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hl.9csxet.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qh.521024.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ar.hnjuh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tc.szsharing.cn

Ruby: (0...10).step(2).to_a
来源：http://hd.gzmigu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fx.shtwfgs.cn

[B12] 跳出多层循环
来源：http://ca.szxytkj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xi.asd995.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://sr.huixinmuqiang.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sx.jianghongdianzi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jt.huixiangedu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xk.nszjky.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pm.muxihuayi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://se.9csxet.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://id.521024.cn

[B13] 判断是否为数字
来源：http://uj.panjiajie.cn

Py:   isinstance(x, (int, float))
来源：http://sn.bookmarksfly.cn

PHP:  is_numeric($x)
来源：http://ia.9csxet.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sj.521024.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ds.haigaiapp.cn

Java: x instanceof Number
来源：http://pm.shtwfgs.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yb.jianghongdianzi.cn

Ruby: x.is_a?(Numeric)
来源：http://xd.521024.cn

C#:   x is int or double or decimal
来源：http://ab.nszjky.cn

[B14] 判断值是否在集合内
来源：http://wi.haigaiapp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dc.gzmigu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nu.shxzukj.cn

JS:   [1, 2, 3].includes(x)
来源：http://jb.hnjuh.cn

TS:   [1, 2, 3].includes(x)
来源：http://xf.wgjwhj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://bo.shxzskj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://iu.shxzskj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ig.shxzskj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cf.9csxet.cn

[B15] 布尔运算与取反
来源：http://kp.yuexingan06.cn

Py:   a and b or not c
来源：http://hv.shxzskj.cn

PHP:  $a && $b || !$c
来源：http://hz.huixiangedu.cn

JS:   a && b || !c
来源：http://ux.shxzukj.cn

TS:   a && b || !c
来源：http://vo.521024.cn

Java: a && b || !c
来源：http://jk.jianghongdianzi.cn

Go:   a && b || !c
来源：http://hn.nszjky.cn

Ruby: a && b || !c
来源：http://vg.jianghongdianzi.cn

C#:   a && b || !c
来源：http://wg.szxytkj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://pc.bjjhwx.cn

Py:   if not data: return
来源：http://jw.bjjhwx.cn

PHP:  if (!$data) { return; }
来源：http://qp.shxzskj.cn

JS:   if (!data) return;
来源：http://zq.colortex.cn

TS:   if (!data) return;
来源：http://zd.shxzukj.cn

Java: if (data == null) return;
来源：http://mo.panjiajie.cn

Go:   if data == nil { return }
来源：http://cq.panjiajie.cn

Ruby: return if data.nil?
来源：http://do.huixiangedu.cn

C#:   if (data == null) return;
来源：http://cy.hnjuh.cn

================================================================================
来源：http://ds.yuexingan06.cn

C. 函数与作用域
来源：http://yl.newstarts.cn

================================================================================
来源：http://xp.muxihuayi.cn

[C01] 定义函数
来源：http://un.jianghongdianzi.cn

Py:   def add(a, b): return a + b
来源：http://lr.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://am.shtwfgs.cn

JS:   function add(a, b) { return a + b; }
来源：http://vr.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bg.chemitech.net.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://jq.huixinmuqiang.cn

Go:   func add(a, b int) int { return a + b }
来源：http://du.huixinmuqiang.cn

Ruby: def add(a, b); a + b; end
来源：http://tk.nszjky.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bn.jianghongdianzi.cn

[C02] 默认参数
来源：http://sr.colortex.cn

Py:   def greet(name="World"): return name
来源：http://al.9csxet.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://rc.lnxyls.cn

JS:   function greet(name = "World") { return name; }
来源：http://im.shxzukj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ez.shxzukj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://sc.nszjky.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dy.bjjhwx.cn

Ruby: def greet(name = "World") = name
来源：http://qr.hnjuh.cn

C#:   string Greet(string name = "World") => name;
来源：http://tx.shtwfgs.cn

[C03] 可变参数
来源：http://ul.jianghongdianzi.cn

Py:   def total(*args): return sum(args)
来源：http://ia.wgjwhj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wa.nicolike.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hr.wgjwhj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zb.asd995.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://aa.chemitech.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jv.huanxung.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ei.nszjky.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kg.szsharing.cn

[C04] 命名参数 / 关键字参数
来源：http://bz.panjiajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pb.panjiajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ld.yuntaijiaju.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fw.huanxung.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gx.9csxet.cn

Java: // 无：用 Builder 模式或 record
来源：http://vs.huanxung.cn

Go:   // 无：用配置结构体参数
来源：http://rb.nszjky.cn

Ruby: f(a: 1, b: 2)
来源：http://mi.huixiangedu.cn

C#:   f(a: 1, b: 2)
来源：http://pe.lnxyls.cn

[C05] 返回多个值
来源：http://yx.asd995.cn

Py:   return a, b
来源：http://ep.huixiangedu.cn

PHP:  return [$a, $b];
来源：http://bg.szxytkj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yf.521024.cn

TS:   return { a, b };
来源：http://wa.huixiangedu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ki.newstarts.cn

Go:   return a, b
来源：http://ug.9csxet.cn

Ruby: return a, b
来源：http://ge.newstarts.cn

C#:   return (a, b);              // ValueTuple
来源：http://ik.yuexingan06.cn

[C06] 匿名函数 / lambda
来源：http://ye.521024.cn

Py:   square = lambda x: x * x
来源：http://dc.jctech888.com.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://rf.haigaiapp.cn

JS:   const square = x => x * x;
来源：http://we.chemitech.net.cn

TS:   const square = (x: number): number => x * x;
来源：http://he.shxzukj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wb.szxytkj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://lf.newstarts.cn

Ruby: square = ->(x) { x * x }
来源：http://ha.haigaiapp.cn

C#:   Func<int, int> square = x => x * x;
来源：http://go.nszjky.cn

[C07] 把函数作为参数传入
来源：http://mq.wgjwhj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ng.hahajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vn.bjjhwx.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://db.huanxung.cn

TS:   arr.map(String)
来源：http://cm.panjiajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dd.nicolike.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vi.hnjuh.cn

Ruby: arr.map(&:upcase)
来源：http://gy.shxzskj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://zx.colortex.cn

[C08] 闭包
来源：http://cl.nszjky.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ng.haigaiapp.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lx.nszjky.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pb.huixiangedu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pw.muxihuayi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yi.hahajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wy.hahajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wo.lnxyls.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yy.bookmarksfly.cn

[C09] 递归
来源：http://ot.hahajie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://su.shxzukj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://py.wgjwhj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gb.bjjhwx.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nw.szxytkj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rj.shtwfgs.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tu.521024.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lp.chemitech.net.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mn.bookmarksfly.cn

[C10] 变量作用域
来源：http://cn.nicolike.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pa.huixiangedu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ff.haigaiapp.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://um.newstarts.cn

TS:   同 JS
来源：http://hd.huixiangedu.cn

Java: 方法内为块级作用域
来源：http://je.szxytkj.cn

Go:   花括号块级作用域
来源：http://ir.yuntaijiaju.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tr.haigaiapp.cn

C#:   块级作用域
来源：http://qi.yuexingan06.cn

[C11] 模块导入与导出
来源：http://dt.hahajie.cn

Py:   from module import func
来源：http://ot.panjiajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xx.jianghongdianzi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://tx.panjiajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xy.nicolike.cn

Java: import java.util.List;
来源：http://ns.yuntaijiaju.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://is.wgjwhj.cn

Ruby: require "json"; require_relative "./util"
来源：http://vn.haigaiapp.cn

C#:   using System.Text;
来源：http://er.yuexingan06.cn

[C12] 立即执行函数 IIFE
来源：http://ir.shxzukj.cn

Py:   (lambda: print("run"))()
来源：http://ou.shtwfgs.cn

PHP:  (function () { echo "run"; })();
来源：http://mp.hahajie.cn

JS:   (() => { console.log("run"); })();
来源：http://nt.nicolike.cn

TS:   (() => { console.log("run"); })();
来源：http://dr.huanxung.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kl.shxzukj.cn

Go:   func() { fmt.Println("run") }()
来源：http://nz.jctech888.com.cn

Ruby: -> { puts "run" }.call
来源：http://wm.wgjwhj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://bp.hnjuh.cn

[C13] 类型声明 / 类型注解
来源：http://nc.asd995.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vs.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gq.colortex.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nw.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xy.gzmigu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qh.muxihuayi.cn

Go:   func add(a, b int) int
来源：http://cd.jianghongdianzi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mr.jianghongdianzi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://kf.nszjky.cn

[C14] 泛型函数
来源：http://ip.newstarts.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://si.9csxet.cn

PHP:  // 无泛型
来源：http://oi.asd995.cn

JS:   // 无泛型
来源：http://hk.shtwfgs.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yg.nszjky.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fr.bookmarksfly.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fc.chemitech.net.cn

Ruby: # 无泛型
来源：http://xd.szsharing.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lu.wgjwhj.cn

[C15] 解构 / 展开参数
来源：http://qa.shtwfgs.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hk.wgjwhj.cn

PHP:  [$a, $b] = $pair;
来源：http://ea.nszjky.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ny.nicolike.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fz.bjjhwx.cn

Java: // 无解构
来源：http://xk.muxihuayi.cn

Go:   // 无解构
来源：http://kc.jctech888.com.cn

Ruby: a, b = pair
来源：http://yo.haigaiapp.cn

C#:   var (a, b) = pair;
来源：http://ga.shxzskj.cn

[C16] 函数 / 方法重载
来源：http://ri.yuexingan06.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jv.nszjky.cn

PHP:  // 无重载
来源：http://rj.yuexingan06.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xu.panjiajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://nq.chemitech.net.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pz.huixiangedu.cn

Go:   // 无重载：用不同函数名
来源：http://fv.wgjwhj.cn

Ruby: # 无重载：靠动态参数
来源：http://vh.521024.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ji.nicolike.cn

================================================================================
来源：http://iu.huixinmuqiang.cn

D. 数组 / 列表 / 集合
来源：http://ul.hnjuh.cn

================================================================================
来源：http://cg.shxzukj.cn

[D01] 创建数组 / 列表
来源：http://yn.lnxyls.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://kr.shxzukj.cn


<!-- 参考信息 -->