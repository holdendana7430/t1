代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qm.huixiangedu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sd.lnxyls.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uu.huixinmuqiang.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ae.huixinmuqiang.cn

Go:   strings.TrimSpace(s)
来源：http://aj.lnxyls.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://an.haigaiapp.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://th.huixiangedu.cn

[A25] 字符串比较
来源：http://cc.newstarts.cn

Py:   s1 == s2; s1 != s2
来源：http://tg.521024.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sy.asd995.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mr.hnjuh.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gm.bjjhwx.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ih.bookmarksfly.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yb.newstarts.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://df.colortex.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hq.asd995.cn

[A26] 类型转换总览
来源：http://wm.szxytkj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yl.yuntaijiaju.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rl.jctech888.com.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hq.colortex.cn

TS:   Number() String() Boolean() x as number
来源：http://ce.521024.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://sr.jianghongdianzi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qg.nszjky.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://qw.huixiangedu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uw.panjiajie.cn

================================================================================
来源：http://kd.szxytkj.cn

B. 流程控制
来源：http://pj.huanxung.cn

================================================================================
来源：http://xg.szxytkj.cn

[B01] 条件判断 if / else
来源：http://tr.huanxung.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://cs.shxzskj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jy.wgjwhj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qc.asd995.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dj.szxytkj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://of.panjiajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://sx.szsharing.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rd.yuexingan06.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sk.yuexingan06.cn

[B02] 多分支 else if / elif
来源：http://bf.chemitech.net.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://oq.bookmarksfly.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ie.jianghongdianzi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xn.521024.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wa.bookmarksfly.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://co.haigaiapp.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://od.szxytkj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mr.colortex.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wn.asd995.cn

[B03] switch / match / case
来源：http://jy.muxihuayi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lg.chemitech.net.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fj.panjiajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wh.huanxung.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ch.gzmigu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vk.lnxyls.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wf.shtwfgs.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ao.panjiajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ry.huixiangedu.cn

[B04] for 计数循环
来源：http://mf.nicolike.cn

Py:   for i in range(10): print(i)
来源：http://nv.shxzskj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kk.panjiajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mi.jctech888.com.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pm.9csxet.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uj.521024.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://na.nicolike.cn

Ruby: 10.times { |i| puts i }
来源：http://xm.newstarts.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vl.nicolike.cn

[B05] 遍历数组 / 列表
来源：http://lf.gzmigu.cn

Py:   for item in arr: print(item)
来源：http://vv.wgjwhj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xk.newstarts.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://pv.lnxyls.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mw.bjjhwx.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yk.newstarts.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nm.bjjhwx.cn

Ruby: arr.each { |item| puts item }
来源：http://eb.colortex.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pv.haigaiapp.cn

[B06] 遍历字典 / 对象
来源：http://kg.huanxung.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ha.yuntaijiaju.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ix.asd995.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ox.szxytkj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zo.wgjwhj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fr.jctech888.com.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://iy.colortex.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tl.9csxet.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://of.yuexingan06.cn

[B07] while 循环
来源：http://mz.lnxyls.cn

Py:   while i < 10: i += 1
来源：http://qh.shxzukj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ou.9csxet.cn

JS:   while (i < 10) { i++; }
来源：http://is.nicolike.cn

TS:   while (i < 10) { i++; }
来源：http://rf.wgjwhj.cn

Java: while (i < 10) { i++; }
来源：http://ok.nicolike.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wf.huanxung.cn

Ruby: while i < 10; i += 1; end
来源：http://mk.jctech888.com.cn

C#:   while (i < 10) { i++; }
来源：http://kq.newstarts.cn

[B08] do-while（至少执行一次）
来源：http://ki.bjjhwx.cn

Py:   # 无 do-while：用 while True + break
来源：http://qq.9csxet.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://yr.nszjky.cn

JS:   do { i++; } while (i < 10);
来源：http://kz.9csxet.cn

TS:   do { i++; } while (i < 10);
来源：http://mc.szxytkj.cn

Java: do { i++; } while (i < 10);
来源：http://nb.muxihuayi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://kx.jctech888.com.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wc.yuexingan06.cn

C#:   do { i++; } while (i < 10);
来源：http://cv.hnjuh.cn

[B09] break 与 continue
来源：http://cs.wgjwhj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kh.nszjky.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jr.9csxet.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ft.shtwfgs.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aj.jctech888.com.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nt.szsharing.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ay.nszjky.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://it.bookmarksfly.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pl.huixinmuqiang.cn

[B10] 遍历同时拿索引
来源：http://tb.gzmigu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sf.muxihuayi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uv.wgjwhj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jo.nicolike.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://is.yuntaijiaju.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gf.panjiajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://av.szxytkj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vy.colortex.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://on.bookmarksfly.cn

