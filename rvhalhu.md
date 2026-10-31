代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://pf.huixiangedu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fm.colortex.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://uw.wgjwhj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ve.bookmarksfly.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wx.huixiangedu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kx.jctech888.com.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://kl.jianghongdianzi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://oo.jianghongdianzi.cn

[A26] 类型转换总览
来源：http://kd.gzmigu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kl.wgjwhj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vr.wgjwhj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://go.521024.cn

TS:   Number() String() Boolean() x as number
来源：http://xw.yuntaijiaju.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wl.lnxyls.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tb.jianghongdianzi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zw.panjiajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kj.shxzskj.cn

================================================================================
来源：http://fl.shxzskj.cn

B. 流程控制
来源：http://ft.bookmarksfly.cn

================================================================================
来源：http://mc.nszjky.cn

[B01] 条件判断 if / else
来源：http://ob.hahajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ot.chemitech.net.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ft.yuexingan06.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xm.gzmigu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wp.jctech888.com.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://yo.asd995.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kr.nszjky.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bn.haigaiapp.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fh.huanxung.cn

[B02] 多分支 else if / elif
来源：http://qc.szxytkj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xn.panjiajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jb.hnjuh.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jp.bjjhwx.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kb.hnjuh.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ls.panjiajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ko.9csxet.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://um.huanxung.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bx.asd995.cn

[B03] switch / match / case
来源：http://uu.yuntaijiaju.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tg.jctech888.com.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nc.colortex.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ci.521024.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yb.shtwfgs.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cw.huixinmuqiang.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kh.huixiangedu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fx.szsharing.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ax.colortex.cn

[B04] for 计数循环
来源：http://bn.szxytkj.cn

Py:   for i in range(10): print(i)
来源：http://cx.hahajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qh.bjjhwx.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iu.hnjuh.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tm.wgjwhj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fh.9csxet.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wc.shxzukj.cn

Ruby: 10.times { |i| puts i }
来源：http://mk.szxytkj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gc.hahajie.cn

[B05] 遍历数组 / 列表
来源：http://pp.huixinmuqiang.cn

Py:   for item in arr: print(item)
来源：http://jx.521024.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zh.hahajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gj.szxytkj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://nd.bookmarksfly.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sy.muxihuayi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cf.panjiajie.cn

Ruby: arr.each { |item| puts item }
来源：http://gn.asd995.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ky.jianghongdianzi.cn

[B06] 遍历字典 / 对象
来源：http://sf.huixinmuqiang.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://lm.shxzukj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zo.gzmigu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ih.yuexingan06.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dt.huanxung.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cf.shtwfgs.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xl.gzmigu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ls.nszjky.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://op.yuexingan06.cn

[B07] while 循环
来源：http://kz.colortex.cn

Py:   while i < 10: i += 1
来源：http://qh.huixiangedu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ws.bookmarksfly.cn

JS:   while (i < 10) { i++; }
来源：http://gn.jctech888.com.cn

TS:   while (i < 10) { i++; }
来源：http://sy.panjiajie.cn

Java: while (i < 10) { i++; }
来源：http://te.huixinmuqiang.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xm.jianghongdianzi.cn

Ruby: while i < 10; i += 1; end
来源：http://zt.szxytkj.cn

C#:   while (i < 10) { i++; }
来源：http://qy.lnxyls.cn

[B08] do-while（至少执行一次）
来源：http://oc.bookmarksfly.cn

Py:   # 无 do-while：用 while True + break
来源：http://qy.szsharing.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mc.yuexingan06.cn

JS:   do { i++; } while (i < 10);
来源：http://sg.colortex.cn

TS:   do { i++; } while (i < 10);
来源：http://nt.9csxet.cn

Java: do { i++; } while (i < 10);
来源：http://fw.yuexingan06.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://dw.bjjhwx.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ha.nicolike.cn

C#:   do { i++; } while (i < 10);
来源：http://go.bjjhwx.cn

[B09] break 与 continue
来源：http://oa.bjjhwx.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://du.jctech888.com.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ge.shtwfgs.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wd.chemitech.net.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nr.9csxet.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ew.huixiangedu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kz.yuntaijiaju.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rp.jctech888.com.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jm.yuntaijiaju.cn

[B10] 遍历同时拿索引
来源：http://kz.asd995.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sl.hnjuh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://oh.521024.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rs.bjjhwx.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vy.bjjhwx.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://eo.hnjuh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://be.shxzukj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fb.lnxyls.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xo.521024.cn

[B11] 生成数字序列 / 区间
来源：http://pf.jctech888.com.cn

Py:   list(range(0, 10, 2))
来源：http://bl.jianghongdianzi.cn

PHP:  range(0, 10, 2);
来源：http://yg.bookmarksfly.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ki.jianghongdianzi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://il.jianghongdianzi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ka.521024.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ks.yuntaijiaju.cn

