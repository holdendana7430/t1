代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://lz.yuntaijiaju.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ev.huixinmuqiang.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://do.shtwfgs.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zf.hnjuh.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rn.521024.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://li.bookmarksfly.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ub.newstarts.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vr.lnxyls.cn

[A26] 类型转换总览
来源：http://iq.yuexingan06.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://oj.bookmarksfly.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gr.panjiajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qp.muxihuayi.cn

TS:   Number() String() Boolean() x as number
来源：http://jo.colortex.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://la.9csxet.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ua.jctech888.com.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ih.jctech888.com.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lw.nicolike.cn

================================================================================
来源：http://bb.jctech888.com.cn

B. 流程控制
来源：http://xr.haigaiapp.cn

================================================================================
来源：http://xp.newstarts.cn

[B01] 条件判断 if / else
来源：http://cr.newstarts.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://pt.nszjky.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wi.szsharing.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vj.huixiangedu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qr.muxihuayi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xc.muxihuayi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ep.hahajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ln.shxzukj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xr.bookmarksfly.cn

[B02] 多分支 else if / elif
来源：http://fg.hahajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xh.lnxyls.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mv.szsharing.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ld.panjiajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mv.haigaiapp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xb.muxihuayi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://su.yuntaijiaju.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rb.muxihuayi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ly.panjiajie.cn

[B03] switch / match / case
来源：http://um.huixiangedu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ga.bookmarksfly.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ou.panjiajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://aw.newstarts.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wu.521024.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hd.nszjky.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://co.lnxyls.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dp.shxzukj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cd.asd995.cn

[B04] for 计数循环
来源：http://sj.panjiajie.cn

Py:   for i in range(10): print(i)
来源：http://ws.yuexingan06.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ji.wgjwhj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zc.bjjhwx.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kb.bookmarksfly.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yw.gzmigu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gf.jctech888.com.cn

Ruby: 10.times { |i| puts i }
来源：http://dm.huixinmuqiang.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pv.haigaiapp.cn

[B05] 遍历数组 / 列表
来源：http://wu.panjiajie.cn

Py:   for item in arr: print(item)
来源：http://ie.nicolike.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://iy.yuntaijiaju.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://cd.nicolike.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ay.gzmigu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sx.huixinmuqiang.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dm.nszjky.cn

Ruby: arr.each { |item| puts item }
来源：http://vl.huixinmuqiang.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://et.9csxet.cn

[B06] 遍历字典 / 对象
来源：http://oi.chemitech.net.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://bc.9csxet.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hq.yuexingan06.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eb.asd995.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rl.bookmarksfly.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lj.jctech888.com.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ab.huixiangedu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vz.shxzukj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yo.colortex.cn

[B07] while 循环
来源：http://pq.shxzskj.cn

Py:   while i < 10: i += 1
来源：http://yr.shtwfgs.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fi.yuntaijiaju.cn

JS:   while (i < 10) { i++; }
来源：http://tg.szxytkj.cn

TS:   while (i < 10) { i++; }
来源：http://ez.huixinmuqiang.cn

Java: while (i < 10) { i++; }
来源：http://wl.shtwfgs.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ij.gzmigu.cn

Ruby: while i < 10; i += 1; end
来源：http://ij.shtwfgs.cn

C#:   while (i < 10) { i++; }
来源：http://pi.jianghongdianzi.cn

[B08] do-while（至少执行一次）
来源：http://eq.panjiajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://ph.szxytkj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://rf.wgjwhj.cn

JS:   do { i++; } while (i < 10);
来源：http://kc.yuexingan06.cn

TS:   do { i++; } while (i < 10);
来源：http://zb.colortex.cn

Java: do { i++; } while (i < 10);
来源：http://ul.jianghongdianzi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://lh.newstarts.cn

Ruby: begin; i += 1; end while i < 10
来源：http://nq.gzmigu.cn

C#:   do { i++; } while (i < 10);
来源：http://ta.huixinmuqiang.cn

[B09] break 与 continue
来源：http://pv.chemitech.net.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ij.muxihuayi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jp.521024.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wb.jianghongdianzi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gm.nszjky.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ko.wgjwhj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rz.hnjuh.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cr.shxzskj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sg.szxytkj.cn

[B10] 遍历同时拿索引
来源：http://vc.yuntaijiaju.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vf.yuexingan06.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yz.chemitech.net.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dm.hnjuh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ip.bookmarksfly.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://na.bookmarksfly.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://og.shxzukj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://va.huanxung.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ry.shxzukj.cn

[B11] 生成数字序列 / 区间
来源：http://lk.huixinmuqiang.cn

Py:   list(range(0, 10, 2))
来源：http://nx.panjiajie.cn

