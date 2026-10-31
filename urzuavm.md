代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bu.hnjuh.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ki.521024.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://sb.newstarts.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pg.nszjky.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bf.shtwfgs.cn

[B02] 多分支 else if / elif
来源：http://rj.hnjuh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hp.shxzukj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lr.wgjwhj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ek.shtwfgs.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jv.huixinmuqiang.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ah.szxytkj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kx.wgjwhj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://do.yuexingan06.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nd.newstarts.cn

[B03] switch / match / case
来源：http://po.huixiangedu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jv.jianghongdianzi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://is.yuntaijiaju.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rn.yuntaijiaju.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kn.hahajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ep.bjjhwx.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nm.colortex.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mj.chemitech.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uq.bjjhwx.cn

[B04] for 计数循环
来源：http://uz.lnxyls.cn

Py:   for i in range(10): print(i)
来源：http://ku.yuexingan06.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mm.521024.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wu.9csxet.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cb.bjjhwx.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cs.yuexingan06.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wb.asd995.cn

Ruby: 10.times { |i| puts i }
来源：http://ch.hahajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wf.gzmigu.cn

[B05] 遍历数组 / 列表
来源：http://ws.9csxet.cn

Py:   for item in arr: print(item)
来源：http://jw.9csxet.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kq.wgjwhj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://pm.haigaiapp.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://kg.yuntaijiaju.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zu.nicolike.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tx.9csxet.cn

Ruby: arr.each { |item| puts item }
来源：http://vi.shxzukj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mr.gzmigu.cn

[B06] 遍历字典 / 对象
来源：http://oo.jianghongdianzi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ls.jianghongdianzi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uz.haigaiapp.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bb.asd995.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://za.9csxet.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ip.9csxet.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sb.yuntaijiaju.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ek.chemitech.net.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ys.bookmarksfly.cn

[B07] while 循环
来源：http://ha.nszjky.cn

Py:   while i < 10: i += 1
来源：http://ii.gzmigu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://rk.gzmigu.cn

JS:   while (i < 10) { i++; }
来源：http://bj.huanxung.cn

TS:   while (i < 10) { i++; }
来源：http://yn.chemitech.net.cn

Java: while (i < 10) { i++; }
来源：http://ax.nszjky.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jh.huixinmuqiang.cn

Ruby: while i < 10; i += 1; end
来源：http://jy.wgjwhj.cn

C#:   while (i < 10) { i++; }
来源：http://fc.bjjhwx.cn

[B08] do-while（至少执行一次）
来源：http://fh.szsharing.cn

Py:   # 无 do-while：用 while True + break
来源：http://vp.yuexingan06.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://oc.bjjhwx.cn

JS:   do { i++; } while (i < 10);
来源：http://nu.newstarts.cn

TS:   do { i++; } while (i < 10);
来源：http://dt.gzmigu.cn

Java: do { i++; } while (i < 10);
来源：http://rx.shtwfgs.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://yd.colortex.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mv.wgjwhj.cn

C#:   do { i++; } while (i < 10);
来源：http://wv.asd995.cn

[B09] break 与 continue
来源：http://ta.hnjuh.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cn.jctech888.com.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://al.jctech888.com.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wb.yuntaijiaju.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hy.jianghongdianzi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://in.szxytkj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ho.jianghongdianzi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ke.szxytkj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kx.bjjhwx.cn

[B10] 遍历同时拿索引
来源：http://ch.yuexingan06.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gc.szxytkj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yp.gzmigu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jf.bjjhwx.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jg.jctech888.com.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sh.szsharing.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dl.huixinmuqiang.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://iq.9csxet.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dy.shxzskj.cn

[B11] 生成数字序列 / 区间
来源：http://hx.haigaiapp.cn

Py:   list(range(0, 10, 2))
来源：http://rl.huixiangedu.cn

PHP:  range(0, 10, 2);
来源：http://wt.szsharing.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rc.chemitech.net.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xd.colortex.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ro.colortex.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cd.shxzskj.cn

Ruby: (0...10).step(2).to_a
来源：http://ky.muxihuayi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bg.wgjwhj.cn

[B12] 跳出多层循环
来源：http://dl.jianghongdianzi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://dh.9csxet.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ln.jianghongdianzi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bf.bjjhwx.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zj.shtwfgs.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ft.szxytkj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sd.shtwfgs.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nw.bookmarksfly.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mn.muxihuayi.cn

[B13] 判断是否为数字
来源：http://mg.shxzskj.cn

Py:   isinstance(x, (int, float))
来源：http://sc.521024.cn

PHP:  is_numeric($x)
来源：http://br.nszjky.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gy.hnjuh.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zu.hahajie.cn

Java: x instanceof Number
来源：http://vg.panjiajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xp.wgjwhj.cn

Ruby: x.is_a?(Numeric)
来源：http://yx.hahajie.cn

C#:   x is int or double or decimal
来源：http://dd.gzmigu.cn

[B14] 判断值是否在集合内
来源：http://fl.huanxung.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cu.9csxet.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kk.gzmigu.cn

