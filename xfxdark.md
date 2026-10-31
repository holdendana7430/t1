代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://du.yuexingan06.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xr.bookmarksfly.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wr.szsharing.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wq.521024.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dt.nszjky.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ne.yuntaijiaju.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://nu.szsharing.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://eq.huanxung.cn

[A26] 类型转换总览
来源：http://uh.lnxyls.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wr.huixinmuqiang.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qg.shtwfgs.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pp.shxzukj.cn

TS:   Number() String() Boolean() x as number
来源：http://tj.bjjhwx.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://oa.muxihuayi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://eh.huanxung.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://cc.bjjhwx.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bi.yuexingan06.cn

================================================================================
来源：http://qo.yuntaijiaju.cn

B. 流程控制
来源：http://mn.bjjhwx.cn

================================================================================
来源：http://zn.panjiajie.cn

[B01] 条件判断 if / else
来源：http://gg.newstarts.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://lg.newstarts.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xs.haigaiapp.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ke.shxzskj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://un.huixiangedu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ja.shtwfgs.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zq.gzmigu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hg.huixinmuqiang.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vt.lnxyls.cn

[B02] 多分支 else if / elif
来源：http://zq.haigaiapp.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ck.huixiangedu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://df.jctech888.com.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gc.colortex.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ta.muxihuayi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gl.colortex.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hb.bjjhwx.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pp.huixinmuqiang.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://um.muxihuayi.cn

[B03] switch / match / case
来源：http://ke.panjiajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://al.gzmigu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fu.muxihuayi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vx.bjjhwx.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jz.panjiajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cf.jianghongdianzi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xt.huanxung.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fs.huixinmuqiang.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ba.bookmarksfly.cn

[B04] for 计数循环
来源：http://pa.szxytkj.cn

Py:   for i in range(10): print(i)
来源：http://ve.szxytkj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ny.hnjuh.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ib.wgjwhj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ln.jianghongdianzi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qd.nszjky.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://le.asd995.cn

Ruby: 10.times { |i| puts i }
来源：http://fj.521024.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gc.chemitech.net.cn

[B05] 遍历数组 / 列表
来源：http://rq.9csxet.cn

Py:   for item in arr: print(item)
来源：http://mf.yuntaijiaju.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fc.nszjky.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hf.521024.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://le.lnxyls.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://mm.yuntaijiaju.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lp.hahajie.cn

Ruby: arr.each { |item| puts item }
来源：http://tm.panjiajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uj.jctech888.com.cn

[B06] 遍历字典 / 对象
来源：http://ae.9csxet.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://is.bookmarksfly.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fr.bookmarksfly.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xv.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nk.hahajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rv.shxzukj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ue.yuexingan06.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://go.szsharing.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tq.jctech888.com.cn

[B07] while 循环
来源：http://rk.jctech888.com.cn

Py:   while i < 10: i += 1
来源：http://on.yuexingan06.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fs.lnxyls.cn

JS:   while (i < 10) { i++; }
来源：http://ez.wgjwhj.cn

TS:   while (i < 10) { i++; }
来源：http://zc.yuexingan06.cn

Java: while (i < 10) { i++; }
来源：http://ni.nszjky.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fq.gzmigu.cn

Ruby: while i < 10; i += 1; end
来源：http://el.hahajie.cn

C#:   while (i < 10) { i++; }
来源：http://ra.yuntaijiaju.cn

[B08] do-while（至少执行一次）
来源：http://cp.panjiajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://cd.huixinmuqiang.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://nw.wgjwhj.cn

JS:   do { i++; } while (i < 10);
来源：http://zw.yuntaijiaju.cn

TS:   do { i++; } while (i < 10);
来源：http://nb.huixiangedu.cn

Java: do { i++; } while (i < 10);
来源：http://ff.jctech888.com.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://lp.haigaiapp.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wr.huixinmuqiang.cn

C#:   do { i++; } while (i < 10);
来源：http://gi.panjiajie.cn

[B09] break 与 continue
来源：http://yp.newstarts.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gz.shxzskj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tr.gzmigu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qp.shxzskj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ha.gzmigu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tp.shxzukj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ro.colortex.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rw.shxzukj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bx.hnjuh.cn

[B10] 遍历同时拿索引
来源：http://us.wgjwhj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jk.bookmarksfly.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ry.szsharing.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qf.shtwfgs.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wg.shxzskj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pe.yuntaijiaju.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hh.huixinmuqiang.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kx.huanxung.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sy.521024.cn

[B11] 生成数字序列 / 区间
来源：http://zs.chemitech.net.cn

Py:   list(range(0, 10, 2))
来源：http://gd.hnjuh.cn

PHP:  range(0, 10, 2);
来源：http://pt.haigaiapp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bp.jctech888.com.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mu.shxzskj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sm.shtwfgs.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://oj.huixinmuqiang.cn

