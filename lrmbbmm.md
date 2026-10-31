代发 wailian999

C#:   s.Length
来源：http://dh.haigaiapp.cn

[A23] 大小写转换
来源：http://qb.yuexingan06.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ol.chemitech.net.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://la.haigaiapp.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ob.gzmigu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gw.jianghongdianzi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cf.shxzukj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kp.huixiangedu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lp.shxzskj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://kq.jctech888.com.cn

[A24] 去除首尾空白
来源：http://mk.bjjhwx.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://td.panjiajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dp.gzmigu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wg.nicolike.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nb.huixiangedu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cc.szxytkj.cn

Go:   strings.TrimSpace(s)
来源：http://vn.asd995.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lq.panjiajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://px.shtwfgs.cn

[A25] 字符串比较
来源：http://nq.asd995.cn

Py:   s1 == s2; s1 != s2
来源：http://iy.bookmarksfly.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tn.huanxung.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ro.yuntaijiaju.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://eq.shxzskj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://do.szsharing.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pt.shtwfgs.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ks.9csxet.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gz.haigaiapp.cn

[A26] 类型转换总览
来源：http://zc.yuntaijiaju.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fe.9csxet.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kk.jctech888.com.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://lz.shxzukj.cn

TS:   Number() String() Boolean() x as number
来源：http://av.wgjwhj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kz.jianghongdianzi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vk.chemitech.net.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ar.wgjwhj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://za.lnxyls.cn

================================================================================
来源：http://fd.asd995.cn

B. 流程控制
来源：http://up.nszjky.cn

================================================================================
来源：http://cp.jctech888.com.cn

[B01] 条件判断 if / else
来源：http://hz.gzmigu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vc.huanxung.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://go.nszjky.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://aq.shtwfgs.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pg.chemitech.net.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://uj.yuntaijiaju.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bm.huixinmuqiang.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pm.hnjuh.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://br.yuntaijiaju.cn

[B02] 多分支 else if / elif
来源：http://gt.bookmarksfly.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yn.nicolike.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://eu.szxytkj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://le.chemitech.net.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://va.wgjwhj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bn.yuntaijiaju.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ck.bookmarksfly.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rx.bookmarksfly.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ki.huanxung.cn

[B03] switch / match / case
来源：http://rs.huixiangedu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sx.9csxet.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mr.newstarts.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ej.wgjwhj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pz.muxihuayi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ry.colortex.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ww.hahajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://oq.nszjky.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qm.szxytkj.cn

[B04] for 计数循环
来源：http://kx.jctech888.com.cn

Py:   for i in range(10): print(i)
来源：http://pq.nicolike.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xn.chemitech.net.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jh.nicolike.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pb.bjjhwx.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ns.521024.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vu.haigaiapp.cn

Ruby: 10.times { |i| puts i }
来源：http://lo.yuexingan06.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ka.chemitech.net.cn

[B05] 遍历数组 / 列表
来源：http://df.muxihuayi.cn

Py:   for item in arr: print(item)
来源：http://wk.huixiangedu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vr.9csxet.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.hahajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://up.szsharing.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://mm.bjjhwx.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://la.huanxung.cn

Ruby: arr.each { |item| puts item }
来源：http://gj.jctech888.com.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jt.nicolike.cn

[B06] 遍历字典 / 对象
来源：http://dn.huanxung.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://bx.panjiajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ez.jianghongdianzi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://aw.lnxyls.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ek.szxytkj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qn.huanxung.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gb.hahajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gj.huixiangedu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://io.colortex.cn

[B07] while 循环
来源：http://sv.jctech888.com.cn

Py:   while i < 10: i += 1
来源：http://ii.9csxet.cn

PHP:  while ($i < 10) { $i++; }
来源：http://on.huanxung.cn

JS:   while (i < 10) { i++; }
来源：http://xc.haigaiapp.cn

TS:   while (i < 10) { i++; }
来源：http://vb.colortex.cn

Java: while (i < 10) { i++; }
来源：http://im.huanxung.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nw.haigaiapp.cn

Ruby: while i < 10; i += 1; end
来源：http://kg.bjjhwx.cn

C#:   while (i < 10) { i++; }
来源：http://uu.hnjuh.cn

[B08] do-while（至少执行一次）
来源：http://ur.jctech888.com.cn

Py:   # 无 do-while：用 while True + break
来源：http://is.yuexingan06.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cu.colortex.cn

JS:   do { i++; } while (i < 10);
来源：http://ir.chemitech.net.cn

TS:   do { i++; } while (i < 10);
来源：http://es.hahajie.cn

Java: do { i++; } while (i < 10);
来源：http://wk.shxzukj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://an.szsharing.cn

