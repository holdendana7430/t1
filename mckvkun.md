代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://on.lnxyls.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bb.yuntaijiaju.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ri.newstarts.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://eo.wgjwhj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mm.521024.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://uk.chemitech.net.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://xw.asd995.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://is.yuntaijiaju.cn

[A26] 类型转换总览
来源：http://nn.gzmigu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wb.shtwfgs.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fw.huixiangedu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wq.colortex.cn

TS:   Number() String() Boolean() x as number
来源：http://af.jctech888.com.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ww.wgjwhj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ea.asd995.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://cq.huixiangedu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ur.jianghongdianzi.cn

================================================================================
来源：http://nu.bjjhwx.cn

B. 流程控制
来源：http://tz.nicolike.cn

================================================================================
来源：http://ly.bjjhwx.cn

[B01] 条件判断 if / else
来源：http://rw.muxihuayi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://uy.colortex.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rb.yuexingan06.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://od.nszjky.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lt.jctech888.com.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://fu.asd995.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ih.yuexingan06.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ab.colortex.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hy.lnxyls.cn

[B02] 多分支 else if / elif
来源：http://wc.wgjwhj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sf.chemitech.net.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ot.shxzskj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ew.bookmarksfly.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jp.jctech888.com.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bh.jctech888.com.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wa.yuexingan06.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ha.9csxet.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pj.szxytkj.cn

[B03] switch / match / case
来源：http://xs.gzmigu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lr.hnjuh.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://an.lnxyls.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ve.wgjwhj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qt.szxytkj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rp.wgjwhj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ky.huixinmuqiang.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zy.521024.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://af.huixinmuqiang.cn

[B04] for 计数循环
来源：http://ec.521024.cn

Py:   for i in range(10): print(i)
来源：http://rs.nicolike.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mo.shxzukj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fz.asd995.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ho.haigaiapp.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://oj.hnjuh.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cw.bjjhwx.cn

Ruby: 10.times { |i| puts i }
来源：http://yw.szsharing.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jp.szsharing.cn

[B05] 遍历数组 / 列表
来源：http://ld.shtwfgs.cn

Py:   for item in arr: print(item)
来源：http://sx.chemitech.net.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vb.nszjky.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://sg.haigaiapp.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bd.colortex.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fq.nicolike.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rx.hahajie.cn

Ruby: arr.each { |item| puts item }
来源：http://ap.shtwfgs.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ci.newstarts.cn

[B06] 遍历字典 / 对象
来源：http://ue.szsharing.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hn.huixiangedu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ut.yuntaijiaju.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://if.panjiajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://di.wgjwhj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wm.newstarts.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ab.9csxet.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ep.huixiangedu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bp.gzmigu.cn

[B07] while 循环
来源：http://yr.bjjhwx.cn

Py:   while i < 10: i += 1
来源：http://xs.nszjky.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xf.bookmarksfly.cn

JS:   while (i < 10) { i++; }
来源：http://xs.9csxet.cn

TS:   while (i < 10) { i++; }
来源：http://fc.colortex.cn

Java: while (i < 10) { i++; }
来源：http://lf.szsharing.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ks.nszjky.cn

Ruby: while i < 10; i += 1; end
来源：http://vb.9csxet.cn

C#:   while (i < 10) { i++; }
来源：http://ja.asd995.cn

[B08] do-while（至少执行一次）
来源：http://tx.hahajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://qd.chemitech.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vj.lnxyls.cn

JS:   do { i++; } while (i < 10);
来源：http://ei.jianghongdianzi.cn

TS:   do { i++; } while (i < 10);
来源：http://no.shxzukj.cn

Java: do { i++; } while (i < 10);
来源：http://gl.hahajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://nd.wgjwhj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ba.haigaiapp.cn

C#:   do { i++; } while (i < 10);
来源：http://im.521024.cn

[B09] break 与 continue
来源：http://jm.asd995.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://of.huixiangedu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ml.wgjwhj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rg.gzmigu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ki.nicolike.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jf.colortex.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gt.hahajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xo.nszjky.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bz.newstarts.cn

[B10] 遍历同时拿索引
来源：http://oh.huixiangedu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xe.huixiangedu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qt.lnxyls.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ti.shxzskj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cc.shtwfgs.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://oo.huixinmuqiang.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dd.newstarts.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tf.shxzukj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xt.nicolike.cn

[B11] 生成数字序列 / 区间
来源：http://lk.muxihuayi.cn

Py:   list(range(0, 10, 2))
来源：http://kf.huixinmuqiang.cn

PHP:  range(0, 10, 2);
来源：http://om.521024.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rl.huixinmuqiang.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pi.bjjhwx.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wp.shxzskj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://si.9csxet.cn

