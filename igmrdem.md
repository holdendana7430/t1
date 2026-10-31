代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://cf.yuexingan06.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://jm.shxzukj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pa.huixiangedu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mt.gzmigu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rc.asd995.cn

[B02] 多分支 else if / elif
来源：http://la.chemitech.net.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dl.shxzukj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fv.521024.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ux.yuexingan06.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wy.jianghongdianzi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cn.szsharing.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://za.nszjky.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vn.haigaiapp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fu.panjiajie.cn

[B03] switch / match / case
来源：http://mc.yuntaijiaju.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ao.yuntaijiaju.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cn.yuexingan06.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dp.hnjuh.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bz.huixiangedu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hh.bookmarksfly.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fc.chemitech.net.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rc.newstarts.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xs.wgjwhj.cn

[B04] for 计数循环
来源：http://lq.hahajie.cn

Py:   for i in range(10): print(i)
来源：http://hl.huanxung.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qr.szxytkj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bw.shxzukj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://as.chemitech.net.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wy.colortex.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://el.newstarts.cn

Ruby: 10.times { |i| puts i }
来源：http://mq.jctech888.com.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fo.asd995.cn

[B05] 遍历数组 / 列表
来源：http://sf.shtwfgs.cn

Py:   for item in arr: print(item)
来源：http://jq.haigaiapp.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pz.gzmigu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://rk.hahajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ua.shtwfgs.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xp.szsharing.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vj.yuntaijiaju.cn

Ruby: arr.each { |item| puts item }
来源：http://ln.panjiajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://eg.lnxyls.cn

[B06] 遍历字典 / 对象
来源：http://vh.yuexingan06.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hl.chemitech.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nn.wgjwhj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sd.chemitech.net.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dd.asd995.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://eh.shxzukj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://id.bjjhwx.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dw.gzmigu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://eh.521024.cn

[B07] while 循环
来源：http://pi.bookmarksfly.cn

Py:   while i < 10: i += 1
来源：http://on.huixiangedu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bd.wgjwhj.cn

JS:   while (i < 10) { i++; }
来源：http://cm.521024.cn

TS:   while (i < 10) { i++; }
来源：http://gr.9csxet.cn

Java: while (i < 10) { i++; }
来源：http://kp.asd995.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ot.panjiajie.cn

Ruby: while i < 10; i += 1; end
来源：http://xp.bjjhwx.cn

C#:   while (i < 10) { i++; }
来源：http://wl.jianghongdianzi.cn

[B08] do-while（至少执行一次）
来源：http://dn.wgjwhj.cn

Py:   # 无 do-while：用 while True + break
来源：http://lv.yuntaijiaju.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://no.nicolike.cn

JS:   do { i++; } while (i < 10);
来源：http://sv.shxzskj.cn

TS:   do { i++; } while (i < 10);
来源：http://oy.521024.cn

Java: do { i++; } while (i < 10);
来源：http://ce.szxytkj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://qz.shxzukj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xw.shxzskj.cn

C#:   do { i++; } while (i < 10);
来源：http://jj.szxytkj.cn

[B09] break 与 continue
来源：http://bq.nicolike.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gc.chemitech.net.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cr.wgjwhj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mt.hnjuh.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yz.lnxyls.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tx.szsharing.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ce.yuntaijiaju.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qj.chemitech.net.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://er.muxihuayi.cn

[B10] 遍历同时拿索引
来源：http://cg.panjiajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://if.colortex.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ez.lnxyls.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jo.521024.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ft.521024.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ri.szxytkj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bh.szsharing.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pn.gzmigu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lb.asd995.cn

[B11] 生成数字序列 / 区间
来源：http://iw.gzmigu.cn

Py:   list(range(0, 10, 2))
来源：http://mc.9csxet.cn

PHP:  range(0, 10, 2);
来源：http://ae.nszjky.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nl.hnjuh.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vs.szsharing.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://oo.chemitech.net.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ur.yuexingan06.cn

Ruby: (0...10).step(2).to_a
来源：http://ka.gzmigu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://aa.asd995.cn

[B12] 跳出多层循环
来源：http://ja.bjjhwx.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://iw.panjiajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gx.szsharing.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xj.colortex.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zo.muxihuayi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dw.gzmigu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://al.yuntaijiaju.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wz.panjiajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ml.nicolike.cn

[B13] 判断是否为数字
来源：http://ph.chemitech.net.cn

Py:   isinstance(x, (int, float))
来源：http://rz.asd995.cn

PHP:  is_numeric($x)
来源：http://id.gzmigu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://th.muxihuayi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ex.yuexingan06.cn

Java: x instanceof Number
来源：http://in.bjjhwx.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ue.wgjwhj.cn

Ruby: x.is_a?(Numeric)
来源：http://od.panjiajie.cn

C#:   x is int or double or decimal
来源：http://td.shxzukj.cn

[B14] 判断值是否在集合内
来源：http://av.hnjuh.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zo.lnxyls.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ng.gzmigu.cn

