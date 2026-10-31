代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://qg.shxzukj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://im.bjjhwx.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lq.colortex.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ht.huixiangedu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dx.gzmigu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xk.shxzskj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://tw.hahajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fh.chemitech.net.cn

[A26] 类型转换总览
来源：http://la.lnxyls.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xb.hahajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uf.hahajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pl.jctech888.com.cn

TS:   Number() String() Boolean() x as number
来源：http://am.jctech888.com.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://oy.huixiangedu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ay.yuexingan06.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rn.hahajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ms.chemitech.net.cn

================================================================================
来源：http://bf.newstarts.cn

B. 流程控制
来源：http://ui.shtwfgs.cn

================================================================================
来源：http://dg.haigaiapp.cn

[B01] 条件判断 if / else
来源：http://mw.nicolike.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bb.hnjuh.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cy.521024.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rz.wgjwhj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ts.muxihuayi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://yr.jctech888.com.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pc.haigaiapp.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tr.nszjky.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ez.szxytkj.cn

[B02] 多分支 else if / elif
来源：http://xp.huixinmuqiang.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sh.jianghongdianzi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ih.bjjhwx.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://af.nicolike.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://km.yuntaijiaju.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ps.hahajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wu.huixiangedu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ly.colortex.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vt.lnxyls.cn

[B03] switch / match / case
来源：http://yk.521024.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rj.szsharing.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wh.huanxung.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gk.9csxet.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lv.chemitech.net.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bh.521024.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rv.shxzukj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pu.shtwfgs.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ds.9csxet.cn

[B04] for 计数循环
来源：http://fn.bookmarksfly.cn

Py:   for i in range(10): print(i)
来源：http://oo.521024.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ir.nszjky.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bk.chemitech.net.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jr.yuexingan06.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hd.yuexingan06.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ul.jctech888.com.cn

Ruby: 10.times { |i| puts i }
来源：http://jq.asd995.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gk.shtwfgs.cn

[B05] 遍历数组 / 列表
来源：http://nk.newstarts.cn

Py:   for item in arr: print(item)
来源：http://bd.hahajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wc.bookmarksfly.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ot.yuexingan06.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://sm.bookmarksfly.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gx.jctech888.com.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xf.yuexingan06.cn

Ruby: arr.each { |item| puts item }
来源：http://jh.bjjhwx.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yl.yuntaijiaju.cn

[B06] 遍历字典 / 对象
来源：http://ep.szxytkj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ry.bjjhwx.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cz.yuntaijiaju.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vh.lnxyls.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cj.lnxyls.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://md.hahajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cz.huixinmuqiang.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bd.panjiajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kz.nicolike.cn

[B07] while 循环
来源：http://sw.wgjwhj.cn

Py:   while i < 10: i += 1
来源：http://ag.panjiajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://jq.shxzskj.cn

JS:   while (i < 10) { i++; }
来源：http://ru.nszjky.cn

TS:   while (i < 10) { i++; }
来源：http://mf.jctech888.com.cn

Java: while (i < 10) { i++; }
来源：http://pg.szxytkj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://by.9csxet.cn

Ruby: while i < 10; i += 1; end
来源：http://dj.jianghongdianzi.cn

C#:   while (i < 10) { i++; }
来源：http://lf.shxzskj.cn

[B08] do-while（至少执行一次）
来源：http://nm.huanxung.cn

Py:   # 无 do-while：用 while True + break
来源：http://sc.hahajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://di.huanxung.cn

JS:   do { i++; } while (i < 10);
来源：http://jx.jctech888.com.cn

TS:   do { i++; } while (i < 10);
来源：http://hw.shtwfgs.cn

Java: do { i++; } while (i < 10);
来源：http://ov.muxihuayi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sm.9csxet.cn

Ruby: begin; i += 1; end while i < 10
来源：http://nu.bookmarksfly.cn

C#:   do { i++; } while (i < 10);
来源：http://ov.jctech888.com.cn

[B09] break 与 continue
来源：http://ol.shtwfgs.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sd.hahajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ig.panjiajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wf.bjjhwx.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qi.jianghongdianzi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://co.haigaiapp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jf.yuntaijiaju.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qm.hnjuh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ui.wgjwhj.cn

[B10] 遍历同时拿索引
来源：http://um.colortex.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yg.wgjwhj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bg.wgjwhj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bb.nicolike.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yo.muxihuayi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zb.wgjwhj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rt.lnxyls.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mm.shxzskj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pw.colortex.cn

[B11] 生成数字序列 / 区间
来源：http://mo.shxzskj.cn

Py:   list(range(0, 10, 2))
来源：http://em.jianghongdianzi.cn

PHP:  range(0, 10, 2);
来源：http://ak.yuexingan06.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://km.huanxung.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kt.huixinmuqiang.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xm.chemitech.net.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nw.nszjky.cn

