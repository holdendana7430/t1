代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ha.shxzskj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://of.gzmigu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ir.hahajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gb.shtwfgs.cn

Go:   strings.TrimSpace(s)
来源：http://yu.9csxet.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vr.hahajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gc.jctech888.com.cn

[A25] 字符串比较
来源：http://st.shxzukj.cn

Py:   s1 == s2; s1 != s2
来源：http://um.shxzukj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ms.muxihuayi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fz.shtwfgs.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vy.colortex.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bt.szxytkj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://np.nicolike.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://eh.gzmigu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pc.wgjwhj.cn

[A26] 类型转换总览
来源：http://td.huixiangedu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dr.shxzukj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://as.nszjky.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ie.chemitech.net.cn

TS:   Number() String() Boolean() x as number
来源：http://qq.yuexingan06.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hu.hahajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dz.asd995.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://qu.gzmigu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mt.bjjhwx.cn

================================================================================
来源：http://qf.asd995.cn

B. 流程控制
来源：http://vk.jctech888.com.cn

================================================================================
来源：http://rz.lnxyls.cn

[B01] 条件判断 if / else
来源：http://lr.nicolike.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://sh.nicolike.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mq.yuntaijiaju.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gi.szsharing.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pq.shxzskj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xa.huanxung.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pi.gzmigu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qm.huixinmuqiang.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cx.nicolike.cn

[B02] 多分支 else if / elif
来源：http://lk.gzmigu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qt.jctech888.com.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qt.haigaiapp.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rk.bookmarksfly.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fq.muxihuayi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xt.shxzukj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fw.hnjuh.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://eu.huanxung.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ig.shtwfgs.cn

[B03] switch / match / case
来源：http://nx.huixiangedu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qa.newstarts.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ta.chemitech.net.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mw.shtwfgs.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://iv.hnjuh.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lt.bookmarksfly.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://aa.muxihuayi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ru.9csxet.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jk.haigaiapp.cn

[B04] for 计数循环
来源：http://gw.szxytkj.cn

Py:   for i in range(10): print(i)
来源：http://xw.bjjhwx.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sg.yuntaijiaju.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iq.nszjky.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fd.gzmigu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mn.panjiajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yd.panjiajie.cn

Ruby: 10.times { |i| puts i }
来源：http://ca.shxzskj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gf.gzmigu.cn

[B05] 遍历数组 / 列表
来源：http://fj.yuntaijiaju.cn

Py:   for item in arr: print(item)
来源：http://vu.muxihuayi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://el.panjiajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://pg.panjiajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://sa.newstarts.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://tj.shxzskj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jm.hnjuh.cn

Ruby: arr.each { |item| puts item }
来源：http://yl.newstarts.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jb.szxytkj.cn

[B06] 遍历字典 / 对象
来源：http://hp.colortex.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://gq.521024.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://je.huixinmuqiang.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wt.chemitech.net.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eu.szsharing.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dx.panjiajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://it.szxytkj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ll.9csxet.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://db.lnxyls.cn

[B07] while 循环
来源：http://cn.gzmigu.cn

Py:   while i < 10: i += 1
来源：http://sy.huixinmuqiang.cn

PHP:  while ($i < 10) { $i++; }
来源：http://um.nicolike.cn

JS:   while (i < 10) { i++; }
来源：http://js.chemitech.net.cn

TS:   while (i < 10) { i++; }
来源：http://cl.haigaiapp.cn

Java: while (i < 10) { i++; }
来源：http://vx.yuexingan06.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bs.muxihuayi.cn

Ruby: while i < 10; i += 1; end
来源：http://zd.huixinmuqiang.cn

C#:   while (i < 10) { i++; }
来源：http://ff.panjiajie.cn

[B08] do-while（至少执行一次）
来源：http://xr.wgjwhj.cn

Py:   # 无 do-while：用 while True + break
来源：http://qf.shxzskj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://gy.gzmigu.cn

JS:   do { i++; } while (i < 10);
来源：http://cr.shxzskj.cn

TS:   do { i++; } while (i < 10);
来源：http://yw.lnxyls.cn

Java: do { i++; } while (i < 10);
来源：http://pd.gzmigu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gm.wgjwhj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jz.gzmigu.cn

C#:   do { i++; } while (i < 10);
来源：http://is.colortex.cn

[B09] break 与 continue
来源：http://yu.jctech888.com.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pw.newstarts.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://di.muxihuayi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ru.huanxung.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sm.lnxyls.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xu.huanxung.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://va.bookmarksfly.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ct.asd995.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kl.bjjhwx.cn

[B10] 遍历同时拿索引
来源：http://en.muxihuayi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dp.shxzukj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nh.lnxyls.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cu.nicolike.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ge.lnxyls.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vy.jctech888.com.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bf.jctech888.com.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yt.szsharing.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://al.nszjky.cn

