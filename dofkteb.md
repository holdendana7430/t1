代发 wailian999

TS:   s.length
来源：http://ap.asd995.cn

Java: s.length()
来源：http://zn.jianghongdianzi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ua.szxytkj.cn

Ruby: s.length
来源：http://mk.nicolike.cn

C#:   s.Length
来源：http://ar.jianghongdianzi.cn

[A23] 大小写转换
来源：http://ni.hnjuh.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://fy.huixiangedu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://af.bookmarksfly.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ev.9csxet.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rw.shxzukj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ir.yuexingan06.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ra.nszjky.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nu.hahajie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://wi.hahajie.cn

[A24] 去除首尾空白
来源：http://ic.wgjwhj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ss.521024.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xe.haigaiapp.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nw.bookmarksfly.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hg.bjjhwx.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ju.huixiangedu.cn

Go:   strings.TrimSpace(s)
来源：http://jc.yuexingan06.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gk.newstarts.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://us.521024.cn

[A25] 字符串比较
来源：http://ei.panjiajie.cn

Py:   s1 == s2; s1 != s2
来源：http://hg.yuexingan06.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://yq.shxzskj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gs.lnxyls.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gx.huixiangedu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mm.hnjuh.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qn.lnxyls.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://wr.hnjuh.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qa.yuntaijiaju.cn

[A26] 类型转换总览
来源：http://gv.huixinmuqiang.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bm.521024.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pw.colortex.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nl.bookmarksfly.cn

TS:   Number() String() Boolean() x as number
来源：http://ta.colortex.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tf.wgjwhj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dl.9csxet.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://fa.colortex.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://og.nszjky.cn

================================================================================
来源：http://cm.panjiajie.cn

B. 流程控制
来源：http://ec.hnjuh.cn

================================================================================
来源：http://qi.shtwfgs.cn

[B01] 条件判断 if / else
来源：http://nc.9csxet.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://py.huixinmuqiang.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hv.bookmarksfly.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qv.colortex.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ne.huixinmuqiang.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://sn.szxytkj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://df.bookmarksfly.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://os.nszjky.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mu.haigaiapp.cn

[B02] 多分支 else if / elif
来源：http://lo.asd995.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pj.wgjwhj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fp.bookmarksfly.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pj.wgjwhj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uq.shxzskj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vg.521024.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ng.shxzskj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yz.yuexingan06.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vn.nicolike.cn

[B03] switch / match / case
来源：http://wi.newstarts.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vw.9csxet.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://oq.shxzukj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xu.521024.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kz.hnjuh.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pv.szxytkj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bx.shxzskj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ou.muxihuayi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nu.wgjwhj.cn

[B04] for 计数循环
来源：http://vj.bjjhwx.cn

Py:   for i in range(10): print(i)
来源：http://im.yuntaijiaju.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xp.521024.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fy.yuexingan06.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ah.9csxet.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kr.nszjky.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nx.bjjhwx.cn

Ruby: 10.times { |i| puts i }
来源：http://zp.huanxung.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ia.lnxyls.cn

[B05] 遍历数组 / 列表
来源：http://fh.newstarts.cn

Py:   for item in arr: print(item)
来源：http://yb.yuntaijiaju.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://da.chemitech.net.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fn.hahajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bl.panjiajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vr.hnjuh.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://es.haigaiapp.cn

Ruby: arr.each { |item| puts item }
来源：http://ib.jctech888.com.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://it.newstarts.cn

[B06] 遍历字典 / 对象
来源：http://vo.shxzukj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://di.szxytkj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xi.haigaiapp.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sb.huanxung.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ex.lnxyls.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tm.szsharing.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nf.nszjky.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ud.szsharing.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ky.hahajie.cn

[B07] while 循环
来源：http://gw.colortex.cn

Py:   while i < 10: i += 1
来源：http://im.yuntaijiaju.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ed.jctech888.com.cn

JS:   while (i < 10) { i++; }
来源：http://wr.asd995.cn

TS:   while (i < 10) { i++; }
来源：http://ep.szsharing.cn

Java: while (i < 10) { i++; }
来源：http://nd.colortex.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nn.hnjuh.cn

Ruby: while i < 10; i += 1; end
来源：http://hv.huixiangedu.cn

C#:   while (i < 10) { i++; }
来源：http://vw.wgjwhj.cn

[B08] do-while（至少执行一次）
来源：http://jv.shxzskj.cn

Py:   # 无 do-while：用 while True + break
来源：http://ra.9csxet.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://rq.colortex.cn

JS:   do { i++; } while (i < 10);
来源：http://ap.huanxung.cn

TS:   do { i++; } while (i < 10);
来源：http://es.szxytkj.cn