Ruby: (0...10).step(2).to_a
来源：http://vy.colortex.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uv.shxzskj.cn

[B12] 跳出多层循环
来源：http://mk.hnjuh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ve.gzmigu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fv.hnjuh.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mu.9csxet.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ck.gzmigu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hj.bjjhwx.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://aj.nicolike.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://os.shtwfgs.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://oy.haigaiapp.cn

[B13] 判断是否为数字
来源：http://uv.bjjhwx.cn

Py:   isinstance(x, (int, float))
来源：http://yv.bookmarksfly.cn

PHP:  is_numeric($x)
来源：http://eh.chemitech.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jm.jctech888.com.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://st.yuntaijiaju.cn

Java: x instanceof Number
来源：http://dl.wgjwhj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vc.yuexingan06.cn

Ruby: x.is_a?(Numeric)
来源：http://bn.chemitech.net.cn

C#:   x is int or double or decimal
来源：http://sw.bookmarksfly.cn

[B14] 判断值是否在集合内
来源：http://pt.lnxyls.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kg.asd995.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ai.hahajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://ip.szxytkj.cn

TS:   [1, 2, 3].includes(x)
来源：http://zy.9csxet.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://it.nszjky.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ks.bjjhwx.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qs.bjjhwx.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hp.nicolike.cn

[B15] 布尔运算与取反
来源：http://lg.hahajie.cn

Py:   a and b or not c
来源：http://cd.wgjwhj.cn

PHP:  $a && $b || !$c
来源：http://zh.521024.cn

JS:   a && b || !c
来源：http://gz.huanxung.cn

TS:   a && b || !c
来源：http://ps.asd995.cn

Java: a && b || !c
来源：http://ts.huixiangedu.cn

Go:   a && b || !c
来源：http://kc.asd995.cn

Ruby: a && b || !c
来源：http://lg.huixiangedu.cn

C#:   a && b || !c
来源：http://fl.9csxet.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ay.huanxung.cn

Py:   if not data: return
来源：http://aj.hahajie.cn

PHP:  if (!$data) { return; }
来源：http://yv.9csxet.cn

JS:   if (!data) return;
来源：http://cp.panjiajie.cn

TS:   if (!data) return;
来源：http://uw.shxzskj.cn

Java: if (data == null) return;
来源：http://ar.huixinmuqiang.cn

Go:   if data == nil { return }
来源：http://xn.bjjhwx.cn

Ruby: return if data.nil?
来源：http://vw.colortex.cn

C#:   if (data == null) return;
来源：http://kp.yuntaijiaju.cn

================================================================================
来源：http://jd.chemitech.net.cn

C. 函数与作用域
来源：http://fl.shxzskj.cn

================================================================================
来源：http://xc.521024.cn

[C01] 定义函数
来源：http://cj.shtwfgs.cn

Py:   def add(a, b): return a + b
来源：http://yo.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mt.hahajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://wk.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ba.9csxet.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://jz.lnxyls.cn

Go:   func add(a, b int) int { return a + b }
来源：http://sa.yuexingan06.cn

Ruby: def add(a, b); a + b; end
来源：http://zb.shxzskj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://he.szsharing.cn

[C02] 默认参数
来源：http://lw.9csxet.cn

Py:   def greet(name="World"): return name
来源：http://zj.szxytkj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fq.yuntaijiaju.cn

JS:   function greet(name = "World") { return name; }
来源：http://uz.hnjuh.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://mg.hnjuh.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ea.panjiajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zv.szxytkj.cn

Ruby: def greet(name = "World") = name
来源：http://se.bjjhwx.cn

C#:   string Greet(string name = "World") => name;
来源：http://nw.szxytkj.cn

[C03] 可变参数
来源：http://nt.yuexingan06.cn

Py:   def total(*args): return sum(args)
来源：http://fv.bookmarksfly.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xg.yuexingan06.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jg.shxzskj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ki.wgjwhj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ny.jianghongdianzi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xa.huixiangedu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://nr.lnxyls.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cn.nicolike.cn

[C04] 命名参数 / 关键字参数
来源：http://bs.nszjky.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vc.newstarts.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ok.hnjuh.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lr.hnjuh.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://if.yuntaijiaju.cn

Java: // 无：用 Builder 模式或 record
来源：http://zl.nicolike.cn

Go:   // 无：用配置结构体参数
来源：http://tg.newstarts.cn

Ruby: f(a: 1, b: 2)
来源：http://bg.shxzskj.cn

C#:   f(a: 1, b: 2)
来源：http://pe.hahajie.cn

[C05] 返回多个值
来源：http://dm.gzmigu.cn

