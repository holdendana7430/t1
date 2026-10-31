代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://ab.yuntaijiaju.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gh.shxzskj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://he.shtwfgs.cn

[A25] 字符串比较
来源：http://wk.wgjwhj.cn

Py:   s1 == s2; s1 != s2
来源：http://wj.yuntaijiaju.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tf.haigaiapp.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fv.nicolike.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cf.521024.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gw.newstarts.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://se.shtwfgs.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://lq.szxytkj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ud.nicolike.cn

[A26] 类型转换总览
来源：http://fj.shxzukj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ep.gzmigu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bc.yuexingan06.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hf.jianghongdianzi.cn

TS:   Number() String() Boolean() x as number
来源：http://un.lnxyls.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bo.9csxet.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://za.nszjky.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://yk.yuexingan06.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://je.wgjwhj.cn

================================================================================
来源：http://km.huixiangedu.cn

B. 流程控制
来源：http://zf.szxytkj.cn

================================================================================
来源：http://ib.haigaiapp.cn

[B01] 条件判断 if / else
来源：http://fo.shxzskj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://qn.shxzskj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zq.hnjuh.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://th.asd995.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://aw.nszjky.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://zb.nszjky.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qh.szsharing.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bi.szxytkj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jk.shxzukj.cn

[B02] 多分支 else if / elif
来源：http://rc.wgjwhj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bm.haigaiapp.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xy.huixinmuqiang.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eq.bookmarksfly.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://am.yuexingan06.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://je.newstarts.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qv.gzmigu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://oo.9csxet.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mm.jctech888.com.cn

[B03] switch / match / case
来源：http://pd.huixiangedu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cp.szxytkj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yz.nicolike.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ua.hnjuh.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nz.huixinmuqiang.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gy.shxzukj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://aa.yuexingan06.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ia.colortex.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ze.szxytkj.cn

[B04] for 计数循环
来源：http://ib.muxihuayi.cn

Py:   for i in range(10): print(i)
来源：http://vv.newstarts.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xz.chemitech.net.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bh.muxihuayi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ki.jctech888.com.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uc.shxzukj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gq.haigaiapp.cn

Ruby: 10.times { |i| puts i }
来源：http://xs.hnjuh.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ha.huixinmuqiang.cn

[B05] 遍历数组 / 列表
来源：http://ow.bjjhwx.cn

Py:   for item in arr: print(item)
来源：http://lm.jctech888.com.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cx.521024.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://le.shtwfgs.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://dl.yuexingan06.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://kx.bookmarksfly.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hf.jctech888.com.cn

Ruby: arr.each { |item| puts item }
来源：http://nc.shxzskj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xu.shxzskj.cn

[B06] 遍历字典 / 对象
来源：http://qo.szsharing.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ir.haigaiapp.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ur.521024.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://la.szxytkj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gy.shtwfgs.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xr.shtwfgs.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://er.hahajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dk.bookmarksfly.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tb.chemitech.net.cn

[B07] while 循环
来源：http://xs.wgjwhj.cn

Py:   while i < 10: i += 1
来源：http://pr.lnxyls.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ss.jianghongdianzi.cn

JS:   while (i < 10) { i++; }
来源：http://jk.haigaiapp.cn

TS:   while (i < 10) { i++; }
来源：http://wo.panjiajie.cn

Java: while (i < 10) { i++; }
来源：http://zr.haigaiapp.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jv.huixiangedu.cn

Ruby: while i < 10; i += 1; end
来源：http://ty.colortex.cn

C#:   while (i < 10) { i++; }
来源：http://jy.jctech888.com.cn

[B08] do-while（至少执行一次）
来源：http://bq.jianghongdianzi.cn

Py:   # 无 do-while：用 while True + break
来源：http://zi.panjiajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vk.newstarts.cn

JS:   do { i++; } while (i < 10);
来源：http://nq.newstarts.cn

TS:   do { i++; } while (i < 10);
来源：http://nz.jctech888.com.cn

Java: do { i++; } while (i < 10);
来源：http://ar.nicolike.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://kn.haigaiapp.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rd.lnxyls.cn

C#:   do { i++; } while (i < 10);
来源：http://dp.9csxet.cn

[B09] break 与 continue
来源：http://tv.asd995.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lf.wgjwhj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xj.bookmarksfly.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vx.shxzukj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kz.nszjky.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uv.nicolike.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xz.colortex.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pq.wgjwhj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hg.muxihuayi.cn

[B10] 遍历同时拿索引
来源：http://cl.szsharing.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nm.haigaiapp.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://eh.521024.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ym.haigaiapp.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fn.jctech888.com.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ug.huanxung.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://po.9csxet.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sc.panjiajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://og.colortex.cn

[B11] 生成数字序列 / 区间
来源：http://jw.panjiajie.cn

