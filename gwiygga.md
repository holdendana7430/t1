代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hi.hahajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mc.haigaiapp.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ag.huixiangedu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mt.shxzskj.cn

Go:   strings.TrimSpace(s)
来源：http://cw.shxzskj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vz.nicolike.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sf.yuntaijiaju.cn

[A25] 字符串比较
来源：http://xr.bjjhwx.cn

Py:   s1 == s2; s1 != s2
来源：http://gj.9csxet.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://oe.huanxung.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ok.haigaiapp.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vk.bookmarksfly.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://eb.muxihuayi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wr.szxytkj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://zi.hahajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://uu.nszjky.cn

[A26] 类型转换总览
来源：http://la.haigaiapp.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://su.yuexingan06.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gv.asd995.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zp.bjjhwx.cn

TS:   Number() String() Boolean() x as number
来源：http://ol.gzmigu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nl.chemitech.net.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://be.muxihuayi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://dt.haigaiapp.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wx.521024.cn

================================================================================
来源：http://hi.huanxung.cn

B. 流程控制
来源：http://xe.shxzskj.cn

================================================================================
来源：http://mf.nszjky.cn

[B01] 条件判断 if / else
来源：http://nl.panjiajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://oz.bjjhwx.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gf.newstarts.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ic.hnjuh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://iq.gzmigu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://tm.haigaiapp.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dk.wgjwhj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ul.szsharing.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tq.huixiangedu.cn

[B02] 多分支 else if / elif
来源：http://ro.shtwfgs.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://eg.chemitech.net.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ah.gzmigu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ec.colortex.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uo.szxytkj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jw.nszjky.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ug.jianghongdianzi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wr.huixinmuqiang.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jg.szxytkj.cn

[B03] switch / match / case
来源：http://op.huixinmuqiang.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cd.nszjky.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uz.bookmarksfly.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gr.wgjwhj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bx.muxihuayi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ds.haigaiapp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ly.chemitech.net.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://oc.asd995.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xu.huixinmuqiang.cn

[B04] for 计数循环
来源：http://en.yuntaijiaju.cn

Py:   for i in range(10): print(i)
来源：http://ks.muxihuayi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://no.bookmarksfly.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vw.wgjwhj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://if.hnjuh.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pi.shtwfgs.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://uf.gzmigu.cn

Ruby: 10.times { |i| puts i }
来源：http://ml.newstarts.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://av.hnjuh.cn

[B05] 遍历数组 / 列表
来源：http://vr.shxzukj.cn

Py:   for item in arr: print(item)
来源：http://vu.shxzskj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tx.bjjhwx.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://mo.asd995.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xx.9csxet.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://th.szsharing.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rj.szxytkj.cn

Ruby: arr.each { |item| puts item }
来源：http://ll.shtwfgs.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qs.yuexingan06.cn

[B06] 遍历字典 / 对象
来源：http://md.colortex.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fl.shxzskj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rk.521024.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nf.9csxet.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nu.shxzskj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ll.haigaiapp.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://io.bjjhwx.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bq.szsharing.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://iq.haigaiapp.cn

[B07] while 循环
来源：http://aw.hahajie.cn

Py:   while i < 10: i += 1
来源：http://yg.nszjky.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ep.muxihuayi.cn

JS:   while (i < 10) { i++; }
来源：http://zc.lnxyls.cn

TS:   while (i < 10) { i++; }
来源：http://bd.shtwfgs.cn

Java: while (i < 10) { i++; }
来源：http://mi.lnxyls.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://be.521024.cn

Ruby: while i < 10; i += 1; end
来源：http://bs.szxytkj.cn

C#:   while (i < 10) { i++; }
来源：http://ln.szsharing.cn

[B08] do-while（至少执行一次）
来源：http://hf.panjiajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://be.shxzskj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pb.szxytkj.cn

JS:   do { i++; } while (i < 10);
来源：http://bn.521024.cn

TS:   do { i++; } while (i < 10);
来源：http://jo.9csxet.cn

Java: do { i++; } while (i < 10);
来源：http://wz.jianghongdianzi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ru.wgjwhj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jh.bjjhwx.cn

C#:   do { i++; } while (i < 10);
来源：http://ko.9csxet.cn

[B09] break 与 continue
来源：http://ux.shxzukj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bq.jianghongdianzi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wb.chemitech.net.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yw.szxytkj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pi.huixinmuqiang.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gl.newstarts.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mf.yuexingan06.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dy.newstarts.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vh.szxytkj.cn

[B10] 遍历同时拿索引
来源：http://kn.shtwfgs.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jq.haigaiapp.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qi.shxzukj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ro.shtwfgs.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mj.haigaiapp.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vn.huanxung.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hg.gzmigu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://be.shxzukj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ow.bjjhwx.cn

