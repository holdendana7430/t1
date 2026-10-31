代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xx.szsharing.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://br.haigaiapp.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://au.jctech888.com.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ba.9csxet.cn

[A26] 类型转换总览
来源：http://fb.chemitech.net.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cm.colortex.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ln.yuexingan06.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://io.shxzukj.cn

TS:   Number() String() Boolean() x as number
来源：http://cl.muxihuayi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://un.huixiangedu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gs.huixiangedu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://xt.haigaiapp.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cw.huanxung.cn

================================================================================
来源：http://gd.huixiangedu.cn

B. 流程控制
来源：http://rt.yuntaijiaju.cn

================================================================================
来源：http://pr.newstarts.cn

[B01] 条件判断 if / else
来源：http://sx.bjjhwx.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://sw.szxytkj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hd.yuntaijiaju.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hs.colortex.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qk.huixiangedu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://jk.hahajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://th.yuntaijiaju.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wo.huanxung.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://by.hahajie.cn

[B02] 多分支 else if / elif
来源：http://jg.shxzukj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ue.huixinmuqiang.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fu.colortex.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cq.haigaiapp.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nb.wgjwhj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lw.asd995.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tc.bookmarksfly.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://sy.asd995.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ik.asd995.cn

[B03] switch / match / case
来源：http://ot.asd995.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dv.colortex.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xp.haigaiapp.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gf.lnxyls.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cq.szsharing.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kb.szxytkj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jz.chemitech.net.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yg.wgjwhj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dp.jctech888.com.cn

[B04] for 计数循环
来源：http://ei.huanxung.cn

Py:   for i in range(10): print(i)
来源：http://uj.bookmarksfly.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pn.huixinmuqiang.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ks.shxzukj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://el.colortex.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ex.yuntaijiaju.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jh.asd995.cn

Ruby: 10.times { |i| puts i }
来源：http://gf.hnjuh.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vo.hnjuh.cn

[B05] 遍历数组 / 列表
来源：http://lv.newstarts.cn

Py:   for item in arr: print(item)
来源：http://ge.chemitech.net.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jp.bjjhwx.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://vb.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xz.colortex.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fr.szsharing.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ld.hnjuh.cn

Ruby: arr.each { |item| puts item }
来源：http://tn.huanxung.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ol.9csxet.cn

[B06] 遍历字典 / 对象
来源：http://fv.hahajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://bv.hahajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vf.wgjwhj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kt.szsharing.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ai.yuntaijiaju.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kg.521024.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lk.9csxet.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pq.wgjwhj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://is.9csxet.cn

[B07] while 循环
来源：http://yp.huixiangedu.cn

Py:   while i < 10: i += 1
来源：http://pa.muxihuayi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://eu.nicolike.cn

JS:   while (i < 10) { i++; }
来源：http://bq.9csxet.cn

TS:   while (i < 10) { i++; }
来源：http://op.bookmarksfly.cn

Java: while (i < 10) { i++; }
来源：http://ol.9csxet.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xl.bookmarksfly.cn

Ruby: while i < 10; i += 1; end
来源：http://pc.jianghongdianzi.cn

C#:   while (i < 10) { i++; }
来源：http://ki.newstarts.cn

[B08] do-while（至少执行一次）
来源：http://zh.yuntaijiaju.cn

Py:   # 无 do-while：用 while True + break
来源：http://gx.hnjuh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ka.colortex.cn

JS:   do { i++; } while (i < 10);
来源：http://ir.huixinmuqiang.cn

TS:   do { i++; } while (i < 10);
来源：http://cs.lnxyls.cn

Java: do { i++; } while (i < 10);
来源：http://yf.jctech888.com.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ok.lnxyls.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ee.chemitech.net.cn

C#:   do { i++; } while (i < 10);
来源：http://qa.szsharing.cn

[B09] break 与 continue
来源：http://wz.newstarts.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hc.shtwfgs.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://oj.gzmigu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cc.nicolike.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yn.huixiangedu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uz.bookmarksfly.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qy.panjiajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pa.9csxet.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://il.bjjhwx.cn

[B10] 遍历同时拿索引
来源：http://vr.colortex.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ed.lnxyls.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://py.nszjky.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vx.jianghongdianzi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://id.9csxet.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lh.chemitech.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mz.yuntaijiaju.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ff.huanxung.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vy.yuexingan06.cn

[B11] 生成数字序列 / 区间
来源：http://mh.szxytkj.cn

Py:   list(range(0, 10, 2))
来源：http://bd.huixinmuqiang.cn

PHP:  range(0, 10, 2);
来源：http://yu.szxytkj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://le.jctech888.com.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uy.muxihuayi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yz.yuexingan06.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pr.yuntaijiaju.cn

