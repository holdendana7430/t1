代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://op.hnjuh.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nm.hnjuh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rh.hnjuh.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pt.colortex.cn

[A26] 类型转换总览
来源：http://lv.huixinmuqiang.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mc.huanxung.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vo.jianghongdianzi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xq.nicolike.cn

TS:   Number() String() Boolean() x as number
来源：http://ue.muxihuayi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zl.gzmigu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dt.wgjwhj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ie.muxihuayi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gg.nicolike.cn

================================================================================
来源：http://ol.wgjwhj.cn

B. 流程控制
来源：http://ul.521024.cn

================================================================================
来源：http://cm.shxzskj.cn

[B01] 条件判断 if / else
来源：http://oj.lnxyls.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://rp.shtwfgs.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wq.szxytkj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://em.huanxung.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wg.newstarts.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://nt.nszjky.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mn.shxzukj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pv.asd995.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wl.muxihuayi.cn

[B02] 多分支 else if / elif
来源：http://en.panjiajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sf.panjiajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sk.shxzskj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://at.szsharing.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jb.nszjky.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yh.nicolike.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hs.nszjky.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pn.szsharing.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ct.bookmarksfly.cn

[B03] switch / match / case
来源：http://fa.nicolike.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ez.nicolike.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://di.wgjwhj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vy.yuexingan06.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zf.bookmarksfly.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://iq.colortex.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hs.hahajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tr.chemitech.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nu.lnxyls.cn

[B04] for 计数循环
来源：http://bf.yuexingan06.cn

Py:   for i in range(10): print(i)
来源：http://nr.521024.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://is.huanxung.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tb.shxzukj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tx.asd995.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ww.asd995.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://da.yuexingan06.cn

Ruby: 10.times { |i| puts i }
来源：http://fv.521024.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pb.hahajie.cn

[B05] 遍历数组 / 列表
来源：http://ga.huixinmuqiang.cn

Py:   for item in arr: print(item)
来源：http://xz.huixiangedu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bj.huixinmuqiang.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ig.newstarts.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ab.jianghongdianzi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://oy.huanxung.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ur.asd995.cn

Ruby: arr.each { |item| puts item }
来源：http://cg.nicolike.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uw.jctech888.com.cn

[B06] 遍历字典 / 对象
来源：http://ez.newstarts.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://bd.colortex.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dh.colortex.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bd.jctech888.com.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yx.huanxung.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rl.szsharing.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vw.jctech888.com.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kv.hnjuh.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://so.jctech888.com.cn

[B07] while 循环
来源：http://ho.shxzukj.cn

Py:   while i < 10: i += 1
来源：http://xu.haigaiapp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://iv.hnjuh.cn

JS:   while (i < 10) { i++; }
来源：http://yx.jctech888.com.cn

TS:   while (i < 10) { i++; }
来源：http://mi.gzmigu.cn

Java: while (i < 10) { i++; }
来源：http://jf.yuntaijiaju.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hg.colortex.cn

Ruby: while i < 10; i += 1; end
来源：http://tq.asd995.cn

C#:   while (i < 10) { i++; }
来源：http://jw.shtwfgs.cn

[B08] do-while（至少执行一次）
来源：http://bm.muxihuayi.cn

Py:   # 无 do-while：用 while True + break
来源：http://dx.colortex.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ou.yuexingan06.cn

JS:   do { i++; } while (i < 10);
来源：http://tq.hnjuh.cn

TS:   do { i++; } while (i < 10);
来源：http://lu.gzmigu.cn

Java: do { i++; } while (i < 10);
来源：http://xv.huixinmuqiang.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://iy.newstarts.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rk.nicolike.cn

C#:   do { i++; } while (i < 10);
来源：http://so.shxzukj.cn

[B09] break 与 continue
来源：http://kr.panjiajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wv.newstarts.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ye.bjjhwx.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bd.bjjhwx.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ts.panjiajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ve.hnjuh.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kp.jctech888.com.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jd.jctech888.com.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sf.huixinmuqiang.cn

[B10] 遍历同时拿索引
来源：http://fq.nszjky.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xk.newstarts.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pl.bjjhwx.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pw.lnxyls.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mr.szxytkj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ev.panjiajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lh.panjiajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yz.nicolike.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cc.9csxet.cn

[B11] 生成数字序列 / 区间
来源：http://rf.521024.cn

Py:   list(range(0, 10, 2))
来源：http://ev.newstarts.cn

PHP:  range(0, 10, 2);
来源：http://bj.panjiajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ss.hahajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ls.jianghongdianzi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ww.nszjky.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cs.gzmigu.cn

Ruby: (0...10).step(2).to_a
来源：http://hn.chemitech.net.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jy.nszjky.cn