Ruby: (0...10).step(2).to_a
来源：http://uz.lnxyls.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://af.nszjky.cn

[B12] 跳出多层循环
来源：http://hi.chemitech.net.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yl.jianghongdianzi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://sa.hahajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lx.colortex.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pl.chemitech.net.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ua.nicolike.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kb.szsharing.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sm.chemitech.net.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ta.9csxet.cn

[B13] 判断是否为数字
来源：http://oo.jctech888.com.cn

Py:   isinstance(x, (int, float))
来源：http://jk.lnxyls.cn

PHP:  is_numeric($x)
来源：http://ja.huanxung.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pm.hnjuh.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kr.9csxet.cn

Java: x instanceof Number
来源：http://yu.chemitech.net.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bi.colortex.cn

Ruby: x.is_a?(Numeric)
来源：http://ji.wgjwhj.cn

C#:   x is int or double or decimal
来源：http://ga.9csxet.cn

[B14] 判断值是否在集合内
来源：http://je.lnxyls.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kr.shxzukj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zh.bookmarksfly.cn

JS:   [1, 2, 3].includes(x)
来源：http://fn.jianghongdianzi.cn

TS:   [1, 2, 3].includes(x)
来源：http://ij.wgjwhj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ju.nszjky.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ui.521024.cn

Ruby: [1, 2, 3].include?(x)
来源：http://kj.jctech888.com.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://de.bjjhwx.cn

[B15] 布尔运算与取反
来源：http://ro.jctech888.com.cn

Py:   a and b or not c
来源：http://ok.panjiajie.cn

PHP:  $a && $b || !$c
来源：http://ag.newstarts.cn

JS:   a && b || !c
来源：http://ha.newstarts.cn

TS:   a && b || !c
来源：http://wv.wgjwhj.cn

Java: a && b || !c
来源：http://qx.bjjhwx.cn

Go:   a && b || !c
来源：http://hl.yuexingan06.cn

Ruby: a && b || !c
来源：http://cu.newstarts.cn

C#:   a && b || !c
来源：http://yh.yuntaijiaju.cn

[B16] 卫语句：不满足条件提前返回
来源：http://dh.bjjhwx.cn

Py:   if not data: return
来源：http://ex.shxzukj.cn

PHP:  if (!$data) { return; }
来源：http://as.521024.cn

JS:   if (!data) return;
来源：http://jc.wgjwhj.cn

TS:   if (!data) return;
来源：http://st.bjjhwx.cn

Java: if (data == null) return;
来源：http://dz.jianghongdianzi.cn

Go:   if data == nil { return }
来源：http://la.shtwfgs.cn

Ruby: return if data.nil?
来源：http://oc.yuexingan06.cn

C#:   if (data == null) return;
来源：http://hh.szxytkj.cn

================================================================================
来源：http://yk.jianghongdianzi.cn

C. 函数与作用域
来源：http://jh.lnxyls.cn

================================================================================
来源：http://wm.muxihuayi.cn

[C01] 定义函数
来源：http://jg.9csxet.cn

Py:   def add(a, b): return a + b
来源：http://rf.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wl.shxzskj.cn

JS:   function add(a, b) { return a + b; }
来源：http://mz.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qd.yuntaijiaju.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://nt.hahajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://pi.haigaiapp.cn

Ruby: def add(a, b); a + b; end
来源：http://pu.huixinmuqiang.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rr.jctech888.com.cn

[C02] 默认参数
来源：http://av.huixiangedu.cn

Py:   def greet(name="World"): return name
来源：http://bl.nicolike.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zh.muxihuayi.cn

JS:   function greet(name = "World") { return name; }
来源：http://gl.huanxung.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ux.jctech888.com.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://km.bookmarksfly.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://uh.muxihuayi.cn

Ruby: def greet(name = "World") = name
来源：http://kt.muxihuayi.cn

C#:   string Greet(string name = "World") => name;
来源：http://jf.colortex.cn

[C03] 可变参数
来源：http://rb.nicolike.cn

Py:   def total(*args): return sum(args)
来源：http://xc.gzmigu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rc.muxihuayi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ji.jctech888.com.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hm.521024.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nd.szxytkj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pn.shxzukj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wo.chemitech.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zv.chemitech.net.cn

[C04] 命名参数 / 关键字参数
来源：http://zm.shtwfgs.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wo.huanxung.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ib.huanxung.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vs.newstarts.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wx.yuntaijiaju.cn

Java: // 无：用 Builder 模式或 record
来源：http://bi.newstarts.cn

Go:   // 无：用配置结构体参数
来源：http://nx.shtwfgs.cn

Ruby: f(a: 1, b: 2)
来源：http://kh.yuntaijiaju.cn

C#:   f(a: 1, b: 2)
来源：http://td.muxihuayi.cn

