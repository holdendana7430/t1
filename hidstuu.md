代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qr.huanxung.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gn.wgjwhj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cu.yuntaijiaju.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://um.muxihuayi.cn

Go:   strings.TrimSpace(s)
来源：http://cs.huanxung.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://uc.lnxyls.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pm.hnjuh.cn

[A25] 字符串比较
来源：http://mv.nicolike.cn

Py:   s1 == s2; s1 != s2
来源：http://uo.hnjuh.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rc.szsharing.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gi.bookmarksfly.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://su.hnjuh.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ow.hnjuh.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://is.huixiangedu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://su.yuexingan06.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xz.yuexingan06.cn

[A26] 类型转换总览
来源：http://oy.hnjuh.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dj.nicolike.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fh.huixiangedu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gp.shtwfgs.cn

TS:   Number() String() Boolean() x as number
来源：http://ko.yuexingan06.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bi.jctech888.com.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xo.newstarts.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://qz.nicolike.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ub.asd995.cn

================================================================================
来源：http://vn.jianghongdianzi.cn

B. 流程控制
来源：http://xk.huanxung.cn

================================================================================
来源：http://ib.gzmigu.cn

[B01] 条件判断 if / else
来源：http://fu.huanxung.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ha.nicolike.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://oz.newstarts.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nt.szxytkj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xx.bjjhwx.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://cs.9csxet.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://uu.chemitech.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pa.lnxyls.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fi.yuexingan06.cn

[B02] 多分支 else if / elif
来源：http://kl.lnxyls.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://th.bjjhwx.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qg.shtwfgs.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qg.bookmarksfly.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ep.nicolike.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wf.lnxyls.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qd.yuntaijiaju.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xb.asd995.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hi.lnxyls.cn

[B03] switch / match / case
来源：http://ys.asd995.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bk.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mj.muxihuayi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ep.nicolike.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bd.521024.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nz.colortex.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://au.huixiangedu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kj.haigaiapp.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zp.szsharing.cn

[B04] for 计数循环
来源：http://gg.szsharing.cn

Py:   for i in range(10): print(i)
来源：http://pk.huanxung.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://aq.lnxyls.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rc.jianghongdianzi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://od.nszjky.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lm.shxzskj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cm.jianghongdianzi.cn

Ruby: 10.times { |i| puts i }
来源：http://iu.panjiajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://da.lnxyls.cn

[B05] 遍历数组 / 列表
来源：http://ep.szsharing.cn

Py:   for item in arr: print(item)
来源：http://zj.521024.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://oh.shxzskj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://co.nicolike.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://nn.lnxyls.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yr.newstarts.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ok.colortex.cn

Ruby: arr.each { |item| puts item }
来源：http://no.nszjky.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://up.chemitech.net.cn

[B06] 遍历字典 / 对象
来源：http://hw.chemitech.net.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://be.hahajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://as.shxzskj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wu.hahajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zb.hahajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dr.bjjhwx.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://oq.muxihuayi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://iz.wgjwhj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cs.huanxung.cn

[B07] while 循环
来源：http://vn.gzmigu.cn

Py:   while i < 10: i += 1
来源：http://fo.nicolike.cn

PHP:  while ($i < 10) { $i++; }
来源：http://eg.huanxung.cn

JS:   while (i < 10) { i++; }
来源：http://gd.haigaiapp.cn

TS:   while (i < 10) { i++; }
来源：http://dt.huixiangedu.cn

Java: while (i < 10) { i++; }
来源：http://pf.colortex.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kt.haigaiapp.cn

Ruby: while i < 10; i += 1; end
来源：http://le.newstarts.cn

C#:   while (i < 10) { i++; }
来源：http://bg.huixinmuqiang.cn

[B08] do-while（至少执行一次）
来源：http://ye.9csxet.cn

Py:   # 无 do-while：用 while True + break
来源：http://bk.hahajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://iu.yuexingan06.cn

JS:   do { i++; } while (i < 10);
来源：http://yn.nszjky.cn

TS:   do { i++; } while (i < 10);
来源：http://hp.colortex.cn

Java: do { i++; } while (i < 10);
来源：http://gq.nicolike.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xg.wgjwhj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://lj.shxzskj.cn

C#:   do { i++; } while (i < 10);
来源：http://bo.yuexingan06.cn

[B09] break 与 continue
来源：http://hx.panjiajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dy.huixinmuqiang.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ve.jctech888.com.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yo.huixiangedu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qo.newstarts.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zo.hahajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ag.bookmarksfly.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ls.huixiangedu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zh.huanxung.cn

[B10] 遍历同时拿索引
来源：http://ph.muxihuayi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sd.9csxet.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zc.shxzukj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://am.jianghongdianzi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ap.colortex.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fq.huixinmuqiang.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mt.huanxung.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nb.shtwfgs.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://oe.chemitech.net.cn