[B12] 跳出多层循环
来源：http://xk.muxihuayi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xl.521024.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://eh.nszjky.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fm.gzmigu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://do.haigaiapp.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ik.huixiangedu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xg.gzmigu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dd.szsharing.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dg.nszjky.cn

[B13] 判断是否为数字
来源：http://yh.shxzukj.cn

Py:   isinstance(x, (int, float))
来源：http://qo.asd995.cn

PHP:  is_numeric($x)
来源：http://jz.chemitech.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dk.shxzukj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wh.bjjhwx.cn

Java: x instanceof Number
来源：http://pi.nszjky.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bc.muxihuayi.cn

Ruby: x.is_a?(Numeric)
来源：http://il.jianghongdianzi.cn

C#:   x is int or double or decimal
来源：http://mw.bjjhwx.cn

[B14] 判断值是否在集合内
来源：http://on.9csxet.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fe.bjjhwx.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hu.chemitech.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://xr.szxytkj.cn

TS:   [1, 2, 3].includes(x)
来源：http://pv.gzmigu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xu.colortex.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yo.huixiangedu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://of.huixinmuqiang.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ow.panjiajie.cn

[B15] 布尔运算与取反
来源：http://hf.jctech888.com.cn

Py:   a and b or not c
来源：http://xp.chemitech.net.cn

PHP:  $a && $b || !$c
来源：http://mx.bjjhwx.cn

JS:   a && b || !c
来源：http://cx.szsharing.cn

TS:   a && b || !c
来源：http://wh.bookmarksfly.cn

Java: a && b || !c
来源：http://rs.newstarts.cn

Go:   a && b || !c
来源：http://hz.yuexingan06.cn

Ruby: a && b || !c
来源：http://ir.9csxet.cn

C#:   a && b || !c
来源：http://gr.huixinmuqiang.cn

[B16] 卫语句：不满足条件提前返回
来源：http://tm.nicolike.cn

Py:   if not data: return
来源：http://yd.wgjwhj.cn

PHP:  if (!$data) { return; }
来源：http://wq.521024.cn

JS:   if (!data) return;
来源：http://ms.jctech888.com.cn

TS:   if (!data) return;
来源：http://qx.nszjky.cn

Java: if (data == null) return;
来源：http://sg.shxzukj.cn

Go:   if data == nil { return }
来源：http://cr.newstarts.cn

Ruby: return if data.nil?
来源：http://xm.shxzukj.cn

C#:   if (data == null) return;
来源：http://ii.wgjwhj.cn

================================================================================
来源：http://zy.szxytkj.cn

C. 函数与作用域
来源：http://zt.chemitech.net.cn

================================================================================
来源：http://xi.newstarts.cn

[C01] 定义函数
来源：http://mm.gzmigu.cn

Py:   def add(a, b): return a + b
来源：http://pg.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bd.panjiajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://vb.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fk.huanxung.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://yq.colortex.cn

Go:   func add(a, b int) int { return a + b }
来源：http://um.bookmarksfly.cn

Ruby: def add(a, b); a + b; end
来源：http://xe.newstarts.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sj.haigaiapp.cn

[C02] 默认参数
来源：http://hm.jianghongdianzi.cn

Py:   def greet(name="World"): return name
来源：http://pg.huanxung.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qf.shtwfgs.cn

JS:   function greet(name = "World") { return name; }
来源：http://sl.haigaiapp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hd.colortex.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ap.huixiangedu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rj.jctech888.com.cn

Ruby: def greet(name = "World") = name
来源：http://fc.szsharing.cn

C#:   string Greet(string name = "World") => name;
来源：http://ts.lnxyls.cn

[C03] 可变参数
来源：http://hb.panjiajie.cn

Py:   def total(*args): return sum(args)
来源：http://uv.huanxung.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://oa.szsharing.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kl.bjjhwx.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://in.huixinmuqiang.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ui.hnjuh.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://si.wgjwhj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ts.huanxung.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qt.muxihuayi.cn

[C04] 命名参数 / 关键字参数
来源：http://jk.wgjwhj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hs.yuexingan06.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tb.wgjwhj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qr.jianghongdianzi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qb.szsharing.cn

Java: // 无：用 Builder 模式或 record
来源：http://en.szxytkj.cn

Go:   // 无：用配置结构体参数
来源：http://po.szxytkj.cn

Ruby: f(a: 1, b: 2)
来源：http://tk.muxihuayi.cn

C#:   f(a: 1, b: 2)
来源：http://hu.hnjuh.cn

[C05] 返回多个值
来源：http://jk.panjiajie.cn

Py:   return a, b
来源：http://ca.colortex.cn

PHP:  return [$a, $b];
来源：http://jk.shxzukj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://lr.szxytkj.cn

