代发 wailian999

TS:   s.length
来源：http://xw.yuntaijiaju.cn

Java: s.length()
来源：http://ud.panjiajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zq.huixinmuqiang.cn

Ruby: s.length
来源：http://bq.gzmigu.cn

C#:   s.Length
来源：http://ic.shxzskj.cn

[A23] 大小写转换
来源：http://dq.huanxung.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://pi.521024.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bb.521024.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://we.521024.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xu.bjjhwx.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mx.szxytkj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kw.szsharing.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yf.szsharing.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://nl.wgjwhj.cn

[A24] 去除首尾空白
来源：http://nk.bjjhwx.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rw.gzmigu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vn.shtwfgs.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://en.shtwfgs.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jc.asd995.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mc.jctech888.com.cn

Go:   strings.TrimSpace(s)
来源：http://yu.gzmigu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fu.shxzukj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sx.shxzskj.cn

[A25] 字符串比较
来源：http://me.shxzukj.cn

Py:   s1 == s2; s1 != s2
来源：http://yp.521024.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ia.huanxung.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pm.yuntaijiaju.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ou.yuexingan06.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lt.bookmarksfly.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yy.bjjhwx.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ws.muxihuayi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jm.gzmigu.cn

[A26] 类型转换总览
来源：http://dc.jianghongdianzi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ww.hnjuh.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xt.huanxung.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://si.9csxet.cn

TS:   Number() String() Boolean() x as number
来源：http://dg.yuexingan06.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qj.nszjky.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tp.yuntaijiaju.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ix.colortex.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tv.hnjuh.cn

================================================================================
来源：http://de.9csxet.cn

B. 流程控制
来源：http://qt.jianghongdianzi.cn

================================================================================
来源：http://rv.nicolike.cn

[B01] 条件判断 if / else
来源：http://py.szsharing.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://gh.nszjky.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tp.colortex.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tp.nszjky.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dv.jctech888.com.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://no.nicolike.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://up.chemitech.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bm.nicolike.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vs.newstarts.cn

[B02] 多分支 else if / elif
来源：http://mr.muxihuayi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bu.521024.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fr.9csxet.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ub.yuntaijiaju.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hm.bookmarksfly.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nv.szxytkj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fk.haigaiapp.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://sw.gzmigu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eq.wgjwhj.cn

[B03] switch / match / case
来源：http://eb.gzmigu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vz.haigaiapp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qg.shxzskj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ew.szxytkj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kg.szxytkj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tu.newstarts.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nb.huixiangedu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ws.szxytkj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fs.szxytkj.cn

[B04] for 计数循环
来源：http://qx.wgjwhj.cn

Py:   for i in range(10): print(i)
来源：http://ao.jctech888.com.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://du.shtwfgs.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wm.huixiangedu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ix.shtwfgs.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hq.muxihuayi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://st.hahajie.cn

Ruby: 10.times { |i| puts i }
来源：http://xd.asd995.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qz.lnxyls.cn

[B05] 遍历数组 / 列表
来源：http://xl.szxytkj.cn

Py:   for item in arr: print(item)
来源：http://ht.szxytkj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wq.newstarts.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://aj.asd995.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://as.muxihuayi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yf.panjiajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ft.szsharing.cn

Ruby: arr.each { |item| puts item }
来源：http://rv.gzmigu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ae.bookmarksfly.cn

[B06] 遍历字典 / 对象
来源：http://vx.nicolike.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://wa.colortex.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uv.nicolike.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ko.huixiangedu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hr.gzmigu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pu.chemitech.net.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://oc.hahajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hm.shtwfgs.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cz.muxihuayi.cn

[B07] while 循环
来源：http://rs.szsharing.cn

Py:   while i < 10: i += 1
来源：http://eo.colortex.cn

PHP:  while ($i < 10) { $i++; }
来源：http://nr.yuntaijiaju.cn

JS:   while (i < 10) { i++; }
来源：http://ri.newstarts.cn

TS:   while (i < 10) { i++; }
来源：http://tg.huanxung.cn

Java: while (i < 10) { i++; }
来源：http://nx.jianghongdianzi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dp.yuexingan06.cn

Ruby: while i < 10; i += 1; end
来源：http://kb.wgjwhj.cn

C#:   while (i < 10) { i++; }
来源：http://ax.asd995.cn

[B08] do-while（至少执行一次）
来源：http://zh.szxytkj.cn

Py:   # 无 do-while：用 while True + break
来源：http://fg.shxzskj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://dm.huixinmuqiang.cn

JS:   do { i++; } while (i < 10);
来源：http://vz.hnjuh.cn

TS:   do { i++; } while (i < 10);
来源：http://fg.huanxung.cn

Java: do { i++; } while (i < 10);
来源：http://uw.szsharing.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ep.nicolike.cn

Ruby: begin; i += 1; end while i < 10
来源：http://nu.jctech888.com.cn

