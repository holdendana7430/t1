代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://nf.shtwfgs.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://yf.haigaiapp.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ux.jctech888.com.cn

[A25] 字符串比较
来源：http://dr.shxzskj.cn

Py:   s1 == s2; s1 != s2
来源：http://ic.jctech888.com.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://un.shxzukj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dh.hahajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nt.chemitech.net.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gj.9csxet.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yk.jctech888.com.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://px.szsharing.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qr.9csxet.cn

[A26] 类型转换总览
来源：http://um.bookmarksfly.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xu.colortex.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dv.hnjuh.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jr.huixinmuqiang.cn

TS:   Number() String() Boolean() x as number
来源：http://la.521024.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pb.hahajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jo.bjjhwx.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://po.chemitech.net.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ur.yuexingan06.cn

================================================================================
来源：http://wu.szsharing.cn

B. 流程控制
来源：http://hq.hahajie.cn

================================================================================
来源：http://hs.huanxung.cn

[B01] 条件判断 if / else
来源：http://td.shtwfgs.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://cw.hnjuh.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sd.colortex.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gs.chemitech.net.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nc.muxihuayi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://kb.huixinmuqiang.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pf.huixiangedu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vv.newstarts.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://by.jianghongdianzi.cn

[B02] 多分支 else if / elif
来源：http://ss.huixiangedu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wl.bookmarksfly.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fn.szxytkj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ns.jctech888.com.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sa.asd995.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://va.szxytkj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ge.newstarts.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nn.nicolike.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vx.szxytkj.cn

[B03] switch / match / case
来源：http://qv.colortex.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sn.521024.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yj.hahajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zd.521024.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vb.asd995.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dz.haigaiapp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jm.lnxyls.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cb.nicolike.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dj.chemitech.net.cn

[B04] for 计数循环
来源：http://bz.huanxung.cn

Py:   for i in range(10): print(i)
来源：http://wy.huixiangedu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ju.szsharing.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oe.szxytkj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://it.hahajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qc.jianghongdianzi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://be.nicolike.cn

Ruby: 10.times { |i| puts i }
来源：http://qk.muxihuayi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lq.newstarts.cn

[B05] 遍历数组 / 列表
来源：http://vs.yuntaijiaju.cn

Py:   for item in arr: print(item)
来源：http://wo.hahajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zo.panjiajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gg.szxytkj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.yuntaijiaju.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sb.newstarts.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fg.muxihuayi.cn

Ruby: arr.each { |item| puts item }
来源：http://lc.nicolike.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ln.lnxyls.cn

[B06] 遍历字典 / 对象
来源：http://le.jianghongdianzi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://dm.colortex.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xg.shxzukj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yf.shtwfgs.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qf.jctech888.com.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://eq.chemitech.net.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cq.huixinmuqiang.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://my.9csxet.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xo.szxytkj.cn

[B07] while 循环
来源：http://gb.shxzskj.cn

Py:   while i < 10: i += 1
来源：http://bh.colortex.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lh.521024.cn

JS:   while (i < 10) { i++; }
来源：http://lf.huixiangedu.cn

TS:   while (i < 10) { i++; }
来源：http://zk.haigaiapp.cn

Java: while (i < 10) { i++; }
来源：http://td.chemitech.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hy.521024.cn

Ruby: while i < 10; i += 1; end
来源：http://yd.yuntaijiaju.cn

C#:   while (i < 10) { i++; }
来源：http://no.muxihuayi.cn

[B08] do-while（至少执行一次）
来源：http://ik.jianghongdianzi.cn

Py:   # 无 do-while：用 while True + break
来源：http://ts.nicolike.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://at.gzmigu.cn

JS:   do { i++; } while (i < 10);
来源：http://ed.jianghongdianzi.cn

TS:   do { i++; } while (i < 10);
来源：http://ln.jctech888.com.cn

Java: do { i++; } while (i < 10);
来源：http://ca.nicolike.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://hh.521024.cn

Ruby: begin; i += 1; end while i < 10
来源：http://yd.colortex.cn

C#:   do { i++; } while (i < 10);
来源：http://hp.lnxyls.cn

[B09] break 与 continue
来源：http://xn.colortex.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vp.yuntaijiaju.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jg.9csxet.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cg.bookmarksfly.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ms.bjjhwx.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hf.nicolike.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jx.9csxet.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://uq.yuexingan06.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mb.huixiangedu.cn

[B10] 遍历同时拿索引
来源：http://yd.chemitech.net.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jv.shxzskj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mt.shtwfgs.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pu.jianghongdianzi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ag.muxihuayi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://eh.hahajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ke.yuntaijiaju.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jg.huixinmuqiang.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xm.bookmarksfly.cn

[B11] 生成数字序列 / 区间
来源：http://tf.muxihuayi.cn

Py:   list(range(0, 10, 2))
来源：http://hw.lnxyls.cn

