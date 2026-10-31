代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ti.wgjwhj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qn.bjjhwx.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eh.gzmigu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qs.nszjky.cn

Go:   strings.TrimSpace(s)
来源：http://hz.yuntaijiaju.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://oi.yuntaijiaju.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mb.colortex.cn

[A25] 字符串比较
来源：http://fk.gzmigu.cn

Py:   s1 == s2; s1 != s2
来源：http://kw.shtwfgs.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rm.yuexingan06.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jq.huanxung.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://sx.colortex.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tk.huixinmuqiang.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://sk.yuntaijiaju.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://tw.nszjky.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dd.jctech888.com.cn

[A26] 类型转换总览
来源：http://zv.nszjky.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ts.shxzskj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fb.asd995.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bd.muxihuayi.cn

TS:   Number() String() Boolean() x as number
来源：http://dd.huixinmuqiang.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mm.521024.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ka.szxytkj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://wk.jctech888.com.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dd.yuntaijiaju.cn

================================================================================
来源：http://sx.lnxyls.cn

B. 流程控制
来源：http://ah.521024.cn

================================================================================
来源：http://ex.lnxyls.cn

[B01] 条件判断 if / else
来源：http://wd.panjiajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://sn.newstarts.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xz.nszjky.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ho.nicolike.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ja.chemitech.net.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://nl.lnxyls.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://no.bjjhwx.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zu.jctech888.com.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zt.yuexingan06.cn

[B02] 多分支 else if / elif
来源：http://zd.yuntaijiaju.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://io.shxzskj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kj.haigaiapp.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dj.newstarts.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lu.hahajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oo.huixiangedu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://th.wgjwhj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://sc.huixinmuqiang.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://an.muxihuayi.cn

[B03] switch / match / case
来源：http://mq.yuntaijiaju.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gn.shxzskj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jc.hahajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ao.asd995.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xr.nszjky.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rq.lnxyls.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dz.nszjky.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uu.panjiajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yk.muxihuayi.cn

[B04] for 计数循环
来源：http://vc.hahajie.cn

Py:   for i in range(10): print(i)
来源：http://av.yuntaijiaju.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zs.haigaiapp.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tj.wgjwhj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gm.nicolike.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xc.gzmigu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vu.bookmarksfly.cn

Ruby: 10.times { |i| puts i }
来源：http://pg.yuntaijiaju.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jf.shxzukj.cn

[B05] 遍历数组 / 列表
来源：http://wi.chemitech.net.cn

Py:   for item in arr: print(item)
来源：http://dq.wgjwhj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qu.yuexingan06.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://md.bookmarksfly.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://lb.shxzukj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jj.jctech888.com.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ds.huixinmuqiang.cn

Ruby: arr.each { |item| puts item }
来源：http://nq.wgjwhj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hc.colortex.cn

[B06] 遍历字典 / 对象
来源：http://zq.muxihuayi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xh.haigaiapp.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rz.colortex.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dn.jianghongdianzi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://na.shxzukj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hk.yuntaijiaju.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zr.jianghongdianzi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qv.huanxung.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kd.hnjuh.cn

[B07] while 循环
来源：http://qu.bookmarksfly.cn

Py:   while i < 10: i += 1
来源：http://fg.lnxyls.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qb.chemitech.net.cn

JS:   while (i < 10) { i++; }
来源：http://jw.jctech888.com.cn

TS:   while (i < 10) { i++; }
来源：http://pa.huixiangedu.cn

Java: while (i < 10) { i++; }
来源：http://uf.szsharing.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://is.hnjuh.cn

Ruby: while i < 10; i += 1; end
来源：http://yv.bookmarksfly.cn

C#:   while (i < 10) { i++; }
来源：http://bs.jianghongdianzi.cn

[B08] do-while（至少执行一次）
来源：http://ck.newstarts.cn

Py:   # 无 do-while：用 while True + break
来源：http://iu.szsharing.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ui.muxihuayi.cn

JS:   do { i++; } while (i < 10);
来源：http://op.newstarts.cn

TS:   do { i++; } while (i < 10);
来源：http://qx.colortex.cn

Java: do { i++; } while (i < 10);
来源：http://gj.newstarts.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://zk.newstarts.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rg.huixiangedu.cn

C#:   do { i++; } while (i < 10);
来源：http://pn.wgjwhj.cn

[B09] break 与 continue
来源：http://vi.huixiangedu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ty.jianghongdianzi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rt.chemitech.net.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hg.asd995.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yp.asd995.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rh.asd995.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ff.chemitech.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wk.huanxung.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ea.huanxung.cn

[B10] 遍历同时拿索引
来源：http://lm.lnxyls.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tg.bjjhwx.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://eg.haigaiapp.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ma.yuexingan06.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xh.hnjuh.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://di.bookmarksfly.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yn.panjiajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rt.shxzukj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://se.szxytkj.cn

