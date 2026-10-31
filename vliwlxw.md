代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://qh.huanxung.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pm.9csxet.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rv.jctech888.com.cn

[A25] 字符串比较
来源：http://kr.jctech888.com.cn

Py:   s1 == s2; s1 != s2
来源：http://wj.jctech888.com.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://am.9csxet.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://eo.bookmarksfly.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yc.nszjky.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://sv.jianghongdianzi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jr.hnjuh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vs.panjiajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sr.shxzskj.cn

[A26] 类型转换总览
来源：http://pd.lnxyls.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://di.yuexingan06.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zk.hnjuh.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xq.szxytkj.cn

TS:   Number() String() Boolean() x as number
来源：http://nk.gzmigu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kx.szsharing.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fy.colortex.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.huanxung.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qw.panjiajie.cn

================================================================================
来源：http://zp.lnxyls.cn

B. 流程控制
来源：http://zl.nicolike.cn

================================================================================
来源：http://xs.hahajie.cn

[B01] 条件判断 if / else
来源：http://bs.muxihuayi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://da.shxzukj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hw.hnjuh.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ac.haigaiapp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dx.jianghongdianzi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://gy.panjiajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fc.shxzskj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://th.bjjhwx.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ek.bookmarksfly.cn

[B02] 多分支 else if / elif
来源：http://yt.huixiangedu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cm.shxzskj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rb.gzmigu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yd.szxytkj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nw.szxytkj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yb.chemitech.net.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://am.lnxyls.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gr.shxzskj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ds.nicolike.cn

[B03] switch / match / case
来源：http://uf.asd995.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zr.nszjky.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ab.hnjuh.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lq.haigaiapp.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ps.gzmigu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ch.newstarts.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jr.jctech888.com.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vw.szxytkj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sd.nicolike.cn

[B04] for 计数循环
来源：http://kv.gzmigu.cn

Py:   for i in range(10): print(i)
来源：http://qh.huixinmuqiang.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pd.shxzukj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mz.huanxung.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bp.bjjhwx.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xy.shxzukj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zz.hnjuh.cn

Ruby: 10.times { |i| puts i }
来源：http://dr.bookmarksfly.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://oh.gzmigu.cn

[B05] 遍历数组 / 列表
来源：http://jl.szsharing.cn

Py:   for item in arr: print(item)
来源：http://ly.huixinmuqiang.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://av.shxzskj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qk.szsharing.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ya.shxzskj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://va.jctech888.com.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zc.szsharing.cn

Ruby: arr.each { |item| puts item }
来源：http://pp.shtwfgs.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bh.muxihuayi.cn

[B06] 遍历字典 / 对象
来源：http://da.shtwfgs.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xy.huanxung.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sc.shxzskj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://km.shtwfgs.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gz.muxihuayi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qd.hahajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ih.hnjuh.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ux.panjiajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.nszjky.cn

[B07] while 循环
来源：http://pd.huixiangedu.cn

Py:   while i < 10: i += 1
来源：http://de.colortex.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zs.gzmigu.cn

JS:   while (i < 10) { i++; }
来源：http://ki.hnjuh.cn

TS:   while (i < 10) { i++; }
来源：http://wt.shtwfgs.cn

Java: while (i < 10) { i++; }
来源：http://mu.gzmigu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wi.szsharing.cn

Ruby: while i < 10; i += 1; end
来源：http://pj.yuexingan06.cn

C#:   while (i < 10) { i++; }
来源：http://do.huixinmuqiang.cn

[B08] do-while（至少执行一次）
来源：http://ou.huanxung.cn

Py:   # 无 do-while：用 while True + break
来源：http://oq.muxihuayi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://iy.szsharing.cn

JS:   do { i++; } while (i < 10);
来源：http://wr.wgjwhj.cn

TS:   do { i++; } while (i < 10);
来源：http://qk.szxytkj.cn

Java: do { i++; } while (i < 10);
来源：http://nt.haigaiapp.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bx.shxzskj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ox.shtwfgs.cn

C#:   do { i++; } while (i < 10);
来源：http://po.lnxyls.cn

[B09] break 与 continue
来源：http://wy.panjiajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://be.shxzukj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qu.nicolike.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bz.wgjwhj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vg.hahajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://le.szsharing.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ug.shtwfgs.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yh.yuntaijiaju.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dg.asd995.cn

[B10] 遍历同时拿索引
来源：http://iv.szsharing.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fx.chemitech.net.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ow.nicolike.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cg.9csxet.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fk.newstarts.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mg.hahajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hk.lnxyls.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uf.hnjuh.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://go.szxytkj.cn

[B11] 生成数字序列 / 区间
来源：http://az.chemitech.net.cn

Py:   list(range(0, 10, 2))
来源：http://xn.chemitech.net.cn

