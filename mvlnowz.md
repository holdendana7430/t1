代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://fs.9csxet.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mz.9csxet.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kc.9csxet.cn

[A25] 字符串比较
来源：http://cm.lnxyls.cn

Py:   s1 == s2; s1 != s2
来源：http://bw.521024.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ay.shxzukj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ns.muxihuayi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ok.hnjuh.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tj.huixinmuqiang.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://iz.hnjuh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://xi.huanxung.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wm.bjjhwx.cn

[A26] 类型转换总览
来源：http://xi.huixinmuqiang.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://io.panjiajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rx.szsharing.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vg.huixinmuqiang.cn

TS:   Number() String() Boolean() x as number
来源：http://nw.521024.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ao.jianghongdianzi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pz.lnxyls.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://qj.newstarts.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ps.colortex.cn

================================================================================
来源：http://xh.yuntaijiaju.cn

B. 流程控制
来源：http://dy.wgjwhj.cn

================================================================================
来源：http://nh.huanxung.cn

[B01] 条件判断 if / else
来源：http://md.jianghongdianzi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dg.bjjhwx.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vg.521024.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tp.hnjuh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qo.shxzukj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://fk.9csxet.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nd.haigaiapp.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ad.asd995.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xm.shxzukj.cn

[B02] 多分支 else if / elif
来源：http://ot.jctech888.com.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ve.huanxung.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rt.521024.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ao.muxihuayi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mc.shtwfgs.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pu.bjjhwx.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ug.gzmigu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tu.shtwfgs.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qg.gzmigu.cn

[B03] switch / match / case
来源：http://eg.yuntaijiaju.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qi.szxytkj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lg.muxihuayi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dl.gzmigu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tj.bjjhwx.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bz.9csxet.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fe.muxihuayi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mu.asd995.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qp.bjjhwx.cn

[B04] for 计数循环
来源：http://ke.nszjky.cn

Py:   for i in range(10): print(i)
来源：http://bt.jctech888.com.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ng.shxzukj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ag.yuntaijiaju.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ru.szsharing.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ty.jctech888.com.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lx.nszjky.cn

Ruby: 10.times { |i| puts i }
来源：http://ql.hnjuh.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gg.haigaiapp.cn

[B05] 遍历数组 / 列表
来源：http://tk.panjiajie.cn

Py:   for item in arr: print(item)
来源：http://eo.panjiajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://je.huanxung.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ax.bookmarksfly.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://dh.shxzukj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qv.haigaiapp.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zf.yuexingan06.cn

Ruby: arr.each { |item| puts item }
来源：http://dd.hahajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ah.shxzukj.cn

[B06] 遍历字典 / 对象
来源：http://us.jianghongdianzi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tz.hahajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ri.nicolike.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hi.chemitech.net.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://on.muxihuayi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://le.bjjhwx.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://la.huanxung.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ow.haigaiapp.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://oi.shxzskj.cn

[B07] while 循环
来源：http://qs.shxzukj.cn

Py:   while i < 10: i += 1
来源：http://nr.bjjhwx.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vq.huixinmuqiang.cn

JS:   while (i < 10) { i++; }
来源：http://va.szsharing.cn

TS:   while (i < 10) { i++; }
来源：http://mr.hnjuh.cn

Java: while (i < 10) { i++; }
来源：http://nn.chemitech.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xp.gzmigu.cn

Ruby: while i < 10; i += 1; end
来源：http://zm.jctech888.com.cn

C#:   while (i < 10) { i++; }
来源：http://do.asd995.cn

[B08] do-while（至少执行一次）
来源：http://wg.yuntaijiaju.cn

Py:   # 无 do-while：用 while True + break
来源：http://be.wgjwhj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://di.szxytkj.cn

JS:   do { i++; } while (i < 10);
来源：http://oa.haigaiapp.cn

TS:   do { i++; } while (i < 10);
来源：http://gt.521024.cn

Java: do { i++; } while (i < 10);
来源：http://gi.muxihuayi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://qe.521024.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rb.jianghongdianzi.cn

C#:   do { i++; } while (i < 10);
来源：http://uv.wgjwhj.cn

[B09] break 与 continue
来源：http://eq.huanxung.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yp.colortex.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nx.bookmarksfly.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ti.shxzukj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kb.nszjky.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rz.huixiangedu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mh.yuexingan06.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lr.huixinmuqiang.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dy.shxzukj.cn

[B10] 遍历同时拿索引
来源：http://pn.panjiajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kg.newstarts.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fk.huixinmuqiang.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jw.panjiajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://av.szxytkj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vu.yuntaijiaju.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xk.panjiajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yh.9csxet.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wy.shxzskj.cn

[B11] 生成数字序列 / 区间
来源：http://ua.chemitech.net.cn

