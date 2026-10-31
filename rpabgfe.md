代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gs.szsharing.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://aq.wgjwhj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hl.hnjuh.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wv.newstarts.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ri.gzmigu.cn

[B02] 多分支 else if / elif
来源：http://ma.newstarts.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zi.panjiajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ol.shtwfgs.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tc.huanxung.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nz.szsharing.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ta.bookmarksfly.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ub.nszjky.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://iu.szxytkj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uc.newstarts.cn

[B03] switch / match / case
来源：http://cs.shxzukj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ze.bookmarksfly.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vr.wgjwhj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rs.9csxet.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hh.colortex.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zb.jctech888.com.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zl.lnxyls.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jb.huixiangedu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wh.nszjky.cn

[B04] for 计数循环
来源：http://gt.muxihuayi.cn

Py:   for i in range(10): print(i)
来源：http://bs.nszjky.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://or.yuexingan06.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rp.jctech888.com.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qs.chemitech.net.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yk.asd995.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hr.huixinmuqiang.cn

Ruby: 10.times { |i| puts i }
来源：http://xf.gzmigu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://oa.haigaiapp.cn

[B05] 遍历数组 / 列表
来源：http://wc.shxzukj.cn

Py:   for item in arr: print(item)
来源：http://yi.colortex.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hm.9csxet.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://jn.9csxet.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://nh.huanxung.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sv.colortex.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vz.lnxyls.cn

Ruby: arr.each { |item| puts item }
来源：http://bi.chemitech.net.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xg.asd995.cn

[B06] 遍历字典 / 对象
来源：http://xc.jianghongdianzi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ve.hnjuh.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ul.szsharing.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eh.bjjhwx.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bj.newstarts.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dw.hnjuh.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cg.newstarts.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://to.shxzskj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://na.szsharing.cn

[B07] while 循环
来源：http://je.asd995.cn

Py:   while i < 10: i += 1
来源：http://dx.nszjky.cn

PHP:  while ($i < 10) { $i++; }
来源：http://kx.jianghongdianzi.cn

JS:   while (i < 10) { i++; }
来源：http://vv.huanxung.cn

TS:   while (i < 10) { i++; }
来源：http://qj.huanxung.cn

Java: while (i < 10) { i++; }
来源：http://sz.bjjhwx.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wl.9csxet.cn

Ruby: while i < 10; i += 1; end
来源：http://jl.yuntaijiaju.cn

C#:   while (i < 10) { i++; }
来源：http://pa.shxzukj.cn

[B08] do-while（至少执行一次）
来源：http://mw.hahajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://mt.yuexingan06.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://oq.szsharing.cn

JS:   do { i++; } while (i < 10);
来源：http://lb.muxihuayi.cn

TS:   do { i++; } while (i < 10);
来源：http://zi.hnjuh.cn

Java: do { i++; } while (i < 10);
来源：http://ja.asd995.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://st.nszjky.cn

Ruby: begin; i += 1; end while i < 10
来源：http://gm.szsharing.cn

C#:   do { i++; } while (i < 10);
来源：http://nr.hahajie.cn

[B09] break 与 continue
来源：http://vg.haigaiapp.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://px.shxzskj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://md.jianghongdianzi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kf.jctech888.com.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ie.jctech888.com.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ow.nicolike.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ds.521024.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://us.asd995.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qj.colortex.cn

[B10] 遍历同时拿索引
来源：http://ix.newstarts.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qn.colortex.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nx.hahajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yg.panjiajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://og.shxzskj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://av.yuexingan06.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qh.lnxyls.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sg.chemitech.net.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zr.shxzukj.cn

[B11] 生成数字序列 / 区间
来源：http://cy.chemitech.net.cn

Py:   list(range(0, 10, 2))
来源：http://rf.huixinmuqiang.cn

PHP:  range(0, 10, 2);
来源：http://vy.haigaiapp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://al.shxzskj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bw.jctech888.com.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rk.521024.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://id.lnxyls.cn

Ruby: (0...10).step(2).to_a
来源：http://ug.nszjky.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://li.yuntaijiaju.cn

[B12] 跳出多层循环
来源：http://ud.shtwfgs.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://mo.asd995.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://rx.shtwfgs.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jm.gzmigu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vt.shtwfgs.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jq.yuntaijiaju.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tl.521024.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ix.shxzskj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gk.yuntaijiaju.cn

[B13] 判断是否为数字
来源：http://zn.chemitech.net.cn

Py:   isinstance(x, (int, float))
来源：http://eb.asd995.cn

PHP:  is_numeric($x)
来源：http://nh.9csxet.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ri.asd995.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lp.panjiajie.cn

Java: x instanceof Number
来源：http://dx.panjiajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ad.huixiangedu.cn

Ruby: x.is_a?(Numeric)
来源：http://pl.szxytkj.cn

C#:   x is int or double or decimal
来源：http://jx.muxihuayi.cn