PHP:  range(0, 10, 2);
来源：http://dg.huixinmuqiang.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vh.asd995.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hj.szsharing.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pu.szsharing.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://al.szxytkj.cn

Ruby: (0...10).step(2).to_a
来源：http://jv.panjiajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ff.jctech888.com.cn

[B12] 跳出多层循环
来源：http://yj.szxytkj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://sn.colortex.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://kh.9csxet.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qf.nicolike.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ao.szsharing.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yw.yuexingan06.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qd.huanxung.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cy.huixinmuqiang.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ha.shtwfgs.cn

[B13] 判断是否为数字
来源：http://hx.gzmigu.cn

Py:   isinstance(x, (int, float))
来源：http://us.nicolike.cn

PHP:  is_numeric($x)
来源：http://yu.asd995.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ps.yuntaijiaju.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jp.panjiajie.cn

Java: x instanceof Number
来源：http://ij.szxytkj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lr.shtwfgs.cn

Ruby: x.is_a?(Numeric)
来源：http://cc.521024.cn

C#:   x is int or double or decimal
来源：http://cg.huixiangedu.cn

[B14] 判断值是否在集合内
来源：http://wz.yuntaijiaju.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://eg.lnxyls.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://do.szsharing.cn

JS:   [1, 2, 3].includes(x)
来源：http://ou.yuntaijiaju.cn

TS:   [1, 2, 3].includes(x)
来源：http://lz.panjiajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://zy.gzmigu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hx.colortex.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qz.haigaiapp.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jt.lnxyls.cn

[B15] 布尔运算与取反
来源：http://ub.huixiangedu.cn

Py:   a and b or not c
来源：http://kw.szxytkj.cn

PHP:  $a && $b || !$c
来源：http://ln.bookmarksfly.cn

JS:   a && b || !c
来源：http://jy.huanxung.cn

TS:   a && b || !c
来源：http://ms.shtwfgs.cn

Java: a && b || !c
来源：http://an.lnxyls.cn

Go:   a && b || !c
来源：http://eo.lnxyls.cn

Ruby: a && b || !c
来源：http://tr.szsharing.cn

C#:   a && b || !c
来源：http://un.huixiangedu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lj.lnxyls.cn

Py:   if not data: return
来源：http://is.yuntaijiaju.cn

PHP:  if (!$data) { return; }
来源：http://zl.hahajie.cn

JS:   if (!data) return;
来源：http://cx.hahajie.cn

TS:   if (!data) return;
来源：http://we.szxytkj.cn

Java: if (data == null) return;
来源：http://hf.huanxung.cn

Go:   if data == nil { return }
来源：http://bz.hahajie.cn

Ruby: return if data.nil?
来源：http://wx.huixinmuqiang.cn

C#:   if (data == null) return;
来源：http://lh.521024.cn

================================================================================
来源：http://ai.9csxet.cn

C. 函数与作用域
来源：http://uw.521024.cn

================================================================================
来源：http://or.521024.cn

[C01] 定义函数
来源：http://hb.szxytkj.cn

Py:   def add(a, b): return a + b
来源：http://hc.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xx.lnxyls.cn

JS:   function add(a, b) { return a + b; }
来源：http://mk.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sk.huixinmuqiang.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://if.haigaiapp.cn

Go:   func add(a, b int) int { return a + b }
来源：http://uo.521024.cn

Ruby: def add(a, b); a + b; end
来源：http://xk.shxzskj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://js.szsharing.cn

[C02] 默认参数
来源：http://zh.nicolike.cn

Py:   def greet(name="World"): return name
来源：http://ec.huixinmuqiang.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xf.muxihuayi.cn

JS:   function greet(name = "World") { return name; }
来源：http://hw.haigaiapp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hg.nicolike.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://tt.jianghongdianzi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qt.wgjwhj.cn

Ruby: def greet(name = "World") = name
来源：http://kr.gzmigu.cn

C#:   string Greet(string name = "World") => name;
来源：http://un.haigaiapp.cn

[C03] 可变参数
来源：http://qo.yuntaijiaju.cn

Py:   def total(*args): return sum(args)
来源：http://ep.wgjwhj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lv.521024.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://me.bookmarksfly.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ez.newstarts.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ge.hnjuh.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pa.huixinmuqiang.cn

Ruby: def total(*nums); nums.sum; end
来源：http://cf.nszjky.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://et.muxihuayi.cn

[C04] 命名参数 / 关键字参数
来源：http://lu.521024.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ah.gzmigu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xv.chemitech.net.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ml.lnxyls.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wz.jianghongdianzi.cn

Java: // 无：用 Builder 模式或 record
来源：http://cf.haigaiapp.cn

Go:   // 无：用配置结构体参数
来源：http://an.colortex.cn