Py:   list(range(0, 10, 2))
来源：http://fr.9csxet.cn

PHP:  range(0, 10, 2);
来源：http://to.nicolike.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kz.haigaiapp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rw.shxzskj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lm.nszjky.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xe.9csxet.cn

Ruby: (0...10).step(2).to_a
来源：http://ig.muxihuayi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mb.nicolike.cn

[B12] 跳出多层循环
来源：http://ib.huixiangedu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://iu.colortex.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://id.jianghongdianzi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bp.wgjwhj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xr.nicolike.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tn.hnjuh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://oj.szxytkj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lo.haigaiapp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gt.shtwfgs.cn

[B13] 判断是否为数字
来源：http://jy.chemitech.net.cn

Py:   isinstance(x, (int, float))
来源：http://lo.nicolike.cn

PHP:  is_numeric($x)
来源：http://sg.hnjuh.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rd.yuexingan06.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jb.wgjwhj.cn

Java: x instanceof Number
来源：http://eu.yuexingan06.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nq.hahajie.cn

Ruby: x.is_a?(Numeric)
来源：http://kz.hnjuh.cn

C#:   x is int or double or decimal
来源：http://ge.jctech888.com.cn

[B14] 判断值是否在集合内
来源：http://it.521024.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://me.panjiajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vi.gzmigu.cn

JS:   [1, 2, 3].includes(x)
来源：http://fe.huixiangedu.cn

TS:   [1, 2, 3].includes(x)
来源：http://hj.szsharing.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://fx.haigaiapp.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xo.yuntaijiaju.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ov.yuntaijiaju.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jianghongdianzi.cn

[B15] 布尔运算与取反
来源：http://cq.chemitech.net.cn

Py:   a and b or not c
来源：http://xj.szsharing.cn

PHP:  $a && $b || !$c
来源：http://ho.yuntaijiaju.cn

JS:   a && b || !c
来源：http://ws.hahajie.cn

TS:   a && b || !c
来源：http://iq.colortex.cn

Java: a && b || !c
来源：http://ri.haigaiapp.cn

Go:   a && b || !c
来源：http://jx.shtwfgs.cn

Ruby: a && b || !c
来源：http://sr.bookmarksfly.cn

C#:   a && b || !c
来源：http://ib.muxihuayi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ke.chemitech.net.cn

Py:   if not data: return
来源：http://hv.wgjwhj.cn

PHP:  if (!$data) { return; }
来源：http://vk.yuexingan06.cn

JS:   if (!data) return;
来源：http://fi.szxytkj.cn

TS:   if (!data) return;
来源：http://mt.szxytkj.cn

Java: if (data == null) return;
来源：http://oz.newstarts.cn

Go:   if data == nil { return }
来源：http://hc.jctech888.com.cn

Ruby: return if data.nil?
来源：http://go.nicolike.cn

C#:   if (data == null) return;
来源：http://kt.lnxyls.cn

================================================================================
来源：http://ys.bjjhwx.cn

C. 函数与作用域
来源：http://sl.szsharing.cn

================================================================================
来源：http://sm.hnjuh.cn

[C01] 定义函数
来源：http://oy.lnxyls.cn

Py:   def add(a, b): return a + b
来源：http://gn.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vk.huanxung.cn

JS:   function add(a, b) { return a + b; }
来源：http://jb.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jx.wgjwhj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dj.9csxet.cn

Go:   func add(a, b int) int { return a + b }
来源：http://pc.huixinmuqiang.cn

Ruby: def add(a, b); a + b; end
来源：http://pm.nszjky.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kv.shxzukj.cn

[C02] 默认参数
来源：http://kg.hahajie.cn

Py:   def greet(name="World"): return name
来源：http://qc.muxihuayi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yk.jctech888.com.cn

JS:   function greet(name = "World") { return name; }
来源：http://iy.bjjhwx.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cn.nszjky.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ay.jianghongdianzi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://re.asd995.cn

Ruby: def greet(name = "World") = name
来源：http://jq.szsharing.cn

C#:   string Greet(string name = "World") => name;
来源：http://fa.jianghongdianzi.cn

[C03] 可变参数
来源：http://zi.asd995.cn

Py:   def total(*args): return sum(args)
来源：http://gd.yuexingan06.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qa.jctech888.com.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qc.newstarts.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jb.gzmigu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://oc.521024.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fm.chemitech.net.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pr.bjjhwx.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rj.haigaiapp.cn

[C04] 命名参数 / 关键字参数
来源：http://is.shxzukj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hs.nicolike.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lh.521024.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://en.bjjhwx.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yv.521024.cn

Java: // 无：用 Builder 模式或 record
来源：http://bf.huixiangedu.cn

Go:   // 无：用配置结构体参数
来源：http://we.szsharing.cn

