代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qk.chemitech.net.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://og.lnxyls.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://wd.huixiangedu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fo.jctech888.com.cn

[A26] 类型转换总览
来源：http://nt.hahajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rv.wgjwhj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bc.hahajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ly.chemitech.net.cn

TS:   Number() String() Boolean() x as number
来源：http://zf.colortex.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pd.9csxet.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nc.gzmigu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ef.yuntaijiaju.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zk.shxzskj.cn

================================================================================
来源：http://bs.lnxyls.cn

B. 流程控制
来源：http://or.jctech888.com.cn

================================================================================
来源：http://fa.jianghongdianzi.cn

[B01] 条件判断 if / else
来源：http://gs.szsharing.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://qz.yuexingan06.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lj.9csxet.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lp.yuexingan06.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lh.yuexingan06.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ax.asd995.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xz.huixiangedu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xr.jianghongdianzi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cb.hnjuh.cn

[B02] 多分支 else if / elif
来源：http://hx.huanxung.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ox.lnxyls.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kc.bookmarksfly.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gg.jianghongdianzi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nd.wgjwhj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fd.szxytkj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ur.yuntaijiaju.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pp.huixinmuqiang.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sy.chemitech.net.cn

[B03] switch / match / case
来源：http://li.asd995.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sb.muxihuayi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ia.colortex.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ra.nicolike.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wo.huixinmuqiang.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gt.bjjhwx.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zw.shxzskj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ul.wgjwhj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jj.szxytkj.cn

[B04] for 计数循环
来源：http://hu.hnjuh.cn

Py:   for i in range(10): print(i)
来源：http://pj.9csxet.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://uo.hnjuh.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://aj.colortex.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qp.huixiangedu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bb.muxihuayi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://uo.muxihuayi.cn

Ruby: 10.times { |i| puts i }
来源：http://yl.yuexingan06.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pe.9csxet.cn

[B05] 遍历数组 / 列表
来源：http://jd.bookmarksfly.cn

Py:   for item in arr: print(item)
来源：http://os.gzmigu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vc.huanxung.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wz.huixinmuqiang.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://jo.jianghongdianzi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://aa.panjiajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vd.nicolike.cn

Ruby: arr.each { |item| puts item }
来源：http://ix.bookmarksfly.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tl.asd995.cn

[B06] 遍历字典 / 对象
来源：http://bz.szxytkj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qf.521024.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ca.gzmigu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yi.jctech888.com.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ml.szxytkj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cn.yuntaijiaju.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gr.huixinmuqiang.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kk.shxzukj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zt.muxihuayi.cn

[B07] while 循环
来源：http://yj.bjjhwx.cn

Py:   while i < 10: i += 1
来源：http://fx.lnxyls.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lc.haigaiapp.cn

JS:   while (i < 10) { i++; }
来源：http://er.yuexingan06.cn

TS:   while (i < 10) { i++; }
来源：http://ed.jctech888.com.cn

Java: while (i < 10) { i++; }
来源：http://jr.gzmigu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qs.bookmarksfly.cn

Ruby: while i < 10; i += 1; end
来源：http://sb.asd995.cn

C#:   while (i < 10) { i++; }
来源：http://rt.shxzskj.cn

[B08] do-while（至少执行一次）
来源：http://yn.9csxet.cn

Py:   # 无 do-while：用 while True + break
来源：http://bh.newstarts.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cq.muxihuayi.cn

JS:   do { i++; } while (i < 10);
来源：http://tr.huixinmuqiang.cn

TS:   do { i++; } while (i < 10);
来源：http://qy.lnxyls.cn

Java: do { i++; } while (i < 10);
来源：http://ia.shtwfgs.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://qg.9csxet.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rd.jianghongdianzi.cn

C#:   do { i++; } while (i < 10);
来源：http://fl.yuntaijiaju.cn

[B09] break 与 continue
来源：http://ck.shxzukj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zn.wgjwhj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jq.yuexingan06.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wb.panjiajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nv.huanxung.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zo.gzmigu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qi.muxihuayi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pg.panjiajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ma.szxytkj.cn

[B10] 遍历同时拿索引
来源：http://is.bjjhwx.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vq.9csxet.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qh.shtwfgs.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dh.szxytkj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qn.haigaiapp.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jf.bookmarksfly.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://la.521024.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://og.chemitech.net.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qa.shxzskj.cn

[B11] 生成数字序列 / 区间
来源：http://ly.shxzukj.cn

Py:   list(range(0, 10, 2))
来源：http://dt.9csxet.cn

PHP:  range(0, 10, 2);
来源：http://ui.gzmigu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sj.yuexingan06.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zz.lnxyls.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://aw.huixinmuqiang.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rw.521024.cn

Ruby: (0...10).step(2).to_a
来源：http://dw.jianghongdianzi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cb.asd995.cn