[B11] 生成数字序列 / 区间
来源：http://yh.jianghongdianzi.cn

Py:   list(range(0, 10, 2))
来源：http://im.asd995.cn

PHP:  range(0, 10, 2);
来源：http://tj.9csxet.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pz.nszjky.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pn.jianghongdianzi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ps.hnjuh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sn.yuntaijiaju.cn

Ruby: (0...10).step(2).to_a
来源：http://se.szsharing.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://br.huixinmuqiang.cn

[B12] 跳出多层循环
来源：http://pg.colortex.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://gv.nicolike.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wy.muxihuayi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ux.wgjwhj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ie.gzmigu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wy.shxzukj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qf.bjjhwx.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wl.panjiajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mw.wgjwhj.cn

[B13] 判断是否为数字
来源：http://ws.gzmigu.cn

Py:   isinstance(x, (int, float))
来源：http://qc.huixinmuqiang.cn

PHP:  is_numeric($x)
来源：http://wh.yuntaijiaju.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cc.nicolike.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jm.wgjwhj.cn

Java: x instanceof Number
来源：http://zn.shtwfgs.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vm.asd995.cn

Ruby: x.is_a?(Numeric)
来源：http://vm.521024.cn

C#:   x is int or double or decimal
来源：http://kr.shxzukj.cn

[B14] 判断值是否在集合内
来源：http://gl.9csxet.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ch.huanxung.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ak.shtwfgs.cn

JS:   [1, 2, 3].includes(x)
来源：http://yp.9csxet.cn

TS:   [1, 2, 3].includes(x)
来源：http://ry.bjjhwx.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://pt.asd995.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qa.nszjky.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vi.newstarts.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ui.521024.cn

[B15] 布尔运算与取反
来源：http://rb.yuntaijiaju.cn

Py:   a and b or not c
来源：http://yh.asd995.cn

PHP:  $a && $b || !$c
来源：http://ks.yuntaijiaju.cn

JS:   a && b || !c
来源：http://qj.jianghongdianzi.cn

TS:   a && b || !c
来源：http://ep.nicolike.cn

Java: a && b || !c
来源：http://ka.nicolike.cn

Go:   a && b || !c
来源：http://mh.shxzukj.cn

Ruby: a && b || !c
来源：http://tp.haigaiapp.cn

C#:   a && b || !c
来源：http://fe.asd995.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ot.jctech888.com.cn

Py:   if not data: return
来源：http://yn.jctech888.com.cn

PHP:  if (!$data) { return; }
来源：http://bu.hahajie.cn

JS:   if (!data) return;
来源：http://cn.szsharing.cn

TS:   if (!data) return;
来源：http://he.shxzukj.cn

Java: if (data == null) return;
来源：http://ns.szxytkj.cn

Go:   if data == nil { return }
来源：http://be.gzmigu.cn

Ruby: return if data.nil?
来源：http://yz.haigaiapp.cn

C#:   if (data == null) return;
来源：http://ya.szsharing.cn

================================================================================
来源：http://mm.gzmigu.cn

C. 函数与作用域
来源：http://ht.yuntaijiaju.cn

================================================================================
来源：http://ej.haigaiapp.cn

[C01] 定义函数
来源：http://mw.shxzukj.cn

Py:   def add(a, b): return a + b
来源：http://tf.muxihuayi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pq.yuntaijiaju.cn

JS:   function add(a, b) { return a + b; }
来源：http://gr.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://at.hahajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xm.yuexingan06.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ab.shxzukj.cn

Ruby: def add(a, b); a + b; end
来源：http://po.yuexingan06.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yc.hnjuh.cn

[C02] 默认参数
来源：http://ob.shxzukj.cn

Py:   def greet(name="World"): return name
来源：http://dg.lnxyls.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ru.hnjuh.cn

JS:   function greet(name = "World") { return name; }
来源：http://qj.hnjuh.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://jj.szxytkj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cm.colortex.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vr.lnxyls.cn

Ruby: def greet(name = "World") = name
来源：http://wj.muxihuayi.cn

C#:   string Greet(string name = "World") => name;
来源：http://sm.panjiajie.cn

[C03] 可变参数
来源：http://en.bjjhwx.cn

Py:   def total(*args): return sum(args)
来源：http://ye.haigaiapp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qt.newstarts.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://uq.huixinmuqiang.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://an.shtwfgs.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ez.wgjwhj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vp.shxzukj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fb.szsharing.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yr.panjiajie.cn

[C04] 命名参数 / 关键字参数
来源：http://ba.nszjky.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mh.yuntaijiaju.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://an.nszjky.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bw.newstarts.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zn.yuntaijiaju.cn