JS:   [1, 2, 3].includes(x)
来源：http://xa.shxzskj.cn

TS:   [1, 2, 3].includes(x)
来源：http://ao.jctech888.com.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gt.chemitech.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nt.colortex.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rp.chemitech.net.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dg.shxzukj.cn

[B15] 布尔运算与取反
来源：http://ur.muxihuayi.cn

Py:   a and b or not c
来源：http://kk.gzmigu.cn

PHP:  $a && $b || !$c
来源：http://tr.yuntaijiaju.cn

JS:   a && b || !c
来源：http://gs.yuexingan06.cn

TS:   a && b || !c
来源：http://ns.hahajie.cn

Java: a && b || !c
来源：http://ar.huixinmuqiang.cn

Go:   a && b || !c
来源：http://xp.nszjky.cn

Ruby: a && b || !c
来源：http://ee.jianghongdianzi.cn

C#:   a && b || !c
来源：http://tt.colortex.cn

[B16] 卫语句：不满足条件提前返回
来源：http://iy.lnxyls.cn

Py:   if not data: return
来源：http://eo.gzmigu.cn

PHP:  if (!$data) { return; }
来源：http://vz.nicolike.cn

JS:   if (!data) return;
来源：http://qj.521024.cn

TS:   if (!data) return;
来源：http://zl.gzmigu.cn

Java: if (data == null) return;
来源：http://fg.hnjuh.cn

Go:   if data == nil { return }
来源：http://ie.bjjhwx.cn

Ruby: return if data.nil?
来源：http://sg.lnxyls.cn

C#:   if (data == null) return;
来源：http://ph.szxytkj.cn

================================================================================
来源：http://iz.huixinmuqiang.cn

C. 函数与作用域
来源：http://fi.huixiangedu.cn

================================================================================
来源：http://id.jianghongdianzi.cn

[C01] 定义函数
来源：http://lc.hahajie.cn

Py:   def add(a, b): return a + b
来源：http://gk.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sd.colortex.cn

JS:   function add(a, b) { return a + b; }
来源：http://iv.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nf.hahajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://up.gzmigu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ll.wgjwhj.cn

Ruby: def add(a, b); a + b; end
来源：http://yb.huixinmuqiang.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sz.huixiangedu.cn

[C02] 默认参数
来源：http://nk.muxihuayi.cn

Py:   def greet(name="World"): return name
来源：http://vq.newstarts.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vn.nicolike.cn

JS:   function greet(name = "World") { return name; }
来源：http://tm.hahajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://na.asd995.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cm.hnjuh.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nu.nicolike.cn

Ruby: def greet(name = "World") = name
来源：http://rl.yuexingan06.cn

C#:   string Greet(string name = "World") => name;
来源：http://rm.9csxet.cn

[C03] 可变参数
来源：http://to.bookmarksfly.cn

Py:   def total(*args): return sum(args)
来源：http://tm.bookmarksfly.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mt.wgjwhj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zl.muxihuayi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ms.newstarts.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kp.nszjky.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lc.huixiangedu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ba.newstarts.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jr.szxytkj.cn

[C04] 命名参数 / 关键字参数
来源：http://sb.bookmarksfly.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sq.9csxet.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wb.szsharing.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xn.bookmarksfly.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nk.huanxung.cn

Java: // 无：用 Builder 模式或 record
来源：http://zh.jctech888.com.cn

Go:   // 无：用配置结构体参数
来源：http://dz.huixinmuqiang.cn

Ruby: f(a: 1, b: 2)
来源：http://nn.huixinmuqiang.cn

C#:   f(a: 1, b: 2)
来源：http://sj.haigaiapp.cn

[C05] 返回多个值
来源：http://bd.huanxung.cn

Py:   return a, b
来源：http://bj.hahajie.cn

PHP:  return [$a, $b];
来源：http://gg.bjjhwx.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xg.haigaiapp.cn

TS:   return { a, b };
来源：http://ac.panjiajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tl.szxytkj.cn

Go:   return a, b
来源：http://nc.szsharing.cn

Ruby: return a, b
来源：http://zh.yuexingan06.cn

C#:   return (a, b);              // ValueTuple
来源：http://nr.nicolike.cn

[C06] 匿名函数 / lambda
来源：http://gu.newstarts.cn

Py:   square = lambda x: x * x
来源：http://nk.hahajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pf.chemitech.net.cn

JS:   const square = x => x * x;
来源：http://uc.bookmarksfly.cn

TS:   const square = (x: number): number => x * x;
来源：http://bu.lnxyls.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://is.hnjuh.cn

Go:   sq := func(x int) int { return x * x }
来源：http://om.nicolike.cn

Ruby: square = ->(x) { x * x }
来源：http://vr.jianghongdianzi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://la.panjiajie.cn

[C07] 把函数作为参数传入
来源：http://pb.nicolike.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ze.newstarts.cn

PHP:  array_map("strtoupper", $arr);
来源：http://qy.huixiangedu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zr.shxzskj.cn

