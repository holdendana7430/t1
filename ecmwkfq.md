代发 wailian999

TS:   s.length
来源：http://si.9csxet.cn

Java: s.length()
来源：http://hf.huixinmuqiang.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ld.hnjuh.cn

Ruby: s.length
来源：http://rd.bookmarksfly.cn

C#:   s.Length
来源：http://js.bjjhwx.cn

[A23] 大小写转换
来源：http://yr.shtwfgs.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://cq.9csxet.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ar.shtwfgs.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nu.szsharing.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bp.yuntaijiaju.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bb.asd995.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rj.szxytkj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qc.shtwfgs.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ed.shxzskj.cn

[A24] 去除首尾空白
来源：http://fl.huixinmuqiang.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://aj.shxzskj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ml.chemitech.net.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kg.bookmarksfly.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oh.huixiangedu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://yw.shtwfgs.cn

Go:   strings.TrimSpace(s)
来源：http://rv.wgjwhj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ms.haigaiapp.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vs.nicolike.cn

[A25] 字符串比较
来源：http://rl.9csxet.cn

Py:   s1 == s2; s1 != s2
来源：http://us.wgjwhj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cz.jctech888.com.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cc.huixinmuqiang.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pb.gzmigu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ex.huixiangedu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wq.jianghongdianzi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ks.521024.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yg.nicolike.cn

[A26] 类型转换总览
来源：http://dv.szsharing.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ev.gzmigu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fx.hahajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mt.nicolike.cn

TS:   Number() String() Boolean() x as number
来源：http://yv.szxytkj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pw.newstarts.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rb.yuexingan06.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://yy.huixinmuqiang.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://em.521024.cn

================================================================================
来源：http://xs.huixinmuqiang.cn

B. 流程控制
来源：http://hy.muxihuayi.cn

================================================================================
来源：http://di.szsharing.cn

[B01] 条件判断 if / else
来源：http://jb.huanxung.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://us.szxytkj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yg.gzmigu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pk.szxytkj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nh.jctech888.com.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://iy.shxzskj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ig.szsharing.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://as.wgjwhj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nx.shxzukj.cn

[B02] 多分支 else if / elif
来源：http://bf.gzmigu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://we.lnxyls.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vf.bjjhwx.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ra.szsharing.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nz.bjjhwx.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fs.huanxung.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qg.nicolike.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mf.huixiangedu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oc.panjiajie.cn

[B03] switch / match / case
来源：http://bz.yuexingan06.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://du.huixinmuqiang.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vt.lnxyls.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mu.chemitech.net.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ni.gzmigu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ng.szxytkj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ms.jianghongdianzi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ma.huixiangedu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ln.bjjhwx.cn

[B04] for 计数循环
来源：http://vf.521024.cn

Py:   for i in range(10): print(i)
来源：http://ek.yuexingan06.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wf.521024.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jk.wgjwhj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kc.lnxyls.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tc.colortex.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bm.shtwfgs.cn

Ruby: 10.times { |i| puts i }
来源：http://nu.huanxung.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lz.yuexingan06.cn

[B05] 遍历数组 / 列表
来源：http://en.jianghongdianzi.cn

Py:   for item in arr: print(item)
来源：http://ac.521024.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ck.chemitech.net.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://vc.muxihuayi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mt.yuntaijiaju.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://bn.hnjuh.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://md.wgjwhj.cn

Ruby: arr.each { |item| puts item }
来源：http://hm.nszjky.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pn.shxzukj.cn

[B06] 遍历字典 / 对象
来源：http://zk.jianghongdianzi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ck.521024.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zh.521024.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oq.yuexingan06.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xn.asd995.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://it.panjiajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ez.521024.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wd.colortex.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yc.gzmigu.cn

[B07] while 循环
来源：http://gz.chemitech.net.cn

Py:   while i < 10: i += 1
来源：http://jn.9csxet.cn

PHP:  while ($i < 10) { $i++; }
来源：http://rj.521024.cn

JS:   while (i < 10) { i++; }
来源：http://hd.lnxyls.cn

TS:   while (i < 10) { i++; }
来源：http://vz.panjiajie.cn

Java: while (i < 10) { i++; }
来源：http://qr.huanxung.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://je.chemitech.net.cn

Ruby: while i < 10; i += 1; end
来源：http://uh.bjjhwx.cn

C#:   while (i < 10) { i++; }
来源：http://vd.chemitech.net.cn

[B08] do-while（至少执行一次）
来源：http://mv.muxihuayi.cn

Py:   # 无 do-while：用 while True + break
来源：http://xu.gzmigu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zf.huixiangedu.cn

JS:   do { i++; } while (i < 10);
来源：http://ma.lnxyls.cn

TS:   do { i++; } while (i < 10);
来源：http://mq.newstarts.cn