Java: do { i++; } while (i < 10);
来源：http://iy.lnxyls.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wk.bookmarksfly.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hc.bjjhwx.cn

C#:   do { i++; } while (i < 10);
来源：http://rm.lnxyls.cn

[B09] break 与 continue
来源：http://ry.hahajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xt.hnjuh.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sn.wgjwhj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oe.newstarts.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bk.gzmigu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bb.huanxung.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xo.hnjuh.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sf.hnjuh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dj.shtwfgs.cn

[B10] 遍历同时拿索引
来源：http://ln.colortex.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ts.hahajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vg.huixiangedu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://po.huixinmuqiang.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://oq.bjjhwx.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ep.haigaiapp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qv.newstarts.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://aa.panjiajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xa.hnjuh.cn

[B11] 生成数字序列 / 区间
来源：http://vl.szxytkj.cn

Py:   list(range(0, 10, 2))
来源：http://fd.bookmarksfly.cn

PHP:  range(0, 10, 2);
来源：http://pn.yuexingan06.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cd.huixiangedu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pp.shxzukj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xl.huixiangedu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sx.huanxung.cn

Ruby: (0...10).step(2).to_a
来源：http://hs.jianghongdianzi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pz.muxihuayi.cn

[B12] 跳出多层循环
来源：http://sr.huixiangedu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://dc.huanxung.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wu.shxzukj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cu.hahajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kk.yuexingan06.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qj.szxytkj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vw.panjiajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ds.shtwfgs.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tz.hahajie.cn

[B13] 判断是否为数字
来源：http://cg.jctech888.com.cn

Py:   isinstance(x, (int, float))
来源：http://by.panjiajie.cn

PHP:  is_numeric($x)
来源：http://sl.521024.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yw.haigaiapp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iy.haigaiapp.cn

Java: x instanceof Number
来源：http://rj.hahajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ud.asd995.cn

Ruby: x.is_a?(Numeric)
来源：http://en.szxytkj.cn

C#:   x is int or double or decimal
来源：http://ac.yuexingan06.cn

[B14] 判断值是否在集合内
来源：http://bg.nicolike.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ro.wgjwhj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bt.hahajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://uw.chemitech.net.cn

TS:   [1, 2, 3].includes(x)
来源：http://tl.bookmarksfly.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kf.bookmarksfly.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nh.wgjwhj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://eb.huanxung.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ll.newstarts.cn

[B15] 布尔运算与取反
来源：http://ln.huixinmuqiang.cn

Py:   a and b or not c
来源：http://me.jctech888.com.cn

PHP:  $a && $b || !$c
来源：http://nx.bjjhwx.cn

JS:   a && b || !c
来源：http://mj.gzmigu.cn

TS:   a && b || !c
来源：http://ob.shtwfgs.cn

Java: a && b || !c
来源：http://hz.szsharing.cn

Go:   a && b || !c
来源：http://kn.asd995.cn

Ruby: a && b || !c
来源：http://jp.huanxung.cn

C#:   a && b || !c
来源：http://ut.hahajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://sf.shtwfgs.cn

Py:   if not data: return
来源：http://fx.9csxet.cn

PHP:  if (!$data) { return; }
来源：http://ev.asd995.cn

JS:   if (!data) return;
来源：http://hb.shxzskj.cn

TS:   if (!data) return;
来源：http://xr.yuntaijiaju.cn

Java: if (data == null) return;
来源：http://og.shxzukj.cn

Go:   if data == nil { return }
来源：http://sx.lnxyls.cn

Ruby: return if data.nil?
来源：http://ql.haigaiapp.cn

C#:   if (data == null) return;
来源：http://bx.szsharing.cn

================================================================================
来源：http://zk.shtwfgs.cn

C. 函数与作用域
来源：http://fa.szxytkj.cn

================================================================================
来源：http://vo.muxihuayi.cn

[C01] 定义函数
来源：http://vx.szsharing.cn

Py:   def add(a, b): return a + b
来源：http://xe.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ht.chemitech.net.cn

JS:   function add(a, b) { return a + b; }
来源：http://ss.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pf.chemitech.net.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://cl.panjiajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://de.gzmigu.cn

Ruby: def add(a, b); a + b; end
来源：http://bb.jianghongdianzi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://td.hnjuh.cn

[C02] 默认参数
来源：http://fv.bjjhwx.cn

Py:   def greet(name="World"): return name
来源：http://hw.szxytkj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ak.521024.cn

JS:   function greet(name = "World") { return name; }
来源：http://wq.szsharing.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://iv.jianghongdianzi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://tw.huixiangedu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qg.521024.cn

Ruby: def greet(name = "World") = name
来源：http://un.jianghongdianzi.cn

