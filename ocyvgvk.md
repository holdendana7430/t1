代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://yb.shxzukj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gk.szxytkj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pv.huanxung.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wo.wgjwhj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jp.lnxyls.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://te.jianghongdianzi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://en.asd995.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://he.panjiajie.cn

[A26] 类型转换总览
来源：http://ya.asd995.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hm.521024.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ln.szsharing.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://il.muxihuayi.cn

TS:   Number() String() Boolean() x as number
来源：http://ch.shxzukj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wj.gzmigu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bt.jianghongdianzi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://di.jctech888.com.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xn.szsharing.cn

================================================================================
来源：http://cd.nicolike.cn

B. 流程控制
来源：http://ur.jctech888.com.cn

================================================================================
来源：http://ws.huixiangedu.cn

[B01] 条件判断 if / else
来源：http://oz.nszjky.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bu.panjiajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tp.bookmarksfly.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qy.lnxyls.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://go.bjjhwx.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ej.nicolike.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dn.jctech888.com.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://my.521024.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nr.haigaiapp.cn

[B02] 多分支 else if / elif
来源：http://mc.huixinmuqiang.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xu.newstarts.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nq.521024.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bx.szsharing.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dl.bookmarksfly.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fh.bjjhwx.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://di.chemitech.net.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ud.nszjky.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sh.panjiajie.cn

[B03] switch / match / case
来源：http://tb.shxzskj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ha.jctech888.com.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://up.hahajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qn.gzmigu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fx.hahajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://db.huixinmuqiang.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mv.muxihuayi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://or.9csxet.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bs.panjiajie.cn

[B04] for 计数循环
来源：http://vc.nicolike.cn

Py:   for i in range(10): print(i)
来源：http://no.szsharing.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xf.gzmigu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ls.szxytkj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gm.asd995.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hv.huixiangedu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ex.yuntaijiaju.cn

Ruby: 10.times { |i| puts i }
来源：http://ek.521024.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ma.nicolike.cn

[B05] 遍历数组 / 列表
来源：http://fa.newstarts.cn

Py:   for item in arr: print(item)
来源：http://nv.gzmigu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ly.shxzskj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://kb.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gv.huixinmuqiang.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://dt.hnjuh.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.huixiangedu.cn

Ruby: arr.each { |item| puts item }
来源：http://vz.shxzukj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://za.colortex.cn

[B06] 遍历字典 / 对象
来源：http://wh.wgjwhj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://yy.yuntaijiaju.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://aa.shxzskj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mi.shxzskj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ii.panjiajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mr.huixinmuqiang.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://es.hnjuh.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wk.yuexingan06.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://en.hnjuh.cn

[B07] while 循环
来源：http://ws.yuexingan06.cn

Py:   while i < 10: i += 1
来源：http://lh.szsharing.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mn.bookmarksfly.cn

JS:   while (i < 10) { i++; }
来源：http://da.shxzukj.cn

TS:   while (i < 10) { i++; }
来源：http://nn.yuntaijiaju.cn

Java: while (i < 10) { i++; }
来源：http://vx.bjjhwx.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ko.szxytkj.cn

Ruby: while i < 10; i += 1; end
来源：http://ad.shxzukj.cn

C#:   while (i < 10) { i++; }
来源：http://ld.shxzskj.cn

[B08] do-while（至少执行一次）
来源：http://bh.yuexingan06.cn

Py:   # 无 do-while：用 while True + break
来源：http://fz.bjjhwx.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xn.wgjwhj.cn

JS:   do { i++; } while (i < 10);
来源：http://it.shtwfgs.cn

TS:   do { i++; } while (i < 10);
来源：http://tr.yuntaijiaju.cn

Java: do { i++; } while (i < 10);
来源：http://ow.521024.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ii.asd995.cn

Ruby: begin; i += 1; end while i < 10
来源：http://eq.jianghongdianzi.cn

C#:   do { i++; } while (i < 10);
来源：http://rr.shtwfgs.cn

[B09] break 与 continue
来源：http://hk.9csxet.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zs.bjjhwx.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vx.muxihuayi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yz.huanxung.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vr.shtwfgs.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gs.huixiangedu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fm.nicolike.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wb.haigaiapp.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sk.szsharing.cn

[B10] 遍历同时拿索引
来源：http://tl.9csxet.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ta.yuexingan06.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ok.yuntaijiaju.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qn.huixinmuqiang.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kk.bookmarksfly.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jc.colortex.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mz.colortex.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bs.bookmarksfly.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ae.gzmigu.cn

[B11] 生成数字序列 / 区间
来源：http://pl.gzmigu.cn

Py:   list(range(0, 10, 2))
来源：http://rm.colortex.cn