PHP:  range(0, 10, 2);
来源：http://zo.hnjuh.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xw.9csxet.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pf.chemitech.net.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tf.bookmarksfly.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://le.yuexingan06.cn

Ruby: (0...10).step(2).to_a
来源：http://iv.wgjwhj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yx.shtwfgs.cn

[B12] 跳出多层循环
来源：http://xa.jianghongdianzi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ef.yuntaijiaju.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://sh.szsharing.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bi.huixinmuqiang.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ek.shtwfgs.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ln.wgjwhj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kh.huanxung.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gm.chemitech.net.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rr.nszjky.cn

[B13] 判断是否为数字
来源：http://rr.chemitech.net.cn

Py:   isinstance(x, (int, float))
来源：http://mc.jianghongdianzi.cn

PHP:  is_numeric($x)
来源：http://ye.nicolike.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gb.chemitech.net.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zk.gzmigu.cn

Java: x instanceof Number
来源：http://yl.chemitech.net.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tk.szsharing.cn

Ruby: x.is_a?(Numeric)
来源：http://gj.lnxyls.cn

C#:   x is int or double or decimal
来源：http://ea.bjjhwx.cn

[B14] 判断值是否在集合内
来源：http://bx.chemitech.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qb.newstarts.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rv.jctech888.com.cn

JS:   [1, 2, 3].includes(x)
来源：http://nb.yuntaijiaju.cn

TS:   [1, 2, 3].includes(x)
来源：http://hr.wgjwhj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://sp.lnxyls.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vi.nicolike.cn

Ruby: [1, 2, 3].include?(x)
来源：http://bo.wgjwhj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://me.bjjhwx.cn

[B15] 布尔运算与取反
来源：http://id.jianghongdianzi.cn

Py:   a and b or not c
来源：http://sb.bookmarksfly.cn

PHP:  $a && $b || !$c
来源：http://sg.huanxung.cn

JS:   a && b || !c
来源：http://oz.hnjuh.cn

TS:   a && b || !c
来源：http://wi.jctech888.com.cn

Java: a && b || !c
来源：http://yl.hnjuh.cn

Go:   a && b || !c
来源：http://rj.hahajie.cn

Ruby: a && b || !c
来源：http://sp.huixiangedu.cn

C#:   a && b || !c
来源：http://lh.nicolike.cn

[B16] 卫语句：不满足条件提前返回
来源：http://cc.huixinmuqiang.cn

Py:   if not data: return
来源：http://mk.lnxyls.cn

PHP:  if (!$data) { return; }
来源：http://vd.bjjhwx.cn

JS:   if (!data) return;
来源：http://bd.gzmigu.cn

TS:   if (!data) return;
来源：http://vi.bjjhwx.cn

Java: if (data == null) return;
来源：http://kv.521024.cn

Go:   if data == nil { return }
来源：http://jc.asd995.cn

Ruby: return if data.nil?
来源：http://bv.haigaiapp.cn

C#:   if (data == null) return;
来源：http://fg.bjjhwx.cn

================================================================================
来源：http://bd.huixiangedu.cn

C. 函数与作用域
来源：http://hm.yuexingan06.cn

================================================================================
来源：http://sp.huanxung.cn

[C01] 定义函数
来源：http://te.huanxung.cn

Py:   def add(a, b): return a + b
来源：http://sq.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vg.colortex.cn

JS:   function add(a, b) { return a + b; }
来源：http://wu.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sb.shxzukj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://cc.nszjky.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ml.shxzukj.cn

Ruby: def add(a, b); a + b; end
来源：http://ki.lnxyls.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dm.colortex.cn

[C02] 默认参数
来源：http://yy.yuexingan06.cn

Py:   def greet(name="World"): return name
来源：http://ea.huanxung.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fw.nicolike.cn

JS:   function greet(name = "World") { return name; }
来源：http://vy.huanxung.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ql.521024.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://gk.huixinmuqiang.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xz.muxihuayi.cn

Ruby: def greet(name = "World") = name
来源：http://zx.nicolike.cn

C#:   string Greet(string name = "World") => name;
来源：http://gj.bookmarksfly.cn

[C03] 可变参数
来源：http://ks.lnxyls.cn

Py:   def total(*args): return sum(args)
来源：http://lz.yuntaijiaju.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ea.szsharing.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bd.gzmigu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://eq.jctech888.com.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jt.nszjky.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ut.haigaiapp.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wu.panjiajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lg.jianghongdianzi.cn

[C04] 命名参数 / 关键字参数
来源：http://bz.newstarts.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jv.huixiangedu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rm.newstarts.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xq.shxzukj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nd.jctech888.com.cn

Java: // 无：用 Builder 模式或 record
来源：http://on.nszjky.cn

Go:   // 无：用配置结构体参数
来源：http://jw.szxytkj.cn