[B11] 生成数字序列 / 区间
来源：http://wo.muxihuayi.cn

Py:   list(range(0, 10, 2))
来源：http://ki.asd995.cn

PHP:  range(0, 10, 2);
来源：http://fs.shtwfgs.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qo.jctech888.com.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://it.huanxung.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mf.shtwfgs.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pu.yuexingan06.cn

Ruby: (0...10).step(2).to_a
来源：http://ii.yuexingan06.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zk.wgjwhj.cn

[B12] 跳出多层循环
来源：http://hb.newstarts.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ds.lnxyls.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://cq.bjjhwx.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ow.jianghongdianzi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wo.bjjhwx.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qy.jctech888.com.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sf.gzmigu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ss.wgjwhj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qh.shxzskj.cn

[B13] 判断是否为数字
来源：http://fu.chemitech.net.cn

Py:   isinstance(x, (int, float))
来源：http://nk.shtwfgs.cn

PHP:  is_numeric($x)
来源：http://ym.shxzskj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://go.hahajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xd.huixiangedu.cn

Java: x instanceof Number
来源：http://xz.shxzskj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://as.jctech888.com.cn

Ruby: x.is_a?(Numeric)
来源：http://ol.huanxung.cn

C#:   x is int or double or decimal
来源：http://zr.bjjhwx.cn

[B14] 判断值是否在集合内
来源：http://yt.521024.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lr.newstarts.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jl.jctech888.com.cn

JS:   [1, 2, 3].includes(x)
来源：http://qb.haigaiapp.cn

TS:   [1, 2, 3].includes(x)
来源：http://aw.colortex.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://nb.9csxet.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zv.haigaiapp.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ca.panjiajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jd.huixinmuqiang.cn

[B15] 布尔运算与取反
来源：http://xz.9csxet.cn

Py:   a and b or not c
来源：http://ci.wgjwhj.cn

PHP:  $a && $b || !$c
来源：http://cx.huanxung.cn

JS:   a && b || !c
来源：http://nl.hahajie.cn

TS:   a && b || !c
来源：http://hr.jianghongdianzi.cn

Java: a && b || !c
来源：http://jx.szxytkj.cn

Go:   a && b || !c
来源：http://mz.521024.cn

Ruby: a && b || !c
来源：http://wi.szxytkj.cn

C#:   a && b || !c
来源：http://nc.huixinmuqiang.cn

[B16] 卫语句：不满足条件提前返回
来源：http://no.hnjuh.cn

Py:   if not data: return
来源：http://kl.haigaiapp.cn

PHP:  if (!$data) { return; }
来源：http://dq.newstarts.cn

JS:   if (!data) return;
来源：http://tx.yuntaijiaju.cn

TS:   if (!data) return;
来源：http://aj.shxzukj.cn

Java: if (data == null) return;
来源：http://kb.newstarts.cn

Go:   if data == nil { return }
来源：http://jl.yuexingan06.cn

Ruby: return if data.nil?
来源：http://zu.nicolike.cn

C#:   if (data == null) return;
来源：http://ps.shtwfgs.cn

================================================================================
来源：http://af.muxihuayi.cn

C. 函数与作用域
来源：http://jc.nszjky.cn

================================================================================
来源：http://em.9csxet.cn

[C01] 定义函数
来源：http://ct.lnxyls.cn

Py:   def add(a, b): return a + b
来源：http://vc.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pl.huanxung.cn

JS:   function add(a, b) { return a + b; }
来源：http://fh.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tv.yuntaijiaju.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://rw.yuexingan06.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vj.shtwfgs.cn

Ruby: def add(a, b); a + b; end
来源：http://bp.szsharing.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tv.asd995.cn

[C02] 默认参数
来源：http://er.yuexingan06.cn

Py:   def greet(name="World"): return name
来源：http://bw.yuntaijiaju.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://mr.521024.cn

JS:   function greet(name = "World") { return name; }
来源：http://si.haigaiapp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://tg.haigaiapp.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rt.muxihuayi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://br.yuntaijiaju.cn

Ruby: def greet(name = "World") = name
来源：http://lu.lnxyls.cn

C#:   string Greet(string name = "World") => name;
来源：http://of.colortex.cn

[C03] 可变参数
来源：http://ub.haigaiapp.cn

Py:   def total(*args): return sum(args)
来源：http://ho.521024.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yk.yuexingan06.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ji.jianghongdianzi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fp.jctech888.com.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vb.panjiajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ui.haigaiapp.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xx.colortex.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gr.newstarts.cn

[C04] 命名参数 / 关键字参数
来源：http://yi.colortex.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ir.colortex.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rs.asd995.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fb.nszjky.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ow.bjjhwx.cn