[B11] 生成数字序列 / 区间
来源：http://ed.colortex.cn

Py:   list(range(0, 10, 2))
来源：http://pm.yuntaijiaju.cn

PHP:  range(0, 10, 2);
来源：http://vz.hahajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wa.9csxet.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ym.muxihuayi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pr.panjiajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://su.yuntaijiaju.cn

Ruby: (0...10).step(2).to_a
来源：http://xo.asd995.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://na.huixiangedu.cn

[B12] 跳出多层循环
来源：http://ca.yuexingan06.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ej.gzmigu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ga.9csxet.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qv.haigaiapp.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wj.shxzskj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cv.bjjhwx.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://db.bjjhwx.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qr.chemitech.net.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ts.shxzskj.cn

[B13] 判断是否为数字
来源：http://pf.colortex.cn

Py:   isinstance(x, (int, float))
来源：http://gm.521024.cn

PHP:  is_numeric($x)
来源：http://fu.521024.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://is.521024.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ht.huixinmuqiang.cn

Java: x instanceof Number
来源：http://bz.yuexingan06.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kb.newstarts.cn

Ruby: x.is_a?(Numeric)
来源：http://dt.yuntaijiaju.cn

C#:   x is int or double or decimal
来源：http://zw.colortex.cn

[B14] 判断值是否在集合内
来源：http://wa.muxihuayi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ak.hnjuh.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vu.asd995.cn

JS:   [1, 2, 3].includes(x)
来源：http://fr.shtwfgs.cn

TS:   [1, 2, 3].includes(x)
来源：http://xk.jianghongdianzi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://pq.bjjhwx.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ee.haigaiapp.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qm.shxzukj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zw.shtwfgs.cn

[B15] 布尔运算与取反
来源：http://ea.huixiangedu.cn

Py:   a and b or not c
来源：http://sx.9csxet.cn

PHP:  $a && $b || !$c
来源：http://st.jctech888.com.cn

JS:   a && b || !c
来源：http://mr.huixiangedu.cn

TS:   a && b || !c
来源：http://hq.521024.cn

Java: a && b || !c
来源：http://pr.hnjuh.cn

Go:   a && b || !c
来源：http://ke.bjjhwx.cn

Ruby: a && b || !c
来源：http://yi.huixiangedu.cn

C#:   a && b || !c
来源：http://zp.shtwfgs.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fa.panjiajie.cn

Py:   if not data: return
来源：http://cs.szxytkj.cn

PHP:  if (!$data) { return; }
来源：http://ds.jianghongdianzi.cn

JS:   if (!data) return;
来源：http://ai.lnxyls.cn

TS:   if (!data) return;
来源：http://ml.szsharing.cn

Java: if (data == null) return;
来源：http://oy.nicolike.cn

Go:   if data == nil { return }
来源：http://py.haigaiapp.cn

Ruby: return if data.nil?
来源：http://wq.huixiangedu.cn

C#:   if (data == null) return;
来源：http://nn.bjjhwx.cn

================================================================================
来源：http://ju.jctech888.com.cn

C. 函数与作用域
来源：http://tn.lnxyls.cn

================================================================================
来源：http://tu.yuntaijiaju.cn

[C01] 定义函数
来源：http://mk.haigaiapp.cn

Py:   def add(a, b): return a + b
来源：http://tt.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ck.hnjuh.cn

JS:   function add(a, b) { return a + b; }
来源：http://kz.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://md.yuntaijiaju.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vn.huixiangedu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://wn.panjiajie.cn

Ruby: def add(a, b); a + b; end
来源：http://am.huanxung.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lh.hnjuh.cn

[C02] 默认参数
来源：http://nr.nicolike.cn

Py:   def greet(name="World"): return name
来源：http://dt.wgjwhj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://sp.szxytkj.cn

JS:   function greet(name = "World") { return name; }
来源：http://dy.haigaiapp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qc.521024.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://mb.haigaiapp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xd.jctech888.com.cn

Ruby: def greet(name = "World") = name
来源：http://zb.chemitech.net.cn

C#:   string Greet(string name = "World") => name;
来源：http://vy.shxzskj.cn

[C03] 可变参数
来源：http://ft.nszjky.cn

Py:   def total(*args): return sum(args)
来源：http://iu.colortex.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vy.szxytkj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ku.szsharing.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ei.jctech888.com.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://eg.szsharing.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gh.wgjwhj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ss.9csxet.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bj.bookmarksfly.cn

[C04] 命名参数 / 关键字参数
来源：http://or.lnxyls.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ih.colortex.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zz.hahajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://il.huixiangedu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yi.nicolike.cn