PHP:  range(0, 10, 2);
来源：http://im.haigaiapp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hc.muxihuayi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lo.haigaiapp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pt.huixinmuqiang.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jz.newstarts.cn

Ruby: (0...10).step(2).to_a
来源：http://uu.huixinmuqiang.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://du.yuntaijiaju.cn

[B12] 跳出多层循环
来源：http://em.shtwfgs.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ko.szxytkj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://va.huanxung.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xp.gzmigu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://aq.gzmigu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qs.huanxung.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://un.colortex.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lo.huanxung.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dr.yuntaijiaju.cn

[B13] 判断是否为数字
来源：http://iz.asd995.cn

Py:   isinstance(x, (int, float))
来源：http://tn.muxihuayi.cn

PHP:  is_numeric($x)
来源：http://wl.huixinmuqiang.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rn.colortex.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pj.huixiangedu.cn

Java: x instanceof Number
来源：http://yx.szsharing.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ji.szsharing.cn

Ruby: x.is_a?(Numeric)
来源：http://nq.huixinmuqiang.cn

C#:   x is int or double or decimal
来源：http://ym.huixiangedu.cn

[B14] 判断值是否在集合内
来源：http://gf.huanxung.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ai.asd995.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mk.asd995.cn

JS:   [1, 2, 3].includes(x)
来源：http://xl.szsharing.cn

TS:   [1, 2, 3].includes(x)
来源：http://fx.asd995.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://pj.9csxet.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dx.nszjky.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jd.lnxyls.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vi.yuexingan06.cn

[B15] 布尔运算与取反
来源：http://rd.yuntaijiaju.cn

Py:   a and b or not c
来源：http://mj.gzmigu.cn

PHP:  $a && $b || !$c
来源：http://ai.yuntaijiaju.cn

JS:   a && b || !c
来源：http://ah.szxytkj.cn

TS:   a && b || !c
来源：http://ac.bjjhwx.cn

Java: a && b || !c
来源：http://al.nszjky.cn

Go:   a && b || !c
来源：http://of.colortex.cn

Ruby: a && b || !c
来源：http://wz.newstarts.cn

C#:   a && b || !c
来源：http://ei.gzmigu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hs.chemitech.net.cn

Py:   if not data: return
来源：http://kz.shxzskj.cn

PHP:  if (!$data) { return; }
来源：http://ir.huixiangedu.cn

JS:   if (!data) return;
来源：http://pr.shtwfgs.cn

TS:   if (!data) return;
来源：http://nm.huixinmuqiang.cn

Java: if (data == null) return;
来源：http://nw.szxytkj.cn

Go:   if data == nil { return }
来源：http://eq.521024.cn

Ruby: return if data.nil?
来源：http://mo.colortex.cn

C#:   if (data == null) return;
来源：http://sn.panjiajie.cn

================================================================================
来源：http://to.jianghongdianzi.cn

C. 函数与作用域
来源：http://rb.shxzskj.cn

================================================================================
来源：http://wo.9csxet.cn

[C01] 定义函数
来源：http://ty.panjiajie.cn

Py:   def add(a, b): return a + b
来源：http://ix.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wl.jianghongdianzi.cn

JS:   function add(a, b) { return a + b; }
来源：http://yu.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sx.hahajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mi.gzmigu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://do.huixiangedu.cn

Ruby: def add(a, b); a + b; end
来源：http://fc.hnjuh.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zs.wgjwhj.cn

[C02] 默认参数
来源：http://mg.shxzukj.cn

Py:   def greet(name="World"): return name
来源：http://xz.bjjhwx.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://eo.yuexingan06.cn

JS:   function greet(name = "World") { return name; }
来源：http://dv.panjiajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ls.asd995.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vf.shtwfgs.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wc.9csxet.cn

Ruby: def greet(name = "World") = name
来源：http://ua.yuntaijiaju.cn

C#:   string Greet(string name = "World") => name;
来源：http://to.nszjky.cn

[C03] 可变参数
来源：http://ke.huixiangedu.cn

Py:   def total(*args): return sum(args)
来源：http://ad.lnxyls.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gb.chemitech.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vl.shxzukj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jy.szsharing.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kw.9csxet.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://os.yuntaijiaju.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hu.szxytkj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wr.521024.cn

[C04] 命名参数 / 关键字参数
来源：http://ie.yuexingan06.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://le.shtwfgs.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jz.panjiajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fa.lnxyls.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yb.jctech888.com.cn

Java: // 无：用 Builder 模式或 record
来源：http://ds.jctech888.com.cn

Go:   // 无：用配置结构体参数
来源：http://ir.jianghongdianzi.cn

Ruby: f(a: 1, b: 2)
来源：http://ic.hahajie.cn