[B14] 判断值是否在集合内
来源：http://bc.shtwfgs.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ot.colortex.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ml.9csxet.cn

JS:   [1, 2, 3].includes(x)
来源：http://si.hahajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://dd.bjjhwx.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://jc.jctech888.com.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xp.szxytkj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ie.lnxyls.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ei.colortex.cn

[B15] 布尔运算与取反
来源：http://hs.shxzskj.cn

Py:   a and b or not c
来源：http://hg.nszjky.cn

PHP:  $a && $b || !$c
来源：http://jh.9csxet.cn

JS:   a && b || !c
来源：http://vx.yuntaijiaju.cn

TS:   a && b || !c
来源：http://uh.colortex.cn

Java: a && b || !c
来源：http://nw.colortex.cn

Go:   a && b || !c
来源：http://eq.nicolike.cn

Ruby: a && b || !c
来源：http://wz.chemitech.net.cn

C#:   a && b || !c
来源：http://tm.nszjky.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vn.panjiajie.cn

Py:   if not data: return
来源：http://ax.nicolike.cn

PHP:  if (!$data) { return; }
来源：http://lp.chemitech.net.cn

JS:   if (!data) return;
来源：http://oz.jctech888.com.cn

TS:   if (!data) return;
来源：http://wd.chemitech.net.cn

Java: if (data == null) return;
来源：http://ta.yuntaijiaju.cn

Go:   if data == nil { return }
来源：http://vh.huanxung.cn

Ruby: return if data.nil?
来源：http://ai.shxzukj.cn

C#:   if (data == null) return;
来源：http://ar.nicolike.cn

================================================================================
来源：http://bf.wgjwhj.cn

C. 函数与作用域
来源：http://wb.panjiajie.cn

================================================================================
来源：http://vk.hnjuh.cn

[C01] 定义函数
来源：http://yc.szsharing.cn

Py:   def add(a, b): return a + b
来源：http://jk.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zp.lnxyls.cn

JS:   function add(a, b) { return a + b; }
来源：http://ng.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rv.nszjky.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dt.bookmarksfly.cn

Go:   func add(a, b int) int { return a + b }
来源：http://sx.bookmarksfly.cn

Ruby: def add(a, b); a + b; end
来源：http://cv.hahajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cy.nicolike.cn

[C02] 默认参数
来源：http://hw.shtwfgs.cn

Py:   def greet(name="World"): return name
来源：http://qv.hahajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tj.gzmigu.cn

JS:   function greet(name = "World") { return name; }
来源：http://cg.hnjuh.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://he.panjiajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dp.newstarts.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kb.yuntaijiaju.cn

Ruby: def greet(name = "World") = name
来源：http://hr.hnjuh.cn

C#:   string Greet(string name = "World") => name;
来源：http://xj.haigaiapp.cn

[C03] 可变参数
来源：http://rr.nicolike.cn

Py:   def total(*args): return sum(args)
来源：http://lc.shtwfgs.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ko.huixiangedu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fd.asd995.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vh.huixiangedu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rc.lnxyls.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://am.wgjwhj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://jj.hahajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cx.hnjuh.cn

[C04] 命名参数 / 关键字参数
来源：http://ho.nszjky.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uf.wgjwhj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vs.szxytkj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ul.muxihuayi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jy.jctech888.com.cn

Java: // 无：用 Builder 模式或 record
来源：http://fk.hnjuh.cn

Go:   // 无：用配置结构体参数
来源：http://ad.521024.cn

Ruby: f(a: 1, b: 2)
来源：http://pz.colortex.cn

C#:   f(a: 1, b: 2)
来源：http://os.szxytkj.cn

[C05] 返回多个值
来源：http://xp.newstarts.cn

Py:   return a, b
来源：http://fi.yuntaijiaju.cn

PHP:  return [$a, $b];
来源：http://ag.yuexingan06.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://kx.yuntaijiaju.cn

TS:   return { a, b };
来源：http://lu.shtwfgs.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xi.asd995.cn

Go:   return a, b
来源：http://gf.chemitech.net.cn

Ruby: return a, b
来源：http://ph.szxytkj.cn

C#:   return (a, b);              // ValueTuple
来源：http://op.jianghongdianzi.cn

[C06] 匿名函数 / lambda
来源：http://ot.nicolike.cn

Py:   square = lambda x: x * x
来源：http://xw.bookmarksfly.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fy.panjiajie.cn

JS:   const square = x => x * x;
来源：http://sk.shxzskj.cn

TS:   const square = (x: number): number => x * x;
来源：http://zr.szxytkj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wy.nszjky.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qm.9csxet.cn

Ruby: square = ->(x) { x * x }
来源：http://vz.hahajie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ow.huixiangedu.cn

[C07] 把函数作为参数传入
来源：http://jf.yuexingan06.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qw.shtwfgs.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ca.521024.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ay.colortex.cn