C#:   string Greet(string name = "World") => name;
来源：http://lx.gzmigu.cn

[C03] 可变参数
来源：http://ks.bookmarksfly.cn

Py:   def total(*args): return sum(args)
来源：http://to.bookmarksfly.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sz.asd995.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ms.bookmarksfly.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xf.shxzskj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://si.panjiajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ul.shxzskj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yy.yuntaijiaju.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kf.shtwfgs.cn

[C04] 命名参数 / 关键字参数
来源：http://qp.panjiajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bj.szxytkj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ap.huixiangedu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://se.haigaiapp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uk.yuexingan06.cn

Java: // 无：用 Builder 模式或 record
来源：http://op.lnxyls.cn

Go:   // 无：用配置结构体参数
来源：http://hb.huixinmuqiang.cn

Ruby: f(a: 1, b: 2)
来源：http://gx.nicolike.cn

C#:   f(a: 1, b: 2)
来源：http://ik.yuexingan06.cn

[C05] 返回多个值
来源：http://go.huanxung.cn

Py:   return a, b
来源：http://in.asd995.cn

PHP:  return [$a, $b];
来源：http://fj.521024.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://uk.wgjwhj.cn

TS:   return { a, b };
来源：http://ak.jianghongdianzi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://uq.szxytkj.cn

Go:   return a, b
来源：http://op.gzmigu.cn

Ruby: return a, b
来源：http://ix.huixiangedu.cn

C#:   return (a, b);              // ValueTuple
来源：http://lj.9csxet.cn

[C06] 匿名函数 / lambda
来源：http://tc.lnxyls.cn

Py:   square = lambda x: x * x
来源：http://ap.yuexingan06.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://jt.newstarts.cn

JS:   const square = x => x * x;
来源：http://tu.asd995.cn

TS:   const square = (x: number): number => x * x;
来源：http://kk.jianghongdianzi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://uh.huixinmuqiang.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ix.lnxyls.cn

Ruby: square = ->(x) { x * x }
来源：http://bg.asd995.cn

C#:   Func<int, int> square = x => x * x;
来源：http://jt.jianghongdianzi.cn

[C07] 把函数作为参数传入
来源：http://oa.huanxung.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jv.gzmigu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jv.muxihuayi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xu.bjjhwx.cn

TS:   arr.map(String)
来源：http://zh.nszjky.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rl.hahajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rf.bookmarksfly.cn

Ruby: arr.map(&:upcase)
来源：http://lt.haigaiapp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wt.huixiangedu.cn

[C08] 闭包
来源：http://wy.muxihuayi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kt.bookmarksfly.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rp.jianghongdianzi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yb.wgjwhj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wl.bjjhwx.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://on.hahajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://eb.huixinmuqiang.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://iz.asd995.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bo.yuexingan06.cn

[C09] 递归
来源：http://te.bjjhwx.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wk.hahajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rz.hahajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://da.gzmigu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zi.bjjhwx.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ac.muxihuayi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wq.szxytkj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jy.yuexingan06.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fl.bookmarksfly.cn

[C10] 变量作用域
来源：http://fa.hnjuh.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wl.panjiajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wk.shxzukj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fa.wgjwhj.cn

TS:   同 JS
来源：http://zy.jianghongdianzi.cn

Java: 方法内为块级作用域
来源：http://kx.haigaiapp.cn

Go:   花括号块级作用域
来源：http://xw.9csxet.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bj.huixiangedu.cn

C#:   块级作用域
来源：http://oa.521024.cn

[C11] 模块导入与导出
来源：http://gl.asd995.cn

Py:   from module import func
来源：http://ji.bjjhwx.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xa.nszjky.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ak.muxihuayi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ln.bookmarksfly.cn

Java: import java.util.List;
来源：http://hp.szsharing.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://oj.shtwfgs.cn

Ruby: require "json"; require_relative "./util"
来源：http://wo.hnjuh.cn

C#:   using System.Text;
来源：http://ms.bookmarksfly.cn

[C12] 立即执行函数 IIFE
来源：http://qc.shxzukj.cn

Py:   (lambda: print("run"))()
来源：http://sz.nicolike.cn

PHP:  (function () { echo "run"; })();
来源：http://ff.huixiangedu.cn

JS:   (() => { console.log("run"); })();
来源：http://tp.yuexingan06.cn

TS:   (() => { console.log("run"); })();
来源：http://ve.gzmigu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hp.asd995.cn

Go:   func() { fmt.Println("run") }()
来源：http://nj.shxzukj.cn

Ruby: -> { puts "run" }.call
来源：http://tl.shxzukj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://bz.hahajie.cn

[C13] 类型声明 / 类型注解
来源：http://xm.9csxet.cn


<!-- 参考信息 -->