代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://ix.nicolike.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lx.szsharing.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://am.newstarts.cn

[A25] 字符串比较
来源：http://mt.lnxyls.cn

Py:   s1 == s2; s1 != s2
来源：http://vm.shtwfgs.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wl.nszjky.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yk.lnxyls.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rj.muxihuayi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://uo.wgjwhj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jf.wgjwhj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rq.huanxung.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://en.shxzskj.cn

[A26] 类型转换总览
来源：http://hu.wgjwhj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lu.szxytkj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://eu.shxzukj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wp.bookmarksfly.cn

TS:   Number() String() Boolean() x as number
来源：http://gq.jianghongdianzi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kt.szxytkj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ws.bookmarksfly.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ac.shxzskj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://le.yuntaijiaju.cn

================================================================================
来源：http://gf.colortex.cn

B. 流程控制
来源：http://ds.shxzskj.cn

================================================================================
来源：http://bb.yuntaijiaju.cn

[B01] 条件判断 if / else
来源：http://gw.huixinmuqiang.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://yw.szsharing.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://du.panjiajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://do.nicolike.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jf.huixinmuqiang.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://em.muxihuayi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hg.lnxyls.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://su.jianghongdianzi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://id.huanxung.cn

[B02] 多分支 else if / elif
来源：http://io.jctech888.com.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mb.nszjky.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yk.shxzukj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://db.9csxet.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yi.hnjuh.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zn.yuntaijiaju.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ud.huixinmuqiang.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://sm.jianghongdianzi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ne.wgjwhj.cn

[B03] switch / match / case
来源：http://gd.bookmarksfly.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dj.hnjuh.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uj.shxzskj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jq.yuntaijiaju.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qh.shxzskj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lq.gzmigu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rb.gzmigu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sg.huixinmuqiang.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ni.gzmigu.cn

[B04] for 计数循环
来源：http://pq.jianghongdianzi.cn

Py:   for i in range(10): print(i)
来源：http://pl.nszjky.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://of.shxzukj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mq.szxytkj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nm.bookmarksfly.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ax.huanxung.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zq.bookmarksfly.cn

Ruby: 10.times { |i| puts i }
来源：http://tq.asd995.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lj.chemitech.net.cn

[B05] 遍历数组 / 列表
来源：http://ni.hahajie.cn

Py:   for item in arr: print(item)
来源：http://le.colortex.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://po.huixiangedu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://vi.yuntaijiaju.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://sb.shxzskj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zs.huixinmuqiang.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://by.lnxyls.cn

Ruby: arr.each { |item| puts item }
来源：http://ax.lnxyls.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://oy.huanxung.cn

[B06] 遍历字典 / 对象
来源：http://yl.asd995.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mk.hnjuh.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vb.panjiajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fe.hnjuh.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ib.gzmigu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sv.9csxet.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rb.muxihuayi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ep.szxytkj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ja.nszjky.cn

[B07] while 循环
来源：http://lc.9csxet.cn

Py:   while i < 10: i += 1
来源：http://sm.521024.cn

PHP:  while ($i < 10) { $i++; }
来源：http://rs.haigaiapp.cn

JS:   while (i < 10) { i++; }
来源：http://xa.wgjwhj.cn

TS:   while (i < 10) { i++; }
来源：http://fu.huixinmuqiang.cn

Java: while (i < 10) { i++; }
来源：http://yz.szsharing.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pt.gzmigu.cn

Ruby: while i < 10; i += 1; end
来源：http://zq.hahajie.cn

C#:   while (i < 10) { i++; }
来源：http://rb.gzmigu.cn

[B08] do-while（至少执行一次）
来源：http://om.shtwfgs.cn

Py:   # 无 do-while：用 while True + break
来源：http://ug.chemitech.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://wn.huanxung.cn

JS:   do { i++; } while (i < 10);
来源：http://vj.yuexingan06.cn

TS:   do { i++; } while (i < 10);
来源：http://hl.9csxet.cn

Java: do { i++; } while (i < 10);
来源：http://tu.shxzskj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://eq.panjiajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ns.newstarts.cn

C#:   do { i++; } while (i < 10);
来源：http://er.asd995.cn

[B09] break 与 continue
来源：http://fl.shtwfgs.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vb.huixinmuqiang.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yz.bjjhwx.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ui.hnjuh.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jb.jianghongdianzi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ul.wgjwhj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yv.nszjky.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qq.bjjhwx.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sr.yuexingan06.cn

[B10] 遍历同时拿索引
来源：http://md.hahajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cw.9csxet.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fw.jctech888.com.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://go.yuexingan06.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://js.szsharing.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ci.lnxyls.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bc.9csxet.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://la.haigaiapp.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zl.panjiajie.cn

[B11] 生成数字序列 / 区间
来源：http://pk.shxzskj.cn