C#:   do { i++; } while (i < 10);
来源：http://qh.yuntaijiaju.cn

[B09] break 与 continue
来源：http://rb.panjiajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://iy.haigaiapp.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hs.jctech888.com.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bj.jctech888.com.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ar.yuntaijiaju.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vw.szxytkj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zv.shtwfgs.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nb.szxytkj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xw.newstarts.cn

[B10] 遍历同时拿索引
来源：http://nz.newstarts.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://uy.haigaiapp.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zj.shxzskj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ll.yuexingan06.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nb.huixiangedu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yu.hnjuh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xq.521024.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nt.szxytkj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yo.nicolike.cn

[B11] 生成数字序列 / 区间
来源：http://jg.bookmarksfly.cn

Py:   list(range(0, 10, 2))
来源：http://ts.nicolike.cn

PHP:  range(0, 10, 2);
来源：http://gg.jianghongdianzi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mj.huixinmuqiang.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ue.panjiajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sk.shtwfgs.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://of.wgjwhj.cn

Ruby: (0...10).step(2).to_a
来源：http://iw.haigaiapp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pw.yuexingan06.cn

[B12] 跳出多层循环
来源：http://rk.szsharing.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ml.wgjwhj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vs.521024.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ra.haigaiapp.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pf.jianghongdianzi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sn.hnjuh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gu.asd995.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://aw.yuexingan06.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bp.haigaiapp.cn

[B13] 判断是否为数字
来源：http://yw.chemitech.net.cn

Py:   isinstance(x, (int, float))
来源：http://tb.haigaiapp.cn

PHP:  is_numeric($x)
来源：http://ni.asd995.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qf.jianghongdianzi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://po.chemitech.net.cn

Java: x instanceof Number
来源：http://zb.shtwfgs.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bi.chemitech.net.cn

Ruby: x.is_a?(Numeric)
来源：http://zs.shtwfgs.cn

C#:   x is int or double or decimal
来源：http://rb.wgjwhj.cn

[B14] 判断值是否在集合内
来源：http://ir.nicolike.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jl.nicolike.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bw.9csxet.cn

JS:   [1, 2, 3].includes(x)
来源：http://hx.szxytkj.cn

TS:   [1, 2, 3].includes(x)
来源：http://ae.haigaiapp.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://jj.521024.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://oi.newstarts.cn

Ruby: [1, 2, 3].include?(x)
来源：http://aq.huixinmuqiang.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zr.hahajie.cn

[B15] 布尔运算与取反
来源：http://tj.nicolike.cn

Py:   a and b or not c
来源：http://zw.jctech888.com.cn

PHP:  $a && $b || !$c
来源：http://fc.yuntaijiaju.cn

JS:   a && b || !c
来源：http://mx.nicolike.cn

TS:   a && b || !c
来源：http://jy.nszjky.cn

Java: a && b || !c
来源：http://us.jctech888.com.cn

Go:   a && b || !c
来源：http://jl.jctech888.com.cn

Ruby: a && b || !c
来源：http://on.chemitech.net.cn

C#:   a && b || !c
来源：http://jk.szsharing.cn

[B16] 卫语句：不满足条件提前返回
来源：http://rs.shtwfgs.cn

Py:   if not data: return
来源：http://ee.colortex.cn

PHP:  if (!$data) { return; }
来源：http://ue.lnxyls.cn

JS:   if (!data) return;
来源：http://fc.gzmigu.cn

TS:   if (!data) return;
来源：http://ql.muxihuayi.cn

Java: if (data == null) return;
来源：http://ss.asd995.cn

Go:   if data == nil { return }
来源：http://tz.lnxyls.cn

Ruby: return if data.nil?
来源：http://hv.gzmigu.cn

C#:   if (data == null) return;
来源：http://hu.muxihuayi.cn

================================================================================
来源：http://od.hahajie.cn

C. 函数与作用域
来源：http://ap.shxzukj.cn

================================================================================
来源：http://oi.yuexingan06.cn

[C01] 定义函数
来源：http://cg.colortex.cn

Py:   def add(a, b): return a + b
来源：http://hq.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qh.jctech888.com.cn

JS:   function add(a, b) { return a + b; }
来源：http://xg.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fp.chemitech.net.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bj.9csxet.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rl.colortex.cn

Ruby: def add(a, b); a + b; end
来源：http://xr.muxihuayi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sg.yuexingan06.cn

[C02] 默认参数
来源：http://oa.yuexingan06.cn

Py:   def greet(name="World"): return name
来源：http://kk.szxytkj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ic.bjjhwx.cn

JS:   function greet(name = "World") { return name; }
来源：http://cy.asd995.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bn.yuntaijiaju.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://nl.jianghongdianzi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cj.bjjhwx.cn

Ruby: def greet(name = "World") = name
来源：http://ra.9csxet.cn