TS:   arr.map(String)
来源：http://aa.wgjwhj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://at.yuntaijiaju.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hm.hnjuh.cn

Ruby: arr.map(&:upcase)
来源：http://aa.jianghongdianzi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wf.shtwfgs.cn

[C08] 闭包
来源：http://op.wgjwhj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kx.yuexingan06.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hh.newstarts.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zv.jianghongdianzi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://oz.hahajie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dm.yuexingan06.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fw.shxzskj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://oo.hnjuh.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://di.jctech888.com.cn

[C09] 递归
来源：http://vy.wgjwhj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bo.asd995.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ec.szxytkj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jt.9csxet.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bu.muxihuayi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ek.hahajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ng.shtwfgs.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lw.gzmigu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zs.nszjky.cn

[C10] 变量作用域
来源：http://gc.nszjky.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zy.jctech888.com.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://uh.colortex.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://in.wgjwhj.cn

TS:   同 JS
来源：http://cy.nszjky.cn

Java: 方法内为块级作用域
来源：http://ec.szsharing.cn

Go:   花括号块级作用域
来源：http://kw.huanxung.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hu.bjjhwx.cn

C#:   块级作用域
来源：http://fo.szsharing.cn

[C11] 模块导入与导出
来源：http://ey.jianghongdianzi.cn

Py:   from module import func
来源：http://kr.colortex.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kx.chemitech.net.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vq.hnjuh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cy.bookmarksfly.cn

Java: import java.util.List;
来源：http://ml.jianghongdianzi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ba.huixinmuqiang.cn

Ruby: require "json"; require_relative "./util"
来源：http://fy.jctech888.com.cn

C#:   using System.Text;
来源：http://lr.szxytkj.cn

[C12] 立即执行函数 IIFE
来源：http://jf.huanxung.cn

Py:   (lambda: print("run"))()
来源：http://vb.9csxet.cn

PHP:  (function () { echo "run"; })();
来源：http://aa.jianghongdianzi.cn

JS:   (() => { console.log("run"); })();
来源：http://ks.521024.cn

TS:   (() => { console.log("run"); })();
来源：http://te.bookmarksfly.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://uh.yuntaijiaju.cn

Go:   func() { fmt.Println("run") }()
来源：http://ib.muxihuayi.cn

Ruby: -> { puts "run" }.call
来源：http://lz.yuntaijiaju.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://cv.lnxyls.cn

[C13] 类型声明 / 类型注解
来源：http://qo.gzmigu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qk.shxzskj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sl.haigaiapp.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tp.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bs.bookmarksfly.cn

Java: int add(int a, int b) { return a + b; }
来源：http://au.nszjky.cn

Go:   func add(a, b int) int
来源：http://xo.panjiajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yl.9csxet.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wo.haigaiapp.cn

[C14] 泛型函数
来源：http://zl.gzmigu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ac.szsharing.cn

PHP:  // 无泛型
来源：http://dn.bjjhwx.cn

JS:   // 无泛型
来源：http://iv.shtwfgs.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gx.wgjwhj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gc.yuexingan06.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ps.bjjhwx.cn

Ruby: # 无泛型
来源：http://zw.wgjwhj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sc.jianghongdianzi.cn

[C15] 解构 / 展开参数
来源：http://jh.9csxet.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ja.yuexingan06.cn

PHP:  [$a, $b] = $pair;
来源：http://lb.jctech888.com.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rs.nicolike.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gz.nszjky.cn

Java: // 无解构
来源：http://nh.shtwfgs.cn

Go:   // 无解构
来源：http://zr.shxzskj.cn

Ruby: a, b = pair
来源：http://aj.gzmigu.cn

C#:   var (a, b) = pair;
来源：http://cr.gzmigu.cn

[C16] 函数 / 方法重载
来源：http://vs.shxzskj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bq.lnxyls.cn

PHP:  // 无重载
来源：http://wn.shxzukj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://uy.jctech888.com.cn

TS:   // 用联合类型或重载签名声明
来源：http://zq.nicolike.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://yl.asd995.cn

Go:   // 无重载：用不同函数名
来源：http://md.chemitech.net.cn

Ruby: # 无重载：靠动态参数
来源：http://lt.shxzskj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fw.jctech888.com.cn

================================================================================
来源：http://fz.huanxung.cn

D. 数组 / 列表 / 集合
来源：http://xt.muxihuayi.cn

================================================================================
来源：http://yk.shtwfgs.cn

[D01] 创建数组 / 列表
来源：http://dg.bookmarksfly.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mp.shxzukj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dd.hahajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sq.huixiangedu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ip.wgjwhj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lz.shxzukj.cn

Go:   arr := []int{1, 2, 3}
来源：http://fy.lnxyls.cn

Ruby: arr = [1, 2, 3]
来源：http://wm.yuntaijiaju.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://st.newstarts.cn

[D02] 追加元素到末尾
来源：http://ft.wgjwhj.cn


<!-- 参考信息 -->