Ruby: (0...10).step(2).to_a
来源：http://jb.nszjky.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gj.szsharing.cn

[B12] 跳出多层循环
来源：http://yd.nszjky.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tf.jianghongdianzi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://jy.szxytkj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jl.yuexingan06.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jv.bookmarksfly.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vc.huixiangedu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fj.jianghongdianzi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://og.chemitech.net.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ra.szsharing.cn

[B13] 判断是否为数字
来源：http://bc.gzmigu.cn

Py:   isinstance(x, (int, float))
来源：http://xb.jianghongdianzi.cn

PHP:  is_numeric($x)
来源：http://zm.panjiajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zb.9csxet.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mh.chemitech.net.cn

Java: x instanceof Number
来源：http://xb.shtwfgs.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vo.yuntaijiaju.cn

Ruby: x.is_a?(Numeric)
来源：http://du.gzmigu.cn

C#:   x is int or double or decimal
来源：http://fs.9csxet.cn

[B14] 判断值是否在集合内
来源：http://vf.huixiangedu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rx.shtwfgs.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zj.szxytkj.cn

JS:   [1, 2, 3].includes(x)
来源：http://wx.nicolike.cn

TS:   [1, 2, 3].includes(x)
来源：http://uq.jctech888.com.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://uu.haigaiapp.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vh.chemitech.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fn.shxzskj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ld.yuexingan06.cn

[B15] 布尔运算与取反
来源：http://hm.szsharing.cn

Py:   a and b or not c
来源：http://rm.wgjwhj.cn

PHP:  $a && $b || !$c
来源：http://vc.panjiajie.cn

JS:   a && b || !c
来源：http://wi.shxzukj.cn

TS:   a && b || !c
来源：http://fy.colortex.cn

Java: a && b || !c
来源：http://fn.shxzukj.cn

Go:   a && b || !c
来源：http://bl.nszjky.cn

Ruby: a && b || !c
来源：http://ac.yuntaijiaju.cn

C#:   a && b || !c
来源：http://df.hahajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://nl.jctech888.com.cn

Py:   if not data: return
来源：http://cn.shxzskj.cn

PHP:  if (!$data) { return; }
来源：http://ia.shtwfgs.cn

JS:   if (!data) return;
来源：http://pi.newstarts.cn

TS:   if (!data) return;
来源：http://cf.haigaiapp.cn

Java: if (data == null) return;
来源：http://ud.huixinmuqiang.cn

Go:   if data == nil { return }
来源：http://wc.shtwfgs.cn

Ruby: return if data.nil?
来源：http://xr.jianghongdianzi.cn

C#:   if (data == null) return;
来源：http://tn.hnjuh.cn

================================================================================
来源：http://gq.lnxyls.cn

C. 函数与作用域
来源：http://mo.nszjky.cn

================================================================================
来源：http://qg.panjiajie.cn

[C01] 定义函数
来源：http://vu.bookmarksfly.cn

Py:   def add(a, b): return a + b
来源：http://ha.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://of.jctech888.com.cn

JS:   function add(a, b) { return a + b; }
来源：http://jx.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qj.lnxyls.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://oq.hahajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://gm.lnxyls.cn

Ruby: def add(a, b); a + b; end
来源：http://qf.shtwfgs.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qx.szxytkj.cn

[C02] 默认参数
来源：http://ln.haigaiapp.cn

Py:   def greet(name="World"): return name
来源：http://rj.gzmigu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hc.bjjhwx.cn

JS:   function greet(name = "World") { return name; }
来源：http://gr.muxihuayi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gt.nszjky.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hj.gzmigu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://re.panjiajie.cn

Ruby: def greet(name = "World") = name
来源：http://av.hahajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://nz.haigaiapp.cn

[C03] 可变参数
来源：http://qd.lnxyls.cn

Py:   def total(*args): return sum(args)
来源：http://rx.asd995.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lg.hnjuh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ym.muxihuayi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zx.jianghongdianzi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ob.bookmarksfly.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ce.szsharing.cn

Ruby: def total(*nums); nums.sum; end
来源：http://kt.muxihuayi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ml.jianghongdianzi.cn

[C04] 命名参数 / 关键字参数
来源：http://ut.jianghongdianzi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jx.haigaiapp.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zd.colortex.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wv.colortex.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mz.asd995.cn

Java: // 无：用 Builder 模式或 record
来源：http://oj.9csxet.cn

Go:   // 无：用配置结构体参数
来源：http://ya.muxihuayi.cn

Ruby: f(a: 1, b: 2)
来源：http://dd.jianghongdianzi.cn

C#:   f(a: 1, b: 2)
来源：http://cp.nszjky.cn