[B12] 跳出多层循环
来源：http://jd.nszjky.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://di.bookmarksfly.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://xo.bjjhwx.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qu.gzmigu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://eh.huixinmuqiang.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hd.asd995.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gd.asd995.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://op.shxzskj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://no.hahajie.cn

[B13] 判断是否为数字
来源：http://hn.haigaiapp.cn

Py:   isinstance(x, (int, float))
来源：http://gj.huanxung.cn

PHP:  is_numeric($x)
来源：http://ll.gzmigu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rb.haigaiapp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://is.bookmarksfly.cn

Java: x instanceof Number
来源：http://hw.lnxyls.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bm.lnxyls.cn

Ruby: x.is_a?(Numeric)
来源：http://vr.nszjky.cn

C#:   x is int or double or decimal
来源：http://bn.muxihuayi.cn

[B14] 判断值是否在集合内
来源：http://pp.szsharing.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uw.panjiajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jy.shtwfgs.cn

JS:   [1, 2, 3].includes(x)
来源：http://nm.huixinmuqiang.cn

TS:   [1, 2, 3].includes(x)
来源：http://on.nicolike.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hj.haigaiapp.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://na.muxihuayi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ln.shxzskj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://la.szxytkj.cn

[B15] 布尔运算与取反
来源：http://yy.huixinmuqiang.cn

Py:   a and b or not c
来源：http://cq.hahajie.cn

PHP:  $a && $b || !$c
来源：http://bu.nicolike.cn

JS:   a && b || !c
来源：http://rp.hnjuh.cn

TS:   a && b || !c
来源：http://za.shxzskj.cn

Java: a && b || !c
来源：http://eu.huixinmuqiang.cn

Go:   a && b || !c
来源：http://xy.yuexingan06.cn

Ruby: a && b || !c
来源：http://ek.jctech888.com.cn

C#:   a && b || !c
来源：http://iq.panjiajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://yw.gzmigu.cn

Py:   if not data: return
来源：http://dk.hnjuh.cn

PHP:  if (!$data) { return; }
来源：http://wa.haigaiapp.cn

JS:   if (!data) return;
来源：http://hc.huixinmuqiang.cn

TS:   if (!data) return;
来源：http://ba.shxzskj.cn

Java: if (data == null) return;
来源：http://bq.jctech888.com.cn

Go:   if data == nil { return }
来源：http://nu.shxzukj.cn

Ruby: return if data.nil?
来源：http://hq.shxzskj.cn

C#:   if (data == null) return;
来源：http://fr.wgjwhj.cn

================================================================================
来源：http://os.gzmigu.cn

C. 函数与作用域
来源：http://aa.yuexingan06.cn

================================================================================
来源：http://of.gzmigu.cn

[C01] 定义函数
来源：http://df.shtwfgs.cn

Py:   def add(a, b): return a + b
来源：http://xs.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://at.hnjuh.cn

JS:   function add(a, b) { return a + b; }
来源：http://nn.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ek.chemitech.net.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bk.shtwfgs.cn

Go:   func add(a, b int) int { return a + b }
来源：http://yi.nszjky.cn

Ruby: def add(a, b); a + b; end
来源：http://sz.wgjwhj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lb.huanxung.cn

[C02] 默认参数
来源：http://tg.bjjhwx.cn

Py:   def greet(name="World"): return name
来源：http://fg.colortex.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wb.huanxung.cn

JS:   function greet(name = "World") { return name; }
来源：http://eg.shxzukj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ni.shtwfgs.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ie.asd995.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ib.hnjuh.cn

Ruby: def greet(name = "World") = name
来源：http://lu.colortex.cn

C#:   string Greet(string name = "World") => name;
来源：http://fv.huixinmuqiang.cn

[C03] 可变参数
来源：http://br.yuexingan06.cn

Py:   def total(*args): return sum(args)
来源：http://ao.muxihuayi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uq.hnjuh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qt.huixiangedu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lv.shxzukj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sl.asd995.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pi.newstarts.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ku.panjiajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ec.521024.cn

[C04] 命名参数 / 关键字参数
来源：http://fc.nicolike.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://up.hahajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xe.yuexingan06.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sh.muxihuayi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://na.hahajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://hb.jianghongdianzi.cn

Go:   // 无：用配置结构体参数
来源：http://gj.asd995.cn

Ruby: f(a: 1, b: 2)
来源：http://co.lnxyls.cn

C#:   f(a: 1, b: 2)
来源：http://ej.asd995.cn

[C05] 返回多个值
来源：http://sz.newstarts.cn

Py:   return a, b
来源：http://io.shtwfgs.cn

PHP:  return [$a, $b];
来源：http://sf.lnxyls.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://bo.nszjky.cn

TS:   return { a, b };
来源：http://mc.hahajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gi.nicolike.cn