PHP:  range(0, 10, 2);
来源：http://sc.chemitech.net.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ry.shtwfgs.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qf.shtwfgs.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fk.lnxyls.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kj.bookmarksfly.cn

Ruby: (0...10).step(2).to_a
来源：http://em.9csxet.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dt.huixinmuqiang.cn

[B12] 跳出多层循环
来源：http://lf.shxzukj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://qz.huixiangedu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zj.haigaiapp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ab.shxzukj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sf.shxzukj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ab.jianghongdianzi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hf.jianghongdianzi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ex.colortex.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tg.gzmigu.cn

[B13] 判断是否为数字
来源：http://ah.gzmigu.cn

Py:   isinstance(x, (int, float))
来源：http://wn.chemitech.net.cn

PHP:  is_numeric($x)
来源：http://ts.huanxung.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qj.9csxet.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bo.szxytkj.cn

Java: x instanceof Number
来源：http://kw.9csxet.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pc.colortex.cn

Ruby: x.is_a?(Numeric)
来源：http://ow.jianghongdianzi.cn

C#:   x is int or double or decimal
来源：http://sd.huanxung.cn

[B14] 判断值是否在集合内
来源：http://ol.jianghongdianzi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zs.hnjuh.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gi.huixiangedu.cn

JS:   [1, 2, 3].includes(x)
来源：http://fv.jianghongdianzi.cn

TS:   [1, 2, 3].includes(x)
来源：http://bg.nszjky.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://bz.shxzskj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pl.chemitech.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jz.chemitech.net.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qb.jctech888.com.cn

[B15] 布尔运算与取反
来源：http://ff.huixiangedu.cn

Py:   a and b or not c
来源：http://nw.lnxyls.cn

PHP:  $a && $b || !$c
来源：http://vf.muxihuayi.cn

JS:   a && b || !c
来源：http://ul.shtwfgs.cn

TS:   a && b || !c
来源：http://ry.panjiajie.cn

Java: a && b || !c
来源：http://na.szxytkj.cn

Go:   a && b || !c
来源：http://vk.colortex.cn

Ruby: a && b || !c
来源：http://mp.wgjwhj.cn

C#:   a && b || !c
来源：http://xf.huixinmuqiang.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jc.asd995.cn

Py:   if not data: return
来源：http://yn.521024.cn

PHP:  if (!$data) { return; }
来源：http://cj.szsharing.cn

JS:   if (!data) return;
来源：http://lr.asd995.cn

TS:   if (!data) return;
来源：http://hh.huixiangedu.cn

Java: if (data == null) return;
来源：http://xu.bookmarksfly.cn

Go:   if data == nil { return }
来源：http://qt.521024.cn

Ruby: return if data.nil?
来源：http://ex.asd995.cn

C#:   if (data == null) return;
来源：http://xr.jianghongdianzi.cn

================================================================================
来源：http://mc.szxytkj.cn

C. 函数与作用域
来源：http://sd.bjjhwx.cn

================================================================================
来源：http://du.chemitech.net.cn

[C01] 定义函数
来源：http://ej.muxihuayi.cn

Py:   def add(a, b): return a + b
来源：http://ap.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wh.wgjwhj.cn

JS:   function add(a, b) { return a + b; }
来源：http://nq.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tx.muxihuayi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zw.muxihuayi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vv.chemitech.net.cn

Ruby: def add(a, b); a + b; end
来源：http://sh.nicolike.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jf.521024.cn

[C02] 默认参数
来源：http://zm.hahajie.cn

Py:   def greet(name="World"): return name
来源：http://pf.wgjwhj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ek.huixinmuqiang.cn

JS:   function greet(name = "World") { return name; }
来源：http://bg.lnxyls.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xx.huixinmuqiang.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rr.jianghongdianzi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yu.hnjuh.cn

Ruby: def greet(name = "World") = name
来源：http://jd.nszjky.cn

C#:   string Greet(string name = "World") => name;
来源：http://ar.nicolike.cn

[C03] 可变参数
来源：http://wg.panjiajie.cn

Py:   def total(*args): return sum(args)
来源：http://sp.gzmigu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ms.newstarts.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zs.wgjwhj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dl.shxzukj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cx.nicolike.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fe.lnxyls.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yg.yuexingan06.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qc.haigaiapp.cn

[C04] 命名参数 / 关键字参数
来源：http://rz.yuntaijiaju.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gu.chemitech.net.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bj.shxzukj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yj.nszjky.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rc.shxzskj.cn

Java: // 无：用 Builder 模式或 record
来源：http://xr.jctech888.com.cn

Go:   // 无：用配置结构体参数
来源：http://cc.9csxet.cn

Ruby: f(a: 1, b: 2)
来源：http://db.shtwfgs.cn

C#:   f(a: 1, b: 2)
来源：http://hd.colortex.cn