Py:   list(range(0, 10, 2))
来源：http://ol.lnxyls.cn

PHP:  range(0, 10, 2);
来源：http://kc.nicolike.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qt.gzmigu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zi.asd995.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cr.521024.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://oc.jctech888.com.cn

Ruby: (0...10).step(2).to_a
来源：http://nf.wgjwhj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vv.colortex.cn

[B12] 跳出多层循环
来源：http://ws.bjjhwx.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wx.panjiajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wn.muxihuayi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://st.panjiajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://in.jianghongdianzi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cq.wgjwhj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wv.jctech888.com.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pk.lnxyls.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uj.yuexingan06.cn

[B13] 判断是否为数字
来源：http://hp.nicolike.cn

Py:   isinstance(x, (int, float))
来源：http://af.9csxet.cn

PHP:  is_numeric($x)
来源：http://ol.9csxet.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gl.shtwfgs.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bk.chemitech.net.cn

Java: x instanceof Number
来源：http://qt.newstarts.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://es.szsharing.cn

Ruby: x.is_a?(Numeric)
来源：http://mn.521024.cn

C#:   x is int or double or decimal
来源：http://um.yuntaijiaju.cn

[B14] 判断值是否在集合内
来源：http://sc.muxihuayi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mk.huixiangedu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mn.hahajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://eg.gzmigu.cn

TS:   [1, 2, 3].includes(x)
来源：http://da.521024.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kg.lnxyls.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nf.521024.cn

Ruby: [1, 2, 3].include?(x)
来源：http://nx.panjiajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nt.bjjhwx.cn

[B15] 布尔运算与取反
来源：http://ta.colortex.cn

Py:   a and b or not c
来源：http://pb.asd995.cn

PHP:  $a && $b || !$c
来源：http://pb.yuexingan06.cn

JS:   a && b || !c
来源：http://hj.huanxung.cn

TS:   a && b || !c
来源：http://cw.9csxet.cn

Java: a && b || !c
来源：http://ls.muxihuayi.cn

Go:   a && b || !c
来源：http://pr.muxihuayi.cn

Ruby: a && b || !c
来源：http://ej.szsharing.cn

C#:   a && b || !c
来源：http://qk.shxzukj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://nv.9csxet.cn

Py:   if not data: return
来源：http://at.521024.cn

PHP:  if (!$data) { return; }
来源：http://kb.panjiajie.cn

JS:   if (!data) return;
来源：http://vi.lnxyls.cn

TS:   if (!data) return;
来源：http://vv.hnjuh.cn

Java: if (data == null) return;
来源：http://vc.bookmarksfly.cn

Go:   if data == nil { return }
来源：http://hu.hnjuh.cn

Ruby: return if data.nil?
来源：http://pt.bjjhwx.cn

C#:   if (data == null) return;
来源：http://od.yuexingan06.cn

================================================================================
来源：http://fa.muxihuayi.cn

C. 函数与作用域
来源：http://kd.shtwfgs.cn

================================================================================
来源：http://eg.bookmarksfly.cn

[C01] 定义函数
来源：http://sm.bookmarksfly.cn

Py:   def add(a, b): return a + b
来源：http://yr.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ly.haigaiapp.cn

JS:   function add(a, b) { return a + b; }
来源：http://qi.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://db.nicolike.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qp.wgjwhj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ml.lnxyls.cn

Ruby: def add(a, b); a + b; end
来源：http://fa.521024.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wn.chemitech.net.cn

[C02] 默认参数
来源：http://qi.lnxyls.cn

Py:   def greet(name="World"): return name
来源：http://nd.bjjhwx.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://si.gzmigu.cn

JS:   function greet(name = "World") { return name; }
来源：http://ki.shxzskj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://li.asd995.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ln.wgjwhj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://af.yuexingan06.cn

Ruby: def greet(name = "World") = name
来源：http://xk.shtwfgs.cn

C#:   string Greet(string name = "World") => name;
来源：http://qp.shxzukj.cn

[C03] 可变参数
来源：http://pr.lnxyls.cn

Py:   def total(*args): return sum(args)
来源：http://vz.szxytkj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pj.chemitech.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pt.jianghongdianzi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jy.asd995.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fh.yuntaijiaju.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xo.bjjhwx.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ha.nszjky.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vc.huanxung.cn

[C04] 命名参数 / 关键字参数
来源：http://cu.szsharing.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sb.colortex.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xs.szxytkj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mp.nicolike.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rv.gzmigu.cn

Java: // 无：用 Builder 模式或 record
来源：http://dy.chemitech.net.cn

Go:   // 无：用配置结构体参数
来源：http://sa.shtwfgs.cn

Ruby: f(a: 1, b: 2)
来源：http://gx.shxzskj.cn