[B11] 生成数字序列 / 区间
来源：http://ak.szsharing.cn

Py:   list(range(0, 10, 2))
来源：http://fq.9csxet.cn

PHP:  range(0, 10, 2);
来源：http://md.huixiangedu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pd.yuexingan06.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qv.hahajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rj.huixinmuqiang.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vp.jctech888.com.cn

Ruby: (0...10).step(2).to_a
来源：http://et.shtwfgs.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mc.huixinmuqiang.cn

[B12] 跳出多层循环
来源：http://ns.nszjky.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://rw.wgjwhj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ce.521024.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rv.asd995.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://np.huanxung.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bk.huanxung.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pm.bookmarksfly.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xu.shtwfgs.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vi.newstarts.cn

[B13] 判断是否为数字
来源：http://iv.bookmarksfly.cn

Py:   isinstance(x, (int, float))
来源：http://il.bookmarksfly.cn

PHP:  is_numeric($x)
来源：http://ys.nicolike.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://it.yuntaijiaju.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mn.huixiangedu.cn

Java: x instanceof Number
来源：http://ni.panjiajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yd.wgjwhj.cn

Ruby: x.is_a?(Numeric)
来源：http://yp.jctech888.com.cn

C#:   x is int or double or decimal
来源：http://ni.chemitech.net.cn

[B14] 判断值是否在集合内
来源：http://tt.bookmarksfly.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nw.huixinmuqiang.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nh.szsharing.cn

JS:   [1, 2, 3].includes(x)
来源：http://ld.chemitech.net.cn

TS:   [1, 2, 3].includes(x)
来源：http://zt.lnxyls.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://cs.bookmarksfly.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://em.muxihuayi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qc.gzmigu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bf.jianghongdianzi.cn

[B15] 布尔运算与取反
来源：http://ic.jctech888.com.cn

Py:   a and b or not c
来源：http://mx.huixiangedu.cn

PHP:  $a && $b || !$c
来源：http://rz.wgjwhj.cn

JS:   a && b || !c
来源：http://zs.asd995.cn

TS:   a && b || !c
来源：http://mk.shxzukj.cn

Java: a && b || !c
来源：http://xw.muxihuayi.cn

Go:   a && b || !c
来源：http://ut.chemitech.net.cn

Ruby: a && b || !c
来源：http://bs.panjiajie.cn

C#:   a && b || !c
来源：http://bh.jctech888.com.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ig.jianghongdianzi.cn

Py:   if not data: return
来源：http://pl.9csxet.cn

PHP:  if (!$data) { return; }
来源：http://ej.huanxung.cn

JS:   if (!data) return;
来源：http://mc.muxihuayi.cn

TS:   if (!data) return;
来源：http://xw.yuntaijiaju.cn

Java: if (data == null) return;
来源：http://xl.wgjwhj.cn

Go:   if data == nil { return }
来源：http://ss.hahajie.cn

Ruby: return if data.nil?
来源：http://ox.bookmarksfly.cn

C#:   if (data == null) return;
来源：http://ai.nszjky.cn

================================================================================
来源：http://vo.bjjhwx.cn

C. 函数与作用域
来源：http://wv.hahajie.cn

================================================================================
来源：http://mj.yuntaijiaju.cn

[C01] 定义函数
来源：http://vg.bjjhwx.cn

Py:   def add(a, b): return a + b
来源：http://sz.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pv.521024.cn

JS:   function add(a, b) { return a + b; }
来源：http://rr.yuexingan06.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kz.chemitech.net.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://rj.szxytkj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://om.wgjwhj.cn

Ruby: def add(a, b); a + b; end
来源：http://wy.huixiangedu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cy.jctech888.com.cn

[C02] 默认参数
来源：http://td.jianghongdianzi.cn

Py:   def greet(name="World"): return name
来源：http://po.lnxyls.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bh.yuexingan06.cn

JS:   function greet(name = "World") { return name; }
来源：http://hz.bjjhwx.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ik.yuntaijiaju.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ot.huixinmuqiang.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://aq.521024.cn

Ruby: def greet(name = "World") = name
来源：http://ss.muxihuayi.cn

C#:   string Greet(string name = "World") => name;
来源：http://lr.lnxyls.cn

[C03] 可变参数
来源：http://zs.bookmarksfly.cn

Py:   def total(*args): return sum(args)
来源：http://xz.yuexingan06.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fn.9csxet.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qy.hnjuh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bo.muxihuayi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bu.nszjky.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ws.bookmarksfly.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pn.jctech888.com.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://on.huanxung.cn

[C04] 命名参数 / 关键字参数
来源：http://rn.lnxyls.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jf.jctech888.com.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xq.panjiajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vq.jianghongdianzi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nt.szxytkj.cn

