代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gw.nszjky.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://mw.nszjky.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jg.shxzukj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ra.huixiangedu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fs.huixiangedu.cn

[B02] 多分支 else if / elif
来源：http://kb.jctech888.com.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xq.asd995.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://js.hahajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pw.bjjhwx.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gh.wgjwhj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nc.bookmarksfly.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mg.nicolike.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://oo.chemitech.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fd.asd995.cn

[B03] switch / match / case
来源：http://ik.9csxet.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ye.lnxyls.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fb.szsharing.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sx.newstarts.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hq.szsharing.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bq.szsharing.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hm.panjiajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dc.bookmarksfly.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hs.nszjky.cn

[B04] for 计数循环
来源：http://vs.huixinmuqiang.cn

Py:   for i in range(10): print(i)
来源：http://zz.yuntaijiaju.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://na.panjiajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yi.lnxyls.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tc.bookmarksfly.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zg.nicolike.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gj.huixiangedu.cn

Ruby: 10.times { |i| puts i }
来源：http://az.shxzskj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jb.muxihuayi.cn

[B05] 遍历数组 / 列表
来源：http://cs.huanxung.cn

Py:   for item in arr: print(item)
来源：http://hs.lnxyls.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bf.panjiajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://va.panjiajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yk.szsharing.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yg.shtwfgs.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://uo.521024.cn

Ruby: arr.each { |item| puts item }
来源：http://zf.huixiangedu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://il.shtwfgs.cn

[B06] 遍历字典 / 对象
来源：http://yq.hahajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pe.hahajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qb.hahajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kb.521024.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://el.jctech888.com.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rx.newstarts.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sq.chemitech.net.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yw.nszjky.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nb.yuexingan06.cn

[B07] while 循环
来源：http://kd.yuexingan06.cn

Py:   while i < 10: i += 1
来源：http://qo.haigaiapp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mf.huanxung.cn

JS:   while (i < 10) { i++; }
来源：http://oz.szxytkj.cn

TS:   while (i < 10) { i++; }
来源：http://fr.hnjuh.cn

Java: while (i < 10) { i++; }
来源：http://aw.bjjhwx.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qh.huixinmuqiang.cn

Ruby: while i < 10; i += 1; end
来源：http://wf.521024.cn

C#:   while (i < 10) { i++; }
来源：http://lm.521024.cn

[B08] do-while（至少执行一次）
来源：http://lu.shxzukj.cn

Py:   # 无 do-while：用 while True + break
来源：http://as.muxihuayi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ga.gzmigu.cn

JS:   do { i++; } while (i < 10);
来源：http://wp.shxzukj.cn

TS:   do { i++; } while (i < 10);
来源：http://of.panjiajie.cn

Java: do { i++; } while (i < 10);
来源：http://zn.hahajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fe.asd995.cn

Ruby: begin; i += 1; end while i < 10
来源：http://dv.yuexingan06.cn

C#:   do { i++; } while (i < 10);
来源：http://rt.521024.cn

[B09] break 与 continue
来源：http://zx.panjiajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://br.shxzskj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lj.yuntaijiaju.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dy.lnxyls.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yj.nicolike.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sr.hnjuh.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vk.panjiajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lo.nicolike.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ui.wgjwhj.cn

[B10] 遍历同时拿索引
来源：http://zf.jianghongdianzi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ne.bookmarksfly.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zh.9csxet.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nw.shtwfgs.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fj.newstarts.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fl.yuntaijiaju.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qz.wgjwhj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://je.gzmigu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://uj.nszjky.cn

[B11] 生成数字序列 / 区间
来源：http://el.gzmigu.cn

Py:   list(range(0, 10, 2))
来源：http://or.9csxet.cn

PHP:  range(0, 10, 2);
来源：http://ol.shtwfgs.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qg.shxzukj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qr.nszjky.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rm.colortex.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vv.521024.cn

Ruby: (0...10).step(2).to_a
来源：http://uc.bookmarksfly.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ua.521024.cn

[B12] 跳出多层循环
来源：http://yb.nicolike.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://sk.yuntaijiaju.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://rp.shxzukj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://iv.521024.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gf.bjjhwx.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zj.panjiajie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hc.huixinmuqiang.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cf.gzmigu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bv.colortex.cn

[B13] 判断是否为数字
来源：http://wy.muxihuayi.cn

Py:   isinstance(x, (int, float))
来源：http://ad.jctech888.com.cn

PHP:  is_numeric($x)
来源：http://jb.jctech888.com.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yw.szsharing.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lk.yuntaijiaju.cn

Java: x instanceof Number
来源：http://cj.shxzskj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://im.bjjhwx.cn

Ruby: x.is_a?(Numeric)
来源：http://og.jctech888.com.cn

C#:   x is int or double or decimal
来源：http://if.huixiangedu.cn

