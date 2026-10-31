代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pa.shxzskj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jh.shtwfgs.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oz.newstarts.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mh.hnjuh.cn

Go:   strings.TrimSpace(s)
来源：http://sl.huixiangedu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rz.huanxung.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ha.nszjky.cn

[A25] 字符串比较
来源：http://af.chemitech.net.cn

Py:   s1 == s2; s1 != s2
来源：http://nx.nszjky.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jq.szsharing.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://uv.szsharing.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zx.huanxung.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zn.panjiajie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://eb.haigaiapp.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ed.huanxung.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fe.521024.cn

[A26] 类型转换总览
来源：http://qp.panjiajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://iq.yuntaijiaju.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pm.nicolike.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ym.newstarts.cn

TS:   Number() String() Boolean() x as number
来源：http://ha.shxzskj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nj.haigaiapp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kk.jctech888.com.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zl.nszjky.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qo.panjiajie.cn

================================================================================
来源：http://ea.hnjuh.cn

B. 流程控制
来源：http://zi.huixinmuqiang.cn

================================================================================
来源：http://qh.521024.cn

[B01] 条件判断 if / else
来源：http://ks.jctech888.com.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xr.9csxet.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xz.9csxet.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ss.shxzukj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sw.haigaiapp.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://kt.jctech888.com.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jz.lnxyls.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://at.jctech888.com.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://li.szxytkj.cn

[B02] 多分支 else if / elif
来源：http://sb.gzmigu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fi.shxzukj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lf.hahajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eo.bjjhwx.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fj.yuexingan06.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xy.muxihuayi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yb.szsharing.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://oe.hnjuh.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yy.yuntaijiaju.cn

[B03] switch / match / case
来源：http://sp.hahajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wn.shxzukj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://li.bjjhwx.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xg.chemitech.net.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ra.newstarts.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xk.shtwfgs.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ls.jctech888.com.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://em.szxytkj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://su.hnjuh.cn

[B04] for 计数循环
来源：http://wf.muxihuayi.cn

Py:   for i in range(10): print(i)
来源：http://ap.haigaiapp.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://eg.huixinmuqiang.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sr.huanxung.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://la.bjjhwx.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://az.nicolike.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gi.huixiangedu.cn

Ruby: 10.times { |i| puts i }
来源：http://bo.nszjky.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hd.jianghongdianzi.cn

[B05] 遍历数组 / 列表
来源：http://rv.9csxet.cn

Py:   for item in arr: print(item)
来源：http://vf.hahajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://po.chemitech.net.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://mi.521024.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://uf.haigaiapp.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vv.yuntaijiaju.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rj.jctech888.com.cn

Ruby: arr.each { |item| puts item }
来源：http://go.huixinmuqiang.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yg.gzmigu.cn

[B06] 遍历字典 / 对象
来源：http://es.haigaiapp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pe.jianghongdianzi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fh.gzmigu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ii.hnjuh.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tw.nicolike.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tp.haigaiapp.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vn.huixiangedu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ux.huanxung.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pd.lnxyls.cn

[B07] while 循环
来源：http://ds.yuntaijiaju.cn

Py:   while i < 10: i += 1
来源：http://kb.shtwfgs.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lw.521024.cn

JS:   while (i < 10) { i++; }
来源：http://zn.jianghongdianzi.cn

TS:   while (i < 10) { i++; }
来源：http://yp.shxzskj.cn

Java: while (i < 10) { i++; }
来源：http://dm.yuexingan06.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jq.panjiajie.cn

Ruby: while i < 10; i += 1; end
来源：http://yo.jianghongdianzi.cn

C#:   while (i < 10) { i++; }
来源：http://ik.yuntaijiaju.cn

[B08] do-while（至少执行一次）
来源：http://zj.shxzskj.cn

Py:   # 无 do-while：用 while True + break
来源：http://zl.yuexingan06.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://wd.huixinmuqiang.cn

JS:   do { i++; } while (i < 10);
来源：http://dd.hahajie.cn

TS:   do { i++; } while (i < 10);
来源：http://ki.huanxung.cn

Java: do { i++; } while (i < 10);
来源：http://nm.shxzskj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xg.muxihuayi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mo.szxytkj.cn

C#:   do { i++; } while (i < 10);
来源：http://pn.szxytkj.cn

[B09] break 与 continue
来源：http://ue.panjiajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://om.newstarts.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zk.lnxyls.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://di.jianghongdianzi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ga.bookmarksfly.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wd.shxzskj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zq.shtwfgs.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jr.bookmarksfly.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rh.wgjwhj.cn

[B10] 遍历同时拿索引
来源：http://yw.shxzskj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zb.panjiajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ag.gzmigu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mn.colortex.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rr.hnjuh.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yv.521024.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ye.newstarts.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ah.shtwfgs.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lw.nszjky.cn

