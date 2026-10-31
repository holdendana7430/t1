代发 wailian999

C#:   s.Length
来源：http://io.gzmigu.cn

[A23] 大小写转换
来源：http://qr.huixinmuqiang.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://hw.huanxung.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zg.gzmigu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wz.panjiajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ew.huixinmuqiang.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vu.jianghongdianzi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ow.szsharing.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://py.newstarts.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ch.hnjuh.cn

[A24] 去除首尾空白
来源：http://kf.bjjhwx.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://om.huanxung.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://oo.lnxyls.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ob.nszjky.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hh.gzmigu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nc.yuntaijiaju.cn

Go:   strings.TrimSpace(s)
来源：http://qq.yuntaijiaju.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lc.asd995.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sw.wgjwhj.cn

[A25] 字符串比较
来源：http://he.nicolike.cn

Py:   s1 == s2; s1 != s2
来源：http://cx.521024.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hy.521024.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ya.huanxung.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gj.wgjwhj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gy.lnxyls.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://aw.hnjuh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://xm.lnxyls.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fp.jctech888.com.cn

[A26] 类型转换总览
来源：http://az.panjiajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rm.nicolike.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lh.muxihuayi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ua.newstarts.cn

TS:   Number() String() Boolean() x as number
来源：http://nc.jianghongdianzi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zp.huixinmuqiang.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fh.yuexingan06.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ex.hnjuh.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qt.lnxyls.cn

================================================================================
来源：http://kv.521024.cn

B. 流程控制
来源：http://ct.shxzskj.cn

================================================================================
来源：http://js.asd995.cn

[B01] 条件判断 if / else
来源：http://sn.hnjuh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ff.newstarts.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ex.szxytkj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nx.huanxung.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zb.yuexingan06.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xi.gzmigu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://st.shxzskj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://uu.colortex.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pb.haigaiapp.cn

[B02] 多分支 else if / elif
来源：http://eo.jianghongdianzi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pd.yuntaijiaju.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://is.gzmigu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oq.colortex.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zq.shxzskj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tj.colortex.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://oc.panjiajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vs.huixinmuqiang.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dg.hnjuh.cn

[B03] switch / match / case
来源：http://if.chemitech.net.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kd.szxytkj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ko.hnjuh.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pu.hnjuh.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ry.chemitech.net.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mb.9csxet.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gb.wgjwhj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xt.hahajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://px.bookmarksfly.cn

[B04] for 计数循环
来源：http://ha.bjjhwx.cn

Py:   for i in range(10): print(i)
来源：http://dx.haigaiapp.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wf.haigaiapp.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rx.huanxung.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yj.hahajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jr.szsharing.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gq.bjjhwx.cn

Ruby: 10.times { |i| puts i }
来源：http://xz.muxihuayi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ld.muxihuayi.cn

[B05] 遍历数组 / 列表
来源：http://kb.yuntaijiaju.cn

Py:   for item in arr: print(item)
来源：http://vv.huixiangedu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xg.shtwfgs.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://iq.shtwfgs.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://zz.asd995.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fg.szxytkj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://do.szxytkj.cn

Ruby: arr.each { |item| puts item }
来源：http://nj.shtwfgs.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bt.yuntaijiaju.cn

[B06] 遍历字典 / 对象
来源：http://lp.haigaiapp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://yy.521024.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://md.asd995.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vg.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ez.asd995.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://al.wgjwhj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kp.hahajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ov.colortex.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xo.chemitech.net.cn

[B07] while 循环
来源：http://zg.hnjuh.cn

Py:   while i < 10: i += 1
来源：http://yx.colortex.cn

PHP:  while ($i < 10) { $i++; }
来源：http://am.shxzskj.cn

JS:   while (i < 10) { i++; }
来源：http://hu.521024.cn

TS:   while (i < 10) { i++; }
来源：http://tq.huixiangedu.cn

Java: while (i < 10) { i++; }
来源：http://ji.newstarts.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zo.szsharing.cn

Ruby: while i < 10; i += 1; end
来源：http://tx.9csxet.cn

C#:   while (i < 10) { i++; }
来源：http://ei.chemitech.net.cn

[B08] do-while（至少执行一次）
来源：http://qn.jctech888.com.cn

Py:   # 无 do-while：用 while True + break
来源：http://ns.chemitech.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ny.huixinmuqiang.cn

JS:   do { i++; } while (i < 10);
来源：http://ae.gzmigu.cn

TS:   do { i++; } while (i < 10);
来源：http://zo.nszjky.cn

Java: do { i++; } while (i < 10);
来源：http://nl.9csxet.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ox.huanxung.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ag.shxzskj.cn