Ruby: (0...10).step(2).to_a
来源：http://bh.nicolike.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dh.huixiangedu.cn

[B12] 跳出多层循环
来源：http://ho.szxytkj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://rw.bookmarksfly.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hx.shtwfgs.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kr.huixiangedu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qn.9csxet.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ie.panjiajie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kw.gzmigu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kh.shtwfgs.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gl.9csxet.cn

[B13] 判断是否为数字
来源：http://mh.jctech888.com.cn

Py:   isinstance(x, (int, float))
来源：http://lq.colortex.cn

PHP:  is_numeric($x)
来源：http://fp.jianghongdianzi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vm.bjjhwx.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zf.huanxung.cn

Java: x instanceof Number
来源：http://cn.chemitech.net.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zb.yuexingan06.cn

Ruby: x.is_a?(Numeric)
来源：http://wn.lnxyls.cn

C#:   x is int or double or decimal
来源：http://vs.huixiangedu.cn

[B14] 判断值是否在集合内
来源：http://ov.huixinmuqiang.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bq.asd995.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bv.yuexingan06.cn

JS:   [1, 2, 3].includes(x)
来源：http://jt.shxzskj.cn

TS:   [1, 2, 3].includes(x)
来源：http://av.muxihuayi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://fp.nszjky.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ao.9csxet.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gn.hahajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://oq.nicolike.cn

[B15] 布尔运算与取反
来源：http://oq.newstarts.cn

Py:   a and b or not c
来源：http://cx.hahajie.cn

PHP:  $a && $b || !$c
来源：http://np.yuexingan06.cn

JS:   a && b || !c
来源：http://bg.jianghongdianzi.cn

TS:   a && b || !c
来源：http://wa.bookmarksfly.cn

Java: a && b || !c
来源：http://pt.asd995.cn

Go:   a && b || !c
来源：http://wx.colortex.cn

Ruby: a && b || !c
来源：http://bv.shxzskj.cn

C#:   a && b || !c
来源：http://pk.jianghongdianzi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ye.hahajie.cn

Py:   if not data: return
来源：http://zm.wgjwhj.cn

PHP:  if (!$data) { return; }
来源：http://qg.gzmigu.cn

JS:   if (!data) return;
来源：http://jj.huixinmuqiang.cn

TS:   if (!data) return;
来源：http://cw.muxihuayi.cn

Java: if (data == null) return;
来源：http://nr.lnxyls.cn

Go:   if data == nil { return }
来源：http://ai.huanxung.cn

Ruby: return if data.nil?
来源：http://px.bjjhwx.cn

C#:   if (data == null) return;
来源：http://ae.panjiajie.cn

================================================================================
来源：http://gw.jctech888.com.cn

C. 函数与作用域
来源：http://uk.shxzukj.cn

================================================================================
来源：http://qs.hahajie.cn

[C01] 定义函数
来源：http://kq.panjiajie.cn

Py:   def add(a, b): return a + b
来源：http://ov.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ht.bookmarksfly.cn

JS:   function add(a, b) { return a + b; }
来源：http://zu.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wx.yuntaijiaju.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bm.gzmigu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xn.wgjwhj.cn

Ruby: def add(a, b); a + b; end
来源：http://gs.huixinmuqiang.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mf.newstarts.cn

[C02] 默认参数
来源：http://bg.wgjwhj.cn

Py:   def greet(name="World"): return name
来源：http://ey.muxihuayi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://au.muxihuayi.cn

JS:   function greet(name = "World") { return name; }
来源：http://re.szsharing.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://pd.shxzukj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://uf.lnxyls.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xz.huixiangedu.cn

Ruby: def greet(name = "World") = name
来源：http://mu.huanxung.cn

C#:   string Greet(string name = "World") => name;
来源：http://gu.yuexingan06.cn

[C03] 可变参数
来源：http://mw.yuexingan06.cn

Py:   def total(*args): return sum(args)
来源：http://mo.panjiajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xc.nszjky.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://am.bookmarksfly.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dy.haigaiapp.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ak.huixiangedu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xi.huixinmuqiang.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xd.haigaiapp.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qt.colortex.cn

[C04] 命名参数 / 关键字参数
来源：http://uy.shtwfgs.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kr.newstarts.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zi.haigaiapp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tp.colortex.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qe.hahajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://xa.szsharing.cn

Go:   // 无：用配置结构体参数
来源：http://li.yuexingan06.cn

Ruby: f(a: 1, b: 2)
来源：http://xp.lnxyls.cn

C#:   f(a: 1, b: 2)
来源：http://ji.panjiajie.cn

[C05] 返回多个值
来源：http://wu.haigaiapp.cn

Py:   return a, b
来源：http://se.521024.cn

PHP:  return [$a, $b];
来源：http://yl.szsharing.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ir.nszjky.cn