[B11] 生成数字序列 / 区间
来源：http://vn.huanxung.cn

Py:   list(range(0, 10, 2))
来源：http://bi.521024.cn

PHP:  range(0, 10, 2);
来源：http://yq.yuexingan06.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lc.jctech888.com.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bj.wgjwhj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vg.wgjwhj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xp.yuntaijiaju.cn

Ruby: (0...10).step(2).to_a
来源：http://ei.szxytkj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pc.szsharing.cn

[B12] 跳出多层循环
来源：http://vh.bookmarksfly.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pm.nszjky.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ot.colortex.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://py.nszjky.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gc.shxzukj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hl.panjiajie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ij.bookmarksfly.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ay.huanxung.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://po.yuexingan06.cn

[B13] 判断是否为数字
来源：http://uj.9csxet.cn

Py:   isinstance(x, (int, float))
来源：http://no.nszjky.cn

PHP:  is_numeric($x)
来源：http://rq.nicolike.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://op.szxytkj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ix.yuexingan06.cn

Java: x instanceof Number
来源：http://br.521024.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yk.panjiajie.cn

Ruby: x.is_a?(Numeric)
来源：http://oh.9csxet.cn

C#:   x is int or double or decimal
来源：http://ga.hnjuh.cn

[B14] 判断值是否在集合内
来源：http://jq.lnxyls.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xq.muxihuayi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ou.szsharing.cn

JS:   [1, 2, 3].includes(x)
来源：http://pg.muxihuayi.cn

TS:   [1, 2, 3].includes(x)
来源：http://gx.haigaiapp.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dj.panjiajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yw.shxzskj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cz.nicolike.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jx.yuntaijiaju.cn

[B15] 布尔运算与取反
来源：http://db.9csxet.cn

Py:   a and b or not c
来源：http://zv.muxihuayi.cn

PHP:  $a && $b || !$c
来源：http://sa.newstarts.cn

JS:   a && b || !c
来源：http://ix.newstarts.cn

TS:   a && b || !c
来源：http://bm.bjjhwx.cn

Java: a && b || !c
来源：http://wp.nszjky.cn

Go:   a && b || !c
来源：http://vc.521024.cn

Ruby: a && b || !c
来源：http://zj.nicolike.cn

C#:   a && b || !c
来源：http://bu.chemitech.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vt.asd995.cn

Py:   if not data: return
来源：http://em.shxzukj.cn

PHP:  if (!$data) { return; }
来源：http://cb.hahajie.cn

JS:   if (!data) return;
来源：http://xd.panjiajie.cn

TS:   if (!data) return;
来源：http://tb.yuntaijiaju.cn

Java: if (data == null) return;
来源：http://lt.huixinmuqiang.cn

Go:   if data == nil { return }
来源：http://wj.szsharing.cn

Ruby: return if data.nil?
来源：http://zw.muxihuayi.cn

C#:   if (data == null) return;
来源：http://xr.9csxet.cn

================================================================================
来源：http://ic.colortex.cn

C. 函数与作用域
来源：http://dd.hnjuh.cn

================================================================================
来源：http://cs.521024.cn

[C01] 定义函数
来源：http://io.gzmigu.cn

Py:   def add(a, b): return a + b
来源：http://lw.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ic.9csxet.cn

JS:   function add(a, b) { return a + b; }
来源：http://by.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zc.hnjuh.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://im.521024.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ui.hnjuh.cn

Ruby: def add(a, b); a + b; end
来源：http://jv.gzmigu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ey.bjjhwx.cn

[C02] 默认参数
来源：http://mc.chemitech.net.cn

Py:   def greet(name="World"): return name
来源：http://vv.lnxyls.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://la.jctech888.com.cn

JS:   function greet(name = "World") { return name; }
来源：http://yo.bjjhwx.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ed.shxzukj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ev.shxzskj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fb.shtwfgs.cn

Ruby: def greet(name = "World") = name
来源：http://tr.huixinmuqiang.cn

C#:   string Greet(string name = "World") => name;
来源：http://gu.gzmigu.cn

[C03] 可变参数
来源：http://jk.newstarts.cn

Py:   def total(*args): return sum(args)
来源：http://fm.jianghongdianzi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yr.muxihuayi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fd.yuntaijiaju.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pi.panjiajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wo.szsharing.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vb.huixiangedu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wi.yuntaijiaju.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gp.gzmigu.cn

[C04] 命名参数 / 关键字参数
来源：http://ap.bjjhwx.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xf.nicolike.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qe.bookmarksfly.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yg.bjjhwx.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rw.yuexingan06.cn