Ruby: f(a: 1, b: 2)
来源：http://ny.huixiangedu.cn

C#:   f(a: 1, b: 2)
来源：http://vk.521024.cn

[C05] 返回多个值
来源：http://ti.wgjwhj.cn

Py:   return a, b
来源：http://jj.jianghongdianzi.cn

PHP:  return [$a, $b];
来源：http://tg.szsharing.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ai.gzmigu.cn

TS:   return { a, b };
来源：http://pu.9csxet.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wn.521024.cn

Go:   return a, b
来源：http://wy.gzmigu.cn

Ruby: return a, b
来源：http://km.szxytkj.cn

C#:   return (a, b);              // ValueTuple
来源：http://mb.jianghongdianzi.cn

[C06] 匿名函数 / lambda
来源：http://ky.yuntaijiaju.cn

Py:   square = lambda x: x * x
来源：http://cj.chemitech.net.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://rj.gzmigu.cn

JS:   const square = x => x * x;
来源：http://lg.lnxyls.cn

TS:   const square = (x: number): number => x * x;
来源：http://vs.bjjhwx.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zg.hahajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://oc.shtwfgs.cn

Ruby: square = ->(x) { x * x }
来源：http://sy.haigaiapp.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ak.nszjky.cn

[C07] 把函数作为参数传入
来源：http://df.shxzukj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kq.colortex.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kx.jctech888.com.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://da.chemitech.net.cn

TS:   arr.map(String)
来源：http://ya.nicolike.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ew.szxytkj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://od.shtwfgs.cn

Ruby: arr.map(&:upcase)
来源：http://ho.colortex.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ch.nicolike.cn

[C08] 闭包
来源：http://gm.colortex.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://oc.colortex.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vo.shxzukj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ar.szsharing.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zq.chemitech.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uf.panjiajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mr.yuntaijiaju.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mo.szxytkj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://le.9csxet.cn

[C09] 递归
来源：http://ba.shxzukj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dg.asd995.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sj.shtwfgs.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ps.yuntaijiaju.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pn.huanxung.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sz.gzmigu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gf.huanxung.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xb.huixinmuqiang.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://je.shxzukj.cn

[C10] 变量作用域
来源：http://uo.hahajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://em.colortex.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zc.hahajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gb.panjiajie.cn

TS:   同 JS
来源：http://ui.nicolike.cn

Java: 方法内为块级作用域
来源：http://dg.shtwfgs.cn

Go:   花括号块级作用域
来源：http://ag.jctech888.com.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qj.nicolike.cn

C#:   块级作用域
来源：http://um.huanxung.cn

[C11] 模块导入与导出
来源：http://qv.bjjhwx.cn

Py:   from module import func
来源：http://hd.muxihuayi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ni.hnjuh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://th.huixinmuqiang.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://or.huixiangedu.cn

Java: import java.util.List;
来源：http://lk.shxzskj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zt.jianghongdianzi.cn

Ruby: require "json"; require_relative "./util"
来源：http://pr.bookmarksfly.cn

C#:   using System.Text;
来源：http://jp.shxzskj.cn

[C12] 立即执行函数 IIFE
来源：http://cp.hnjuh.cn

Py:   (lambda: print("run"))()
来源：http://ll.bookmarksfly.cn

PHP:  (function () { echo "run"; })();
来源：http://rj.521024.cn

JS:   (() => { console.log("run"); })();
来源：http://qx.huixiangedu.cn

TS:   (() => { console.log("run"); })();
来源：http://qp.panjiajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cb.yuexingan06.cn

Go:   func() { fmt.Println("run") }()
来源：http://ch.wgjwhj.cn

Ruby: -> { puts "run" }.call
来源：http://tp.huixinmuqiang.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://hm.nszjky.cn

[C13] 类型声明 / 类型注解
来源：http://db.521024.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://me.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://he.nszjky.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://my.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pd.colortex.cn

Java: int add(int a, int b) { return a + b; }
来源：http://gu.chemitech.net.cn

Go:   func add(a, b int) int
来源：http://dh.lnxyls.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nw.yuntaijiaju.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xj.shtwfgs.cn

[C14] 泛型函数
来源：http://xn.nicolike.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yu.gzmigu.cn

PHP:  // 无泛型
来源：http://wb.nicolike.cn

JS:   // 无泛型
来源：http://mr.newstarts.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://an.jianghongdianzi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ct.shxzukj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hp.bookmarksfly.cn

Ruby: # 无泛型
来源：http://ph.yuexingan06.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ki.bjjhwx.cn

[C15] 解构 / 展开参数
来源：http://zo.haigaiapp.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zp.hnjuh.cn

PHP:  [$a, $b] = $pair;
来源：http://gg.nszjky.cn


<!-- 参考信息 -->