[B11] 生成数字序列 / 区间
来源：http://lc.yuexingan06.cn

Py:   list(range(0, 10, 2))
来源：http://lb.panjiajie.cn

PHP:  range(0, 10, 2);
来源：http://yv.521024.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ii.szxytkj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://il.yuntaijiaju.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://du.nszjky.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sb.shxzskj.cn

Ruby: (0...10).step(2).to_a
来源：http://ch.haigaiapp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yl.yuntaijiaju.cn

[B12] 跳出多层循环
来源：http://td.gzmigu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://og.bookmarksfly.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://pr.chemitech.net.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vt.nszjky.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kn.huixinmuqiang.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vx.gzmigu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://md.nicolike.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://eg.nicolike.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kj.hnjuh.cn

[B13] 判断是否为数字
来源：http://pz.yuexingan06.cn

Py:   isinstance(x, (int, float))
来源：http://gh.wgjwhj.cn

PHP:  is_numeric($x)
来源：http://sc.huixiangedu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gv.hahajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rk.huixiangedu.cn

Java: x instanceof Number
来源：http://fk.chemitech.net.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cp.lnxyls.cn

Ruby: x.is_a?(Numeric)
来源：http://iy.lnxyls.cn

C#:   x is int or double or decimal
来源：http://ly.bjjhwx.cn

[B14] 判断值是否在集合内
来源：http://qs.huixiangedu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tv.colortex.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zv.szxytkj.cn

JS:   [1, 2, 3].includes(x)
来源：http://yt.hnjuh.cn

TS:   [1, 2, 3].includes(x)
来源：http://qv.newstarts.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://nu.yuntaijiaju.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://da.chemitech.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://an.newstarts.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://aj.huixinmuqiang.cn

[B15] 布尔运算与取反
来源：http://jc.colortex.cn

Py:   a and b or not c
来源：http://yv.bjjhwx.cn

PHP:  $a && $b || !$c
来源：http://nd.521024.cn

JS:   a && b || !c
来源：http://fk.szxytkj.cn

TS:   a && b || !c
来源：http://ne.huixiangedu.cn

Java: a && b || !c
来源：http://rb.lnxyls.cn

Go:   a && b || !c
来源：http://hl.szxytkj.cn

Ruby: a && b || !c
来源：http://dp.jctech888.com.cn

C#:   a && b || !c
来源：http://xi.haigaiapp.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ce.asd995.cn

Py:   if not data: return
来源：http://og.asd995.cn

PHP:  if (!$data) { return; }
来源：http://pa.nszjky.cn

JS:   if (!data) return;
来源：http://cj.521024.cn

TS:   if (!data) return;
来源：http://ge.huixinmuqiang.cn

Java: if (data == null) return;
来源：http://fb.colortex.cn

Go:   if data == nil { return }
来源：http://it.lnxyls.cn

Ruby: return if data.nil?
来源：http://cf.jctech888.com.cn

C#:   if (data == null) return;
来源：http://iz.gzmigu.cn

================================================================================
来源：http://tw.haigaiapp.cn

C. 函数与作用域
来源：http://es.jianghongdianzi.cn

================================================================================
来源：http://xx.panjiajie.cn

[C01] 定义函数
来源：http://ym.521024.cn

Py:   def add(a, b): return a + b
来源：http://hc.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vx.szxytkj.cn

JS:   function add(a, b) { return a + b; }
来源：http://su.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://am.hahajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vl.asd995.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mg.muxihuayi.cn

Ruby: def add(a, b); a + b; end
来源：http://zn.newstarts.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sg.521024.cn

[C02] 默认参数
来源：http://wa.szsharing.cn

Py:   def greet(name="World"): return name
来源：http://zp.huixinmuqiang.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hj.muxihuayi.cn

JS:   function greet(name = "World") { return name; }
来源：http://sl.gzmigu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vy.newstarts.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wy.yuntaijiaju.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fi.hahajie.cn

Ruby: def greet(name = "World") = name
来源：http://su.huixiangedu.cn

C#:   string Greet(string name = "World") => name;
来源：http://mk.newstarts.cn

[C03] 可变参数
来源：http://ab.huanxung.cn

Py:   def total(*args): return sum(args)
来源：http://pf.huixiangedu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pn.lnxyls.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sq.haigaiapp.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vt.asd995.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://or.shtwfgs.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://am.9csxet.cn

Ruby: def total(*nums); nums.sum; end
来源：http://im.chemitech.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://td.shtwfgs.cn

[C04] 命名参数 / 关键字参数
来源：http://yl.newstarts.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lr.hahajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://oq.9csxet.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ll.jctech888.com.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://br.asd995.cn

