代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rr.nszjky.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lo.bookmarksfly.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://dz.colortex.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rf.yuexingan06.cn

[A26] 类型转换总览
来源：http://is.szsharing.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bo.nicolike.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fk.nszjky.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://os.nicolike.cn

TS:   Number() String() Boolean() x as number
来源：http://hv.wgjwhj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nr.huanxung.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vy.colortex.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://qt.newstarts.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://li.wgjwhj.cn

================================================================================
来源：http://ju.huanxung.cn

B. 流程控制
来源：http://sv.asd995.cn

================================================================================
来源：http://qg.jctech888.com.cn

[B01] 条件判断 if / else
来源：http://mq.shtwfgs.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ow.shxzskj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://au.bjjhwx.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dv.asd995.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gh.szsharing.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ji.nicolike.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fd.newstarts.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yy.521024.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ko.521024.cn

[B02] 多分支 else if / elif
来源：http://kz.nszjky.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vz.szxytkj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gm.colortex.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qf.panjiajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mb.gzmigu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gs.9csxet.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tu.wgjwhj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ul.nszjky.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qf.gzmigu.cn

[B03] switch / match / case
来源：http://td.huixinmuqiang.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ci.9csxet.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hq.gzmigu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ti.nicolike.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pa.yuexingan06.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jd.muxihuayi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ap.nszjky.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tl.colortex.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hk.gzmigu.cn

[B04] for 计数循环
来源：http://al.yuexingan06.cn

Py:   for i in range(10): print(i)
来源：http://fy.newstarts.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vo.hahajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://he.gzmigu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tn.nszjky.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jf.szsharing.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ia.newstarts.cn

Ruby: 10.times { |i| puts i }
来源：http://vw.yuexingan06.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://av.nicolike.cn

[B05] 遍历数组 / 列表
来源：http://we.bookmarksfly.cn

Py:   for item in arr: print(item)
来源：http://cn.colortex.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jf.chemitech.net.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ez.muxihuayi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yr.gzmigu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ix.haigaiapp.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://iq.jctech888.com.cn

Ruby: arr.each { |item| puts item }
来源：http://cr.huixiangedu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uw.huixinmuqiang.cn

[B06] 遍历字典 / 对象
来源：http://jf.muxihuayi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://rz.nszjky.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dd.asd995.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ux.haigaiapp.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ci.yuexingan06.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sn.bookmarksfly.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lo.yuntaijiaju.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://em.gzmigu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gg.panjiajie.cn

[B07] while 循环
来源：http://zp.bookmarksfly.cn

Py:   while i < 10: i += 1
来源：http://zt.bookmarksfly.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ni.jianghongdianzi.cn

JS:   while (i < 10) { i++; }
来源：http://hm.521024.cn

TS:   while (i < 10) { i++; }
来源：http://wh.bjjhwx.cn

Java: while (i < 10) { i++; }
来源：http://zw.newstarts.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tu.hahajie.cn

Ruby: while i < 10; i += 1; end
来源：http://sg.gzmigu.cn

C#:   while (i < 10) { i++; }
来源：http://mv.wgjwhj.cn

[B08] do-while（至少执行一次）
来源：http://ql.jianghongdianzi.cn

Py:   # 无 do-while：用 while True + break
来源：http://qw.jianghongdianzi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://md.szsharing.cn

JS:   do { i++; } while (i < 10);
来源：http://fa.shtwfgs.cn

TS:   do { i++; } while (i < 10);
来源：http://mg.colortex.cn

Java: do { i++; } while (i < 10);
来源：http://rq.newstarts.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://zb.yuntaijiaju.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ot.yuntaijiaju.cn

C#:   do { i++; } while (i < 10);
来源：http://hs.521024.cn

[B09] break 与 continue
来源：http://by.yuexingan06.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sy.huixiangedu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rd.panjiajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sz.szxytkj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bh.shxzskj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ob.jctech888.com.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wn.yuntaijiaju.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dp.gzmigu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jp.lnxyls.cn

[B10] 遍历同时拿索引
来源：http://rl.bookmarksfly.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://js.bookmarksfly.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ra.haigaiapp.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ma.newstarts.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ve.szxytkj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ce.panjiajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ci.huixinmuqiang.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fa.nszjky.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ar.hnjuh.cn

[B11] 生成数字序列 / 区间
来源：http://rx.jianghongdianzi.cn

Py:   list(range(0, 10, 2))
来源：http://vp.muxihuayi.cn

PHP:  range(0, 10, 2);
来源：http://id.yuntaijiaju.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fv.shxzskj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yf.newstarts.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zw.hnjuh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hc.nicolike.cn

Ruby: (0...10).step(2).to_a
来源：http://zy.chemitech.net.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kf.colortex.cn