Ruby: (0...10).step(2).to_a
来源：http://vn.muxihuayi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xc.chemitech.net.cn

[B12] 跳出多层循环
来源：http://tm.jianghongdianzi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hh.wgjwhj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://po.colortex.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qu.szxytkj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jj.hnjuh.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mf.9csxet.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qm.gzmigu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qv.yuntaijiaju.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://go.colortex.cn

[B13] 判断是否为数字
来源：http://tu.bjjhwx.cn

Py:   isinstance(x, (int, float))
来源：http://zz.shtwfgs.cn

PHP:  is_numeric($x)
来源：http://wv.colortex.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nl.wgjwhj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dm.jctech888.com.cn

Java: x instanceof Number
来源：http://nq.hahajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xc.shxzskj.cn

Ruby: x.is_a?(Numeric)
来源：http://if.lnxyls.cn

C#:   x is int or double or decimal
来源：http://iv.nicolike.cn

[B14] 判断值是否在集合内
来源：http://yj.wgjwhj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wp.shtwfgs.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tz.asd995.cn

JS:   [1, 2, 3].includes(x)
来源：http://rv.newstarts.cn

TS:   [1, 2, 3].includes(x)
来源：http://qg.bjjhwx.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://zv.muxihuayi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zi.jctech888.com.cn

Ruby: [1, 2, 3].include?(x)
来源：http://iy.wgjwhj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zv.nicolike.cn

[B15] 布尔运算与取反
来源：http://vd.huixinmuqiang.cn

Py:   a and b or not c
来源：http://lv.nszjky.cn

PHP:  $a && $b || !$c
来源：http://pw.nicolike.cn

JS:   a && b || !c
来源：http://hz.jianghongdianzi.cn

TS:   a && b || !c
来源：http://nc.haigaiapp.cn

Java: a && b || !c
来源：http://ry.muxihuayi.cn

Go:   a && b || !c
来源：http://bx.bookmarksfly.cn

Ruby: a && b || !c
来源：http://gs.wgjwhj.cn

C#:   a && b || !c
来源：http://yu.muxihuayi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jj.nszjky.cn

Py:   if not data: return
来源：http://qr.muxihuayi.cn

PHP:  if (!$data) { return; }
来源：http://il.newstarts.cn

JS:   if (!data) return;
来源：http://ec.muxihuayi.cn

TS:   if (!data) return;
来源：http://kv.jianghongdianzi.cn

Java: if (data == null) return;
来源：http://nh.huanxung.cn

Go:   if data == nil { return }
来源：http://ir.muxihuayi.cn

Ruby: return if data.nil?
来源：http://xy.haigaiapp.cn

C#:   if (data == null) return;
来源：http://mm.shxzskj.cn

================================================================================
来源：http://uz.shxzukj.cn

C. 函数与作用域
来源：http://zp.shxzskj.cn

================================================================================
来源：http://it.jctech888.com.cn

[C01] 定义函数
来源：http://cg.bjjhwx.cn

Py:   def add(a, b): return a + b
来源：http://dk.muxihuayi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gu.bookmarksfly.cn

JS:   function add(a, b) { return a + b; }
来源：http://ay.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dt.yuntaijiaju.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fr.bjjhwx.cn

Go:   func add(a, b int) int { return a + b }
来源：http://eb.haigaiapp.cn

Ruby: def add(a, b); a + b; end
来源：http://hh.huixiangedu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ay.nicolike.cn

[C02] 默认参数
来源：http://ld.shtwfgs.cn

Py:   def greet(name="World"): return name
来源：http://nm.nszjky.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ln.huixiangedu.cn

JS:   function greet(name = "World") { return name; }
来源：http://mc.haigaiapp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wc.jianghongdianzi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zo.muxihuayi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jh.shtwfgs.cn

Ruby: def greet(name = "World") = name
来源：http://bj.szxytkj.cn

C#:   string Greet(string name = "World") => name;
来源：http://br.haigaiapp.cn

[C03] 可变参数
来源：http://qk.newstarts.cn

Py:   def total(*args): return sum(args)
来源：http://cj.shxzskj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kw.yuntaijiaju.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yf.9csxet.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bw.szsharing.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://un.huixinmuqiang.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nz.shtwfgs.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ev.szxytkj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pz.shtwfgs.cn

[C04] 命名参数 / 关键字参数
来源：http://oi.bookmarksfly.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cd.yuexingan06.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cl.jianghongdianzi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://id.muxihuayi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bq.jctech888.com.cn

Java: // 无：用 Builder 模式或 record
来源：http://bv.bookmarksfly.cn

Go:   // 无：用配置结构体参数
来源：http://jk.huixinmuqiang.cn

Ruby: f(a: 1, b: 2)
来源：http://df.521024.cn

C#:   f(a: 1, b: 2)
来源：http://ll.szxytkj.cn

[C05] 返回多个值
来源：http://dh.wgjwhj.cn