JS:   [1, 2, 3].includes(x)
来源：http://qq.yuntaijiaju.cn

TS:   [1, 2, 3].includes(x)
来源：http://jy.hahajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://in.colortex.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://eh.nszjky.cn

Ruby: [1, 2, 3].include?(x)
来源：http://hi.jianghongdianzi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ll.newstarts.cn

[B15] 布尔运算与取反
来源：http://pp.jctech888.com.cn

Py:   a and b or not c
来源：http://ju.shxzskj.cn

PHP:  $a && $b || !$c
来源：http://zk.wgjwhj.cn

JS:   a && b || !c
来源：http://vm.bjjhwx.cn

TS:   a && b || !c
来源：http://lf.asd995.cn

Java: a && b || !c
来源：http://mf.huanxung.cn

Go:   a && b || !c
来源：http://eq.yuexingan06.cn

Ruby: a && b || !c
来源：http://pt.huixiangedu.cn

C#:   a && b || !c
来源：http://iw.hnjuh.cn

[B16] 卫语句：不满足条件提前返回
来源：http://kb.panjiajie.cn

Py:   if not data: return
来源：http://vb.hnjuh.cn

PHP:  if (!$data) { return; }
来源：http://cg.521024.cn

JS:   if (!data) return;
来源：http://xo.huixinmuqiang.cn

TS:   if (!data) return;
来源：http://jf.hnjuh.cn

Java: if (data == null) return;
来源：http://bg.panjiajie.cn

Go:   if data == nil { return }
来源：http://zq.lnxyls.cn

Ruby: return if data.nil?
来源：http://sh.lnxyls.cn

C#:   if (data == null) return;
来源：http://xn.newstarts.cn

================================================================================
来源：http://ky.newstarts.cn

C. 函数与作用域
来源：http://mm.bookmarksfly.cn

================================================================================
来源：http://sl.huixiangedu.cn

[C01] 定义函数
来源：http://oz.hnjuh.cn

Py:   def add(a, b): return a + b
来源：http://co.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ot.haigaiapp.cn

JS:   function add(a, b) { return a + b; }
来源：http://ts.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ou.nszjky.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vd.huanxung.cn

Go:   func add(a, b int) int { return a + b }
来源：http://pq.haigaiapp.cn

Ruby: def add(a, b); a + b; end
来源：http://lc.muxihuayi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qz.chemitech.net.cn

[C02] 默认参数
来源：http://fx.yuntaijiaju.cn

Py:   def greet(name="World"): return name
来源：http://kb.yuexingan06.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://sn.huixiangedu.cn

JS:   function greet(name = "World") { return name; }
来源：http://bi.hahajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bw.jctech888.com.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dl.yuexingan06.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gh.panjiajie.cn

Ruby: def greet(name = "World") = name
来源：http://jv.newstarts.cn

C#:   string Greet(string name = "World") => name;
来源：http://pk.chemitech.net.cn

[C03] 可变参数
来源：http://zc.haigaiapp.cn

Py:   def total(*args): return sum(args)
来源：http://uq.haigaiapp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sq.lnxyls.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lg.gzmigu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qg.nszjky.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dn.haigaiapp.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kl.colortex.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wh.jianghongdianzi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xu.lnxyls.cn

[C04] 命名参数 / 关键字参数
来源：http://dg.huixinmuqiang.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://of.jctech888.com.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nv.asd995.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zc.521024.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wu.bookmarksfly.cn

Java: // 无：用 Builder 模式或 record
来源：http://bx.shxzukj.cn

Go:   // 无：用配置结构体参数
来源：http://oe.chemitech.net.cn

Ruby: f(a: 1, b: 2)
来源：http://oe.jctech888.com.cn

C#:   f(a: 1, b: 2)
来源：http://ku.colortex.cn

[C05] 返回多个值
来源：http://gt.9csxet.cn

Py:   return a, b
来源：http://gk.shtwfgs.cn

PHP:  return [$a, $b];
来源：http://nf.nicolike.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ke.hnjuh.cn

TS:   return { a, b };
来源：http://cc.colortex.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://it.huixinmuqiang.cn

Go:   return a, b
来源：http://fq.huixinmuqiang.cn

Ruby: return a, b
来源：http://yx.wgjwhj.cn

C#:   return (a, b);              // ValueTuple
来源：http://zo.huanxung.cn

[C06] 匿名函数 / lambda
来源：http://fs.colortex.cn

Py:   square = lambda x: x * x
来源：http://ud.yuexingan06.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wv.jctech888.com.cn

JS:   const square = x => x * x;
来源：http://qo.szxytkj.cn

TS:   const square = (x: number): number => x * x;
来源：http://ak.newstarts.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gi.yuntaijiaju.cn

Go:   sq := func(x int) int { return x * x }
来源：http://bn.hahajie.cn

Ruby: square = ->(x) { x * x }
来源：http://wr.521024.cn

C#:   Func<int, int> square = x => x * x;
来源：http://tx.huanxung.cn