[B12] 跳出多层循环
来源：http://ej.shxzskj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://lo.jianghongdianzi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ia.huixinmuqiang.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zr.nicolike.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bk.newstarts.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ay.shxzukj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lb.newstarts.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ki.huanxung.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xa.muxihuayi.cn

[B13] 判断是否为数字
来源：http://in.muxihuayi.cn

Py:   isinstance(x, (int, float))
来源：http://lv.jianghongdianzi.cn

PHP:  is_numeric($x)
来源：http://jc.colortex.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qj.shtwfgs.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dr.colortex.cn

Java: x instanceof Number
来源：http://uu.szsharing.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://az.521024.cn

Ruby: x.is_a?(Numeric)
来源：http://gb.colortex.cn

C#:   x is int or double or decimal
来源：http://uf.panjiajie.cn

[B14] 判断值是否在集合内
来源：http://ay.yuexingan06.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lq.hnjuh.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fq.lnxyls.cn

JS:   [1, 2, 3].includes(x)
来源：http://pp.wgjwhj.cn

TS:   [1, 2, 3].includes(x)
来源：http://yu.lnxyls.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qr.asd995.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hj.szxytkj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://bv.huixinmuqiang.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://io.muxihuayi.cn

[B15] 布尔运算与取反
来源：http://xy.haigaiapp.cn

Py:   a and b or not c
来源：http://rj.hnjuh.cn

PHP:  $a && $b || !$c
来源：http://qi.haigaiapp.cn

JS:   a && b || !c
来源：http://pn.muxihuayi.cn

TS:   a && b || !c
来源：http://wc.hahajie.cn

Java: a && b || !c
来源：http://kh.szsharing.cn

Go:   a && b || !c
来源：http://ps.huixiangedu.cn

Ruby: a && b || !c
来源：http://sa.shxzskj.cn

C#:   a && b || !c
来源：http://st.nicolike.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hc.shxzskj.cn

Py:   if not data: return
来源：http://sy.szxytkj.cn

PHP:  if (!$data) { return; }
来源：http://ga.shtwfgs.cn

JS:   if (!data) return;
来源：http://sf.521024.cn

TS:   if (!data) return;
来源：http://ti.hahajie.cn

Java: if (data == null) return;
来源：http://bs.shxzukj.cn

Go:   if data == nil { return }
来源：http://rc.bookmarksfly.cn

Ruby: return if data.nil?
来源：http://nr.nicolike.cn

C#:   if (data == null) return;
来源：http://hb.nszjky.cn

================================================================================
来源：http://bj.yuntaijiaju.cn

C. 函数与作用域
来源：http://kh.gzmigu.cn

================================================================================
来源：http://fr.hnjuh.cn

[C01] 定义函数
来源：http://dt.gzmigu.cn

Py:   def add(a, b): return a + b
来源：http://fw.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xw.huixiangedu.cn

JS:   function add(a, b) { return a + b; }
来源：http://jo.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xs.hahajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://kf.wgjwhj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mp.shtwfgs.cn

Ruby: def add(a, b); a + b; end
来源：http://kh.nicolike.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ur.panjiajie.cn

[C02] 默认参数
来源：http://sh.newstarts.cn

Py:   def greet(name="World"): return name
来源：http://fo.panjiajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://mz.panjiajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://px.9csxet.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qy.jctech888.com.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wt.huixinmuqiang.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lf.panjiajie.cn

Ruby: def greet(name = "World") = name
来源：http://kn.colortex.cn

C#:   string Greet(string name = "World") => name;
来源：http://ya.9csxet.cn

[C03] 可变参数
来源：http://uy.shtwfgs.cn

Py:   def total(*args): return sum(args)
来源：http://bv.shxzukj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bo.yuntaijiaju.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ea.jctech888.com.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wh.huixinmuqiang.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vk.huixiangedu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yf.huixiangedu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ln.bookmarksfly.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yg.yuntaijiaju.cn

[C04] 命名参数 / 关键字参数
来源：http://os.shxzskj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gr.newstarts.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zm.yuexingan06.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ll.521024.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ci.yuntaijiaju.cn

Java: // 无：用 Builder 模式或 record
来源：http://td.chemitech.net.cn

Go:   // 无：用配置结构体参数
来源：http://bo.bookmarksfly.cn

Ruby: f(a: 1, b: 2)
来源：http://ko.nicolike.cn

C#:   f(a: 1, b: 2)
来源：http://su.huanxung.cn

[C05] 返回多个值
来源：http://pt.gzmigu.cn

Py:   return a, b
来源：http://ds.huixiangedu.cn

PHP:  return [$a, $b];
来源：http://iy.hahajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yu.panjiajie.cn

TS:   return { a, b };
来源：http://aa.521024.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ar.nicolike.cn