Java: // 无：用 Builder 模式或 record
来源：http://ex.newstarts.cn

Go:   // 无：用配置结构体参数
来源：http://zp.shtwfgs.cn

Ruby: f(a: 1, b: 2)
来源：http://rc.hnjuh.cn

C#:   f(a: 1, b: 2)
来源：http://qh.yuntaijiaju.cn

[C05] 返回多个值
来源：http://yk.asd995.cn

Py:   return a, b
来源：http://oa.colortex.cn

PHP:  return [$a, $b];
来源：http://vn.asd995.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qu.hnjuh.cn

TS:   return { a, b };
来源：http://em.shtwfgs.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://on.chemitech.net.cn

Go:   return a, b
来源：http://rk.hahajie.cn

Ruby: return a, b
来源：http://ji.lnxyls.cn

C#:   return (a, b);              // ValueTuple
来源：http://gg.hahajie.cn

[C06] 匿名函数 / lambda
来源：http://qr.nicolike.cn

Py:   square = lambda x: x * x
来源：http://pg.chemitech.net.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://au.9csxet.cn

JS:   const square = x => x * x;
来源：http://ir.nszjky.cn

TS:   const square = (x: number): number => x * x;
来源：http://ne.shtwfgs.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pd.szxytkj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://oz.yuntaijiaju.cn

Ruby: square = ->(x) { x * x }
来源：http://lx.asd995.cn

C#:   Func<int, int> square = x => x * x;
来源：http://kb.huixiangedu.cn

[C07] 把函数作为参数传入
来源：http://az.huixiangedu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://uu.hahajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://js.bjjhwx.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://up.chemitech.net.cn

TS:   arr.map(String)
来源：http://sf.chemitech.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://eg.nszjky.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wd.newstarts.cn

Ruby: arr.map(&:upcase)
来源：http://wk.wgjwhj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fl.huixinmuqiang.cn

[C08] 闭包
来源：http://mz.haigaiapp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fd.haigaiapp.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vk.shxzukj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rd.szxytkj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cf.newstarts.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lh.shxzukj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ev.shxzukj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ff.asd995.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ti.lnxyls.cn

[C09] 递归
来源：http://ne.nszjky.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zt.9csxet.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://aa.9csxet.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qg.huixinmuqiang.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hw.newstarts.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pp.jianghongdianzi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qf.jianghongdianzi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yl.yuntaijiaju.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tb.jianghongdianzi.cn

[C10] 变量作用域
来源：http://dn.haigaiapp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mu.huixinmuqiang.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wg.asd995.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yv.huanxung.cn

TS:   同 JS
来源：http://mm.shxzukj.cn

Java: 方法内为块级作用域
来源：http://qr.521024.cn

Go:   花括号块级作用域
来源：http://xf.panjiajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vp.huixinmuqiang.cn

C#:   块级作用域
来源：http://pn.jctech888.com.cn

[C11] 模块导入与导出
来源：http://ad.huixiangedu.cn

Py:   from module import func
来源：http://el.nicolike.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://fs.yuexingan06.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://mc.wgjwhj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kg.haigaiapp.cn

Java: import java.util.List;
来源：http://dr.chemitech.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ah.newstarts.cn

Ruby: require "json"; require_relative "./util"
来源：http://av.shxzskj.cn

C#:   using System.Text;
来源：http://cw.jianghongdianzi.cn

[C12] 立即执行函数 IIFE
来源：http://xg.haigaiapp.cn

Py:   (lambda: print("run"))()
来源：http://ha.szxytkj.cn

PHP:  (function () { echo "run"; })();
来源：http://vi.521024.cn

JS:   (() => { console.log("run"); })();
来源：http://tj.lnxyls.cn

TS:   (() => { console.log("run"); })();
来源：http://pu.shtwfgs.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pb.jctech888.com.cn

Go:   func() { fmt.Println("run") }()
来源：http://ek.newstarts.cn

Ruby: -> { puts "run" }.call
来源：http://fk.jianghongdianzi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zz.shtwfgs.cn

[C13] 类型声明 / 类型注解
来源：http://qp.huixiangedu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rl.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ut.bookmarksfly.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wc.panjiajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hj.szsharing.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ie.jianghongdianzi.cn

Go:   func add(a, b int) int
来源：http://nb.hahajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ay.colortex.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bi.szsharing.cn

[C14] 泛型函数
来源：http://lg.szxytkj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ib.hnjuh.cn

PHP:  // 无泛型
来源：http://zx.bjjhwx.cn

JS:   // 无泛型
来源：http://ut.9csxet.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://df.huixiangedu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://iw.huixiangedu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yx.shtwfgs.cn

Ruby: # 无泛型
来源：http://yb.nicolike.cn


<!-- 参考信息 -->