TS:   arr.map(String)
来源：http://kf.nszjky.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ds.chemitech.net.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zd.lnxyls.cn

Ruby: arr.map(&:upcase)
来源：http://xb.huixinmuqiang.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://be.shtwfgs.cn

[C08] 闭包
来源：http://fe.huixinmuqiang.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qw.lnxyls.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rc.chemitech.net.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://aj.panjiajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ul.huixinmuqiang.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ua.newstarts.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://es.muxihuayi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qh.hnjuh.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://it.szxytkj.cn

[C09] 递归
来源：http://ga.nszjky.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xp.shxzukj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://eo.nicolike.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dp.gzmigu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dt.szsharing.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kw.colortex.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ix.yuexingan06.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hy.bjjhwx.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sa.chemitech.net.cn

[C10] 变量作用域
来源：http://jf.szxytkj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rg.shxzskj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ft.hnjuh.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ar.shxzukj.cn

TS:   同 JS
来源：http://wx.newstarts.cn

Java: 方法内为块级作用域
来源：http://bw.szxytkj.cn

Go:   花括号块级作用域
来源：http://eg.szxytkj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yu.huixiangedu.cn

C#:   块级作用域
来源：http://hl.hnjuh.cn

[C11] 模块导入与导出
来源：http://xo.colortex.cn

Py:   from module import func
来源：http://ku.yuexingan06.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zx.nicolike.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gq.newstarts.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gz.9csxet.cn

Java: import java.util.List;
来源：http://nc.asd995.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cn.panjiajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://qs.nszjky.cn

C#:   using System.Text;
来源：http://os.newstarts.cn

[C12] 立即执行函数 IIFE
来源：http://xr.nicolike.cn

Py:   (lambda: print("run"))()
来源：http://kk.szxytkj.cn

PHP:  (function () { echo "run"; })();
来源：http://fk.jctech888.com.cn

JS:   (() => { console.log("run"); })();
来源：http://xz.panjiajie.cn

TS:   (() => { console.log("run"); })();
来源：http://dz.huanxung.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xc.shxzskj.cn

Go:   func() { fmt.Println("run") }()
来源：http://mh.yuexingan06.cn

Ruby: -> { puts "run" }.call
来源：http://ys.haigaiapp.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ci.jianghongdianzi.cn

[C13] 类型声明 / 类型注解
来源：http://dj.shxzskj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ac.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pu.hahajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ta.panjiajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://td.chemitech.net.cn

Java: int add(int a, int b) { return a + b; }
来源：http://aw.szxytkj.cn

Go:   func add(a, b int) int
来源：http://vv.yuexingan06.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vo.shxzukj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://no.huixiangedu.cn

[C14] 泛型函数
来源：http://fh.yuntaijiaju.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cf.hnjuh.cn

PHP:  // 无泛型
来源：http://qj.muxihuayi.cn

JS:   // 无泛型
来源：http://hh.bookmarksfly.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://re.chemitech.net.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jx.yuexingan06.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wj.chemitech.net.cn

Ruby: # 无泛型
来源：http://yj.panjiajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cl.szxytkj.cn

[C15] 解构 / 展开参数
来源：http://pw.asd995.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tz.muxihuayi.cn

PHP:  [$a, $b] = $pair;
来源：http://vy.hahajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gw.nszjky.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://op.newstarts.cn

Java: // 无解构
来源：http://ja.9csxet.cn

Go:   // 无解构
来源：http://bq.panjiajie.cn

Ruby: a, b = pair
来源：http://ow.yuexingan06.cn

C#:   var (a, b) = pair;
来源：http://td.bookmarksfly.cn

[C16] 函数 / 方法重载
来源：http://hr.haigaiapp.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fp.huixinmuqiang.cn

PHP:  // 无重载
来源：http://pp.shxzukj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ql.szsharing.cn

TS:   // 用联合类型或重载签名声明
来源：http://yd.lnxyls.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://lt.chemitech.net.cn

Go:   // 无重载：用不同函数名
来源：http://lb.bookmarksfly.cn

Ruby: # 无重载：靠动态参数
来源：http://fw.shtwfgs.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://wc.muxihuayi.cn

================================================================================
来源：http://zh.yuexingan06.cn

D. 数组 / 列表 / 集合
来源：http://ii.hahajie.cn

================================================================================
来源：http://or.jctech888.com.cn

[D01] 创建数组 / 列表
来源：http://ni.szsharing.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fd.chemitech.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://is.asd995.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://oi.hnjuh.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://mv.nszjky.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gl.shxzukj.cn

Go:   arr := []int{1, 2, 3}
来源：http://rb.hnjuh.cn

Ruby: arr = [1, 2, 3]
来源：http://jg.gzmigu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pv.yuntaijiaju.cn

[D02] 追加元素到末尾
来源：http://cr.szxytkj.cn


<!-- 参考信息 -->