Java: // 无：用 Builder 模式或 record
来源：http://hr.asd995.cn

Go:   // 无：用配置结构体参数
来源：http://af.huixinmuqiang.cn

Ruby: f(a: 1, b: 2)
来源：http://bt.panjiajie.cn

C#:   f(a: 1, b: 2)
来源：http://ly.haigaiapp.cn

[C05] 返回多个值
来源：http://ro.bookmarksfly.cn

Py:   return a, b
来源：http://fp.huanxung.cn

PHP:  return [$a, $b];
来源：http://jt.yuntaijiaju.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yt.muxihuayi.cn

TS:   return { a, b };
来源：http://or.yuexingan06.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lr.bookmarksfly.cn

Go:   return a, b
来源：http://sy.huanxung.cn

Ruby: return a, b
来源：http://gb.lnxyls.cn

C#:   return (a, b);              // ValueTuple
来源：http://qx.muxihuayi.cn

[C06] 匿名函数 / lambda
来源：http://ns.hnjuh.cn

Py:   square = lambda x: x * x
来源：http://qu.bookmarksfly.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ac.szxytkj.cn

JS:   const square = x => x * x;
来源：http://fy.jctech888.com.cn

TS:   const square = (x: number): number => x * x;
来源：http://qk.hahajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cx.muxihuayi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rm.nicolike.cn

Ruby: square = ->(x) { x * x }
来源：http://br.lnxyls.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wn.shxzukj.cn

[C07] 把函数作为参数传入
来源：http://ma.nicolike.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sq.shtwfgs.cn

PHP:  array_map("strtoupper", $arr);
来源：http://rs.521024.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rs.shxzskj.cn

TS:   arr.map(String)
来源：http://wf.521024.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wl.chemitech.net.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zy.yuexingan06.cn

Ruby: arr.map(&:upcase)
来源：http://ri.nszjky.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hu.jctech888.com.cn

[C08] 闭包
来源：http://vu.huixinmuqiang.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xe.wgjwhj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ct.nicolike.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kn.lnxyls.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dr.yuntaijiaju.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uy.huanxung.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bu.bookmarksfly.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zc.bjjhwx.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ua.jctech888.com.cn

[C09] 递归
来源：http://xw.muxihuayi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://oa.szxytkj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ic.haigaiapp.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zs.yuntaijiaju.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yn.jctech888.com.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rg.hnjuh.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ht.haigaiapp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ko.shtwfgs.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ik.jianghongdianzi.cn

[C10] 变量作用域
来源：http://fg.shxzskj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sl.yuntaijiaju.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ef.huixinmuqiang.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mp.colortex.cn

TS:   同 JS
来源：http://sl.nicolike.cn

Java: 方法内为块级作用域
来源：http://qv.huanxung.cn

Go:   花括号块级作用域
来源：http://dc.521024.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fu.muxihuayi.cn

C#:   块级作用域
来源：http://yv.shtwfgs.cn

[C11] 模块导入与导出
来源：http://ae.huixinmuqiang.cn

Py:   from module import func
来源：http://mj.shxzukj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ui.9csxet.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://pq.lnxyls.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ky.shxzskj.cn

Java: import java.util.List;
来源：http://ea.bjjhwx.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tb.jctech888.com.cn

Ruby: require "json"; require_relative "./util"
来源：http://gs.shxzukj.cn

C#:   using System.Text;
来源：http://eq.bjjhwx.cn

[C12] 立即执行函数 IIFE
来源：http://ku.hahajie.cn

Py:   (lambda: print("run"))()
来源：http://gv.hnjuh.cn

PHP:  (function () { echo "run"; })();
来源：http://qv.gzmigu.cn

JS:   (() => { console.log("run"); })();
来源：http://fu.hnjuh.cn

TS:   (() => { console.log("run"); })();
来源：http://is.chemitech.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ba.huixinmuqiang.cn

Go:   func() { fmt.Println("run") }()
来源：http://zm.colortex.cn

Ruby: -> { puts "run" }.call
来源：http://yy.gzmigu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pz.yuexingan06.cn

[C13] 类型声明 / 类型注解
来源：http://he.yuexingan06.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ef.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bc.szsharing.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qj.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ww.shtwfgs.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xf.newstarts.cn

Go:   func add(a, b int) int
来源：http://ms.shxzskj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xv.hahajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xc.521024.cn

[C14] 泛型函数
来源：http://wl.lnxyls.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ob.panjiajie.cn

PHP:  // 无泛型
来源：http://yf.shtwfgs.cn

JS:   // 无泛型
来源：http://hi.szsharing.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ys.hahajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lg.shxzukj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dc.521024.cn

Ruby: # 无泛型
来源：http://gn.muxihuayi.cn


<!-- 参考信息 -->