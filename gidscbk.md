代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nl.asd995.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://px.yuexingan06.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nj.huanxung.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://om.521024.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zv.gzmigu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://bw.shtwfgs.cn

[A24] 去除首尾空白
来源：http://jx.shxzskj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mu.panjiajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zb.gzmigu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ne.huixinmuqiang.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ry.bookmarksfly.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ce.huixiangedu.cn

Go:   strings.TrimSpace(s)
来源：http://hj.muxihuayi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xc.szxytkj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://il.lnxyls.cn

[A25] 字符串比较
来源：http://yr.haigaiapp.cn

Py:   s1 == s2; s1 != s2
来源：http://rn.9csxet.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qu.wgjwhj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://it.bjjhwx.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tq.wgjwhj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ju.colortex.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://aa.bookmarksfly.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://co.haigaiapp.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vj.newstarts.cn

[A26] 类型转换总览
来源：http://fa.bjjhwx.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dv.szsharing.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yo.colortex.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cj.shxzskj.cn

TS:   Number() String() Boolean() x as number
来源：http://na.szxytkj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xh.panjiajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ky.huixiangedu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vp.colortex.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kf.jctech888.com.cn

================================================================================
来源：http://fl.haigaiapp.cn

B. 流程控制
来源：http://yf.newstarts.cn

================================================================================
来源：http://kt.huixinmuqiang.cn

[B01] 条件判断 if / else
来源：http://kp.haigaiapp.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://kt.shtwfgs.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xo.szsharing.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bh.newstarts.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ct.gzmigu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qg.bookmarksfly.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vt.muxihuayi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gk.521024.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://df.szxytkj.cn

[B02] 多分支 else if / elif
来源：http://sg.hnjuh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ju.huixinmuqiang.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sl.bjjhwx.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ou.hahajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qb.hahajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xe.chemitech.net.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ir.shxzskj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zg.shtwfgs.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://di.hahajie.cn

[B03] switch / match / case
来源：http://ty.colortex.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vs.huixiangedu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sq.huanxung.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fo.yuexingan06.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ns.huixiangedu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ft.newstarts.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bp.yuntaijiaju.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://od.nszjky.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xr.huanxung.cn

[B04] for 计数循环
来源：http://fe.shxzukj.cn

Py:   for i in range(10): print(i)
来源：http://qq.muxihuayi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://we.gzmigu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pc.jianghongdianzi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tr.shxzskj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nf.nszjky.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ab.yuntaijiaju.cn

Ruby: 10.times { |i| puts i }
来源：http://xf.hahajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fd.szsharing.cn

[B05] 遍历数组 / 列表
来源：http://hv.huixiangedu.cn

Py:   for item in arr: print(item)
来源：http://cg.gzmigu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jm.szxytkj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ys.shxzskj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yo.nicolike.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zy.jianghongdianzi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://iq.shxzukj.cn

Ruby: arr.each { |item| puts item }
来源：http://yu.wgjwhj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gn.huixiangedu.cn

[B06] 遍历字典 / 对象
来源：http://uj.shxzskj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ns.shxzskj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://at.huixiangedu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://me.hahajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://na.chemitech.net.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ds.9csxet.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ce.nicolike.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sp.nszjky.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xk.bookmarksfly.cn

[B07] while 循环
来源：http://yd.szxytkj.cn

Py:   while i < 10: i += 1
来源：http://vg.wgjwhj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ds.nicolike.cn

JS:   while (i < 10) { i++; }
来源：http://fm.yuexingan06.cn

TS:   while (i < 10) { i++; }
来源：http://os.panjiajie.cn

Java: while (i < 10) { i++; }
来源：http://zi.szxytkj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zo.nicolike.cn

Ruby: while i < 10; i += 1; end
来源：http://ah.szxytkj.cn

C#:   while (i < 10) { i++; }
来源：http://cc.nszjky.cn

[B08] do-while（至少执行一次）
来源：http://dh.jianghongdianzi.cn

Py:   # 无 do-while：用 while True + break
来源：http://ng.lnxyls.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vr.shtwfgs.cn

JS:   do { i++; } while (i < 10);
来源：http://ob.haigaiapp.cn

TS:   do { i++; } while (i < 10);
来源：http://ve.hahajie.cn

Java: do { i++; } while (i < 10);
来源：http://nx.huanxung.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://eh.szsharing.cn

Ruby: begin; i += 1; end while i < 10
来源：http://gl.haigaiapp.cn

C#:   do { i++; } while (i < 10);
来源：http://ya.bookmarksfly.cn

[B09] break 与 continue
来源：http://zb.bookmarksfly.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qy.szxytkj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://py.shxzskj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://on.hnjuh.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gg.bjjhwx.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ai.bookmarksfly.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zu.hahajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://co.muxihuayi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xa.nicolike.cn