C#:   f(a: 1, b: 2)
来源：http://da.panjiajie.cn

[C05] 返回多个值
来源：http://mb.huanxung.cn

Py:   return a, b
来源：http://dj.chemitech.net.cn

PHP:  return [$a, $b];
来源：http://do.muxihuayi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jo.huanxung.cn

TS:   return { a, b };
来源：http://fb.shtwfgs.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://np.bookmarksfly.cn

Go:   return a, b
来源：http://ui.haigaiapp.cn

Ruby: return a, b
来源：http://tb.szxytkj.cn

C#:   return (a, b);              // ValueTuple
来源：http://co.bookmarksfly.cn

[C06] 匿名函数 / lambda
来源：http://ln.shxzskj.cn

Py:   square = lambda x: x * x
来源：http://md.haigaiapp.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ix.9csxet.cn

JS:   const square = x => x * x;
来源：http://qi.gzmigu.cn

TS:   const square = (x: number): number => x * x;
来源：http://cw.jianghongdianzi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bs.lnxyls.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xh.colortex.cn

Ruby: square = ->(x) { x * x }
来源：http://ib.hahajie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://pi.szxytkj.cn

[C07] 把函数作为参数传入
来源：http://hz.szxytkj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wv.hahajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://cj.huixiangedu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fo.nszjky.cn

TS:   arr.map(String)
来源：http://or.haigaiapp.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ag.newstarts.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qx.hahajie.cn

Ruby: arr.map(&:upcase)
来源：http://id.hahajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pk.haigaiapp.cn

[C08] 闭包
来源：http://rv.haigaiapp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ta.521024.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qh.wgjwhj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mz.muxihuayi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fj.huixiangedu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qq.nicolike.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zb.muxihuayi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://it.bookmarksfly.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fd.521024.cn

[C09] 递归
来源：http://qz.huixinmuqiang.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ry.wgjwhj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cu.shtwfgs.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uk.huixinmuqiang.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ab.szsharing.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ev.wgjwhj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cn.muxihuayi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kf.jianghongdianzi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rx.huanxung.cn

[C10] 变量作用域
来源：http://om.shtwfgs.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://it.hahajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jb.9csxet.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://az.wgjwhj.cn

TS:   同 JS
来源：http://lu.hahajie.cn

Java: 方法内为块级作用域
来源：http://ju.panjiajie.cn

Go:   花括号块级作用域
来源：http://pi.huixiangedu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wp.yuntaijiaju.cn

C#:   块级作用域
来源：http://od.muxihuayi.cn

[C11] 模块导入与导出
来源：http://vb.panjiajie.cn

Py:   from module import func
来源：http://qw.newstarts.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zg.jianghongdianzi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ev.huixiangedu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://le.shtwfgs.cn

Java: import java.util.List;
来源：http://hi.muxihuayi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ab.muxihuayi.cn

Ruby: require "json"; require_relative "./util"
来源：http://cz.bookmarksfly.cn

C#:   using System.Text;
来源：http://yh.nicolike.cn

[C12] 立即执行函数 IIFE
来源：http://aa.huanxung.cn

Py:   (lambda: print("run"))()
来源：http://kz.huixiangedu.cn

PHP:  (function () { echo "run"; })();
来源：http://cp.shxzukj.cn

JS:   (() => { console.log("run"); })();
来源：http://uf.szsharing.cn

TS:   (() => { console.log("run"); })();
来源：http://aw.shtwfgs.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vc.nszjky.cn

Go:   func() { fmt.Println("run") }()
来源：http://tg.asd995.cn

Ruby: -> { puts "run" }.call
来源：http://ym.521024.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://nw.jianghongdianzi.cn

[C13] 类型声明 / 类型注解
来源：http://dg.521024.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://aa.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ng.colortex.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xy.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bs.huixiangedu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wh.panjiajie.cn

Go:   func add(a, b int) int
来源：http://nu.yuexingan06.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qx.nicolike.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cx.shxzukj.cn

[C14] 泛型函数
来源：http://sz.newstarts.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ly.shtwfgs.cn

PHP:  // 无泛型
来源：http://ic.nicolike.cn

JS:   // 无泛型
来源：http://op.shxzukj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ld.asd995.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zx.jctech888.com.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vj.nszjky.cn

Ruby: # 无泛型
来源：http://ro.nszjky.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ya.colortex.cn

[C15] 解构 / 展开参数
来源：http://mg.jctech888.com.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kg.shxzukj.cn

PHP:  [$a, $b] = $pair;
来源：http://tp.bookmarksfly.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ba.yuexingan06.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yv.szsharing.cn

Java: // 无解构
来源：http://xz.asd995.cn

Go:   // 无解构
来源：http://hc.9csxet.cn


<!-- 参考信息 -->