Java: // 无：用 Builder 模式或 record
来源：http://xq.9csxet.cn

Go:   // 无：用配置结构体参数
来源：http://kg.huixinmuqiang.cn

Ruby: f(a: 1, b: 2)
来源：http://or.lnxyls.cn

C#:   f(a: 1, b: 2)
来源：http://jr.9csxet.cn

[C05] 返回多个值
来源：http://ru.wgjwhj.cn

Py:   return a, b
来源：http://zn.szsharing.cn

PHP:  return [$a, $b];
来源：http://wz.asd995.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://oa.chemitech.net.cn

TS:   return { a, b };
来源：http://hm.shtwfgs.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vs.yuntaijiaju.cn

Go:   return a, b
来源：http://rl.hnjuh.cn

Ruby: return a, b
来源：http://rd.lnxyls.cn

C#:   return (a, b);              // ValueTuple
来源：http://oo.szsharing.cn

[C06] 匿名函数 / lambda
来源：http://qn.jctech888.com.cn

Py:   square = lambda x: x * x
来源：http://cq.9csxet.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ky.muxihuayi.cn

JS:   const square = x => x * x;
来源：http://su.bjjhwx.cn

TS:   const square = (x: number): number => x * x;
来源：http://cu.jctech888.com.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ps.jianghongdianzi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zz.chemitech.net.cn

Ruby: square = ->(x) { x * x }
来源：http://fu.nicolike.cn

C#:   Func<int, int> square = x => x * x;
来源：http://gz.hahajie.cn

[C07] 把函数作为参数传入
来源：http://nr.hnjuh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fd.lnxyls.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hz.haigaiapp.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bx.jianghongdianzi.cn

TS:   arr.map(String)
来源：http://na.huixinmuqiang.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ps.asd995.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pt.szsharing.cn

Ruby: arr.map(&:upcase)
来源：http://cr.yuntaijiaju.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ie.shtwfgs.cn

[C08] 闭包
来源：http://of.nszjky.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ya.jianghongdianzi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gs.521024.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://um.muxihuayi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ne.nszjky.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zn.chemitech.net.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kx.shtwfgs.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gm.shxzskj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ip.shxzskj.cn

[C09] 递归
来源：http://eh.521024.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://td.lnxyls.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://am.nszjky.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cv.9csxet.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ux.lnxyls.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ji.szsharing.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ta.521024.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://eg.shtwfgs.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fw.jianghongdianzi.cn

[C10] 变量作用域
来源：http://ph.hahajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sl.521024.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kv.haigaiapp.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ku.haigaiapp.cn

TS:   同 JS
来源：http://lb.bookmarksfly.cn

Java: 方法内为块级作用域
来源：http://is.huixiangedu.cn

Go:   花括号块级作用域
来源：http://dr.huanxung.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kh.hahajie.cn

C#:   块级作用域
来源：http://gp.jctech888.com.cn

[C11] 模块导入与导出
来源：http://gj.shxzskj.cn

Py:   from module import func
来源：http://tz.szxytkj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://fa.nicolike.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kz.bjjhwx.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lw.yuexingan06.cn

Java: import java.util.List;
来源：http://vi.shxzskj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wz.asd995.cn

Ruby: require "json"; require_relative "./util"
来源：http://bt.wgjwhj.cn

C#:   using System.Text;
来源：http://kq.muxihuayi.cn

[C12] 立即执行函数 IIFE
来源：http://wd.huixiangedu.cn

Py:   (lambda: print("run"))()
来源：http://bm.hahajie.cn

PHP:  (function () { echo "run"; })();
来源：http://ej.yuexingan06.cn

JS:   (() => { console.log("run"); })();
来源：http://zm.haigaiapp.cn

TS:   (() => { console.log("run"); })();
来源：http://xp.colortex.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cs.newstarts.cn

Go:   func() { fmt.Println("run") }()
来源：http://sh.huanxung.cn

Ruby: -> { puts "run" }.call
来源：http://zu.colortex.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://np.shxzskj.cn

[C13] 类型声明 / 类型注解
来源：http://la.jianghongdianzi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kb.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ag.yuexingan06.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ew.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lz.muxihuayi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://bv.shxzukj.cn

Go:   func add(a, b int) int
来源：http://du.bjjhwx.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fo.gzmigu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://jc.yuexingan06.cn

[C14] 泛型函数
来源：http://oz.gzmigu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fx.muxihuayi.cn

PHP:  // 无泛型
来源：http://bl.chemitech.net.cn

JS:   // 无泛型
来源：http://oi.jianghongdianzi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rd.521024.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ka.shxzukj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ji.wgjwhj.cn

Ruby: # 无泛型
来源：http://av.shxzskj.cn


<!-- 参考信息 -->