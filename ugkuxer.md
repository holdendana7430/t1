代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://ji.9csxet.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mk.shxzskj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zr.szxytkj.cn

[A25] 字符串比较
来源：http://tj.9csxet.cn

Py:   s1 == s2; s1 != s2
来源：http://vj.gzmigu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zd.yuexingan06.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wx.shxzskj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qo.szxytkj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://oc.shtwfgs.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dm.colortex.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ky.szxytkj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ik.nszjky.cn

[A26] 类型转换总览
来源：http://pk.nszjky.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ya.huixiangedu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cv.hahajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ib.haigaiapp.cn

TS:   Number() String() Boolean() x as number
来源：http://ax.nicolike.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dc.521024.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fr.shxzukj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://tu.jianghongdianzi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ej.huixinmuqiang.cn

================================================================================
来源：http://qr.wgjwhj.cn

B. 流程控制
来源：http://lz.shtwfgs.cn

================================================================================
来源：http://zz.chemitech.net.cn

[B01] 条件判断 if / else
来源：http://mt.szxytkj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://yn.colortex.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ma.shxzukj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zc.wgjwhj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zy.szxytkj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://mg.shtwfgs.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jb.huixinmuqiang.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ug.huanxung.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ut.shtwfgs.cn

[B02] 多分支 else if / elif
来源：http://fx.muxihuayi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kg.huixinmuqiang.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ju.shtwfgs.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ot.colortex.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rz.szxytkj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pj.yuexingan06.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://aj.jctech888.com.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kn.shxzukj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ob.jianghongdianzi.cn

[B03] switch / match / case
来源：http://sf.huanxung.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xy.bookmarksfly.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uz.nicolike.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ca.bookmarksfly.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nk.wgjwhj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zo.shtwfgs.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nn.panjiajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yb.shxzukj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kh.huixinmuqiang.cn

[B04] for 计数循环
来源：http://zo.huixinmuqiang.cn

Py:   for i in range(10): print(i)
来源：http://hm.shxzskj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jn.newstarts.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ii.lnxyls.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ti.bjjhwx.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nt.huanxung.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ea.9csxet.cn

Ruby: 10.times { |i| puts i }
来源：http://sk.shxzukj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hc.asd995.cn

[B05] 遍历数组 / 列表
来源：http://er.jianghongdianzi.cn

Py:   for item in arr: print(item)
来源：http://zz.colortex.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ul.jianghongdianzi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qh.haigaiapp.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://vb.nszjky.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yc.muxihuayi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lh.9csxet.cn

Ruby: arr.each { |item| puts item }
来源：http://eb.hahajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://to.chemitech.net.cn

[B06] 遍历字典 / 对象
来源：http://rz.yuntaijiaju.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://cz.gzmigu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hb.newstarts.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lk.521024.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mj.bjjhwx.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yp.panjiajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wi.521024.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nw.jianghongdianzi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ay.yuexingan06.cn

[B07] while 循环
来源：http://tf.haigaiapp.cn

Py:   while i < 10: i += 1
来源：http://jm.jianghongdianzi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hl.yuntaijiaju.cn

JS:   while (i < 10) { i++; }
来源：http://pw.9csxet.cn

TS:   while (i < 10) { i++; }
来源：http://xf.chemitech.net.cn

Java: while (i < 10) { i++; }
来源：http://mt.shxzskj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vd.huixinmuqiang.cn

Ruby: while i < 10; i += 1; end
来源：http://ds.haigaiapp.cn

C#:   while (i < 10) { i++; }
来源：http://nv.hahajie.cn

[B08] do-while（至少执行一次）
来源：http://xt.yuntaijiaju.cn

Py:   # 无 do-while：用 while True + break
来源：http://kh.wgjwhj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ca.hnjuh.cn

JS:   do { i++; } while (i < 10);
来源：http://kw.nszjky.cn

TS:   do { i++; } while (i < 10);
来源：http://uv.huanxung.cn

Java: do { i++; } while (i < 10);
来源：http://cs.shtwfgs.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sh.521024.cn

Ruby: begin; i += 1; end while i < 10
来源：http://dr.jctech888.com.cn

C#:   do { i++; } while (i < 10);
来源：http://mp.bookmarksfly.cn

[B09] break 与 continue
来源：http://uz.huixiangedu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rq.szxytkj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qk.haigaiapp.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ep.jctech888.com.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lh.yuexingan06.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rg.hahajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://uq.nicolike.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dc.haigaiapp.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ff.muxihuayi.cn

[B10] 遍历同时拿索引
来源：http://tb.bjjhwx.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ap.chemitech.net.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wi.chemitech.net.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nc.hahajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jn.jianghongdianzi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kq.huanxung.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wu.jctech888.com.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nm.huanxung.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gk.shxzukj.cn

[B11] 生成数字序列 / 区间
来源：http://cf.lnxyls.cn