Java: do { i++; } while (i < 10);
来源：http://ab.shtwfgs.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://de.muxihuayi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ul.nszjky.cn

C#:   do { i++; } while (i < 10);
来源：http://yg.panjiajie.cn

[B09] break 与 continue
来源：http://ju.shxzskj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ql.bookmarksfly.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cc.hahajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fx.jctech888.com.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://em.9csxet.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jk.colortex.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xq.szxytkj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://km.szsharing.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://me.huanxung.cn

[B10] 遍历同时拿索引
来源：http://aq.szxytkj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zm.huixiangedu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hk.huixiangedu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jo.asd995.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ez.newstarts.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dz.bjjhwx.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://su.muxihuayi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mw.huixiangedu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://px.lnxyls.cn

[B11] 生成数字序列 / 区间
来源：http://lp.wgjwhj.cn

Py:   list(range(0, 10, 2))
来源：http://li.huixiangedu.cn

PHP:  range(0, 10, 2);
来源：http://xs.yuexingan06.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sb.huanxung.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://el.521024.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://js.hahajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vr.huanxung.cn

Ruby: (0...10).step(2).to_a
来源：http://hb.asd995.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ze.521024.cn

[B12] 跳出多层循环
来源：http://nd.asd995.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://rm.hnjuh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ff.huixiangedu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wt.lnxyls.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zf.asd995.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ln.gzmigu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qz.muxihuayi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cb.jctech888.com.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bq.jianghongdianzi.cn

[B13] 判断是否为数字
来源：http://uj.9csxet.cn

Py:   isinstance(x, (int, float))
来源：http://du.lnxyls.cn

PHP:  is_numeric($x)
来源：http://fi.gzmigu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://co.lnxyls.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ek.chemitech.net.cn

Java: x instanceof Number
来源：http://mm.colortex.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sz.huixinmuqiang.cn

Ruby: x.is_a?(Numeric)
来源：http://yd.lnxyls.cn

C#:   x is int or double or decimal
来源：http://qj.hahajie.cn

[B14] 判断值是否在集合内
来源：http://ls.9csxet.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://te.colortex.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ij.nszjky.cn

JS:   [1, 2, 3].includes(x)
来源：http://fx.huanxung.cn

TS:   [1, 2, 3].includes(x)
来源：http://oq.panjiajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ga.panjiajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yl.bookmarksfly.cn

Ruby: [1, 2, 3].include?(x)
来源：http://un.gzmigu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vf.gzmigu.cn

[B15] 布尔运算与取反
来源：http://ue.huanxung.cn

Py:   a and b or not c
来源：http://no.bjjhwx.cn

PHP:  $a && $b || !$c
来源：http://ic.hnjuh.cn

JS:   a && b || !c
来源：http://yc.szxytkj.cn

TS:   a && b || !c
来源：http://sh.asd995.cn

Java: a && b || !c
来源：http://hn.haigaiapp.cn

Go:   a && b || !c
来源：http://qy.jctech888.com.cn

Ruby: a && b || !c
来源：http://jn.yuntaijiaju.cn

C#:   a && b || !c
来源：http://mn.asd995.cn

[B16] 卫语句：不满足条件提前返回
来源：http://mu.bookmarksfly.cn

Py:   if not data: return
来源：http://ir.hahajie.cn

PHP:  if (!$data) { return; }
来源：http://id.bjjhwx.cn

JS:   if (!data) return;
来源：http://np.bookmarksfly.cn

TS:   if (!data) return;
来源：http://hr.521024.cn

Java: if (data == null) return;
来源：http://kz.jianghongdianzi.cn

Go:   if data == nil { return }
来源：http://fm.huanxung.cn

Ruby: return if data.nil?
来源：http://gd.huixinmuqiang.cn

C#:   if (data == null) return;
来源：http://zy.521024.cn

================================================================================
来源：http://ha.colortex.cn

C. 函数与作用域
来源：http://md.haigaiapp.cn

================================================================================
来源：http://cc.gzmigu.cn

[C01] 定义函数
来源：http://me.nszjky.cn

Py:   def add(a, b): return a + b
来源：http://hl.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zu.yuexingan06.cn

JS:   function add(a, b) { return a + b; }
来源：http://rs.panjiajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ku.yuexingan06.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gq.bjjhwx.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mr.bookmarksfly.cn

Ruby: def add(a, b); a + b; end
来源：http://jl.shtwfgs.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ha.newstarts.cn

[C02] 默认参数
来源：http://tr.9csxet.cn

Py:   def greet(name="World"): return name
来源：http://dz.nszjky.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fw.bjjhwx.cn

JS:   function greet(name = "World") { return name; }
来源：http://gu.jianghongdianzi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qt.szsharing.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://tm.huanxung.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fx.szxytkj.cn