[C05] 返回多个值
来源：http://gx.shtwfgs.cn

Py:   return a, b
来源：http://ln.yuntaijiaju.cn

PHP:  return [$a, $b];
来源：http://lb.nszjky.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://bz.chemitech.net.cn

TS:   return { a, b };
来源：http://sp.9csxet.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kt.huanxung.cn

Go:   return a, b
来源：http://en.9csxet.cn

Ruby: return a, b
来源：http://or.lnxyls.cn

C#:   return (a, b);              // ValueTuple
来源：http://xm.hnjuh.cn

[C06] 匿名函数 / lambda
来源：http://ol.huixiangedu.cn

Py:   square = lambda x: x * x
来源：http://me.shxzskj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://nv.huixiangedu.cn

JS:   const square = x => x * x;
来源：http://lt.huixiangedu.cn

TS:   const square = (x: number): number => x * x;
来源：http://lc.521024.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rc.huanxung.cn

Go:   sq := func(x int) int { return x * x }
来源：http://mr.lnxyls.cn

Ruby: square = ->(x) { x * x }
来源：http://xw.chemitech.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ac.nicolike.cn

[C07] 把函数作为参数传入
来源：http://dl.newstarts.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xg.bookmarksfly.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hy.chemitech.net.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://se.gzmigu.cn

TS:   arr.map(String)
来源：http://cl.asd995.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fm.yuntaijiaju.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sx.yuntaijiaju.cn

Ruby: arr.map(&:upcase)
来源：http://jl.szsharing.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://eb.9csxet.cn

[C08] 闭包
来源：http://hb.huixiangedu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qr.nicolike.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lv.hnjuh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ei.lnxyls.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jp.hahajie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hu.szsharing.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kw.nszjky.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qp.shtwfgs.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yl.huanxung.cn

[C09] 递归
来源：http://fa.newstarts.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ju.gzmigu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vo.newstarts.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ec.huixiangedu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zx.bjjhwx.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ly.gzmigu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://eh.lnxyls.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ym.bjjhwx.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zd.asd995.cn

[C10] 变量作用域
来源：http://nf.szsharing.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pg.jctech888.com.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://be.chemitech.net.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hb.nicolike.cn

TS:   同 JS
来源：http://xh.muxihuayi.cn

Java: 方法内为块级作用域
来源：http://fq.bjjhwx.cn

Go:   花括号块级作用域
来源：http://ci.chemitech.net.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hg.lnxyls.cn

C#:   块级作用域
来源：http://qd.haigaiapp.cn

[C11] 模块导入与导出
来源：http://gh.nicolike.cn

Py:   from module import func
来源：http://se.bookmarksfly.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mz.lnxyls.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://mp.nszjky.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tf.lnxyls.cn

Java: import java.util.List;
来源：http://fo.yuntaijiaju.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fh.wgjwhj.cn

Ruby: require "json"; require_relative "./util"
来源：http://ol.shxzskj.cn

C#:   using System.Text;
来源：http://gq.jianghongdianzi.cn

[C12] 立即执行函数 IIFE
来源：http://ze.gzmigu.cn

Py:   (lambda: print("run"))()
来源：http://uy.yuntaijiaju.cn

PHP:  (function () { echo "run"; })();
来源：http://ty.jctech888.com.cn

JS:   (() => { console.log("run"); })();
来源：http://wz.shxzukj.cn

TS:   (() => { console.log("run"); })();
来源：http://fz.haigaiapp.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hh.haigaiapp.cn

Go:   func() { fmt.Println("run") }()
来源：http://bd.yuntaijiaju.cn

Ruby: -> { puts "run" }.call
来源：http://bo.chemitech.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fh.bjjhwx.cn

[C13] 类型声明 / 类型注解
来源：http://yc.hahajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jm.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qd.lnxyls.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tm.szxytkj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cc.hnjuh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://gr.yuntaijiaju.cn

Go:   func add(a, b int) int
来源：http://ol.gzmigu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rl.nszjky.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wq.nicolike.cn

[C14] 泛型函数
来源：http://og.szxytkj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qp.szsharing.cn

PHP:  // 无泛型
来源：http://ek.lnxyls.cn

JS:   // 无泛型
来源：http://ci.shtwfgs.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kt.nszjky.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zr.hahajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://le.hahajie.cn

Ruby: # 无泛型
来源：http://db.nszjky.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wj.panjiajie.cn

[C15] 解构 / 展开参数
来源：http://nk.panjiajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gr.newstarts.cn

PHP:  [$a, $b] = $pair;
来源：http://ko.shxzukj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://oy.bookmarksfly.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bd.521024.cn

Java: // 无解构
来源：http://as.huixiangedu.cn

Go:   // 无解构
来源：http://ah.9csxet.cn


<!-- 参考信息 -->