Java: // 无：用 Builder 模式或 record
来源：http://ys.newstarts.cn

Go:   // 无：用配置结构体参数
来源：http://ac.shxzskj.cn

Ruby: f(a: 1, b: 2)
来源：http://cb.chemitech.net.cn

C#:   f(a: 1, b: 2)
来源：http://ly.muxihuayi.cn

[C05] 返回多个值
来源：http://eu.yuntaijiaju.cn

Py:   return a, b
来源：http://rf.newstarts.cn

PHP:  return [$a, $b];
来源：http://he.wgjwhj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ay.colortex.cn

TS:   return { a, b };
来源：http://yw.nicolike.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hp.lnxyls.cn

Go:   return a, b
来源：http://jg.chemitech.net.cn

Ruby: return a, b
来源：http://ck.hnjuh.cn

C#:   return (a, b);              // ValueTuple
来源：http://rb.nicolike.cn

[C06] 匿名函数 / lambda
来源：http://al.wgjwhj.cn

Py:   square = lambda x: x * x
来源：http://nm.szsharing.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://et.nszjky.cn

JS:   const square = x => x * x;
来源：http://tu.szxytkj.cn

TS:   const square = (x: number): number => x * x;
来源：http://ch.bookmarksfly.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://od.huixinmuqiang.cn

Go:   sq := func(x int) int { return x * x }
来源：http://oz.jctech888.com.cn

Ruby: square = ->(x) { x * x }
来源：http://bn.colortex.cn

C#:   Func<int, int> square = x => x * x;
来源：http://nl.muxihuayi.cn

[C07] 把函数作为参数传入
来源：http://vt.jianghongdianzi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vk.szxytkj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://nf.nszjky.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wg.muxihuayi.cn

TS:   arr.map(String)
来源：http://qj.hnjuh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xj.haigaiapp.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dh.szxytkj.cn

Ruby: arr.map(&:upcase)
来源：http://fb.gzmigu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://po.hahajie.cn

[C08] 闭包
来源：http://th.jctech888.com.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nw.shtwfgs.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ga.hnjuh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lg.9csxet.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://iw.panjiajie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pl.9csxet.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hp.jctech888.com.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://em.muxihuayi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lb.hnjuh.cn

[C09] 递归
来源：http://zq.nszjky.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://id.shxzukj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dy.hnjuh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wy.haigaiapp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bn.nszjky.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tl.panjiajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nc.colortex.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://it.521024.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hr.521024.cn

[C10] 变量作用域
来源：http://ex.panjiajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vs.bookmarksfly.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yw.yuntaijiaju.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fv.jctech888.com.cn

TS:   同 JS
来源：http://zv.hahajie.cn

Java: 方法内为块级作用域
来源：http://oj.521024.cn

Go:   花括号块级作用域
来源：http://xx.bjjhwx.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tj.gzmigu.cn

C#:   块级作用域
来源：http://sm.huanxung.cn

[C11] 模块导入与导出
来源：http://kf.shxzskj.cn

Py:   from module import func
来源：http://dc.yuexingan06.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ue.gzmigu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ma.huixiangedu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://at.colortex.cn

Java: import java.util.List;
来源：http://yo.hahajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ap.szsharing.cn

Ruby: require "json"; require_relative "./util"
来源：http://bc.colortex.cn

C#:   using System.Text;
来源：http://ds.wgjwhj.cn

[C12] 立即执行函数 IIFE
来源：http://sk.wgjwhj.cn

Py:   (lambda: print("run"))()
来源：http://lw.bjjhwx.cn

PHP:  (function () { echo "run"; })();
来源：http://vk.gzmigu.cn

JS:   (() => { console.log("run"); })();
来源：http://yd.9csxet.cn

TS:   (() => { console.log("run"); })();
来源：http://ds.hnjuh.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://th.hahajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://cy.jctech888.com.cn

Ruby: -> { puts "run" }.call
来源：http://wi.jctech888.com.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ie.haigaiapp.cn

[C13] 类型声明 / 类型注解
来源：http://lr.panjiajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://em.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tc.nicolike.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://el.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rv.hahajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://li.huixiangedu.cn

Go:   func add(a, b int) int
来源：http://jx.bookmarksfly.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ml.9csxet.cn

C#:   int Add(int a, int b) => a + b;
来源：http://kh.nicolike.cn

[C14] 泛型函数
来源：http://bj.nicolike.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fq.yuntaijiaju.cn

PHP:  // 无泛型
来源：http://hp.yuntaijiaju.cn

JS:   // 无泛型
来源：http://ja.bookmarksfly.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://or.yuexingan06.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zf.jianghongdianzi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kt.huixinmuqiang.cn

Ruby: # 无泛型
来源：http://um.szxytkj.cn


<!-- 参考信息 -->