Py:   list(range(0, 10, 2))
来源：http://qr.shtwfgs.cn

PHP:  range(0, 10, 2);
来源：http://hk.bjjhwx.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fm.nszjky.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cx.lnxyls.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ps.muxihuayi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dx.shxzukj.cn

Ruby: (0...10).step(2).to_a
来源：http://nl.gzmigu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wj.shxzukj.cn

[B12] 跳出多层循环
来源：http://iz.jctech888.com.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://qn.colortex.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://tj.9csxet.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ls.9csxet.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wm.nicolike.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://di.haigaiapp.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sm.nicolike.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gt.9csxet.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sf.hnjuh.cn

[B13] 判断是否为数字
来源：http://wo.shtwfgs.cn

Py:   isinstance(x, (int, float))
来源：http://up.shxzukj.cn

PHP:  is_numeric($x)
来源：http://cl.hahajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://by.shxzskj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kp.shtwfgs.cn

Java: x instanceof Number
来源：http://ug.nszjky.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pm.hahajie.cn

Ruby: x.is_a?(Numeric)
来源：http://na.huanxung.cn

C#:   x is int or double or decimal
来源：http://pr.szsharing.cn

[B14] 判断值是否在集合内
来源：http://af.shtwfgs.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ew.hahajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ec.panjiajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://by.chemitech.net.cn

TS:   [1, 2, 3].includes(x)
来源：http://zj.huixinmuqiang.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://sl.huixiangedu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bo.jctech888.com.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ia.asd995.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://af.panjiajie.cn

[B15] 布尔运算与取反
来源：http://sm.nicolike.cn

Py:   a and b or not c
来源：http://sd.asd995.cn

PHP:  $a && $b || !$c
来源：http://tz.yuntaijiaju.cn

JS:   a && b || !c
来源：http://uw.wgjwhj.cn

TS:   a && b || !c
来源：http://oy.521024.cn

Java: a && b || !c
来源：http://fq.lnxyls.cn

Go:   a && b || !c
来源：http://ia.gzmigu.cn

Ruby: a && b || !c
来源：http://af.gzmigu.cn

C#:   a && b || !c
来源：http://ve.shtwfgs.cn

[B16] 卫语句：不满足条件提前返回
来源：http://kg.haigaiapp.cn

Py:   if not data: return
来源：http://in.huixinmuqiang.cn

PHP:  if (!$data) { return; }
来源：http://tv.gzmigu.cn

JS:   if (!data) return;
来源：http://nl.shxzskj.cn

TS:   if (!data) return;
来源：http://ac.hnjuh.cn

Java: if (data == null) return;
来源：http://yr.gzmigu.cn

Go:   if data == nil { return }
来源：http://od.yuntaijiaju.cn

Ruby: return if data.nil?
来源：http://bh.9csxet.cn

C#:   if (data == null) return;
来源：http://oy.muxihuayi.cn

================================================================================
来源：http://mm.szxytkj.cn

C. 函数与作用域
来源：http://ee.chemitech.net.cn

================================================================================
来源：http://vb.shxzukj.cn

[C01] 定义函数
来源：http://bk.nszjky.cn

Py:   def add(a, b): return a + b
来源：http://rr.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aw.huanxung.cn

JS:   function add(a, b) { return a + b; }
来源：http://ho.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ae.9csxet.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://tx.shxzskj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vc.yuntaijiaju.cn

Ruby: def add(a, b); a + b; end
来源：http://wv.newstarts.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dz.bjjhwx.cn

[C02] 默认参数
来源：http://qq.9csxet.cn

Py:   def greet(name="World"): return name
来源：http://ep.yuexingan06.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://jx.9csxet.cn

JS:   function greet(name = "World") { return name; }
来源：http://vy.huanxung.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fa.yuexingan06.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://sa.9csxet.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ay.szxytkj.cn

Ruby: def greet(name = "World") = name
来源：http://xo.huanxung.cn

C#:   string Greet(string name = "World") => name;
来源：http://fq.bjjhwx.cn

[C03] 可变参数
来源：http://li.colortex.cn

Py:   def total(*args): return sum(args)
来源：http://ok.huixinmuqiang.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://du.asd995.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qa.jctech888.com.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gv.gzmigu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://oa.nszjky.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cj.asd995.cn

Ruby: def total(*nums); nums.sum; end
来源：http://jy.huixiangedu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ng.hahajie.cn

[C04] 命名参数 / 关键字参数
来源：http://lx.gzmigu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://du.jctech888.com.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xl.lnxyls.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ga.huixiangedu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://aq.newstarts.cn

Java: // 无：用 Builder 模式或 record
来源：http://fa.szsharing.cn

Go:   // 无：用配置结构体参数
来源：http://cd.asd995.cn