Go:   return a, b
来源：http://ne.haigaiapp.cn

Ruby: return a, b
来源：http://iw.shxzukj.cn

C#:   return (a, b);              // ValueTuple
来源：http://aa.wgjwhj.cn

[C06] 匿名函数 / lambda
来源：http://fc.huanxung.cn

Py:   square = lambda x: x * x
来源：http://zi.shxzskj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://tj.9csxet.cn

JS:   const square = x => x * x;
来源：http://hf.gzmigu.cn

TS:   const square = (x: number): number => x * x;
来源：http://ud.huixinmuqiang.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ta.chemitech.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://bn.yuntaijiaju.cn

Ruby: square = ->(x) { x * x }
来源：http://wl.newstarts.cn

C#:   Func<int, int> square = x => x * x;
来源：http://mf.lnxyls.cn

[C07] 把函数作为参数传入
来源：http://mt.jctech888.com.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pn.bjjhwx.cn

PHP:  array_map("strtoupper", $arr);
来源：http://us.nszjky.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gh.yuexingan06.cn

TS:   arr.map(String)
来源：http://jf.szsharing.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cl.bookmarksfly.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rn.521024.cn

Ruby: arr.map(&:upcase)
来源：http://ho.newstarts.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mm.bjjhwx.cn

[C08] 闭包
来源：http://uj.jctech888.com.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vz.bjjhwx.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rf.shxzukj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rc.chemitech.net.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lf.haigaiapp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://id.yuexingan06.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cf.9csxet.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mu.shxzukj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rf.yuntaijiaju.cn

[C09] 递归
来源：http://cg.huanxung.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://st.yuntaijiaju.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gl.wgjwhj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dj.yuntaijiaju.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zj.gzmigu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gq.newstarts.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jj.hahajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xo.newstarts.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dh.9csxet.cn

[C10] 变量作用域
来源：http://qg.hahajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mw.hnjuh.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://by.huanxung.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gw.asd995.cn

TS:   同 JS
来源：http://cj.colortex.cn

Java: 方法内为块级作用域
来源：http://nv.lnxyls.cn

Go:   花括号块级作用域
来源：http://uz.jianghongdianzi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ta.chemitech.net.cn

C#:   块级作用域
来源：http://od.9csxet.cn

[C11] 模块导入与导出
来源：http://vq.panjiajie.cn

Py:   from module import func
来源：http://md.szxytkj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zl.gzmigu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gc.lnxyls.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bn.huixinmuqiang.cn

Java: import java.util.List;
来源：http://rs.jianghongdianzi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sf.9csxet.cn

Ruby: require "json"; require_relative "./util"
来源：http://fs.chemitech.net.cn

C#:   using System.Text;
来源：http://ss.szsharing.cn

[C12] 立即执行函数 IIFE
来源：http://cm.huixiangedu.cn

Py:   (lambda: print("run"))()
来源：http://lx.muxihuayi.cn

PHP:  (function () { echo "run"; })();
来源：http://kj.nicolike.cn

JS:   (() => { console.log("run"); })();
来源：http://dv.asd995.cn

TS:   (() => { console.log("run"); })();
来源：http://ko.lnxyls.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ge.muxihuayi.cn

Go:   func() { fmt.Println("run") }()
来源：http://mv.asd995.cn

Ruby: -> { puts "run" }.call
来源：http://ty.muxihuayi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://md.yuntaijiaju.cn

[C13] 类型声明 / 类型注解
来源：http://cc.bookmarksfly.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vx.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dl.bookmarksfly.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qg.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yv.gzmigu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fk.asd995.cn

Go:   func add(a, b int) int
来源：http://aw.colortex.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tc.hnjuh.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ir.muxihuayi.cn

[C14] 泛型函数
来源：http://pt.nicolike.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ig.panjiajie.cn

PHP:  // 无泛型
来源：http://nb.szxytkj.cn

JS:   // 无泛型
来源：http://ui.jctech888.com.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ip.chemitech.net.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lb.huixiangedu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://se.haigaiapp.cn

Ruby: # 无泛型
来源：http://uy.yuntaijiaju.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xw.nicolike.cn

[C15] 解构 / 展开参数
来源：http://na.521024.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mg.szxytkj.cn

PHP:  [$a, $b] = $pair;
来源：http://ey.huixiangedu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pa.colortex.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qe.szsharing.cn

Java: // 无解构
来源：http://dd.wgjwhj.cn

Go:   // 无解构
来源：http://fc.yuexingan06.cn

Ruby: a, b = pair
来源：http://ey.chemitech.net.cn

C#:   var (a, b) = pair;
来源：http://bh.huanxung.cn

[C16] 函数 / 方法重载
来源：http://yd.chemitech.net.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sf.yuexingan06.cn


<!-- 参考信息 -->