Py:   list(range(0, 10, 2))
来源：http://au.hahajie.cn

PHP:  range(0, 10, 2);
来源：http://fp.yuntaijiaju.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iw.hnjuh.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mp.haigaiapp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zn.szsharing.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xz.yuexingan06.cn

Ruby: (0...10).step(2).to_a
来源：http://cq.9csxet.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hu.lnxyls.cn

[B12] 跳出多层循环
来源：http://sj.asd995.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://dk.nicolike.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://pe.bookmarksfly.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zz.newstarts.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zs.haigaiapp.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lz.shxzskj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yi.huanxung.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rq.muxihuayi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ne.colortex.cn

[B13] 判断是否为数字
来源：http://lx.hahajie.cn

Py:   isinstance(x, (int, float))
来源：http://ry.yuexingan06.cn

PHP:  is_numeric($x)
来源：http://tl.yuexingan06.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hu.yuexingan06.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zq.panjiajie.cn

Java: x instanceof Number
来源：http://vs.521024.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ku.yuntaijiaju.cn

Ruby: x.is_a?(Numeric)
来源：http://mo.nicolike.cn

C#:   x is int or double or decimal
来源：http://ig.huixinmuqiang.cn

[B14] 判断值是否在集合内
来源：http://nd.muxihuayi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://io.shtwfgs.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ef.nszjky.cn

JS:   [1, 2, 3].includes(x)
来源：http://dy.szsharing.cn

TS:   [1, 2, 3].includes(x)
来源：http://gx.jctech888.com.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://fu.szsharing.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bn.shxzukj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gp.chemitech.net.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ma.hnjuh.cn

[B15] 布尔运算与取反
来源：http://ry.gzmigu.cn

Py:   a and b or not c
来源：http://qm.huixiangedu.cn

PHP:  $a && $b || !$c
来源：http://xv.panjiajie.cn

JS:   a && b || !c
来源：http://sn.bookmarksfly.cn

TS:   a && b || !c
来源：http://gi.huanxung.cn

Java: a && b || !c
来源：http://sb.yuntaijiaju.cn

Go:   a && b || !c
来源：http://ib.shxzukj.cn

Ruby: a && b || !c
来源：http://by.shtwfgs.cn

C#:   a && b || !c
来源：http://wq.shxzskj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vq.asd995.cn

Py:   if not data: return
来源：http://zx.521024.cn

PHP:  if (!$data) { return; }
来源：http://ou.gzmigu.cn

JS:   if (!data) return;
来源：http://et.chemitech.net.cn

TS:   if (!data) return;
来源：http://vg.gzmigu.cn

Java: if (data == null) return;
来源：http://fm.bookmarksfly.cn

Go:   if data == nil { return }
来源：http://bd.haigaiapp.cn

Ruby: return if data.nil?
来源：http://yx.jctech888.com.cn

C#:   if (data == null) return;
来源：http://ne.szsharing.cn

================================================================================
来源：http://cv.huixinmuqiang.cn

C. 函数与作用域
来源：http://gd.huanxung.cn

================================================================================
来源：http://de.haigaiapp.cn

[C01] 定义函数
来源：http://ah.bookmarksfly.cn

Py:   def add(a, b): return a + b
来源：http://pa.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qd.bjjhwx.cn

JS:   function add(a, b) { return a + b; }
来源：http://ao.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iu.szxytkj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://pp.jctech888.com.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hl.521024.cn

Ruby: def add(a, b); a + b; end
来源：http://om.yuntaijiaju.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ws.muxihuayi.cn

[C02] 默认参数
来源：http://ml.shxzukj.cn

Py:   def greet(name="World"): return name
来源：http://cl.hahajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lq.newstarts.cn

JS:   function greet(name = "World") { return name; }
来源：http://xj.gzmigu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://kf.colortex.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hm.huixinmuqiang.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hi.muxihuayi.cn

Ruby: def greet(name = "World") = name
来源：http://wo.chemitech.net.cn

C#:   string Greet(string name = "World") => name;
来源：http://zz.lnxyls.cn

[C03] 可变参数
来源：http://wv.huixinmuqiang.cn

Py:   def total(*args): return sum(args)
来源：http://wh.huixinmuqiang.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bk.nszjky.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://au.wgjwhj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mo.shtwfgs.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://js.asd995.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tl.521024.cn

Ruby: def total(*nums); nums.sum; end
来源：http://jq.haigaiapp.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jd.newstarts.cn

[C04] 命名参数 / 关键字参数
来源：http://bi.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sw.jctech888.com.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qe.szxytkj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yi.haigaiapp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zh.nicolike.cn

Java: // 无：用 Builder 模式或 record
来源：http://sx.huixiangedu.cn

Go:   // 无：用配置结构体参数
来源：http://vr.yuntaijiaju.cn

Ruby: f(a: 1, b: 2)
来源：http://ig.9csxet.cn