Ruby: f(a: 1, b: 2)
来源：http://mx.bookmarksfly.cn

C#:   f(a: 1, b: 2)
来源：http://uh.yuntaijiaju.cn

[C05] 返回多个值
来源：http://nh.hnjuh.cn

Py:   return a, b
来源：http://vs.hnjuh.cn

PHP:  return [$a, $b];
来源：http://yh.wgjwhj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fj.9csxet.cn

TS:   return { a, b };
来源：http://ch.muxihuayi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://af.asd995.cn

Go:   return a, b
来源：http://qn.colortex.cn

Ruby: return a, b
来源：http://dm.lnxyls.cn

C#:   return (a, b);              // ValueTuple
来源：http://yz.shxzskj.cn

[C06] 匿名函数 / lambda
来源：http://iz.muxihuayi.cn

Py:   square = lambda x: x * x
来源：http://kw.bjjhwx.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bk.hahajie.cn

JS:   const square = x => x * x;
来源：http://ji.huixiangedu.cn

TS:   const square = (x: number): number => x * x;
来源：http://uc.nszjky.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xd.shtwfgs.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ly.shxzskj.cn

Ruby: square = ->(x) { x * x }
来源：http://vl.muxihuayi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://pg.szsharing.cn

[C07] 把函数作为参数传入
来源：http://qy.panjiajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sl.521024.cn

PHP:  array_map("strtoupper", $arr);
来源：http://yh.shxzukj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fo.nicolike.cn

TS:   arr.map(String)
来源：http://ns.bookmarksfly.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rm.yuexingan06.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ro.szsharing.cn

Ruby: arr.map(&:upcase)
来源：http://gp.yuexingan06.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://sd.yuexingan06.cn

[C08] 闭包
来源：http://ld.colortex.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vj.colortex.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ve.lnxyls.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ii.szsharing.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sf.newstarts.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ge.huixinmuqiang.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vl.shtwfgs.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://al.hahajie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fq.huixinmuqiang.cn

[C09] 递归
来源：http://ff.newstarts.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ov.szsharing.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sx.shxzukj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yl.yuexingan06.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jc.szxytkj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://df.hnjuh.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gz.shxzskj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tb.jianghongdianzi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vb.muxihuayi.cn

[C10] 变量作用域
来源：http://oo.szxytkj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fo.hahajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rp.szxytkj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dy.yuntaijiaju.cn

TS:   同 JS
来源：http://ij.521024.cn

Java: 方法内为块级作用域
来源：http://af.hahajie.cn

Go:   花括号块级作用域
来源：http://zu.shxzskj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lr.panjiajie.cn

C#:   块级作用域
来源：http://wb.hahajie.cn

[C11] 模块导入与导出
来源：http://wn.panjiajie.cn

Py:   from module import func
来源：http://hk.hnjuh.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ml.huixinmuqiang.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://as.haigaiapp.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tj.yuexingan06.cn

Java: import java.util.List;
来源：http://gy.521024.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tt.yuexingan06.cn

Ruby: require "json"; require_relative "./util"
来源：http://yh.bookmarksfly.cn

C#:   using System.Text;
来源：http://bi.huixiangedu.cn

[C12] 立即执行函数 IIFE
来源：http://kd.521024.cn

Py:   (lambda: print("run"))()
来源：http://kl.huixinmuqiang.cn

PHP:  (function () { echo "run"; })();
来源：http://dk.lnxyls.cn

JS:   (() => { console.log("run"); })();
来源：http://bq.nszjky.cn

TS:   (() => { console.log("run"); })();
来源：http://ax.yuexingan06.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ke.lnxyls.cn

Go:   func() { fmt.Println("run") }()
来源：http://ou.9csxet.cn

Ruby: -> { puts "run" }.call
来源：http://mn.newstarts.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ug.9csxet.cn

[C13] 类型声明 / 类型注解
来源：http://zx.asd995.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hj.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nd.9csxet.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cl.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cp.hahajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cy.bookmarksfly.cn

Go:   func add(a, b int) int
来源：http://uo.szsharing.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wt.lnxyls.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gu.bjjhwx.cn

[C14] 泛型函数
来源：http://vg.shxzukj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kn.huanxung.cn

PHP:  // 无泛型
来源：http://uy.nicolike.cn

JS:   // 无泛型
来源：http://ma.lnxyls.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vm.gzmigu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rf.shxzskj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vp.shxzukj.cn

Ruby: # 无泛型
来源：http://vs.9csxet.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ej.asd995.cn

[C15] 解构 / 展开参数
来源：http://vu.yuntaijiaju.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cp.huixinmuqiang.cn

PHP:  [$a, $b] = $pair;
来源：http://rt.szxytkj.cn


<!-- 参考信息 -->