C#:   do { i++; } while (i < 10);
来源：http://ru.szsharing.cn

[B09] break 与 continue
来源：http://ih.shxzukj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vb.hahajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xo.shtwfgs.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pk.huixinmuqiang.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hq.szxytkj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pq.shtwfgs.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tx.asd995.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yq.colortex.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ch.shxzskj.cn

[B10] 遍历同时拿索引
来源：http://ut.szsharing.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ms.nszjky.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://oe.szxytkj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yu.colortex.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vo.szsharing.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wd.bjjhwx.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://th.hahajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cn.521024.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dq.yuexingan06.cn

[B11] 生成数字序列 / 区间
来源：http://sa.muxihuayi.cn

Py:   list(range(0, 10, 2))
来源：http://qg.shtwfgs.cn

PHP:  range(0, 10, 2);
来源：http://us.yuntaijiaju.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://do.shxzskj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yq.nicolike.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qi.nicolike.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rb.wgjwhj.cn

Ruby: (0...10).step(2).to_a
来源：http://sl.nicolike.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ci.bjjhwx.cn

[B12] 跳出多层循环
来源：http://fp.hnjuh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ld.bjjhwx.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://jp.panjiajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ct.haigaiapp.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fc.huanxung.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ow.yuntaijiaju.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gx.asd995.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jx.521024.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bg.huixinmuqiang.cn

[B13] 判断是否为数字
来源：http://jo.shtwfgs.cn

Py:   isinstance(x, (int, float))
来源：http://ww.huixiangedu.cn

PHP:  is_numeric($x)
来源：http://uj.9csxet.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yg.haigaiapp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pu.nszjky.cn

Java: x instanceof Number
来源：http://uv.muxihuayi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ln.asd995.cn

Ruby: x.is_a?(Numeric)
来源：http://jp.jianghongdianzi.cn

C#:   x is int or double or decimal
来源：http://ij.shtwfgs.cn

[B14] 判断值是否在集合内
来源：http://xb.muxihuayi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mn.bookmarksfly.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bv.bjjhwx.cn

JS:   [1, 2, 3].includes(x)
来源：http://go.haigaiapp.cn

TS:   [1, 2, 3].includes(x)
来源：http://bs.shxzskj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qw.szxytkj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ld.bookmarksfly.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jo.521024.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://en.chemitech.net.cn

[B15] 布尔运算与取反
来源：http://ee.hahajie.cn

Py:   a and b or not c
来源：http://ps.nszjky.cn

PHP:  $a && $b || !$c
来源：http://jy.asd995.cn

JS:   a && b || !c
来源：http://oq.gzmigu.cn

TS:   a && b || !c
来源：http://ym.9csxet.cn

Java: a && b || !c
来源：http://dx.newstarts.cn

Go:   a && b || !c
来源：http://dx.jianghongdianzi.cn

Ruby: a && b || !c
来源：http://ip.newstarts.cn

C#:   a && b || !c
来源：http://mm.gzmigu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lj.9csxet.cn

Py:   if not data: return
来源：http://pp.asd995.cn

PHP:  if (!$data) { return; }
来源：http://yf.newstarts.cn

JS:   if (!data) return;
来源：http://fb.lnxyls.cn

TS:   if (!data) return;
来源：http://ad.haigaiapp.cn

Java: if (data == null) return;
来源：http://fl.nicolike.cn

Go:   if data == nil { return }
来源：http://su.jianghongdianzi.cn

Ruby: return if data.nil?
来源：http://yb.wgjwhj.cn

C#:   if (data == null) return;
来源：http://tc.chemitech.net.cn

================================================================================
来源：http://sk.shxzukj.cn

C. 函数与作用域
来源：http://fx.szsharing.cn

================================================================================
来源：http://mg.521024.cn

[C01] 定义函数
来源：http://ip.huixiangedu.cn

Py:   def add(a, b): return a + b
来源：http://nd.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oa.shxzskj.cn

JS:   function add(a, b) { return a + b; }
来源：http://cj.huixinmuqiang.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qb.hnjuh.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ie.jctech888.com.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ca.wgjwhj.cn

Ruby: def add(a, b); a + b; end
来源：http://au.jctech888.com.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fl.wgjwhj.cn

[C02] 默认参数
来源：http://il.shxzskj.cn

Py:   def greet(name="World"): return name
来源：http://xm.shxzskj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yh.yuexingan06.cn

JS:   function greet(name = "World") { return name; }
来源：http://qw.9csxet.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zp.jianghongdianzi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://th.521024.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://in.lnxyls.cn

Ruby: def greet(name = "World") = name
来源：http://aa.lnxyls.cn

C#:   string Greet(string name = "World") => name;
来源：http://ub.yuntaijiaju.cn