[C05] 返回多个值
来源：http://da.9csxet.cn

Py:   return a, b
来源：http://fi.lnxyls.cn

PHP:  return [$a, $b];
来源：http://py.newstarts.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zb.lnxyls.cn

TS:   return { a, b };
来源：http://jp.shxzskj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mc.panjiajie.cn

Go:   return a, b
来源：http://nu.newstarts.cn

Ruby: return a, b
来源：http://ur.hahajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://zt.bookmarksfly.cn

[C06] 匿名函数 / lambda
来源：http://gq.hnjuh.cn

Py:   square = lambda x: x * x
来源：http://up.hnjuh.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pu.muxihuayi.cn

JS:   const square = x => x * x;
来源：http://rv.szsharing.cn

TS:   const square = (x: number): number => x * x;
来源：http://hr.jctech888.com.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ff.huixiangedu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wk.hnjuh.cn

Ruby: square = ->(x) { x * x }
来源：http://yc.szsharing.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dn.521024.cn

[C07] 把函数作为参数传入
来源：http://vj.chemitech.net.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://du.shxzskj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xb.wgjwhj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tu.haigaiapp.cn

TS:   arr.map(String)
来源：http://oj.huixiangedu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mx.huixinmuqiang.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fg.bookmarksfly.cn

Ruby: arr.map(&:upcase)
来源：http://pj.hahajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ib.jianghongdianzi.cn

[C08] 闭包
来源：http://mr.9csxet.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ph.gzmigu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ei.jianghongdianzi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ts.hnjuh.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jq.shtwfgs.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tn.521024.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rl.bookmarksfly.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://aq.hnjuh.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bj.colortex.cn

[C09] 递归
来源：http://ep.hahajie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vi.hnjuh.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zi.nszjky.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yh.shtwfgs.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yy.muxihuayi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cy.chemitech.net.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fe.szxytkj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hg.jianghongdianzi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wg.yuntaijiaju.cn

[C10] 变量作用域
来源：http://gd.szsharing.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://km.lnxyls.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zp.jianghongdianzi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ig.wgjwhj.cn

TS:   同 JS
来源：http://nf.huixinmuqiang.cn

Java: 方法内为块级作用域
来源：http://kl.yuexingan06.cn

Go:   花括号块级作用域
来源：http://vi.chemitech.net.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ci.chemitech.net.cn

C#:   块级作用域
来源：http://dx.panjiajie.cn

[C11] 模块导入与导出
来源：http://qp.huanxung.cn

Py:   from module import func
来源：http://vv.wgjwhj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zz.huixinmuqiang.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rb.chemitech.net.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ct.shxzukj.cn

Java: import java.util.List;
来源：http://xu.jianghongdianzi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bs.shxzskj.cn

Ruby: require "json"; require_relative "./util"
来源：http://sf.521024.cn

C#:   using System.Text;
来源：http://kg.chemitech.net.cn

[C12] 立即执行函数 IIFE
来源：http://by.yuexingan06.cn

Py:   (lambda: print("run"))()
来源：http://li.bjjhwx.cn

PHP:  (function () { echo "run"; })();
来源：http://kq.nszjky.cn

JS:   (() => { console.log("run"); })();
来源：http://wf.muxihuayi.cn

TS:   (() => { console.log("run"); })();
来源：http://li.chemitech.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ee.wgjwhj.cn

Go:   func() { fmt.Println("run") }()
来源：http://nz.newstarts.cn

Ruby: -> { puts "run" }.call
来源：http://vp.9csxet.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://nh.muxihuayi.cn

[C13] 类型声明 / 类型注解
来源：http://zt.gzmigu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tp.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://os.jctech888.com.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jt.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ep.huixinmuqiang.cn

Java: int add(int a, int b) { return a + b; }
来源：http://nw.yuntaijiaju.cn

Go:   func add(a, b int) int
来源：http://bq.panjiajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://oh.huixinmuqiang.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gj.yuntaijiaju.cn

[C14] 泛型函数
来源：http://uw.yuexingan06.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rc.colortex.cn

PHP:  // 无泛型
来源：http://jh.bookmarksfly.cn

JS:   // 无泛型
来源：http://bo.haigaiapp.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pz.shxzukj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cv.jctech888.com.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ay.jctech888.com.cn

Ruby: # 无泛型
来源：http://tg.shtwfgs.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zt.lnxyls.cn

[C15] 解构 / 展开参数
来源：http://zo.panjiajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rs.hnjuh.cn

PHP:  [$a, $b] = $pair;
来源：http://yi.hahajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tv.hnjuh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jw.nszjky.cn

Java: // 无解构
来源：http://ol.nszjky.cn

Go:   // 无解构
来源：http://fv.nicolike.cn


<!-- 参考信息 -->