Java: // 无：用 Builder 模式或 record
来源：http://fw.muxihuayi.cn

Go:   // 无：用配置结构体参数
来源：http://au.colortex.cn

Ruby: f(a: 1, b: 2)
来源：http://ly.hnjuh.cn

C#:   f(a: 1, b: 2)
来源：http://vb.shxzskj.cn

[C05] 返回多个值
来源：http://ft.szxytkj.cn

Py:   return a, b
来源：http://pu.yuntaijiaju.cn

PHP:  return [$a, $b];
来源：http://ar.shxzukj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zn.gzmigu.cn

TS:   return { a, b };
来源：http://ko.shxzukj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qu.jctech888.com.cn

Go:   return a, b
来源：http://yq.hahajie.cn

Ruby: return a, b
来源：http://qx.szsharing.cn

C#:   return (a, b);              // ValueTuple
来源：http://ga.yuexingan06.cn

[C06] 匿名函数 / lambda
来源：http://yj.521024.cn

Py:   square = lambda x: x * x
来源：http://ed.wgjwhj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ok.shtwfgs.cn

JS:   const square = x => x * x;
来源：http://kf.gzmigu.cn

TS:   const square = (x: number): number => x * x;
来源：http://uv.gzmigu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xv.jianghongdianzi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ow.shtwfgs.cn

Ruby: square = ->(x) { x * x }
来源：http://ze.521024.cn

C#:   Func<int, int> square = x => x * x;
来源：http://nl.szxytkj.cn

[C07] 把函数作为参数传入
来源：http://nu.colortex.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fm.jianghongdianzi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ba.bjjhwx.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ud.bjjhwx.cn

TS:   arr.map(String)
来源：http://ny.shxzskj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pv.panjiajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ob.bjjhwx.cn

Ruby: arr.map(&:upcase)
来源：http://yk.nicolike.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gr.521024.cn

[C08] 闭包
来源：http://tc.shxzukj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xx.huixinmuqiang.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ro.jctech888.com.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kx.shtwfgs.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uk.nszjky.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bi.newstarts.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://iq.lnxyls.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cj.yuntaijiaju.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xt.muxihuayi.cn

[C09] 递归
来源：http://fl.huanxung.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kp.nszjky.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tz.shxzskj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://os.bjjhwx.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ol.huixinmuqiang.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ng.lnxyls.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://na.chemitech.net.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ww.huixiangedu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vo.gzmigu.cn

[C10] 变量作用域
来源：http://ro.shxzskj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bm.huixiangedu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ns.jctech888.com.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yy.huixiangedu.cn

TS:   同 JS
来源：http://fa.shtwfgs.cn

Java: 方法内为块级作用域
来源：http://zd.haigaiapp.cn

Go:   花括号块级作用域
来源：http://xn.yuntaijiaju.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ud.jctech888.com.cn

C#:   块级作用域
来源：http://hu.jianghongdianzi.cn

[C11] 模块导入与导出
来源：http://jo.colortex.cn

Py:   from module import func
来源：http://cj.colortex.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://oa.shxzskj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://yc.newstarts.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pc.haigaiapp.cn

Java: import java.util.List;
来源：http://xf.hahajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uv.yuntaijiaju.cn

Ruby: require "json"; require_relative "./util"
来源：http://ql.huixinmuqiang.cn

C#:   using System.Text;
来源：http://gc.asd995.cn

[C12] 立即执行函数 IIFE
来源：http://zq.nszjky.cn

Py:   (lambda: print("run"))()
来源：http://xy.newstarts.cn

PHP:  (function () { echo "run"; })();
来源：http://hk.lnxyls.cn

JS:   (() => { console.log("run"); })();
来源：http://yi.muxihuayi.cn

TS:   (() => { console.log("run"); })();
来源：http://ww.nicolike.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ww.521024.cn

Go:   func() { fmt.Println("run") }()
来源：http://ps.bookmarksfly.cn

Ruby: -> { puts "run" }.call
来源：http://ix.shxzskj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mx.huixinmuqiang.cn

[C13] 类型声明 / 类型注解
来源：http://vy.hnjuh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fq.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://en.colortex.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rm.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://aq.wgjwhj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://zk.chemitech.net.cn

Go:   func add(a, b int) int
来源：http://jw.nicolike.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ne.shxzukj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://sp.huixiangedu.cn

[C14] 泛型函数
来源：http://mh.9csxet.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://eb.lnxyls.cn

PHP:  // 无泛型
来源：http://su.szxytkj.cn

JS:   // 无泛型
来源：http://il.huixinmuqiang.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ef.asd995.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://me.newstarts.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xj.nicolike.cn

Ruby: # 无泛型
来源：http://rp.hnjuh.cn


<!-- 参考信息 -->