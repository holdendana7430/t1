代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://lx.huixiangedu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://uu.9csxet.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sf.shxzskj.cn

[A25] 字符串比较
来源：http://tr.shxzskj.cn

Py:   s1 == s2; s1 != s2
来源：http://gm.hahajie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mg.huixiangedu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qc.yuexingan06.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qh.hahajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://it.huixiangedu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ic.lnxyls.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://xc.panjiajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qe.bookmarksfly.cn

[A26] 类型转换总览
来源：http://mt.9csxet.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ao.bjjhwx.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ix.shxzukj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vo.521024.cn

TS:   Number() String() Boolean() x as number
来源：http://zk.bjjhwx.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vq.haigaiapp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tw.newstarts.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://es.newstarts.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hq.nszjky.cn

================================================================================
来源：http://ay.szsharing.cn

B. 流程控制
来源：http://et.szsharing.cn

================================================================================
来源：http://vt.yuntaijiaju.cn

[B01] 条件判断 if / else
来源：http://tn.shxzukj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://zi.jctech888.com.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hk.chemitech.net.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cw.nszjky.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vl.bjjhwx.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://hh.yuntaijiaju.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zs.nicolike.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cf.wgjwhj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cs.jctech888.com.cn

[B02] 多分支 else if / elif
来源：http://yc.colortex.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cl.shtwfgs.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gz.panjiajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hp.haigaiapp.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qy.colortex.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ri.nszjky.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ua.lnxyls.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ks.wgjwhj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ju.nszjky.cn

[B03] switch / match / case
来源：http://cr.newstarts.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://as.521024.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://to.colortex.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vh.bjjhwx.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yw.newstarts.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://eq.chemitech.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ro.521024.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://py.newstarts.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zc.shtwfgs.cn

[B04] for 计数循环
来源：http://ig.panjiajie.cn

Py:   for i in range(10): print(i)
来源：http://tu.chemitech.net.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://so.newstarts.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wz.muxihuayi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ah.chemitech.net.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nj.asd995.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cn.hnjuh.cn

Ruby: 10.times { |i| puts i }
来源：http://pd.panjiajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ux.9csxet.cn

[B05] 遍历数组 / 列表
来源：http://sd.bookmarksfly.cn

Py:   for item in arr: print(item)
来源：http://ac.nszjky.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ds.bjjhwx.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gz.huixiangedu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://cc.haigaiapp.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ha.huixinmuqiang.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ya.huixiangedu.cn

Ruby: arr.each { |item| puts item }
来源：http://dd.muxihuayi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ft.9csxet.cn

[B06] 遍历字典 / 对象
来源：http://bt.nszjky.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://iw.jctech888.com.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://he.asd995.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ab.nicolike.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jj.nszjky.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xz.szxytkj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://in.muxihuayi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ts.colortex.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lr.szsharing.cn

[B07] while 循环
来源：http://na.shxzukj.cn

Py:   while i < 10: i += 1
来源：http://cd.huixiangedu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://dh.shxzukj.cn

JS:   while (i < 10) { i++; }
来源：http://fi.nicolike.cn

TS:   while (i < 10) { i++; }
来源：http://jv.colortex.cn

Java: while (i < 10) { i++; }
来源：http://rr.huixinmuqiang.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vv.bookmarksfly.cn

Ruby: while i < 10; i += 1; end
来源：http://sa.huanxung.cn

C#:   while (i < 10) { i++; }
来源：http://lz.newstarts.cn

[B08] do-while（至少执行一次）
来源：http://ki.hnjuh.cn

Py:   # 无 do-while：用 while True + break
来源：http://fd.9csxet.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zy.huixiangedu.cn

JS:   do { i++; } while (i < 10);
来源：http://ui.chemitech.net.cn

TS:   do { i++; } while (i < 10);
来源：http://uz.bookmarksfly.cn

Java: do { i++; } while (i < 10);
来源：http://we.gzmigu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://uk.shtwfgs.cn

Ruby: begin; i += 1; end while i < 10
来源：http://is.muxihuayi.cn

C#:   do { i++; } while (i < 10);
来源：http://gt.szsharing.cn

[B09] break 与 continue
来源：http://ke.bjjhwx.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://le.gzmigu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jv.hnjuh.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bm.jctech888.com.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qa.shxzskj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://et.haigaiapp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://io.521024.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ig.colortex.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xb.newstarts.cn

[B10] 遍历同时拿索引
来源：http://nr.yuexingan06.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cd.huanxung.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wt.jctech888.com.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rw.newstarts.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ms.huanxung.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bg.nszjky.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jb.newstarts.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ox.9csxet.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ho.huanxung.cn

[B11] 生成数字序列 / 区间
来源：http://ne.shtwfgs.cn

Py:   list(range(0, 10, 2))
来源：http://hr.haigaiapp.cn