C#:   f(a: 1, b: 2)
来源：http://vp.huixinmuqiang.cn

[C05] 返回多个值
来源：http://le.jctech888.com.cn

Py:   return a, b
来源：http://us.9csxet.cn

PHP:  return [$a, $b];
来源：http://mm.gzmigu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ip.haigaiapp.cn

TS:   return { a, b };
来源：http://sv.asd995.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ie.nszjky.cn

Go:   return a, b
来源：http://pj.huixinmuqiang.cn

Ruby: return a, b
来源：http://hx.shxzskj.cn

C#:   return (a, b);              // ValueTuple
来源：http://tx.huixinmuqiang.cn

[C06] 匿名函数 / lambda
来源：http://hy.asd995.cn

Py:   square = lambda x: x * x
来源：http://ql.panjiajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qw.huanxung.cn

JS:   const square = x => x * x;
来源：http://cp.nszjky.cn

TS:   const square = (x: number): number => x * x;
来源：http://qg.shtwfgs.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qc.huixinmuqiang.cn

Go:   sq := func(x int) int { return x * x }
来源：http://lg.bjjhwx.cn

Ruby: square = ->(x) { x * x }
来源：http://xn.nicolike.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xc.hahajie.cn

[C07] 把函数作为参数传入
来源：http://of.jianghongdianzi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ze.chemitech.net.cn

PHP:  array_map("strtoupper", $arr);
来源：http://eh.shxzskj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ay.shxzukj.cn

TS:   arr.map(String)
来源：http://xx.huixiangedu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sd.chemitech.net.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ky.huixinmuqiang.cn

Ruby: arr.map(&:upcase)
来源：http://io.gzmigu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hv.huanxung.cn

[C08] 闭包
来源：http://of.colortex.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ei.shxzukj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nv.yuntaijiaju.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gy.huixiangedu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ld.nicolike.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ay.huanxung.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jy.jctech888.com.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kj.bjjhwx.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ul.9csxet.cn

[C09] 递归
来源：http://ql.yuntaijiaju.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cr.szxytkj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bz.newstarts.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ko.panjiajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qb.szxytkj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gw.panjiajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sw.asd995.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bf.shxzukj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://to.szxytkj.cn

[C10] 变量作用域
来源：http://aj.yuntaijiaju.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://la.panjiajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fu.bookmarksfly.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zb.szsharing.cn

TS:   同 JS
来源：http://mw.nicolike.cn

Java: 方法内为块级作用域
来源：http://kg.lnxyls.cn

Go:   花括号块级作用域
来源：http://ko.haigaiapp.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://co.shtwfgs.cn

C#:   块级作用域
来源：http://et.huanxung.cn

[C11] 模块导入与导出
来源：http://rw.chemitech.net.cn

Py:   from module import func
来源：http://rl.asd995.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xc.huixiangedu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://sm.jianghongdianzi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://db.bjjhwx.cn

Java: import java.util.List;
来源：http://wp.huanxung.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cb.shtwfgs.cn

Ruby: require "json"; require_relative "./util"
来源：http://dz.szxytkj.cn

C#:   using System.Text;
来源：http://ed.huixinmuqiang.cn

[C12] 立即执行函数 IIFE
来源：http://sf.gzmigu.cn

Py:   (lambda: print("run"))()
来源：http://tx.muxihuayi.cn

PHP:  (function () { echo "run"; })();
来源：http://ky.jctech888.com.cn

JS:   (() => { console.log("run"); })();
来源：http://zq.shtwfgs.cn

TS:   (() => { console.log("run"); })();
来源：http://ht.hnjuh.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ml.chemitech.net.cn

Go:   func() { fmt.Println("run") }()
来源：http://dy.521024.cn

Ruby: -> { puts "run" }.call
来源：http://zn.jianghongdianzi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gk.yuntaijiaju.cn

[C13] 类型声明 / 类型注解
来源：http://ih.huixinmuqiang.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ic.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hx.muxihuayi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xv.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xl.nszjky.cn

Java: int add(int a, int b) { return a + b; }
来源：http://iu.bjjhwx.cn

Go:   func add(a, b int) int
来源：http://sq.szsharing.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tc.huixinmuqiang.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gj.bookmarksfly.cn

[C14] 泛型函数
来源：http://ut.shxzskj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ai.panjiajie.cn

PHP:  // 无泛型
来源：http://wf.hahajie.cn

JS:   // 无泛型
来源：http://up.lnxyls.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zk.hnjuh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nt.bookmarksfly.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kj.jctech888.com.cn

Ruby: # 无泛型
来源：http://gx.9csxet.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qg.gzmigu.cn

[C15] 解构 / 展开参数
来源：http://zl.521024.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kw.panjiajie.cn

PHP:  [$a, $b] = $pair;
来源：http://bw.bjjhwx.cn


<!-- 参考信息 -->