Py:   return a, b
来源：http://bk.yuntaijiaju.cn

PHP:  return [$a, $b];
来源：http://gq.nszjky.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://al.huanxung.cn

TS:   return { a, b };
来源：http://cc.colortex.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rj.huixinmuqiang.cn

Go:   return a, b
来源：http://zw.huixinmuqiang.cn

Ruby: return a, b
来源：http://zm.jianghongdianzi.cn

C#:   return (a, b);              // ValueTuple
来源：http://jb.huixinmuqiang.cn

[C06] 匿名函数 / lambda
来源：http://di.haigaiapp.cn

Py:   square = lambda x: x * x
来源：http://dw.hahajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://cm.huixinmuqiang.cn

JS:   const square = x => x * x;
来源：http://ks.huanxung.cn

TS:   const square = (x: number): number => x * x;
来源：http://qx.lnxyls.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sy.yuntaijiaju.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ot.haigaiapp.cn

Ruby: square = ->(x) { x * x }
来源：http://py.shtwfgs.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zr.wgjwhj.cn

[C07] 把函数作为参数传入
来源：http://cv.nicolike.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jy.panjiajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ut.muxihuayi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://el.nszjky.cn

TS:   arr.map(String)
来源：http://lg.521024.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rc.huixiangedu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nb.gzmigu.cn

Ruby: arr.map(&:upcase)
来源：http://mi.haigaiapp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://lk.jctech888.com.cn

[C08] 闭包
来源：http://pe.haigaiapp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ub.hnjuh.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kw.521024.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hm.nicolike.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cy.9csxet.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zd.panjiajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mq.shtwfgs.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mf.gzmigu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jm.shxzskj.cn

[C09] 递归
来源：http://mq.colortex.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nj.hahajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ri.yuntaijiaju.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://od.nicolike.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vt.newstarts.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bz.shtwfgs.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ta.nicolike.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ij.nszjky.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ui.521024.cn

[C10] 变量作用域
来源：http://eh.huixiangedu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wb.shtwfgs.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ph.shxzukj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gy.nszjky.cn

TS:   同 JS
来源：http://oa.wgjwhj.cn

Java: 方法内为块级作用域
来源：http://xa.9csxet.cn

Go:   花括号块级作用域
来源：http://sp.huanxung.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hx.szsharing.cn

C#:   块级作用域
来源：http://wv.nicolike.cn

[C11] 模块导入与导出
来源：http://ji.wgjwhj.cn

Py:   from module import func
来源：http://uf.hahajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://fp.shxzukj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://wn.huixinmuqiang.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xn.yuexingan06.cn

Java: import java.util.List;
来源：http://jd.gzmigu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bl.wgjwhj.cn

Ruby: require "json"; require_relative "./util"
来源：http://if.huixiangedu.cn

C#:   using System.Text;
来源：http://rn.haigaiapp.cn

[C12] 立即执行函数 IIFE
来源：http://wu.huixiangedu.cn

Py:   (lambda: print("run"))()
来源：http://bu.shxzukj.cn

PHP:  (function () { echo "run"; })();
来源：http://ov.shtwfgs.cn

JS:   (() => { console.log("run"); })();
来源：http://wb.huanxung.cn

TS:   (() => { console.log("run"); })();
来源：http://oz.yuexingan06.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nk.521024.cn

Go:   func() { fmt.Println("run") }()
来源：http://pp.nicolike.cn

Ruby: -> { puts "run" }.call
来源：http://wg.colortex.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://iy.hnjuh.cn

[C13] 类型声明 / 类型注解
来源：http://dm.nicolike.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://uw.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pq.bjjhwx.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ik.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mh.huanxung.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mt.shxzukj.cn

Go:   func add(a, b int) int
来源：http://ip.lnxyls.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gj.panjiajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://uk.newstarts.cn

[C14] 泛型函数
来源：http://yt.jctech888.com.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hx.9csxet.cn

PHP:  // 无泛型
来源：http://mx.chemitech.net.cn

JS:   // 无泛型
来源：http://mu.9csxet.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mk.muxihuayi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gm.shxzukj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ro.shxzukj.cn

Ruby: # 无泛型
来源：http://zr.hnjuh.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://uz.hahajie.cn

[C15] 解构 / 展开参数
来源：http://vg.jianghongdianzi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pv.wgjwhj.cn

PHP:  [$a, $b] = $pair;
来源：http://gd.jctech888.com.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://co.nicolike.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dz.szsharing.cn

Java: // 无解构
来源：http://xp.shxzskj.cn

Go:   // 无解构
来源：http://mr.jianghongdianzi.cn


<!-- 参考信息 -->