Ruby: begin; i += 1; end while i < 10
来源：http://th.huixiangedu.cn

C#:   do { i++; } while (i < 10);
来源：http://rh.huixiangedu.cn

[B09] break 与 continue
来源：http://ep.wgjwhj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cq.jianghongdianzi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wq.bjjhwx.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ro.nszjky.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yn.bookmarksfly.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yz.haigaiapp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ci.haigaiapp.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nn.haigaiapp.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pa.panjiajie.cn

[B10] 遍历同时拿索引
来源：http://fu.shxzukj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ld.muxihuayi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pa.521024.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xx.huixiangedu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cd.newstarts.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ua.hnjuh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://oc.hahajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uv.gzmigu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ns.bjjhwx.cn

[B11] 生成数字序列 / 区间
来源：http://zq.colortex.cn

Py:   list(range(0, 10, 2))
来源：http://pv.asd995.cn

PHP:  range(0, 10, 2);
来源：http://uz.panjiajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mx.haigaiapp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kv.colortex.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sh.jianghongdianzi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bu.chemitech.net.cn

Ruby: (0...10).step(2).to_a
来源：http://ic.bjjhwx.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vh.shxzskj.cn

[B12] 跳出多层循环
来源：http://qr.shxzskj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://np.shtwfgs.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wp.asd995.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ep.hahajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bn.huixiangedu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bl.bookmarksfly.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tu.yuntaijiaju.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xx.jianghongdianzi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nk.szsharing.cn

[B13] 判断是否为数字
来源：http://iy.shxzskj.cn

Py:   isinstance(x, (int, float))
来源：http://dy.haigaiapp.cn

PHP:  is_numeric($x)
来源：http://th.nszjky.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ta.colortex.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gb.gzmigu.cn

Java: x instanceof Number
来源：http://ss.hnjuh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://oc.jctech888.com.cn

Ruby: x.is_a?(Numeric)
来源：http://or.shxzukj.cn

C#:   x is int or double or decimal
来源：http://sv.panjiajie.cn

[B14] 判断值是否在集合内
来源：http://dv.nszjky.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nm.shtwfgs.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lv.chemitech.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://cu.9csxet.cn

TS:   [1, 2, 3].includes(x)
来源：http://ak.newstarts.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ub.bjjhwx.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ss.shxzukj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://hw.hahajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cv.huixiangedu.cn

[B15] 布尔运算与取反
来源：http://rx.shxzskj.cn

Py:   a and b or not c
来源：http://vz.huixinmuqiang.cn

PHP:  $a && $b || !$c
来源：http://ao.yuntaijiaju.cn

JS:   a && b || !c
来源：http://uw.colortex.cn

TS:   a && b || !c
来源：http://jl.szsharing.cn

Java: a && b || !c
来源：http://bn.yuexingan06.cn

Go:   a && b || !c
来源：http://zl.muxihuayi.cn

Ruby: a && b || !c
来源：http://nw.huixiangedu.cn

C#:   a && b || !c
来源：http://pj.yuexingan06.cn

[B16] 卫语句：不满足条件提前返回
来源：http://db.huanxung.cn

Py:   if not data: return
来源：http://at.muxihuayi.cn

PHP:  if (!$data) { return; }
来源：http://tx.9csxet.cn

JS:   if (!data) return;
来源：http://cr.colortex.cn

TS:   if (!data) return;
来源：http://po.nicolike.cn

Java: if (data == null) return;
来源：http://jb.huixinmuqiang.cn

Go:   if data == nil { return }
来源：http://df.huixinmuqiang.cn

Ruby: return if data.nil?
来源：http://vr.yuexingan06.cn

C#:   if (data == null) return;
来源：http://ol.newstarts.cn

================================================================================
来源：http://ep.shxzskj.cn

C. 函数与作用域
来源：http://ao.chemitech.net.cn

================================================================================
来源：http://ih.panjiajie.cn

[C01] 定义函数
来源：http://to.9csxet.cn

Py:   def add(a, b): return a + b
来源：http://fg.hahajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://du.lnxyls.cn

JS:   function add(a, b) { return a + b; }
来源：http://qr.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://if.nicolike.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hf.huixiangedu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ym.asd995.cn

Ruby: def add(a, b); a + b; end
来源：http://rx.hahajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wg.wgjwhj.cn

[C02] 默认参数
来源：http://yi.huixiangedu.cn

Py:   def greet(name="World"): return name
来源：http://tb.yuntaijiaju.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ah.nicolike.cn

JS:   function greet(name = "World") { return name; }
来源：http://ju.newstarts.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://la.chemitech.net.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://pa.521024.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pe.nicolike.cn

Ruby: def greet(name = "World") = name
来源：http://to.nszjky.cn