[B14] 判断值是否在集合内
来源：http://jz.muxihuayi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fy.colortex.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sq.9csxet.cn

JS:   [1, 2, 3].includes(x)
来源：http://ej.yuexingan06.cn

TS:   [1, 2, 3].includes(x)
来源：http://zy.huixinmuqiang.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://lg.huixiangedu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tx.shxzskj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qv.521024.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mo.9csxet.cn

[B15] 布尔运算与取反
来源：http://zx.yuexingan06.cn

Py:   a and b or not c
来源：http://gi.yuntaijiaju.cn

PHP:  $a && $b || !$c
来源：http://ig.yuntaijiaju.cn

JS:   a && b || !c
来源：http://px.521024.cn

TS:   a && b || !c
来源：http://qc.huanxung.cn

Java: a && b || !c
来源：http://yu.hahajie.cn

Go:   a && b || !c
来源：http://xh.shtwfgs.cn

Ruby: a && b || !c
来源：http://op.szsharing.cn

C#:   a && b || !c
来源：http://ds.shxzskj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://sp.jianghongdianzi.cn

Py:   if not data: return
来源：http://el.nszjky.cn

PHP:  if (!$data) { return; }
来源：http://vy.muxihuayi.cn

JS:   if (!data) return;
来源：http://fw.newstarts.cn

TS:   if (!data) return;
来源：http://vy.yuntaijiaju.cn

Java: if (data == null) return;
来源：http://wv.muxihuayi.cn

Go:   if data == nil { return }
来源：http://dv.shxzukj.cn

Ruby: return if data.nil?
来源：http://zi.chemitech.net.cn

C#:   if (data == null) return;
来源：http://ts.muxihuayi.cn

================================================================================
来源：http://bk.gzmigu.cn

C. 函数与作用域
来源：http://xf.newstarts.cn

================================================================================
来源：http://uj.muxihuayi.cn

[C01] 定义函数
来源：http://tp.wgjwhj.cn

Py:   def add(a, b): return a + b
来源：http://ap.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jx.huixiangedu.cn

JS:   function add(a, b) { return a + b; }
来源：http://gi.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pz.521024.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://tq.bookmarksfly.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vi.colortex.cn

Ruby: def add(a, b); a + b; end
来源：http://hl.bjjhwx.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sr.hahajie.cn

[C02] 默认参数
来源：http://be.shtwfgs.cn

Py:   def greet(name="World"): return name
来源：http://fy.shxzskj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://gp.colortex.cn

JS:   function greet(name = "World") { return name; }
来源：http://pm.gzmigu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://pb.huanxung.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hp.hnjuh.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qc.shxzukj.cn

Ruby: def greet(name = "World") = name
来源：http://pr.shxzukj.cn

C#:   string Greet(string name = "World") => name;
来源：http://lr.bookmarksfly.cn

[C03] 可变参数
来源：http://aw.521024.cn

Py:   def total(*args): return sum(args)
来源：http://vs.bjjhwx.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://be.lnxyls.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pp.chemitech.net.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vr.jctech888.com.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sv.521024.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ez.hnjuh.cn

Ruby: def total(*nums); nums.sum; end
来源：http://cr.nszjky.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cw.9csxet.cn

[C04] 命名参数 / 关键字参数
来源：http://hi.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cn.panjiajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://he.hnjuh.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gl.jctech888.com.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dl.szsharing.cn

Java: // 无：用 Builder 模式或 record
来源：http://jg.nszjky.cn

Go:   // 无：用配置结构体参数
来源：http://jj.shtwfgs.cn

Ruby: f(a: 1, b: 2)
来源：http://cm.hahajie.cn

C#:   f(a: 1, b: 2)
来源：http://ip.521024.cn

[C05] 返回多个值
来源：http://dh.huixiangedu.cn

Py:   return a, b
来源：http://ob.jctech888.com.cn

PHP:  return [$a, $b];
来源：http://aw.yuntaijiaju.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jc.asd995.cn

TS:   return { a, b };
来源：http://yy.nicolike.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wf.newstarts.cn

Go:   return a, b
来源：http://ya.panjiajie.cn

Ruby: return a, b
来源：http://ho.chemitech.net.cn

C#:   return (a, b);              // ValueTuple
来源：http://cs.haigaiapp.cn

[C06] 匿名函数 / lambda
来源：http://cf.asd995.cn

Py:   square = lambda x: x * x
来源：http://vo.szsharing.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pi.bjjhwx.cn

JS:   const square = x => x * x;
来源：http://hg.shxzskj.cn

TS:   const square = (x: number): number => x * x;
来源：http://hx.huixiangedu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://re.huixinmuqiang.cn

Go:   sq := func(x int) int { return x * x }
来源：http://pi.newstarts.cn

Ruby: square = ->(x) { x * x }
来源：http://dw.huanxung.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bj.521024.cn