PHP:  range(0, 10, 2);
来源：http://hq.hnjuh.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xc.newstarts.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kc.yuntaijiaju.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xv.bookmarksfly.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://be.hnjuh.cn

Ruby: (0...10).step(2).to_a
来源：http://zb.huixinmuqiang.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ks.haigaiapp.cn

[B12] 跳出多层循环
来源：http://lz.nszjky.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://iw.lnxyls.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://iu.nicolike.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zg.shtwfgs.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://eg.wgjwhj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://by.yuntaijiaju.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ys.muxihuayi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://uo.newstarts.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jw.huixiangedu.cn

[B13] 判断是否为数字
来源：http://wz.szxytkj.cn

Py:   isinstance(x, (int, float))
来源：http://sp.521024.cn

PHP:  is_numeric($x)
来源：http://xf.yuexingan06.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ju.9csxet.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ci.jctech888.com.cn

Java: x instanceof Number
来源：http://cl.wgjwhj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pf.huixiangedu.cn

Ruby: x.is_a?(Numeric)
来源：http://ja.bjjhwx.cn

C#:   x is int or double or decimal
来源：http://uz.lnxyls.cn

[B14] 判断值是否在集合内
来源：http://bq.9csxet.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://st.nszjky.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ta.szsharing.cn

JS:   [1, 2, 3].includes(x)
来源：http://ak.szsharing.cn

TS:   [1, 2, 3].includes(x)
来源：http://mt.bjjhwx.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ns.panjiajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://aj.huanxung.cn

Ruby: [1, 2, 3].include?(x)
来源：http://bf.nszjky.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xv.521024.cn

[B15] 布尔运算与取反
来源：http://px.gzmigu.cn

Py:   a and b or not c
来源：http://xq.gzmigu.cn

PHP:  $a && $b || !$c
来源：http://ru.yuexingan06.cn

JS:   a && b || !c
来源：http://qr.colortex.cn

TS:   a && b || !c
来源：http://ch.szsharing.cn

Java: a && b || !c
来源：http://pp.bookmarksfly.cn

Go:   a && b || !c
来源：http://xb.asd995.cn

Ruby: a && b || !c
来源：http://jh.szsharing.cn

C#:   a && b || !c
来源：http://od.9csxet.cn

[B16] 卫语句：不满足条件提前返回
来源：http://em.muxihuayi.cn

Py:   if not data: return
来源：http://bj.yuexingan06.cn

PHP:  if (!$data) { return; }
来源：http://we.jianghongdianzi.cn

JS:   if (!data) return;
来源：http://kr.nicolike.cn

TS:   if (!data) return;
来源：http://wh.jctech888.com.cn

Java: if (data == null) return;
来源：http://cx.jctech888.com.cn

Go:   if data == nil { return }
来源：http://lh.shtwfgs.cn

Ruby: return if data.nil?
来源：http://ee.panjiajie.cn

C#:   if (data == null) return;
来源：http://ug.gzmigu.cn

================================================================================
来源：http://ep.nicolike.cn

C. 函数与作用域
来源：http://ld.nszjky.cn

================================================================================
来源：http://ym.colortex.cn

[C01] 定义函数
来源：http://zs.bookmarksfly.cn

Py:   def add(a, b): return a + b
来源：http://xv.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ov.szsharing.cn

JS:   function add(a, b) { return a + b; }
来源：http://mo.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dt.haigaiapp.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wf.yuexingan06.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ws.lnxyls.cn

Ruby: def add(a, b); a + b; end
来源：http://ko.gzmigu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hh.muxihuayi.cn

[C02] 默认参数
来源：http://mh.shtwfgs.cn

Py:   def greet(name="World"): return name
来源：http://ai.szxytkj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xl.szsharing.cn

JS:   function greet(name = "World") { return name; }
来源：http://ut.jctech888.com.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://nb.lnxyls.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://yd.gzmigu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zi.huanxung.cn

Ruby: def greet(name = "World") = name
来源：http://fo.gzmigu.cn

C#:   string Greet(string name = "World") => name;
来源：http://mx.panjiajie.cn

[C03] 可变参数
来源：http://zk.nszjky.cn

Py:   def total(*args): return sum(args)
来源：http://jj.hnjuh.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dp.lnxyls.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gv.yuntaijiaju.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dy.chemitech.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gy.yuexingan06.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fc.nicolike.cn

Ruby: def total(*nums); nums.sum; end
来源：http://eg.newstarts.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yf.wgjwhj.cn

[C04] 命名参数 / 关键字参数
来源：http://zw.yuexingan06.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nn.521024.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rf.hahajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.szsharing.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qz.szsharing.cn

Java: // 无：用 Builder 模式或 record
来源：http://oo.chemitech.net.cn

Go:   // 无：用配置结构体参数
来源：http://gy.szsharing.cn

Ruby: f(a: 1, b: 2)
来源：http://gl.panjiajie.cn