[B10] 遍历同时拿索引
来源：http://ef.chemitech.net.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ur.9csxet.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xg.panjiajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tf.nicolike.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ew.lnxyls.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nx.szxytkj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tt.jianghongdianzi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yu.huixiangedu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ez.jctech888.com.cn

[B11] 生成数字序列 / 区间
来源：http://xy.bjjhwx.cn

Py:   list(range(0, 10, 2))
来源：http://qv.yuexingan06.cn

PHP:  range(0, 10, 2);
来源：http://ee.nszjky.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xk.shtwfgs.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ls.huixinmuqiang.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ux.shtwfgs.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kt.bookmarksfly.cn

Ruby: (0...10).step(2).to_a
来源：http://iy.muxihuayi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jq.panjiajie.cn

[B12] 跳出多层循环
来源：http://pv.haigaiapp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://af.newstarts.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://eg.huixinmuqiang.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dd.newstarts.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mz.gzmigu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rk.chemitech.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ij.asd995.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pq.nicolike.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sn.shxzskj.cn

[B13] 判断是否为数字
来源：http://sh.huixiangedu.cn

Py:   isinstance(x, (int, float))
来源：http://rh.newstarts.cn

PHP:  is_numeric($x)
来源：http://dr.shxzskj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ve.jctech888.com.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xt.jianghongdianzi.cn

Java: x instanceof Number
来源：http://wu.hnjuh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uk.9csxet.cn

Ruby: x.is_a?(Numeric)
来源：http://pq.nszjky.cn

C#:   x is int or double or decimal
来源：http://ue.newstarts.cn

[B14] 判断值是否在集合内
来源：http://pl.bjjhwx.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ev.haigaiapp.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gj.szsharing.cn

JS:   [1, 2, 3].includes(x)
来源：http://fq.newstarts.cn

TS:   [1, 2, 3].includes(x)
来源：http://mx.szsharing.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://it.chemitech.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ob.lnxyls.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gm.gzmigu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xp.szsharing.cn

[B15] 布尔运算与取反
来源：http://hq.yuntaijiaju.cn

Py:   a and b or not c
来源：http://tv.hnjuh.cn

PHP:  $a && $b || !$c
来源：http://vw.muxihuayi.cn

JS:   a && b || !c
来源：http://xs.asd995.cn

TS:   a && b || !c
来源：http://cc.szsharing.cn

Java: a && b || !c
来源：http://sw.bookmarksfly.cn

Go:   a && b || !c
来源：http://no.shxzskj.cn

Ruby: a && b || !c
来源：http://rm.nicolike.cn

C#:   a && b || !c
来源：http://py.haigaiapp.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jb.szsharing.cn

Py:   if not data: return
来源：http://zc.szsharing.cn

PHP:  if (!$data) { return; }
来源：http://xz.yuexingan06.cn

JS:   if (!data) return;
来源：http://fs.szxytkj.cn

TS:   if (!data) return;
来源：http://je.521024.cn

Java: if (data == null) return;
来源：http://au.jctech888.com.cn

Go:   if data == nil { return }
来源：http://pt.haigaiapp.cn

Ruby: return if data.nil?
来源：http://sb.huixiangedu.cn

C#:   if (data == null) return;
来源：http://vl.szsharing.cn

================================================================================
来源：http://ys.haigaiapp.cn

C. 函数与作用域
来源：http://pu.bjjhwx.cn

================================================================================
来源：http://dx.wgjwhj.cn

[C01] 定义函数
来源：http://yk.yuntaijiaju.cn

Py:   def add(a, b): return a + b
来源：http://lr.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uj.haigaiapp.cn

JS:   function add(a, b) { return a + b; }
来源：http://qh.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iv.hnjuh.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://kp.shxzskj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qv.asd995.cn

Ruby: def add(a, b); a + b; end
来源：http://uc.shxzskj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ml.shxzskj.cn

[C02] 默认参数
来源：http://ao.yuexingan06.cn

Py:   def greet(name="World"): return name
来源：http://jb.huanxung.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qh.nicolike.cn

JS:   function greet(name = "World") { return name; }
来源：http://pd.jctech888.com.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://dq.huanxung.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wk.huanxung.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://eh.panjiajie.cn

Ruby: def greet(name = "World") = name
来源：http://yq.hnjuh.cn

C#:   string Greet(string name = "World") => name;
来源：http://ff.bookmarksfly.cn

[C03] 可变参数
来源：http://bg.nicolike.cn

Py:   def total(*args): return sum(args)
来源：http://wj.yuntaijiaju.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ki.panjiajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yj.asd995.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ry.gzmigu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kx.huixinmuqiang.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yj.nszjky.cn

