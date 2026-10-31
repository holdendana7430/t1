代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kg.haigaiapp.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kl.shtwfgs.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tc.521024.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cb.shxzskj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lx.bookmarksfly.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ya.lnxyls.cn

[A24] 去除首尾空白
来源：http://mz.szxytkj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rr.wgjwhj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pn.nicolike.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://po.hnjuh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://am.huixiangedu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tm.chemitech.net.cn

Go:   strings.TrimSpace(s)
来源：http://yy.szxytkj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pc.hnjuh.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nj.lnxyls.cn

[A25] 字符串比较
来源：http://dc.muxihuayi.cn

Py:   s1 == s2; s1 != s2
来源：http://sa.hahajie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jt.chemitech.net.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wz.shxzskj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kn.jianghongdianzi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fx.jianghongdianzi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://up.jianghongdianzi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ul.bjjhwx.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://de.muxihuayi.cn

[A26] 类型转换总览
来源：http://dk.huixiangedu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mk.panjiajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ki.yuntaijiaju.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nd.jianghongdianzi.cn

TS:   Number() String() Boolean() x as number
来源：http://bg.huanxung.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jn.yuntaijiaju.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tx.gzmigu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://cb.521024.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ld.muxihuayi.cn

================================================================================
来源：http://wy.nicolike.cn

B. 流程控制
来源：http://gw.chemitech.net.cn

================================================================================
来源：http://jn.gzmigu.cn

[B01] 条件判断 if / else
来源：http://fm.nicolike.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bo.panjiajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rg.yuexingan06.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nx.chemitech.net.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ps.nszjky.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bm.hnjuh.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lb.haigaiapp.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lj.panjiajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jm.yuntaijiaju.cn

[B02] 多分支 else if / elif
来源：http://lp.szxytkj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yt.hnjuh.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://eb.shtwfgs.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://da.nicolike.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ad.wgjwhj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nr.nicolike.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mw.521024.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nf.jianghongdianzi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hj.huixiangedu.cn

[B03] switch / match / case
来源：http://xt.bjjhwx.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hg.huixinmuqiang.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lj.nszjky.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yk.szxytkj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ju.bookmarksfly.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lt.hnjuh.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://im.huanxung.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wk.huanxung.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://px.huanxung.cn

[B04] for 计数循环
来源：http://qo.hnjuh.cn

Py:   for i in range(10): print(i)
来源：http://mg.bookmarksfly.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://km.bjjhwx.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ha.hahajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://do.haigaiapp.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://oi.szsharing.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bk.panjiajie.cn

Ruby: 10.times { |i| puts i }
来源：http://ne.shxzskj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ab.nicolike.cn

[B05] 遍历数组 / 列表
来源：http://ij.521024.cn

Py:   for item in arr: print(item)
来源：http://eu.yuntaijiaju.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hs.newstarts.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qs.yuexingan06.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bu.bookmarksfly.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ol.gzmigu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ex.huanxung.cn

Ruby: arr.each { |item| puts item }
来源：http://wn.gzmigu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ed.panjiajie.cn

[B06] 遍历字典 / 对象
来源：http://dx.521024.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qz.gzmigu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ha.haigaiapp.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ib.bookmarksfly.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jc.gzmigu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cl.521024.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rh.szsharing.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kw.nicolike.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rf.bjjhwx.cn

[B07] while 循环
来源：http://kg.hahajie.cn

Py:   while i < 10: i += 1
来源：http://mb.newstarts.cn

PHP:  while ($i < 10) { $i++; }
来源：http://cj.shtwfgs.cn

JS:   while (i < 10) { i++; }
来源：http://il.newstarts.cn

TS:   while (i < 10) { i++; }
来源：http://gn.shxzskj.cn

Java: while (i < 10) { i++; }
来源：http://sj.bookmarksfly.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zl.hnjuh.cn

Ruby: while i < 10; i += 1; end
来源：http://ha.lnxyls.cn

C#:   while (i < 10) { i++; }
来源：http://sv.wgjwhj.cn

[B08] do-while（至少执行一次）
来源：http://bl.hahajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://yg.bjjhwx.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://dg.hahajie.cn

JS:   do { i++; } while (i < 10);
来源：http://rq.chemitech.net.cn

TS:   do { i++; } while (i < 10);
来源：http://iu.hahajie.cn

Java: do { i++; } while (i < 10);
来源：http://wg.gzmigu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sw.huixiangedu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ex.9csxet.cn

C#:   do { i++; } while (i < 10);
来源：http://jo.jctech888.com.cn

[B09] break 与 continue
来源：http://xm.chemitech.net.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wr.9csxet.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rz.panjiajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pe.wgjwhj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://be.huixiangedu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ed.yuexingan06.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://df.nszjky.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fr.szsharing.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iu.nszjky.cn