C#:   f(a: 1, b: 2)
来源：http://bg.yuexingan06.cn

[C05] 返回多个值
来源：http://fv.gzmigu.cn

Py:   return a, b
来源：http://fk.yuexingan06.cn

PHP:  return [$a, $b];
来源：http://jm.huanxung.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qr.wgjwhj.cn

TS:   return { a, b };
来源：http://at.huixinmuqiang.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ec.shxzukj.cn

Go:   return a, b
来源：http://un.lnxyls.cn

Ruby: return a, b
来源：http://cp.chemitech.net.cn

C#:   return (a, b);              // ValueTuple
来源：http://nz.bookmarksfly.cn

[C06] 匿名函数 / lambda
来源：http://oz.szxytkj.cn

Py:   square = lambda x: x * x
来源：http://ia.asd995.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://mb.lnxyls.cn

JS:   const square = x => x * x;
来源：http://dh.hnjuh.cn

TS:   const square = (x: number): number => x * x;
来源：http://df.panjiajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dp.hahajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ii.shxzskj.cn

Ruby: square = ->(x) { x * x }
来源：http://fy.yuntaijiaju.cn

C#:   Func<int, int> square = x => x * x;
来源：http://il.yuntaijiaju.cn

[C07] 把函数作为参数传入
来源：http://hh.huixinmuqiang.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qo.yuntaijiaju.cn

PHP:  array_map("strtoupper", $arr);
来源：http://yr.wgjwhj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gj.nszjky.cn

TS:   arr.map(String)
来源：http://tx.nszjky.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tt.wgjwhj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wx.gzmigu.cn

Ruby: arr.map(&:upcase)
来源：http://wq.yuntaijiaju.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://di.haigaiapp.cn

[C08] 闭包
来源：http://zr.yuntaijiaju.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://go.wgjwhj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fr.shtwfgs.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fr.521024.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ff.panjiajie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hc.bookmarksfly.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fj.shtwfgs.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ws.hnjuh.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mk.shtwfgs.cn

[C09] 递归
来源：http://ns.bookmarksfly.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nm.hahajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ak.521024.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jv.bjjhwx.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pb.hahajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fv.jctech888.com.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uu.bookmarksfly.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ma.huanxung.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xy.hnjuh.cn

[C10] 变量作用域
来源：http://lo.shxzukj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://el.newstarts.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kc.szxytkj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bt.huixinmuqiang.cn

TS:   同 JS
来源：http://mg.shxzskj.cn

Java: 方法内为块级作用域
来源：http://tk.521024.cn

Go:   花括号块级作用域
来源：http://jq.panjiajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gf.bjjhwx.cn

C#:   块级作用域
来源：http://rl.jctech888.com.cn

[C11] 模块导入与导出
来源：http://nj.yuexingan06.cn

Py:   from module import func
来源：http://kb.hnjuh.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xl.szsharing.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://bb.shxzskj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mq.shxzukj.cn

Java: import java.util.List;
来源：http://ok.shtwfgs.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vf.huixiangedu.cn

Ruby: require "json"; require_relative "./util"
来源：http://qx.nicolike.cn

C#:   using System.Text;
来源：http://iy.huixinmuqiang.cn

[C12] 立即执行函数 IIFE
来源：http://fs.shtwfgs.cn

Py:   (lambda: print("run"))()
来源：http://ep.nszjky.cn

PHP:  (function () { echo "run"; })();
来源：http://sa.hnjuh.cn

JS:   (() => { console.log("run"); })();
来源：http://ax.gzmigu.cn

TS:   (() => { console.log("run"); })();
来源：http://ib.hahajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gp.shxzskj.cn

Go:   func() { fmt.Println("run") }()
来源：http://jh.chemitech.net.cn

Ruby: -> { puts "run" }.call
来源：http://yq.huixinmuqiang.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fd.szsharing.cn

[C13] 类型声明 / 类型注解
来源：http://xy.521024.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hs.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ti.muxihuayi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ox.hahajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cf.hnjuh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://dl.521024.cn

Go:   func add(a, b int) int
来源：http://dp.shxzskj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ql.huixinmuqiang.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gs.newstarts.cn

[C14] 泛型函数
来源：http://ix.jctech888.com.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://si.panjiajie.cn

PHP:  // 无泛型
来源：http://qp.jianghongdianzi.cn

JS:   // 无泛型
来源：http://zk.huixinmuqiang.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://py.newstarts.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://li.lnxyls.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mh.yuexingan06.cn

Ruby: # 无泛型
来源：http://yt.jianghongdianzi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fj.lnxyls.cn

[C15] 解构 / 展开参数
来源：http://rp.shxzukj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://uv.gzmigu.cn

PHP:  [$a, $b] = $pair;
来源：http://yh.huixiangedu.cn


<!-- 参考信息 -->