TS:   return { a, b };
来源：http://hy.szsharing.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qg.colortex.cn

Go:   return a, b
来源：http://nt.huixinmuqiang.cn

Ruby: return a, b
来源：http://rr.hnjuh.cn

C#:   return (a, b);              // ValueTuple
来源：http://ij.nicolike.cn

[C06] 匿名函数 / lambda
来源：http://mb.521024.cn

Py:   square = lambda x: x * x
来源：http://yq.hahajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://gl.chemitech.net.cn

JS:   const square = x => x * x;
来源：http://ye.muxihuayi.cn

TS:   const square = (x: number): number => x * x;
来源：http://lx.nicolike.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lk.hnjuh.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ok.szxytkj.cn

Ruby: square = ->(x) { x * x }
来源：http://ly.jianghongdianzi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://gh.jctech888.com.cn

[C07] 把函数作为参数传入
来源：http://km.nszjky.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ok.szxytkj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://mf.haigaiapp.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cj.huanxung.cn

TS:   arr.map(String)
来源：http://fm.nszjky.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vj.shxzskj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ta.jctech888.com.cn

Ruby: arr.map(&:upcase)
来源：http://mu.panjiajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://zx.asd995.cn

[C08] 闭包
来源：http://yg.szxytkj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ep.wgjwhj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pf.huanxung.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kk.nszjky.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://di.huanxung.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vk.huixinmuqiang.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hv.wgjwhj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mv.asd995.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kg.bjjhwx.cn

[C09] 递归
来源：http://ms.asd995.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nr.bjjhwx.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wn.huanxung.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bs.huanxung.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zi.gzmigu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vo.521024.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nr.huixiangedu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qp.521024.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ot.newstarts.cn

[C10] 变量作用域
来源：http://ln.bjjhwx.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yu.szxytkj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hm.asd995.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cq.lnxyls.cn

TS:   同 JS
来源：http://ok.nicolike.cn

Java: 方法内为块级作用域
来源：http://hw.hahajie.cn

Go:   花括号块级作用域
来源：http://gb.asd995.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yj.wgjwhj.cn

C#:   块级作用域
来源：http://sh.nicolike.cn

[C11] 模块导入与导出
来源：http://rp.yuntaijiaju.cn

Py:   from module import func
来源：http://jm.bjjhwx.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://lb.bjjhwx.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jn.haigaiapp.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qb.bjjhwx.cn

Java: import java.util.List;
来源：http://mq.yuntaijiaju.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pr.newstarts.cn

Ruby: require "json"; require_relative "./util"
来源：http://pe.muxihuayi.cn

C#:   using System.Text;
来源：http://mu.shxzskj.cn

[C12] 立即执行函数 IIFE
来源：http://iw.shxzukj.cn

Py:   (lambda: print("run"))()
来源：http://du.asd995.cn

PHP:  (function () { echo "run"; })();
来源：http://xm.szsharing.cn

JS:   (() => { console.log("run"); })();
来源：http://qb.haigaiapp.cn

TS:   (() => { console.log("run"); })();
来源：http://ur.huixiangedu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fg.gzmigu.cn

Go:   func() { fmt.Println("run") }()
来源：http://bq.huixiangedu.cn

Ruby: -> { puts "run" }.call
来源：http://qh.muxihuayi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jw.haigaiapp.cn

[C13] 类型声明 / 类型注解
来源：http://dq.nszjky.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://os.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fm.panjiajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://oa.yuexingan06.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rm.bookmarksfly.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cu.huixiangedu.cn

Go:   func add(a, b int) int
来源：http://fl.bookmarksfly.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pm.bjjhwx.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ne.bjjhwx.cn

[C14] 泛型函数
来源：http://fs.asd995.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nl.shtwfgs.cn

PHP:  // 无泛型
来源：http://zz.haigaiapp.cn

JS:   // 无泛型
来源：http://kh.bookmarksfly.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hk.yuexingan06.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uf.szsharing.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qs.yuexingan06.cn

Ruby: # 无泛型
来源：http://mw.huanxung.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ck.huanxung.cn

[C15] 解构 / 展开参数
来源：http://yc.asd995.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ot.szsharing.cn

PHP:  [$a, $b] = $pair;
来源：http://no.bjjhwx.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fl.asd995.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://am.521024.cn

Java: // 无解构
来源：http://bk.bjjhwx.cn

Go:   // 无解构
来源：http://qo.gzmigu.cn

Ruby: a, b = pair
来源：http://or.huanxung.cn

C#:   var (a, b) = pair;
来源：http://zm.chemitech.net.cn

[C16] 函数 / 方法重载
来源：http://ou.9csxet.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fx.lnxyls.cn


<!-- 参考信息 -->