TS:   return { a, b };
来源：http://nx.jianghongdianzi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gi.asd995.cn

Go:   return a, b
来源：http://cz.gzmigu.cn

Ruby: return a, b
来源：http://fg.huanxung.cn

C#:   return (a, b);              // ValueTuple
来源：http://at.gzmigu.cn

[C06] 匿名函数 / lambda
来源：http://vo.szsharing.cn

Py:   square = lambda x: x * x
来源：http://pv.bookmarksfly.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://sy.jctech888.com.cn

JS:   const square = x => x * x;
来源：http://jf.lnxyls.cn

TS:   const square = (x: number): number => x * x;
来源：http://yu.bjjhwx.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ty.jianghongdianzi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jh.9csxet.cn

Ruby: square = ->(x) { x * x }
来源：http://eu.yuntaijiaju.cn

C#:   Func<int, int> square = x => x * x;
来源：http://se.521024.cn

[C07] 把函数作为参数传入
来源：http://hm.muxihuayi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dk.yuntaijiaju.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kl.521024.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xl.wgjwhj.cn

TS:   arr.map(String)
来源：http://xh.szxytkj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ou.9csxet.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uw.lnxyls.cn

Ruby: arr.map(&:upcase)
来源：http://rx.huixinmuqiang.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://si.colortex.cn

[C08] 闭包
来源：http://lf.huixinmuqiang.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://se.szxytkj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://de.shxzukj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bi.szsharing.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dx.wgjwhj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tx.newstarts.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lb.nszjky.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ct.9csxet.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ee.wgjwhj.cn

[C09] 递归
来源：http://vt.huanxung.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pm.hnjuh.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qn.nicolike.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://om.jctech888.com.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gx.shxzukj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ra.nicolike.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://px.521024.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://er.wgjwhj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jg.panjiajie.cn

[C10] 变量作用域
来源：http://ui.gzmigu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bg.jianghongdianzi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ga.bjjhwx.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ov.newstarts.cn

TS:   同 JS
来源：http://gl.yuexingan06.cn

Java: 方法内为块级作用域
来源：http://is.colortex.cn

Go:   花括号块级作用域
来源：http://du.hnjuh.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rt.nicolike.cn

C#:   块级作用域
来源：http://sj.szxytkj.cn

[C11] 模块导入与导出
来源：http://jd.jianghongdianzi.cn

Py:   from module import func
来源：http://dn.nicolike.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://za.yuexingan06.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ia.yuntaijiaju.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pb.hahajie.cn

Java: import java.util.List;
来源：http://ps.wgjwhj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cp.newstarts.cn

Ruby: require "json"; require_relative "./util"
来源：http://mv.shxzskj.cn

C#:   using System.Text;
来源：http://gr.asd995.cn

[C12] 立即执行函数 IIFE
来源：http://re.huixinmuqiang.cn

Py:   (lambda: print("run"))()
来源：http://np.lnxyls.cn

PHP:  (function () { echo "run"; })();
来源：http://rq.lnxyls.cn

JS:   (() => { console.log("run"); })();
来源：http://ga.jctech888.com.cn

TS:   (() => { console.log("run"); })();
来源：http://uj.jianghongdianzi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hv.521024.cn

Go:   func() { fmt.Println("run") }()
来源：http://us.bookmarksfly.cn

Ruby: -> { puts "run" }.call
来源：http://ua.9csxet.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fn.muxihuayi.cn

[C13] 类型声明 / 类型注解
来源：http://wj.wgjwhj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://py.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qe.asd995.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ie.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://py.newstarts.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ik.9csxet.cn

Go:   func add(a, b int) int
来源：http://rr.szxytkj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://px.szxytkj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vh.shxzskj.cn

[C14] 泛型函数
来源：http://la.521024.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uk.nicolike.cn

PHP:  // 无泛型
来源：http://ck.9csxet.cn

JS:   // 无泛型
来源：http://cf.haigaiapp.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tx.haigaiapp.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://on.nszjky.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ij.jctech888.com.cn

Ruby: # 无泛型
来源：http://qi.521024.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://df.huixinmuqiang.cn

[C15] 解构 / 展开参数
来源：http://az.yuexingan06.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://py.nicolike.cn

PHP:  [$a, $b] = $pair;
来源：http://sc.hnjuh.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ho.9csxet.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tz.hnjuh.cn

Java: // 无解构
来源：http://qx.szxytkj.cn

Go:   // 无解构
来源：http://bq.yuexingan06.cn

Ruby: a, b = pair
来源：http://hv.chemitech.net.cn

C#:   var (a, b) = pair;
来源：http://dl.gzmigu.cn

[C16] 函数 / 方法重载
来源：http://nr.colortex.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kd.jctech888.com.cn


<!-- 参考信息 -->