[C05] 返回多个值
来源：http://wj.gzmigu.cn

Py:   return a, b
来源：http://pm.lnxyls.cn

PHP:  return [$a, $b];
来源：http://rj.huixiangedu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zp.shxzukj.cn

TS:   return { a, b };
来源：http://uk.nszjky.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://aq.bjjhwx.cn

Go:   return a, b
来源：http://jl.newstarts.cn

Ruby: return a, b
来源：http://av.521024.cn

C#:   return (a, b);              // ValueTuple
来源：http://zy.yuexingan06.cn

[C06] 匿名函数 / lambda
来源：http://qe.chemitech.net.cn

Py:   square = lambda x: x * x
来源：http://qh.9csxet.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pe.jianghongdianzi.cn

JS:   const square = x => x * x;
来源：http://oy.jianghongdianzi.cn

TS:   const square = (x: number): number => x * x;
来源：http://ut.newstarts.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mw.huixiangedu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://eo.szxytkj.cn

Ruby: square = ->(x) { x * x }
来源：http://oc.yuntaijiaju.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ky.nszjky.cn

[C07] 把函数作为参数传入
来源：http://jq.szsharing.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://er.shxzukj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://mn.asd995.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://em.huanxung.cn

TS:   arr.map(String)
来源：http://ze.yuntaijiaju.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gm.jctech888.com.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gf.panjiajie.cn

Ruby: arr.map(&:upcase)
来源：http://ql.chemitech.net.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qr.panjiajie.cn

[C08] 闭包
来源：http://yx.shxzukj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mf.9csxet.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ga.muxihuayi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gh.hnjuh.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ul.muxihuayi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rp.shxzukj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rq.huixiangedu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ec.yuntaijiaju.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vn.yuntaijiaju.cn

[C09] 递归
来源：http://ts.huixinmuqiang.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xy.521024.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ge.hnjuh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cx.521024.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fy.bookmarksfly.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ib.shtwfgs.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fi.shxzukj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://br.hahajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pa.wgjwhj.cn

[C10] 变量作用域
来源：http://bu.hahajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xy.lnxyls.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pq.haigaiapp.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://be.huixinmuqiang.cn

TS:   同 JS
来源：http://xa.asd995.cn

Java: 方法内为块级作用域
来源：http://ro.9csxet.cn

Go:   花括号块级作用域
来源：http://fy.nszjky.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pu.colortex.cn

C#:   块级作用域
来源：http://ca.wgjwhj.cn

[C11] 模块导入与导出
来源：http://so.colortex.cn

Py:   from module import func
来源：http://wo.hahajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://yw.shxzukj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://yb.wgjwhj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ox.huanxung.cn

Java: import java.util.List;
来源：http://ws.nszjky.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://aa.chemitech.net.cn

Ruby: require "json"; require_relative "./util"
来源：http://hp.huixiangedu.cn

C#:   using System.Text;
来源：http://ft.yuexingan06.cn

[C12] 立即执行函数 IIFE
来源：http://yr.panjiajie.cn

Py:   (lambda: print("run"))()
来源：http://ds.newstarts.cn

PHP:  (function () { echo "run"; })();
来源：http://ky.jianghongdianzi.cn

JS:   (() => { console.log("run"); })();
来源：http://yl.muxihuayi.cn

TS:   (() => { console.log("run"); })();
来源：http://ya.jctech888.com.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ue.shxzukj.cn

Go:   func() { fmt.Println("run") }()
来源：http://fk.bjjhwx.cn

Ruby: -> { puts "run" }.call
来源：http://gs.szxytkj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gz.jctech888.com.cn

[C13] 类型声明 / 类型注解
来源：http://kc.shxzukj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fw.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kz.nszjky.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sb.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ul.yuexingan06.cn

Java: int add(int a, int b) { return a + b; }
来源：http://sw.521024.cn

Go:   func add(a, b int) int
来源：http://cs.lnxyls.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wb.hahajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://jg.szxytkj.cn

[C14] 泛型函数
来源：http://fw.bookmarksfly.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pq.muxihuayi.cn

PHP:  // 无泛型
来源：http://xy.jianghongdianzi.cn

JS:   // 无泛型
来源：http://id.muxihuayi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ac.wgjwhj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bz.colortex.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zw.panjiajie.cn

Ruby: # 无泛型
来源：http://gu.521024.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kh.huanxung.cn

[C15] 解构 / 展开参数
来源：http://de.9csxet.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kr.lnxyls.cn

PHP:  [$a, $b] = $pair;
来源：http://nz.huanxung.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rv.nicolike.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://da.chemitech.net.cn

Java: // 无解构
来源：http://fh.yuntaijiaju.cn

Go:   // 无解构
来源：http://aw.jianghongdianzi.cn


<!-- 参考信息 -->