Ruby: f(a: 1, b: 2)
来源：http://fw.shxzukj.cn

C#:   f(a: 1, b: 2)
来源：http://xe.jianghongdianzi.cn

[C05] 返回多个值
来源：http://uc.wgjwhj.cn

Py:   return a, b
来源：http://rr.huanxung.cn

PHP:  return [$a, $b];
来源：http://ol.huanxung.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wg.szxytkj.cn

TS:   return { a, b };
来源：http://qz.9csxet.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ks.gzmigu.cn

Go:   return a, b
来源：http://ea.haigaiapp.cn

Ruby: return a, b
来源：http://sf.szsharing.cn

C#:   return (a, b);              // ValueTuple
来源：http://jm.gzmigu.cn

[C06] 匿名函数 / lambda
来源：http://gs.colortex.cn

Py:   square = lambda x: x * x
来源：http://dl.panjiajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://hl.gzmigu.cn

JS:   const square = x => x * x;
来源：http://ku.chemitech.net.cn

TS:   const square = (x: number): number => x * x;
来源：http://uo.nszjky.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vv.yuexingan06.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ra.yuexingan06.cn

Ruby: square = ->(x) { x * x }
来源：http://wp.521024.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hy.jctech888.com.cn

[C07] 把函数作为参数传入
来源：http://cj.shxzukj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nl.521024.cn

PHP:  array_map("strtoupper", $arr);
来源：http://tz.muxihuayi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nx.panjiajie.cn

TS:   arr.map(String)
来源：http://yt.bjjhwx.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://eu.muxihuayi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kg.jianghongdianzi.cn

Ruby: arr.map(&:upcase)
来源：http://bu.bjjhwx.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hy.gzmigu.cn

[C08] 闭包
来源：http://rk.jctech888.com.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://np.newstarts.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ck.9csxet.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ly.jianghongdianzi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nw.shxzskj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dk.shtwfgs.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jz.asd995.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ua.bjjhwx.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ha.wgjwhj.cn

[C09] 递归
来源：http://vm.huixiangedu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pe.jianghongdianzi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://el.bookmarksfly.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cb.newstarts.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ui.jianghongdianzi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tq.szsharing.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ij.jianghongdianzi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ey.wgjwhj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cs.jctech888.com.cn

[C10] 变量作用域
来源：http://td.panjiajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ak.jianghongdianzi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ej.bookmarksfly.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ve.panjiajie.cn

TS:   同 JS
来源：http://yl.huanxung.cn

Java: 方法内为块级作用域
来源：http://tt.haigaiapp.cn

Go:   花括号块级作用域
来源：http://ho.yuntaijiaju.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wb.nicolike.cn

C#:   块级作用域
来源：http://ns.muxihuayi.cn

[C11] 模块导入与导出
来源：http://qp.hahajie.cn

Py:   from module import func
来源：http://em.gzmigu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://rn.szsharing.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vw.colortex.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hs.hnjuh.cn

Java: import java.util.List;
来源：http://zb.521024.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sp.jctech888.com.cn

Ruby: require "json"; require_relative "./util"
来源：http://wk.9csxet.cn

C#:   using System.Text;
来源：http://yb.521024.cn

[C12] 立即执行函数 IIFE
来源：http://ng.shtwfgs.cn

Py:   (lambda: print("run"))()
来源：http://qa.huixinmuqiang.cn

PHP:  (function () { echo "run"; })();
来源：http://ot.wgjwhj.cn

JS:   (() => { console.log("run"); })();
来源：http://df.newstarts.cn

TS:   (() => { console.log("run"); })();
来源：http://ej.shxzskj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://eb.haigaiapp.cn

Go:   func() { fmt.Println("run") }()
来源：http://ye.lnxyls.cn

Ruby: -> { puts "run" }.call
来源：http://hi.panjiajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ih.521024.cn

[C13] 类型声明 / 类型注解
来源：http://it.shxzukj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xv.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ki.yuntaijiaju.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bn.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ar.panjiajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://br.yuntaijiaju.cn

Go:   func add(a, b int) int
来源：http://hj.yuexingan06.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sl.newstarts.cn

C#:   int Add(int a, int b) => a + b;
来源：http://yo.panjiajie.cn

[C14] 泛型函数
来源：http://dv.newstarts.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fo.9csxet.cn

PHP:  // 无泛型
来源：http://fd.szsharing.cn

JS:   // 无泛型
来源：http://oi.huixiangedu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ne.huixiangedu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ik.huixiangedu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dr.panjiajie.cn

Ruby: # 无泛型
来源：http://ey.huanxung.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tv.colortex.cn

[C15] 解构 / 展开参数
来源：http://dv.nicolike.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sa.muxihuayi.cn

PHP:  [$a, $b] = $pair;
来源：http://du.haigaiapp.cn


<!-- 参考信息 -->