Go:   return a, b
来源：http://gn.lnxyls.cn

Ruby: return a, b
来源：http://rp.nszjky.cn

C#:   return (a, b);              // ValueTuple
来源：http://np.yuexingan06.cn

[C06] 匿名函数 / lambda
来源：http://rn.shtwfgs.cn

Py:   square = lambda x: x * x
来源：http://ad.shtwfgs.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://nf.szxytkj.cn

JS:   const square = x => x * x;
来源：http://yq.hnjuh.cn

TS:   const square = (x: number): number => x * x;
来源：http://ka.nicolike.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mi.bjjhwx.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xv.szxytkj.cn

Ruby: square = ->(x) { x * x }
来源：http://xy.bookmarksfly.cn

C#:   Func<int, int> square = x => x * x;
来源：http://rz.bookmarksfly.cn

[C07] 把函数作为参数传入
来源：http://mc.wgjwhj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fc.panjiajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jc.yuntaijiaju.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bx.muxihuayi.cn

TS:   arr.map(String)
来源：http://uy.521024.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rf.huixiangedu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nv.newstarts.cn

Ruby: arr.map(&:upcase)
来源：http://uw.521024.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://oa.yuntaijiaju.cn

[C08] 闭包
来源：http://yv.yuntaijiaju.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kt.jianghongdianzi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ks.szxytkj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zn.huixinmuqiang.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://az.haigaiapp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://az.shxzukj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kw.bookmarksfly.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ao.huixinmuqiang.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wo.haigaiapp.cn

[C09] 递归
来源：http://hy.huixiangedu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kf.huixinmuqiang.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hp.jctech888.com.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wu.newstarts.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hn.shxzukj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yn.nszjky.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xi.huixinmuqiang.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ba.shtwfgs.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ol.panjiajie.cn

[C10] 变量作用域
来源：http://yw.hahajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://it.szxytkj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wg.huixinmuqiang.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fg.gzmigu.cn

TS:   同 JS
来源：http://nh.huixiangedu.cn

Java: 方法内为块级作用域
来源：http://xx.colortex.cn

Go:   花括号块级作用域
来源：http://ad.shtwfgs.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sx.chemitech.net.cn

C#:   块级作用域
来源：http://zx.bjjhwx.cn

[C11] 模块导入与导出
来源：http://wi.hahajie.cn

Py:   from module import func
来源：http://yl.nicolike.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ts.9csxet.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://io.yuexingan06.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ke.huixiangedu.cn

Java: import java.util.List;
来源：http://js.szxytkj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fk.haigaiapp.cn

Ruby: require "json"; require_relative "./util"
来源：http://na.yuntaijiaju.cn

C#:   using System.Text;
来源：http://hj.nszjky.cn

[C12] 立即执行函数 IIFE
来源：http://ou.szsharing.cn

Py:   (lambda: print("run"))()
来源：http://pe.9csxet.cn

PHP:  (function () { echo "run"; })();
来源：http://si.lnxyls.cn

JS:   (() => { console.log("run"); })();
来源：http://zc.chemitech.net.cn

TS:   (() => { console.log("run"); })();
来源：http://mc.newstarts.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://aq.shxzukj.cn

Go:   func() { fmt.Println("run") }()
来源：http://ro.yuexingan06.cn

Ruby: -> { puts "run" }.call
来源：http://wh.nszjky.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://kw.szsharing.cn

[C13] 类型声明 / 类型注解
来源：http://us.huanxung.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dw.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zi.bookmarksfly.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jr.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://us.huanxung.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qd.szsharing.cn

Go:   func add(a, b int) int
来源：http://wb.szxytkj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://if.asd995.cn

C#:   int Add(int a, int b) => a + b;
来源：http://su.gzmigu.cn

[C14] 泛型函数
来源：http://hf.wgjwhj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://st.asd995.cn

PHP:  // 无泛型
来源：http://vc.newstarts.cn

JS:   // 无泛型
来源：http://zf.9csxet.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://at.newstarts.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yt.nicolike.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://at.asd995.cn

Ruby: # 无泛型
来源：http://do.muxihuayi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tp.asd995.cn

[C15] 解构 / 展开参数
来源：http://ht.huixinmuqiang.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qk.lnxyls.cn

PHP:  [$a, $b] = $pair;
来源：http://zi.huixinmuqiang.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vk.hahajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hv.szxytkj.cn

Java: // 无解构
来源：http://he.bjjhwx.cn

Go:   // 无解构
来源：http://sl.muxihuayi.cn

Ruby: a, b = pair
来源：http://up.yuntaijiaju.cn

C#:   var (a, b) = pair;
来源：http://jy.huixiangedu.cn

[C16] 函数 / 方法重载
来源：http://tc.shxzskj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tr.shxzskj.cn


<!-- 参考信息 -->