[B10] 遍历同时拿索引
来源：http://gz.chemitech.net.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yz.hahajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yn.panjiajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mp.nicolike.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gg.nicolike.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vb.muxihuayi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kr.colortex.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://de.lnxyls.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xs.shxzukj.cn

[B11] 生成数字序列 / 区间
来源：http://ni.bookmarksfly.cn

Py:   list(range(0, 10, 2))
来源：http://hg.chemitech.net.cn

PHP:  range(0, 10, 2);
来源：http://op.bjjhwx.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uz.shtwfgs.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://om.shtwfgs.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fw.bookmarksfly.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vl.jctech888.com.cn

Ruby: (0...10).step(2).to_a
来源：http://sd.nicolike.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fs.9csxet.cn

[B12] 跳出多层循环
来源：http://wc.jianghongdianzi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://li.panjiajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ys.hahajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xe.huanxung.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ln.muxihuayi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://oy.szsharing.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dr.huixiangedu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ao.yuexingan06.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://el.jianghongdianzi.cn

[B13] 判断是否为数字
来源：http://fx.nszjky.cn

Py:   isinstance(x, (int, float))
来源：http://dm.jctech888.com.cn

PHP:  is_numeric($x)
来源：http://rr.huanxung.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sj.nszjky.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://db.nicolike.cn

Java: x instanceof Number
来源：http://el.haigaiapp.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jj.gzmigu.cn

Ruby: x.is_a?(Numeric)
来源：http://vs.nicolike.cn

C#:   x is int or double or decimal
来源：http://tn.jctech888.com.cn

[B14] 判断值是否在集合内
来源：http://uh.521024.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://sg.jianghongdianzi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zp.gzmigu.cn

JS:   [1, 2, 3].includes(x)
来源：http://oe.bookmarksfly.cn

TS:   [1, 2, 3].includes(x)
来源：http://ju.hnjuh.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ei.jianghongdianzi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ai.yuntaijiaju.cn

Ruby: [1, 2, 3].include?(x)
来源：http://lq.yuexingan06.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rd.bookmarksfly.cn

[B15] 布尔运算与取反
来源：http://ts.nicolike.cn

Py:   a and b or not c
来源：http://wy.panjiajie.cn

PHP:  $a && $b || !$c
来源：http://kg.nicolike.cn

JS:   a && b || !c
来源：http://ip.shxzukj.cn

TS:   a && b || !c
来源：http://vg.huanxung.cn

Java: a && b || !c
来源：http://uw.521024.cn

Go:   a && b || !c
来源：http://wc.bookmarksfly.cn

Ruby: a && b || !c
来源：http://sr.haigaiapp.cn

C#:   a && b || !c
来源：http://jr.shxzskj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://eo.lnxyls.cn

Py:   if not data: return
来源：http://ow.shxzskj.cn

PHP:  if (!$data) { return; }
来源：http://wo.colortex.cn

JS:   if (!data) return;
来源：http://ma.szsharing.cn

TS:   if (!data) return;
来源：http://cf.muxihuayi.cn

Java: if (data == null) return;
来源：http://mc.szsharing.cn

Go:   if data == nil { return }
来源：http://ny.asd995.cn

Ruby: return if data.nil?
来源：http://iw.huixiangedu.cn

C#:   if (data == null) return;
来源：http://ro.yuexingan06.cn

================================================================================
来源：http://nu.gzmigu.cn

C. 函数与作用域
来源：http://hk.colortex.cn

================================================================================
来源：http://wh.yuexingan06.cn

[C01] 定义函数
来源：http://re.shxzukj.cn

Py:   def add(a, b): return a + b
来源：http://xs.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pe.colortex.cn

JS:   function add(a, b) { return a + b; }
来源：http://wn.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bp.lnxyls.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://tu.szxytkj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hn.hnjuh.cn

Ruby: def add(a, b); a + b; end
来源：http://yg.asd995.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yr.nszjky.cn

[C02] 默认参数
来源：http://my.huanxung.cn

Py:   def greet(name="World"): return name
来源：http://tr.huanxung.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xm.bjjhwx.cn

JS:   function greet(name = "World") { return name; }
来源：http://ms.521024.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gj.hnjuh.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ei.nicolike.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rn.yuexingan06.cn

Ruby: def greet(name = "World") = name
来源：http://so.newstarts.cn

C#:   string Greet(string name = "World") => name;
来源：http://hd.shxzukj.cn

[C03] 可变参数
来源：http://xa.jctech888.com.cn

Py:   def total(*args): return sum(args)
来源：http://oi.huixiangedu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qz.shxzukj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gp.wgjwhj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nb.shtwfgs.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sh.521024.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ou.shtwfgs.cn