Java: // 无：用 Builder 模式或 record
来源：http://ci.shtwfgs.cn

Go:   // 无：用配置结构体参数
来源：http://rw.chemitech.net.cn

Ruby: f(a: 1, b: 2)
来源：http://pv.hahajie.cn

C#:   f(a: 1, b: 2)
来源：http://yu.jianghongdianzi.cn

[C05] 返回多个值
来源：http://sy.szxytkj.cn

Py:   return a, b
来源：http://ng.bookmarksfly.cn

PHP:  return [$a, $b];
来源：http://nv.jctech888.com.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://rx.huixinmuqiang.cn

TS:   return { a, b };
来源：http://wj.hnjuh.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pf.szxytkj.cn

Go:   return a, b
来源：http://pd.jianghongdianzi.cn

Ruby: return a, b
来源：http://pz.bookmarksfly.cn

C#:   return (a, b);              // ValueTuple
来源：http://za.asd995.cn

[C06] 匿名函数 / lambda
来源：http://ib.hnjuh.cn

Py:   square = lambda x: x * x
来源：http://bo.huixiangedu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pe.muxihuayi.cn

JS:   const square = x => x * x;
来源：http://nt.521024.cn

TS:   const square = (x: number): number => x * x;
来源：http://dt.jianghongdianzi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nb.haigaiapp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kn.bjjhwx.cn

Ruby: square = ->(x) { x * x }
来源：http://uk.bjjhwx.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hs.huixiangedu.cn

[C07] 把函数作为参数传入
来源：http://iv.shxzukj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bn.newstarts.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vs.bjjhwx.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vu.9csxet.cn

TS:   arr.map(String)
来源：http://ra.asd995.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hh.huixinmuqiang.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fh.bjjhwx.cn

Ruby: arr.map(&:upcase)
来源：http://gq.huixiangedu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://uh.haigaiapp.cn

[C08] 闭包
来源：http://ln.muxihuayi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kd.521024.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ax.nicolike.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lt.szsharing.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xx.muxihuayi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://il.shxzukj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ns.bjjhwx.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ib.colortex.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://og.huanxung.cn

[C09] 递归
来源：http://by.haigaiapp.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yg.shxzukj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ok.huixiangedu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tk.jianghongdianzi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kh.huixiangedu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://it.chemitech.net.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://li.shxzukj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zo.9csxet.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ej.jianghongdianzi.cn

[C10] 变量作用域
来源：http://kd.asd995.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://se.huanxung.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cl.panjiajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dy.hnjuh.cn

TS:   同 JS
来源：http://kx.wgjwhj.cn

Java: 方法内为块级作用域
来源：http://mw.muxihuayi.cn

Go:   花括号块级作用域
来源：http://on.haigaiapp.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wy.hahajie.cn

C#:   块级作用域
来源：http://rh.yuntaijiaju.cn

[C11] 模块导入与导出
来源：http://ly.huixiangedu.cn

Py:   from module import func
来源：http://uv.haigaiapp.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hb.szxytkj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qm.szxytkj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kx.wgjwhj.cn

Java: import java.util.List;
来源：http://to.lnxyls.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tq.hahajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://ng.wgjwhj.cn

C#:   using System.Text;
来源：http://lc.szsharing.cn

[C12] 立即执行函数 IIFE
来源：http://xc.yuntaijiaju.cn

Py:   (lambda: print("run"))()
来源：http://zz.nicolike.cn

PHP:  (function () { echo "run"; })();
来源：http://pv.colortex.cn

JS:   (() => { console.log("run"); })();
来源：http://db.panjiajie.cn

TS:   (() => { console.log("run"); })();
来源：http://sj.bookmarksfly.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tz.bookmarksfly.cn

Go:   func() { fmt.Println("run") }()
来源：http://du.huixiangedu.cn

Ruby: -> { puts "run" }.call
来源：http://on.bookmarksfly.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://nf.asd995.cn

[C13] 类型声明 / 类型注解
来源：http://wy.huixiangedu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qw.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hw.shxzukj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mu.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pv.nszjky.cn

Java: int add(int a, int b) { return a + b; }
来源：http://th.chemitech.net.cn

Go:   func add(a, b int) int
来源：http://vq.hahajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mb.nszjky.cn

C#:   int Add(int a, int b) => a + b;
来源：http://sm.colortex.cn

[C14] 泛型函数
来源：http://rb.bjjhwx.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uu.jctech888.com.cn

PHP:  // 无泛型
来源：http://rt.hnjuh.cn

JS:   // 无泛型
来源：http://lg.shxzskj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qj.bookmarksfly.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rx.hahajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kp.shxzukj.cn

Ruby: # 无泛型
来源：http://uh.jianghongdianzi.cn


<!-- 参考信息 -->