C#:   string Greet(string name = "World") => name;
来源：http://su.huanxung.cn

[C03] 可变参数
来源：http://kj.gzmigu.cn

Py:   def total(*args): return sum(args)
来源：http://sj.hnjuh.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hg.9csxet.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dc.hnjuh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cf.panjiajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lg.haigaiapp.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cf.jianghongdianzi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://be.gzmigu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nm.wgjwhj.cn

[C04] 命名参数 / 关键字参数
来源：http://df.nicolike.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gw.panjiajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lw.shtwfgs.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qu.shxzukj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ol.gzmigu.cn

Java: // 无：用 Builder 模式或 record
来源：http://ri.gzmigu.cn

Go:   // 无：用配置结构体参数
来源：http://ry.muxihuayi.cn

Ruby: f(a: 1, b: 2)
来源：http://am.szxytkj.cn

C#:   f(a: 1, b: 2)
来源：http://oy.jctech888.com.cn

[C05] 返回多个值
来源：http://sp.newstarts.cn

Py:   return a, b
来源：http://iv.huixinmuqiang.cn

PHP:  return [$a, $b];
来源：http://zn.lnxyls.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ts.521024.cn

TS:   return { a, b };
来源：http://kb.chemitech.net.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ol.nszjky.cn

Go:   return a, b
来源：http://mm.colortex.cn

Ruby: return a, b
来源：http://av.huixiangedu.cn

C#:   return (a, b);              // ValueTuple
来源：http://ip.hahajie.cn

[C06] 匿名函数 / lambda
来源：http://cr.shxzukj.cn

Py:   square = lambda x: x * x
来源：http://hf.shxzskj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://kw.szxytkj.cn

JS:   const square = x => x * x;
来源：http://yx.asd995.cn

TS:   const square = (x: number): number => x * x;
来源：http://yt.chemitech.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ab.panjiajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wg.yuexingan06.cn

Ruby: square = ->(x) { x * x }
来源：http://wh.jianghongdianzi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://pg.wgjwhj.cn

[C07] 把函数作为参数传入
来源：http://ef.gzmigu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://om.huanxung.cn

PHP:  array_map("strtoupper", $arr);
来源：http://qc.chemitech.net.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nx.yuntaijiaju.cn

TS:   arr.map(String)
来源：http://lx.panjiajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fp.asd995.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xi.muxihuayi.cn

Ruby: arr.map(&:upcase)
来源：http://my.chemitech.net.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qr.huanxung.cn

[C08] 闭包
来源：http://wq.shxzukj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://si.521024.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ho.9csxet.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jj.shxzukj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://op.nicolike.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tj.bookmarksfly.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ah.huixiangedu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fk.muxihuayi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fh.jianghongdianzi.cn

[C09] 递归
来源：http://ad.muxihuayi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hv.gzmigu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kv.hahajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fj.szxytkj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gd.szsharing.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pm.haigaiapp.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zd.gzmigu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dg.huanxung.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://is.nszjky.cn

[C10] 变量作用域
来源：http://sj.nszjky.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rp.521024.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://sv.bookmarksfly.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tq.huanxung.cn

TS:   同 JS
来源：http://qk.muxihuayi.cn

Java: 方法内为块级作用域
来源：http://yl.jctech888.com.cn

Go:   花括号块级作用域
来源：http://qa.hahajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fo.shtwfgs.cn

C#:   块级作用域
来源：http://ok.nicolike.cn

[C11] 模块导入与导出
来源：http://hw.newstarts.cn

Py:   from module import func
来源：http://ka.bjjhwx.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ru.jianghongdianzi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://tt.nicolike.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wm.nszjky.cn

Java: import java.util.List;
来源：http://ks.hnjuh.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hi.nicolike.cn

Ruby: require "json"; require_relative "./util"
来源：http://ut.yuntaijiaju.cn

C#:   using System.Text;
来源：http://xy.shtwfgs.cn

[C12] 立即执行函数 IIFE
来源：http://jg.shxzskj.cn

Py:   (lambda: print("run"))()
来源：http://up.hnjuh.cn

PHP:  (function () { echo "run"; })();
来源：http://yx.nicolike.cn

JS:   (() => { console.log("run"); })();
来源：http://mn.yuexingan06.cn

TS:   (() => { console.log("run"); })();
来源：http://ba.yuexingan06.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jk.asd995.cn

Go:   func() { fmt.Println("run") }()
来源：http://ss.chemitech.net.cn

Ruby: -> { puts "run" }.call
来源：http://fm.jctech888.com.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ba.lnxyls.cn

[C13] 类型声明 / 类型注解
来源：http://ga.9csxet.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://me.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://od.jctech888.com.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cg.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yo.gzmigu.cn


<!-- 参考信息 -->