[C07] 把函数作为参数传入
来源：http://ac.hahajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ub.shxzskj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ai.jctech888.com.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qm.huanxung.cn

TS:   arr.map(String)
来源：http://hm.yuntaijiaju.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ps.lnxyls.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ix.newstarts.cn

Ruby: arr.map(&:upcase)
来源：http://vc.wgjwhj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ur.panjiajie.cn

[C08] 闭包
来源：http://ln.huixiangedu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vg.huixiangedu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ny.shxzukj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mr.shtwfgs.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lt.gzmigu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://us.szsharing.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ik.nicolike.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xy.yuntaijiaju.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uu.bookmarksfly.cn

[C09] 递归
来源：http://ri.newstarts.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://oq.huanxung.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gn.lnxyls.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://um.bookmarksfly.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://be.nszjky.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tp.newstarts.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uv.asd995.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xx.panjiajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://al.chemitech.net.cn

[C10] 变量作用域
来源：http://si.hnjuh.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ud.szxytkj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ew.lnxyls.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://go.jianghongdianzi.cn

TS:   同 JS
来源：http://ex.asd995.cn

Java: 方法内为块级作用域
来源：http://pd.huixinmuqiang.cn

Go:   花括号块级作用域
来源：http://iw.bjjhwx.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wq.haigaiapp.cn

C#:   块级作用域
来源：http://dn.newstarts.cn

[C11] 模块导入与导出
来源：http://sh.panjiajie.cn

Py:   from module import func
来源：http://ch.szxytkj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pq.bjjhwx.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vi.asd995.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yi.wgjwhj.cn

Java: import java.util.List;
来源：http://jr.yuntaijiaju.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://je.521024.cn

Ruby: require "json"; require_relative "./util"
来源：http://oc.yuntaijiaju.cn

C#:   using System.Text;
来源：http://sx.nszjky.cn

[C12] 立即执行函数 IIFE
来源：http://wv.9csxet.cn

Py:   (lambda: print("run"))()
来源：http://hz.szxytkj.cn

PHP:  (function () { echo "run"; })();
来源：http://bk.lnxyls.cn

JS:   (() => { console.log("run"); })();
来源：http://pq.huanxung.cn

TS:   (() => { console.log("run"); })();
来源：http://cc.wgjwhj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ih.yuexingan06.cn

Go:   func() { fmt.Println("run") }()
来源：http://bm.szsharing.cn

Ruby: -> { puts "run" }.call
来源：http://uy.muxihuayi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://tc.bookmarksfly.cn

[C13] 类型声明 / 类型注解
来源：http://xd.shxzukj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fj.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wv.huixiangedu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://oj.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gs.nszjky.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cu.szsharing.cn

Go:   func add(a, b int) int
来源：http://hg.huixiangedu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hs.lnxyls.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bq.colortex.cn

[C14] 泛型函数
来源：http://nj.yuntaijiaju.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nb.szxytkj.cn

PHP:  // 无泛型
来源：http://qt.bookmarksfly.cn

JS:   // 无泛型
来源：http://bg.hahajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nw.asd995.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fb.9csxet.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jw.bookmarksfly.cn

Ruby: # 无泛型
来源：http://oi.521024.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://it.huixinmuqiang.cn

[C15] 解构 / 展开参数
来源：http://zj.huanxung.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xg.nicolike.cn

PHP:  [$a, $b] = $pair;
来源：http://ha.yuntaijiaju.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ys.chemitech.net.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://og.yuntaijiaju.cn

Java: // 无解构
来源：http://xd.colortex.cn

Go:   // 无解构
来源：http://nq.szxytkj.cn

Ruby: a, b = pair
来源：http://ec.shxzskj.cn

C#:   var (a, b) = pair;
来源：http://au.gzmigu.cn

[C16] 函数 / 方法重载
来源：http://aj.haigaiapp.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.muxihuayi.cn

PHP:  // 无重载
来源：http://js.yuntaijiaju.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://nu.521024.cn

TS:   // 用联合类型或重载签名声明
来源：http://ll.muxihuayi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://sz.shtwfgs.cn

Go:   // 无重载：用不同函数名
来源：http://wt.lnxyls.cn

Ruby: # 无重载：靠动态参数
来源：http://of.huixinmuqiang.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://kv.yuntaijiaju.cn

================================================================================
来源：http://xd.9csxet.cn

D. 数组 / 列表 / 集合
来源：http://eo.huixiangedu.cn

================================================================================
来源：http://oe.chemitech.net.cn

[D01] 创建数组 / 列表
来源：http://id.muxihuayi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ao.haigaiapp.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lk.huixiangedu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nj.colortex.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://cz.muxihuayi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dm.shxzukj.cn

Go:   arr := []int{1, 2, 3}
来源：http://pd.colortex.cn

Ruby: arr = [1, 2, 3]
来源：http://nm.hahajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jx.hnjuh.cn

[D02] 追加元素到末尾
来源：http://eh.9csxet.cn


<!-- 参考信息 -->