C#:   string Greet(string name = "World") => name;
来源：http://yt.wgjwhj.cn

[C03] 可变参数
来源：http://qi.colortex.cn

Py:   def total(*args): return sum(args)
来源：http://fw.huixinmuqiang.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xp.haigaiapp.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vl.lnxyls.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ev.colortex.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cj.lnxyls.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mu.muxihuayi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zg.yuntaijiaju.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xv.nicolike.cn

[C04] 命名参数 / 关键字参数
来源：http://gc.jianghongdianzi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ix.asd995.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ux.huixiangedu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://am.yuntaijiaju.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hg.bookmarksfly.cn

Java: // 无：用 Builder 模式或 record
来源：http://xp.colortex.cn

Go:   // 无：用配置结构体参数
来源：http://sm.gzmigu.cn

Ruby: f(a: 1, b: 2)
来源：http://gf.asd995.cn

C#:   f(a: 1, b: 2)
来源：http://bo.panjiajie.cn

[C05] 返回多个值
来源：http://wi.huixiangedu.cn

Py:   return a, b
来源：http://vx.huixinmuqiang.cn

PHP:  return [$a, $b];
来源：http://ic.huixinmuqiang.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://eq.521024.cn

TS:   return { a, b };
来源：http://fd.lnxyls.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://eu.szsharing.cn

Go:   return a, b
来源：http://fu.gzmigu.cn

Ruby: return a, b
来源：http://du.szxytkj.cn

C#:   return (a, b);              // ValueTuple
来源：http://in.shtwfgs.cn

[C06] 匿名函数 / lambda
来源：http://am.chemitech.net.cn

Py:   square = lambda x: x * x
来源：http://is.jianghongdianzi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://jr.jctech888.com.cn

JS:   const square = x => x * x;
来源：http://go.colortex.cn

TS:   const square = (x: number): number => x * x;
来源：http://dr.bjjhwx.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qi.nszjky.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fb.panjiajie.cn

Ruby: square = ->(x) { x * x }
来源：http://kb.bookmarksfly.cn

C#:   Func<int, int> square = x => x * x;
来源：http://vg.huixinmuqiang.cn

[C07] 把函数作为参数传入
来源：http://gj.haigaiapp.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zp.colortex.cn

PHP:  array_map("strtoupper", $arr);
来源：http://no.huixinmuqiang.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gi.hnjuh.cn

TS:   arr.map(String)
来源：http://fk.9csxet.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zn.szxytkj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nr.nszjky.cn

Ruby: arr.map(&:upcase)
来源：http://da.asd995.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xq.yuexingan06.cn

[C08] 闭包
来源：http://is.bjjhwx.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tv.nszjky.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xb.yuexingan06.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zc.huixiangedu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jr.shxzskj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ks.bjjhwx.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sb.shxzskj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uf.9csxet.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://te.gzmigu.cn

[C09] 递归
来源：http://ul.panjiajie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nv.jctech888.com.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mn.yuntaijiaju.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cb.yuntaijiaju.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uh.521024.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hw.yuntaijiaju.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pf.muxihuayi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wu.bookmarksfly.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fr.panjiajie.cn

[C10] 变量作用域
来源：http://eb.colortex.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mg.jianghongdianzi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ii.hahajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bn.nszjky.cn

TS:   同 JS
来源：http://gz.huanxung.cn

Java: 方法内为块级作用域
来源：http://ll.huixiangedu.cn

Go:   花括号块级作用域
来源：http://kp.colortex.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ox.yuexingan06.cn

C#:   块级作用域
来源：http://dy.bookmarksfly.cn

[C11] 模块导入与导出
来源：http://ui.newstarts.cn

Py:   from module import func
来源：http://gw.nicolike.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://gr.asd995.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jg.nicolike.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wl.jctech888.com.cn

Java: import java.util.List;
来源：http://rg.haigaiapp.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bb.chemitech.net.cn

Ruby: require "json"; require_relative "./util"
来源：http://ph.bjjhwx.cn

C#:   using System.Text;
来源：http://kb.haigaiapp.cn

[C12] 立即执行函数 IIFE
来源：http://fp.hnjuh.cn

Py:   (lambda: print("run"))()
来源：http://jj.lnxyls.cn

PHP:  (function () { echo "run"; })();
来源：http://lp.asd995.cn

JS:   (() => { console.log("run"); })();
来源：http://cn.huixinmuqiang.cn

TS:   (() => { console.log("run"); })();
来源：http://ke.szsharing.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pm.szxytkj.cn

Go:   func() { fmt.Println("run") }()
来源：http://sk.hahajie.cn

Ruby: -> { puts "run" }.call
来源：http://hf.jctech888.com.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://cs.bjjhwx.cn

[C13] 类型声明 / 类型注解
来源：http://ir.hahajie.cn


<!-- 参考信息 -->