Ruby: f(a: 1, b: 2)
来源：http://jj.chemitech.net.cn

C#:   f(a: 1, b: 2)
来源：http://ho.9csxet.cn

[C05] 返回多个值
来源：http://zd.panjiajie.cn

Py:   return a, b
来源：http://bx.hahajie.cn

PHP:  return [$a, $b];
来源：http://gx.nszjky.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pe.colortex.cn

TS:   return { a, b };
来源：http://ur.asd995.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tq.chemitech.net.cn

Go:   return a, b
来源：http://wq.chemitech.net.cn

Ruby: return a, b
来源：http://lg.huixiangedu.cn

C#:   return (a, b);              // ValueTuple
来源：http://cn.panjiajie.cn

[C06] 匿名函数 / lambda
来源：http://le.haigaiapp.cn

Py:   square = lambda x: x * x
来源：http://le.huixinmuqiang.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://mz.haigaiapp.cn

JS:   const square = x => x * x;
来源：http://uv.muxihuayi.cn

TS:   const square = (x: number): number => x * x;
来源：http://xq.jianghongdianzi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dp.wgjwhj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kc.huixinmuqiang.cn

Ruby: square = ->(x) { x * x }
来源：http://wo.lnxyls.cn

C#:   Func<int, int> square = x => x * x;
来源：http://jp.hahajie.cn

[C07] 把函数作为参数传入
来源：http://hh.9csxet.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://uh.521024.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jj.bjjhwx.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cj.asd995.cn

TS:   arr.map(String)
来源：http://gu.jctech888.com.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ls.wgjwhj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://eb.shxzskj.cn

Ruby: arr.map(&:upcase)
来源：http://os.9csxet.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://vf.haigaiapp.cn

[C08] 闭包
来源：http://if.lnxyls.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lb.szsharing.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://op.colortex.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://al.jctech888.com.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://an.nicolike.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dl.yuexingan06.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ua.panjiajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lo.muxihuayi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mi.chemitech.net.cn

[C09] 递归
来源：http://za.huixiangedu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ef.521024.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hv.huixiangedu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cz.huixinmuqiang.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mx.bookmarksfly.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ez.szsharing.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zu.shxzukj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zc.panjiajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pq.haigaiapp.cn

[C10] 变量作用域
来源：http://dh.hnjuh.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jr.hnjuh.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://oc.jctech888.com.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yl.wgjwhj.cn

TS:   同 JS
来源：http://lt.muxihuayi.cn

Java: 方法内为块级作用域
来源：http://jl.hnjuh.cn

Go:   花括号块级作用域
来源：http://xa.muxihuayi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nc.lnxyls.cn

C#:   块级作用域
来源：http://xz.chemitech.net.cn

[C11] 模块导入与导出
来源：http://xa.szsharing.cn

Py:   from module import func
来源：http://gt.shxzukj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ze.huanxung.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://mb.hnjuh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ve.chemitech.net.cn

Java: import java.util.List;
来源：http://mj.lnxyls.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gj.nicolike.cn

Ruby: require "json"; require_relative "./util"
来源：http://xi.colortex.cn

C#:   using System.Text;
来源：http://lb.huixiangedu.cn

[C12] 立即执行函数 IIFE
来源：http://fp.huanxung.cn

Py:   (lambda: print("run"))()
来源：http://bx.huanxung.cn

PHP:  (function () { echo "run"; })();
来源：http://yw.haigaiapp.cn

JS:   (() => { console.log("run"); })();
来源：http://vr.panjiajie.cn

TS:   (() => { console.log("run"); })();
来源：http://rx.huixiangedu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zh.521024.cn

Go:   func() { fmt.Println("run") }()
来源：http://dl.colortex.cn

Ruby: -> { puts "run" }.call
来源：http://ao.bookmarksfly.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xk.bookmarksfly.cn

[C13] 类型声明 / 类型注解
来源：http://wu.panjiajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://er.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://np.bjjhwx.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zy.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ar.jianghongdianzi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://nk.jctech888.com.cn

Go:   func add(a, b int) int
来源：http://rf.huixiangedu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zo.haigaiapp.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ye.szxytkj.cn

[C14] 泛型函数
来源：http://vd.gzmigu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://id.muxihuayi.cn

PHP:  // 无泛型
来源：http://ap.yuntaijiaju.cn

JS:   // 无泛型
来源：http://pv.shtwfgs.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xw.lnxyls.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bh.hnjuh.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gc.yuntaijiaju.cn

Ruby: # 无泛型
来源：http://jn.shxzukj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cb.panjiajie.cn

[C15] 解构 / 展开参数
来源：http://lf.521024.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mv.huanxung.cn

PHP:  [$a, $b] = $pair;
来源：http://ac.jctech888.com.cn


<!-- 参考信息 -->