Ruby: def total(*nums); nums.sum; end
来源：http://eu.hahajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ia.shxzukj.cn

[C04] 命名参数 / 关键字参数
来源：http://jz.shxzskj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kk.chemitech.net.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://on.gzmigu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://oc.jianghongdianzi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wm.9csxet.cn

Java: // 无：用 Builder 模式或 record
来源：http://gj.yuntaijiaju.cn

Go:   // 无：用配置结构体参数
来源：http://tu.yuntaijiaju.cn

Ruby: f(a: 1, b: 2)
来源：http://mt.szxytkj.cn

C#:   f(a: 1, b: 2)
来源：http://mx.shxzskj.cn

[C05] 返回多个值
来源：http://ts.huixiangedu.cn

Py:   return a, b
来源：http://lb.huixinmuqiang.cn

PHP:  return [$a, $b];
来源：http://mr.yuntaijiaju.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qs.hahajie.cn

TS:   return { a, b };
来源：http://ej.nicolike.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://eh.shtwfgs.cn

Go:   return a, b
来源：http://pv.jianghongdianzi.cn

Ruby: return a, b
来源：http://yw.szxytkj.cn

C#:   return (a, b);              // ValueTuple
来源：http://tq.hahajie.cn

[C06] 匿名函数 / lambda
来源：http://yp.wgjwhj.cn

Py:   square = lambda x: x * x
来源：http://lb.jctech888.com.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ln.gzmigu.cn

JS:   const square = x => x * x;
来源：http://vo.newstarts.cn

TS:   const square = (x: number): number => x * x;
来源：http://yx.nszjky.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tj.shtwfgs.cn

Go:   sq := func(x int) int { return x * x }
来源：http://tc.bookmarksfly.cn

Ruby: square = ->(x) { x * x }
来源：http://ho.newstarts.cn

C#:   Func<int, int> square = x => x * x;
来源：http://pq.9csxet.cn

[C07] 把函数作为参数传入
来源：http://ec.jianghongdianzi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ge.hahajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ca.asd995.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hc.yuntaijiaju.cn

TS:   arr.map(String)
来源：http://nq.chemitech.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zr.9csxet.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ys.muxihuayi.cn

Ruby: arr.map(&:upcase)
来源：http://bn.jianghongdianzi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mo.jctech888.com.cn

[C08] 闭包
来源：http://tl.yuexingan06.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qi.szxytkj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yk.gzmigu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jk.muxihuayi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fy.asd995.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zv.shxzskj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wa.bjjhwx.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dc.lnxyls.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fd.bjjhwx.cn

[C09] 递归
来源：http://lr.szsharing.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://oc.asd995.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://iy.nszjky.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lj.shxzukj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rk.shxzukj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://su.colortex.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://di.asd995.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ia.panjiajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ds.panjiajie.cn

[C10] 变量作用域
来源：http://ok.haigaiapp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hj.shxzukj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ce.9csxet.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pg.lnxyls.cn

TS:   同 JS
来源：http://ok.yuexingan06.cn

Java: 方法内为块级作用域
来源：http://pu.huixiangedu.cn

Go:   花括号块级作用域
来源：http://lg.huixiangedu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ih.haigaiapp.cn

C#:   块级作用域
来源：http://tq.lnxyls.cn

[C11] 模块导入与导出
来源：http://ma.colortex.cn

Py:   from module import func
来源：http://wv.shxzukj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bs.szsharing.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://za.shtwfgs.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ym.jianghongdianzi.cn

Java: import java.util.List;
来源：http://wb.yuntaijiaju.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ok.yuntaijiaju.cn

Ruby: require "json"; require_relative "./util"
来源：http://vj.nszjky.cn

C#:   using System.Text;
来源：http://pr.colortex.cn

[C12] 立即执行函数 IIFE
来源：http://ch.shtwfgs.cn

Py:   (lambda: print("run"))()
来源：http://wn.nicolike.cn

PHP:  (function () { echo "run"; })();
来源：http://oo.gzmigu.cn

JS:   (() => { console.log("run"); })();
来源：http://kh.bjjhwx.cn

TS:   (() => { console.log("run"); })();
来源：http://ld.jianghongdianzi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://iv.asd995.cn

Go:   func() { fmt.Println("run") }()
来源：http://ea.nicolike.cn

Ruby: -> { puts "run" }.call
来源：http://ws.panjiajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wa.yuexingan06.cn

[C13] 类型声明 / 类型注解
来源：http://am.panjiajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ne.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zz.bjjhwx.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://oe.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uy.bookmarksfly.cn

Java: int add(int a, int b) { return a + b; }
来源：http://pa.9csxet.cn

Go:   func add(a, b int) int
来源：http://ci.yuexingan06.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nj.9csxet.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ja.jianghongdianzi.cn


<!-- 参考信息 -->