[C07] 把函数作为参数传入
来源：http://if.jianghongdianzi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ur.huixiangedu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://mr.wgjwhj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gs.shxzskj.cn

TS:   arr.map(String)
来源：http://pl.panjiajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kk.asd995.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cv.521024.cn

Ruby: arr.map(&:upcase)
来源：http://md.jctech888.com.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ba.chemitech.net.cn

[C08] 闭包
来源：http://ie.jianghongdianzi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zr.bookmarksfly.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yv.hahajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uy.huixiangedu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ng.9csxet.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qf.bookmarksfly.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bj.chemitech.net.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wg.huixiangedu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dz.hnjuh.cn

[C09] 递归
来源：http://cg.hahajie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vw.hnjuh.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wl.521024.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://td.wgjwhj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hc.9csxet.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bv.hnjuh.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ct.shxzukj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://et.nszjky.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://by.huanxung.cn

[C10] 变量作用域
来源：http://tf.hnjuh.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wg.colortex.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tj.bjjhwx.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jj.muxihuayi.cn

TS:   同 JS
来源：http://gi.jctech888.com.cn

Java: 方法内为块级作用域
来源：http://zb.haigaiapp.cn

Go:   花括号块级作用域
来源：http://in.nicolike.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://al.shxzukj.cn

C#:   块级作用域
来源：http://xy.9csxet.cn

[C11] 模块导入与导出
来源：http://vl.colortex.cn

Py:   from module import func
来源：http://jb.jianghongdianzi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wq.huixiangedu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://iq.huanxung.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vf.lnxyls.cn

Java: import java.util.List;
来源：http://wq.bjjhwx.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://au.bookmarksfly.cn

Ruby: require "json"; require_relative "./util"
来源：http://oz.hnjuh.cn

C#:   using System.Text;
来源：http://yv.muxihuayi.cn

[C12] 立即执行函数 IIFE
来源：http://ab.hahajie.cn

Py:   (lambda: print("run"))()
来源：http://lk.colortex.cn

PHP:  (function () { echo "run"; })();
来源：http://ir.bjjhwx.cn

JS:   (() => { console.log("run"); })();
来源：http://yb.colortex.cn

TS:   (() => { console.log("run"); })();
来源：http://js.hahajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ct.bookmarksfly.cn

Go:   func() { fmt.Println("run") }()
来源：http://av.jctech888.com.cn

Ruby: -> { puts "run" }.call
来源：http://gk.9csxet.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qm.chemitech.net.cn

[C13] 类型声明 / 类型注解
来源：http://tk.huixinmuqiang.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yp.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ov.jianghongdianzi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mg.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ap.bookmarksfly.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jo.shxzskj.cn

Go:   func add(a, b int) int
来源：http://uq.jctech888.com.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qm.jianghongdianzi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://sq.szsharing.cn

[C14] 泛型函数
来源：http://qt.shxzskj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://go.521024.cn

PHP:  // 无泛型
来源：http://bk.hahajie.cn

JS:   // 无泛型
来源：http://ld.newstarts.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vm.shxzskj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kz.huixinmuqiang.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lk.9csxet.cn

Ruby: # 无泛型
来源：http://kq.newstarts.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vu.shtwfgs.cn

[C15] 解构 / 展开参数
来源：http://ku.lnxyls.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xw.lnxyls.cn

PHP:  [$a, $b] = $pair;
来源：http://zb.nszjky.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://it.newstarts.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dl.colortex.cn

Java: // 无解构
来源：http://ko.nicolike.cn

Go:   // 无解构
来源：http://xh.hahajie.cn

Ruby: a, b = pair
来源：http://eo.newstarts.cn

C#:   var (a, b) = pair;
来源：http://bp.bookmarksfly.cn

[C16] 函数 / 方法重载
来源：http://er.szxytkj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pv.9csxet.cn

PHP:  // 无重载
来源：http://os.521024.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://un.newstarts.cn

TS:   // 用联合类型或重载签名声明
来源：http://ue.asd995.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://yc.521024.cn

Go:   // 无重载：用不同函数名
来源：http://oh.muxihuayi.cn

Ruby: # 无重载：靠动态参数
来源：http://qn.shxzukj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qr.yuexingan06.cn

================================================================================
来源：http://un.huixiangedu.cn

D. 数组 / 列表 / 集合
来源：http://es.lnxyls.cn

================================================================================
来源：http://zu.newstarts.cn

[D01] 创建数组 / 列表
来源：http://ty.shxzukj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fs.shxzukj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ir.nicolike.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jq.hnjuh.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wv.bookmarksfly.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ee.bjjhwx.cn

Go:   arr := []int{1, 2, 3}
来源：http://qq.colortex.cn

Ruby: arr = [1, 2, 3]
来源：http://hj.gzmigu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nb.nszjky.cn

[D02] 追加元素到末尾
来源：http://yr.szsharing.cn


<!-- 参考信息 -->