Ruby: def total(*nums); nums.sum; end
来源：http://lp.shxzskj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zd.yuexingan06.cn

[C04] 命名参数 / 关键字参数
来源：http://tf.panjiajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://iz.shxzukj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cg.haigaiapp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hm.shxzskj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tt.huanxung.cn

Java: // 无：用 Builder 模式或 record
来源：http://hb.yuntaijiaju.cn

Go:   // 无：用配置结构体参数
来源：http://zk.lnxyls.cn

Ruby: f(a: 1, b: 2)
来源：http://yz.asd995.cn

C#:   f(a: 1, b: 2)
来源：http://sl.jctech888.com.cn

[C05] 返回多个值
来源：http://ec.hahajie.cn

Py:   return a, b
来源：http://vv.muxihuayi.cn

PHP:  return [$a, $b];
来源：http://ty.hahajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xg.asd995.cn

TS:   return { a, b };
来源：http://ld.szsharing.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mv.yuexingan06.cn

Go:   return a, b
来源：http://kn.shtwfgs.cn

Ruby: return a, b
来源：http://qf.yuexingan06.cn

C#:   return (a, b);              // ValueTuple
来源：http://iz.newstarts.cn

[C06] 匿名函数 / lambda
来源：http://qo.bookmarksfly.cn

Py:   square = lambda x: x * x
来源：http://cb.shxzukj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bm.gzmigu.cn

JS:   const square = x => x * x;
来源：http://zo.muxihuayi.cn

TS:   const square = (x: number): number => x * x;
来源：http://it.shxzskj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ac.huixiangedu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zo.asd995.cn

Ruby: square = ->(x) { x * x }
来源：http://pf.shxzskj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ob.jctech888.com.cn

[C07] 把函数作为参数传入
来源：http://ht.haigaiapp.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qg.jctech888.com.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ll.gzmigu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ti.bjjhwx.cn

TS:   arr.map(String)
来源：http://ev.huixiangedu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uc.huixinmuqiang.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dl.yuexingan06.cn

Ruby: arr.map(&:upcase)
来源：http://pv.hahajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jy.jctech888.com.cn

[C08] 闭包
来源：http://xm.huanxung.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pw.huixiangedu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gh.asd995.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vb.lnxyls.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wr.521024.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cw.newstarts.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rz.huixinmuqiang.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://md.shtwfgs.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ic.shxzskj.cn

[C09] 递归
来源：http://xn.wgjwhj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ae.huixinmuqiang.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bi.haigaiapp.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rl.521024.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hp.colortex.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hj.jianghongdianzi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://eh.panjiajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sn.nszjky.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ir.bjjhwx.cn

[C10] 变量作用域
来源：http://tv.szxytkj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xc.szxytkj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hx.szsharing.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ci.gzmigu.cn

TS:   同 JS
来源：http://bc.huixiangedu.cn

Java: 方法内为块级作用域
来源：http://ua.huanxung.cn

Go:   花括号块级作用域
来源：http://kt.shtwfgs.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fx.huixiangedu.cn

C#:   块级作用域
来源：http://qq.bjjhwx.cn

[C11] 模块导入与导出
来源：http://jp.yuexingan06.cn

Py:   from module import func
来源：http://fz.hnjuh.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://jl.yuntaijiaju.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rx.szxytkj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rk.nszjky.cn

Java: import java.util.List;
来源：http://re.yuntaijiaju.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ka.huixiangedu.cn

Ruby: require "json"; require_relative "./util"
来源：http://hn.panjiajie.cn

C#:   using System.Text;
来源：http://hw.bjjhwx.cn

[C12] 立即执行函数 IIFE
来源：http://sq.shxzskj.cn

Py:   (lambda: print("run"))()
来源：http://sx.colortex.cn

PHP:  (function () { echo "run"; })();
来源：http://hs.9csxet.cn

JS:   (() => { console.log("run"); })();
来源：http://ll.521024.cn

TS:   (() => { console.log("run"); })();
来源：http://lc.nicolike.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ku.wgjwhj.cn

Go:   func() { fmt.Println("run") }()
来源：http://up.shxzukj.cn

Ruby: -> { puts "run" }.call
来源：http://ey.bjjhwx.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://eq.nicolike.cn

[C13] 类型声明 / 类型注解
来源：http://hr.shxzskj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nl.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ji.521024.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bs.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lw.jctech888.com.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ki.hahajie.cn

Go:   func add(a, b int) int
来源：http://nf.asd995.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vh.newstarts.cn

C#:   int Add(int a, int b) => a + b;
来源：http://dt.lnxyls.cn


<!-- 参考信息 -->