C#:   f(a: 1, b: 2)
来源：http://yk.chemitech.net.cn

[C05] 返回多个值
来源：http://wl.jianghongdianzi.cn

Py:   return a, b
来源：http://hh.huixinmuqiang.cn

PHP:  return [$a, $b];
来源：http://kx.yuntaijiaju.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dv.bookmarksfly.cn

TS:   return { a, b };
来源：http://hz.haigaiapp.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ik.colortex.cn

Go:   return a, b
来源：http://wd.yuexingan06.cn

Ruby: return a, b
来源：http://rc.bjjhwx.cn

C#:   return (a, b);              // ValueTuple
来源：http://hx.huanxung.cn

[C06] 匿名函数 / lambda
来源：http://gc.bjjhwx.cn

Py:   square = lambda x: x * x
来源：http://ch.lnxyls.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://us.9csxet.cn

JS:   const square = x => x * x;
来源：http://gz.shxzskj.cn

TS:   const square = (x: number): number => x * x;
来源：http://ln.hnjuh.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fn.huixiangedu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kb.asd995.cn

Ruby: square = ->(x) { x * x }
来源：http://xz.haigaiapp.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ed.yuntaijiaju.cn

[C07] 把函数作为参数传入
来源：http://tq.521024.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qs.jctech888.com.cn

PHP:  array_map("strtoupper", $arr);
来源：http://tq.hahajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://os.nicolike.cn

TS:   arr.map(String)
来源：http://hb.yuexingan06.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://oe.9csxet.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yy.bjjhwx.cn

Ruby: arr.map(&:upcase)
来源：http://jl.huanxung.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xa.colortex.cn

[C08] 闭包
来源：http://cc.gzmigu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ym.huanxung.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xn.bjjhwx.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gk.jianghongdianzi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yf.521024.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bp.chemitech.net.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://er.shxzukj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wv.bookmarksfly.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pm.wgjwhj.cn

[C09] 递归
来源：http://jz.shxzskj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zm.haigaiapp.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tx.asd995.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wt.jctech888.com.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://at.nszjky.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sk.hnjuh.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qx.chemitech.net.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://no.wgjwhj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kk.521024.cn

[C10] 变量作用域
来源：http://wb.shxzukj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hd.muxihuayi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yr.yuntaijiaju.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fy.jianghongdianzi.cn

TS:   同 JS
来源：http://fb.haigaiapp.cn

Java: 方法内为块级作用域
来源：http://qc.colortex.cn

Go:   花括号块级作用域
来源：http://gc.nszjky.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gi.hahajie.cn

C#:   块级作用域
来源：http://ti.yuexingan06.cn

[C11] 模块导入与导出
来源：http://uv.yuntaijiaju.cn

Py:   from module import func
来源：http://fl.bookmarksfly.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zu.wgjwhj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://oe.nicolike.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ii.shxzskj.cn

Java: import java.util.List;
来源：http://nt.9csxet.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://so.bookmarksfly.cn

Ruby: require "json"; require_relative "./util"
来源：http://bu.colortex.cn

C#:   using System.Text;
来源：http://rn.chemitech.net.cn

[C12] 立即执行函数 IIFE
来源：http://be.nszjky.cn

Py:   (lambda: print("run"))()
来源：http://ah.lnxyls.cn

PHP:  (function () { echo "run"; })();
来源：http://fq.chemitech.net.cn

JS:   (() => { console.log("run"); })();
来源：http://zx.chemitech.net.cn

TS:   (() => { console.log("run"); })();
来源：http://cw.huixinmuqiang.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bs.lnxyls.cn

Go:   func() { fmt.Println("run") }()
来源：http://cj.colortex.cn

Ruby: -> { puts "run" }.call
来源：http://pf.9csxet.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://bu.shtwfgs.cn

[C13] 类型声明 / 类型注解
来源：http://fi.9csxet.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ys.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kq.wgjwhj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ah.szxytkj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wy.jctech888.com.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xc.muxihuayi.cn

Go:   func add(a, b int) int
来源：http://vt.jctech888.com.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://si.yuexingan06.cn

C#:   int Add(int a, int b) => a + b;
来源：http://rv.shtwfgs.cn

[C14] 泛型函数
来源：http://wd.chemitech.net.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mi.yuexingan06.cn

PHP:  // 无泛型
来源：http://md.jianghongdianzi.cn

JS:   // 无泛型
来源：http://or.jianghongdianzi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yh.521024.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lu.nicolike.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://it.muxihuayi.cn

Ruby: # 无泛型
来源：http://cy.panjiajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mg.nicolike.cn

[C15] 解构 / 展开参数
来源：http://ie.colortex.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tc.huixinmuqiang.cn

PHP:  [$a, $b] = $pair;
来源：http://vv.szsharing.cn


<!-- 参考信息 -->