[C03] 可变参数
来源：http://ay.szxytkj.cn

Py:   def total(*args): return sum(args)
来源：http://gc.szsharing.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fq.gzmigu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://oi.szsharing.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ac.huanxung.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://re.huixinmuqiang.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gz.szxytkj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://es.hahajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://et.szxytkj.cn

[C04] 命名参数 / 关键字参数
来源：http://cp.szxytkj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mo.yuexingan06.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mv.hnjuh.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ai.huixinmuqiang.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fr.shxzukj.cn

Java: // 无：用 Builder 模式或 record
来源：http://gd.chemitech.net.cn

Go:   // 无：用配置结构体参数
来源：http://gr.newstarts.cn

Ruby: f(a: 1, b: 2)
来源：http://sd.9csxet.cn

C#:   f(a: 1, b: 2)
来源：http://il.shtwfgs.cn

[C05] 返回多个值
来源：http://yc.bookmarksfly.cn

Py:   return a, b
来源：http://qj.shtwfgs.cn

PHP:  return [$a, $b];
来源：http://oe.gzmigu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://tt.hnjuh.cn

TS:   return { a, b };
来源：http://zn.haigaiapp.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ky.gzmigu.cn

Go:   return a, b
来源：http://qd.szxytkj.cn

Ruby: return a, b
来源：http://nk.nszjky.cn

C#:   return (a, b);              // ValueTuple
来源：http://va.panjiajie.cn

[C06] 匿名函数 / lambda
来源：http://qo.shxzukj.cn

Py:   square = lambda x: x * x
来源：http://oc.hahajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fd.bookmarksfly.cn

JS:   const square = x => x * x;
来源：http://qq.lnxyls.cn

TS:   const square = (x: number): number => x * x;
来源：http://qs.9csxet.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wo.521024.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wo.asd995.cn

Ruby: square = ->(x) { x * x }
来源：http://nr.huanxung.cn

C#:   Func<int, int> square = x => x * x;
来源：http://pc.huixiangedu.cn

[C07] 把函数作为参数传入
来源：http://dc.panjiajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lb.521024.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zv.jianghongdianzi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gn.hahajie.cn

TS:   arr.map(String)
来源：http://gv.huanxung.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yg.hnjuh.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zm.huanxung.cn

Ruby: arr.map(&:upcase)
来源：http://mb.huanxung.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ss.shxzukj.cn

[C08] 闭包
来源：http://yf.hnjuh.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ao.szsharing.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hk.bjjhwx.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ef.colortex.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ni.shxzskj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wm.asd995.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hb.wgjwhj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://iw.jctech888.com.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nb.szxytkj.cn

[C09] 递归
来源：http://pd.gzmigu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bw.nicolike.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ta.9csxet.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nz.chemitech.net.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ib.nicolike.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bk.chemitech.net.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rp.9csxet.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vz.wgjwhj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ec.haigaiapp.cn

[C10] 变量作用域
来源：http://fl.huixinmuqiang.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fc.hahajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://as.szxytkj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://em.panjiajie.cn

TS:   同 JS
来源：http://wg.9csxet.cn

Java: 方法内为块级作用域
来源：http://tw.shxzukj.cn

Go:   花括号块级作用域
来源：http://po.jctech888.com.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sb.shxzskj.cn

C#:   块级作用域
来源：http://rv.bookmarksfly.cn

[C11] 模块导入与导出
来源：http://in.wgjwhj.cn

Py:   from module import func
来源：http://uc.9csxet.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ik.gzmigu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vu.shxzskj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lx.haigaiapp.cn

Java: import java.util.List;
来源：http://dz.shxzskj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://je.colortex.cn

Ruby: require "json"; require_relative "./util"
来源：http://ew.jianghongdianzi.cn

C#:   using System.Text;
来源：http://dj.muxihuayi.cn

[C12] 立即执行函数 IIFE
来源：http://zb.huanxung.cn

Py:   (lambda: print("run"))()
来源：http://cz.szsharing.cn

PHP:  (function () { echo "run"; })();
来源：http://hg.yuexingan06.cn

JS:   (() => { console.log("run"); })();
来源：http://qg.szxytkj.cn

TS:   (() => { console.log("run"); })();
来源：http://xy.shtwfgs.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ov.colortex.cn

Go:   func() { fmt.Println("run") }()
来源：http://qw.jctech888.com.cn

Ruby: -> { puts "run" }.call
来源：http://tw.9csxet.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://kj.wgjwhj.cn

[C13] 类型声明 / 类型注解
来源：http://rt.newstarts.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://av.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ut.wgjwhj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bt.hahajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kc.nicolike.cn


<!-- 参考信息 -->