Py:   return a, b
来源：http://yi.yuexingan06.cn

PHP:  return [$a, $b];
来源：http://ob.szsharing.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://oh.bookmarksfly.cn

TS:   return { a, b };
来源：http://tw.haigaiapp.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wb.shxzukj.cn

Go:   return a, b
来源：http://ep.muxihuayi.cn

Ruby: return a, b
来源：http://zn.nicolike.cn

C#:   return (a, b);              // ValueTuple
来源：http://ud.wgjwhj.cn

[C06] 匿名函数 / lambda
来源：http://ze.huixiangedu.cn

Py:   square = lambda x: x * x
来源：http://dn.gzmigu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://cr.jctech888.com.cn

JS:   const square = x => x * x;
来源：http://kb.shxzskj.cn

TS:   const square = (x: number): number => x * x;
来源：http://or.chemitech.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ah.newstarts.cn

Go:   sq := func(x int) int { return x * x }
来源：http://za.nszjky.cn

Ruby: square = ->(x) { x * x }
来源：http://si.colortex.cn

C#:   Func<int, int> square = x => x * x;
来源：http://mi.muxihuayi.cn

[C07] 把函数作为参数传入
来源：http://sq.shxzukj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zp.bookmarksfly.cn

PHP:  array_map("strtoupper", $arr);
来源：http://cy.hnjuh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kn.yuexingan06.cn

TS:   arr.map(String)
来源：http://me.bookmarksfly.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wd.521024.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zx.nicolike.cn

Ruby: arr.map(&:upcase)
来源：http://oz.shxzskj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mc.panjiajie.cn

[C08] 闭包
来源：http://uc.huanxung.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gs.shxzskj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bt.hahajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ie.asd995.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xd.nszjky.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xy.szxytkj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ej.hahajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://im.nicolike.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://za.nicolike.cn

[C09] 递归
来源：http://yl.yuntaijiaju.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uo.gzmigu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qs.shxzukj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eg.jianghongdianzi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uh.wgjwhj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mu.haigaiapp.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ao.nszjky.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lh.shxzskj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://re.521024.cn

[C10] 变量作用域
来源：http://kf.shxzskj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pr.wgjwhj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wu.hnjuh.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://um.yuexingan06.cn

TS:   同 JS
来源：http://ow.521024.cn

Java: 方法内为块级作用域
来源：http://ph.wgjwhj.cn

Go:   花括号块级作用域
来源：http://do.wgjwhj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xg.panjiajie.cn

C#:   块级作用域
来源：http://yt.muxihuayi.cn

[C11] 模块导入与导出
来源：http://ug.lnxyls.cn

Py:   from module import func
来源：http://at.shxzukj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://be.huixiangedu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://wr.colortex.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://on.newstarts.cn

Java: import java.util.List;
来源：http://kx.panjiajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cj.bjjhwx.cn

Ruby: require "json"; require_relative "./util"
来源：http://uw.asd995.cn

C#:   using System.Text;
来源：http://hr.gzmigu.cn

[C12] 立即执行函数 IIFE
来源：http://mj.huixiangedu.cn

Py:   (lambda: print("run"))()
来源：http://pp.hnjuh.cn

PHP:  (function () { echo "run"; })();
来源：http://zn.shxzskj.cn

JS:   (() => { console.log("run"); })();
来源：http://ee.jianghongdianzi.cn

TS:   (() => { console.log("run"); })();
来源：http://es.huixinmuqiang.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rk.yuntaijiaju.cn

Go:   func() { fmt.Println("run") }()
来源：http://sz.huixinmuqiang.cn

Ruby: -> { puts "run" }.call
来源：http://nf.nszjky.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zo.shxzskj.cn

[C13] 类型声明 / 类型注解
来源：http://gs.nicolike.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sl.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mh.gzmigu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vk.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nn.huixinmuqiang.cn

Java: int add(int a, int b) { return a + b; }
来源：http://rm.jctech888.com.cn

Go:   func add(a, b int) int
来源：http://vi.yuntaijiaju.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://if.shxzukj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://oe.jctech888.com.cn

[C14] 泛型函数
来源：http://po.muxihuayi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zr.lnxyls.cn

PHP:  // 无泛型
来源：http://yg.asd995.cn

JS:   // 无泛型
来源：http://ko.bookmarksfly.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lc.newstarts.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xa.muxihuayi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wg.nicolike.cn

Ruby: # 无泛型
来源：http://zy.colortex.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://la.hnjuh.cn

[C15] 解构 / 展开参数
来源：http://rr.nszjky.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gi.jctech888.com.cn

PHP:  [$a, $b] = $pair;
来源：http://zq.gzmigu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lv.haigaiapp.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mq.chemitech.net.cn

Java: // 无解构
来源：http://ca.asd995.cn

Go:   // 无解构
来源：http://gd.bookmarksfly.cn


<!-- 参考信息 -->