Ruby: def greet(name = "World") = name
来源：http://ys.newstarts.cn

C#:   string Greet(string name = "World") => name;
来源：http://af.nicolike.cn

[C03] 可变参数
来源：http://hn.hnjuh.cn

Py:   def total(*args): return sum(args)
来源：http://zg.wgjwhj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://av.muxihuayi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fr.nicolike.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ub.yuntaijiaju.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nd.shxzskj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cr.shtwfgs.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zh.huanxung.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ov.shtwfgs.cn

[C04] 命名参数 / 关键字参数
来源：http://lq.521024.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://va.wgjwhj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://au.wgjwhj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://aw.nicolike.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hc.wgjwhj.cn

Java: // 无：用 Builder 模式或 record
来源：http://ee.lnxyls.cn

Go:   // 无：用配置结构体参数
来源：http://zt.szsharing.cn

Ruby: f(a: 1, b: 2)
来源：http://pj.yuntaijiaju.cn

C#:   f(a: 1, b: 2)
来源：http://jt.hahajie.cn

[C05] 返回多个值
来源：http://zl.wgjwhj.cn

Py:   return a, b
来源：http://ph.huanxung.cn

PHP:  return [$a, $b];
来源：http://mb.huanxung.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://nw.huixiangedu.cn

TS:   return { a, b };
来源：http://ez.colortex.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mo.newstarts.cn

Go:   return a, b
来源：http://ga.shxzukj.cn

Ruby: return a, b
来源：http://pt.huixiangedu.cn

C#:   return (a, b);              // ValueTuple
来源：http://wf.shxzskj.cn

[C06] 匿名函数 / lambda
来源：http://xp.jianghongdianzi.cn

Py:   square = lambda x: x * x
来源：http://me.szsharing.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qb.jianghongdianzi.cn

JS:   const square = x => x * x;
来源：http://hf.jianghongdianzi.cn

TS:   const square = (x: number): number => x * x;
来源：http://cq.jianghongdianzi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://es.huanxung.cn

Go:   sq := func(x int) int { return x * x }
来源：http://cp.9csxet.cn

Ruby: square = ->(x) { x * x }
来源：http://gx.chemitech.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://cd.huixinmuqiang.cn

[C07] 把函数作为参数传入
来源：http://vx.muxihuayi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://av.shxzukj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://nq.shxzskj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rx.huixinmuqiang.cn

TS:   arr.map(String)
来源：http://qo.szxytkj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://iv.nszjky.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ue.haigaiapp.cn

Ruby: arr.map(&:upcase)
来源：http://jx.hahajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://lp.chemitech.net.cn

[C08] 闭包
来源：http://oe.jctech888.com.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ru.lnxyls.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tg.huixiangedu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nn.nszjky.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ej.szsharing.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wh.newstarts.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ti.haigaiapp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cl.huixinmuqiang.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gy.huanxung.cn

[C09] 递归
来源：http://nk.yuexingan06.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nv.szxytkj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dr.hahajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yx.szxytkj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hr.huanxung.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nt.shxzukj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pl.szxytkj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ap.lnxyls.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tz.jianghongdianzi.cn

[C10] 变量作用域
来源：http://yj.gzmigu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ac.yuexingan06.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ly.shxzskj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dn.nicolike.cn

TS:   同 JS
来源：http://uf.nicolike.cn

Java: 方法内为块级作用域
来源：http://fh.shxzskj.cn

Go:   花括号块级作用域
来源：http://yp.szxytkj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ut.jianghongdianzi.cn

C#:   块级作用域
来源：http://gy.lnxyls.cn

[C11] 模块导入与导出
来源：http://oe.bjjhwx.cn

Py:   from module import func
来源：http://rp.asd995.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ep.shxzskj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ox.newstarts.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qr.jctech888.com.cn

Java: import java.util.List;
来源：http://jj.yuntaijiaju.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ov.haigaiapp.cn

Ruby: require "json"; require_relative "./util"
来源：http://qc.yuntaijiaju.cn

C#:   using System.Text;
来源：http://xo.huanxung.cn

[C12] 立即执行函数 IIFE
来源：http://yx.9csxet.cn

Py:   (lambda: print("run"))()
来源：http://qp.gzmigu.cn

PHP:  (function () { echo "run"; })();
来源：http://zu.nicolike.cn

JS:   (() => { console.log("run"); })();
来源：http://ie.yuntaijiaju.cn

TS:   (() => { console.log("run"); })();
来源：http://jt.hnjuh.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sv.nszjky.cn

Go:   func() { fmt.Println("run") }()
来源：http://ga.colortex.cn

Ruby: -> { puts "run" }.call
来源：http://xy.szsharing.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xm.muxihuayi.cn

[C13] 类型声明 / 类型注解
来源：http://cd.hahajie.cn


<!-- 参考信息 -->