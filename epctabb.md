代发 wailian999

TS:   s.length
来源：http://jb.nszjky.cn

Java: s.length()
来源：http://zg.huanxung.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://il.lnxyls.cn

Ruby: s.length
来源：http://pt.bjjhwx.cn

C#:   s.Length
来源：http://hv.shxzukj.cn

[A23] 大小写转换
来源：http://zt.521024.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://fo.huixiangedu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vv.chemitech.net.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://eh.hahajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://me.hnjuh.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qy.lnxyls.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pl.panjiajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ni.panjiajie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qq.bjjhwx.cn

[A24] 去除首尾空白
来源：http://lt.shxzskj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hs.jianghongdianzi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ud.asd995.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jb.huixiangedu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://by.bjjhwx.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wg.szsharing.cn

Go:   strings.TrimSpace(s)
来源：http://ix.gzmigu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hj.yuexingan06.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xa.jctech888.com.cn

[A25] 字符串比较
来源：http://vb.shxzukj.cn

Py:   s1 == s2; s1 != s2
来源：http://gl.hnjuh.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kg.hnjuh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://oh.jianghongdianzi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nv.hnjuh.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://eq.colortex.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vv.asd995.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://jh.hahajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pf.yuntaijiaju.cn

[A26] 类型转换总览
来源：http://gb.bjjhwx.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hg.yuntaijiaju.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kq.asd995.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qs.shxzskj.cn

TS:   Number() String() Boolean() x as number
来源：http://yv.shxzukj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://be.gzmigu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hp.hnjuh.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://kb.shxzukj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://sc.shxzukj.cn

================================================================================
来源：http://tp.shtwfgs.cn

B. 流程控制
来源：http://po.shtwfgs.cn

================================================================================
来源：http://dt.yuexingan06.cn

[B01] 条件判断 if / else
来源：http://dg.newstarts.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://jd.wgjwhj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nc.9csxet.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gn.szsharing.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pf.szsharing.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://an.asd995.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ue.bjjhwx.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zm.jctech888.com.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kc.asd995.cn

[B02] 多分支 else if / elif
来源：http://ut.9csxet.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://po.shtwfgs.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gm.521024.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ra.newstarts.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ey.yuexingan06.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dq.hnjuh.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qa.nszjky.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vu.521024.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ms.wgjwhj.cn

[B03] switch / match / case
来源：http://nh.szsharing.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ky.shxzskj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dm.yuntaijiaju.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gh.bookmarksfly.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qk.szsharing.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zk.521024.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uy.lnxyls.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dy.yuexingan06.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sp.gzmigu.cn

[B04] for 计数循环
来源：http://bx.yuntaijiaju.cn

Py:   for i in range(10): print(i)
来源：http://ss.panjiajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://iy.shtwfgs.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ku.lnxyls.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rz.shxzskj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xw.szsharing.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mp.lnxyls.cn

Ruby: 10.times { |i| puts i }
来源：http://mk.asd995.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wc.muxihuayi.cn

[B05] 遍历数组 / 列表
来源：http://kn.bookmarksfly.cn

Py:   for item in arr: print(item)
来源：http://wl.9csxet.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xi.bookmarksfly.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gh.nicolike.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yy.yuntaijiaju.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lx.szsharing.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ul.yuntaijiaju.cn

Ruby: arr.each { |item| puts item }
来源：http://qt.muxihuayi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wc.gzmigu.cn

[B06] 遍历字典 / 对象
来源：http://os.shtwfgs.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ad.bookmarksfly.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jc.bookmarksfly.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mx.newstarts.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ty.huanxung.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://da.yuexingan06.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qh.yuexingan06.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gc.hnjuh.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yo.wgjwhj.cn

[B07] while 循环
来源：http://io.colortex.cn

Py:   while i < 10: i += 1
来源：http://sa.nicolike.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gc.nicolike.cn

JS:   while (i < 10) { i++; }
来源：http://gl.panjiajie.cn

TS:   while (i < 10) { i++; }
来源：http://ey.szxytkj.cn

Java: while (i < 10) { i++; }
来源：http://yi.shxzukj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rd.hnjuh.cn

Ruby: while i < 10; i += 1; end
来源：http://pi.huixiangedu.cn

C#:   while (i < 10) { i++; }
来源：http://kx.shxzukj.cn

[B08] do-while（至少执行一次）
来源：http://ev.bjjhwx.cn

Py:   # 无 do-while：用 while True + break
来源：http://de.521024.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jp.shxzskj.cn

JS:   do { i++; } while (i < 10);
来源：http://bx.hnjuh.cn

TS:   do { i++; } while (i < 10);
来源：http://ky.shtwfgs.cn

Java: do { i++; } while (i < 10);
来源：http://uq.yuexingan06.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fy.nicolike.cn

Ruby: begin; i += 1; end while i < 10
来源：http://du.jctech888.com.cn

C#:   do { i++; } while (i < 10);
来源：http://sx.panjiajie.cn

[B09] break 与 continue
来源：http://xl.huixiangedu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nd.shxzukj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://al.bookmarksfly.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zp.shtwfgs.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pq.shtwfgs.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mm.colortex.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rf.asd995.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xz.huixinmuqiang.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zx.gzmigu.cn

[B10] 遍历同时拿索引
来源：http://kd.newstarts.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jn.shxzskj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ss.hahajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hw.szsharing.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nx.shxzskj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jd.szsharing.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://eq.yuntaijiaju.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://eq.yuntaijiaju.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fq.yuntaijiaju.cn

[B11] 生成数字序列 / 区间
来源：http://ar.huanxung.cn

Py:   list(range(0, 10, 2))
来源：http://xi.nszjky.cn

PHP:  range(0, 10, 2);
来源：http://dl.jianghongdianzi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rn.shxzukj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gv.yuexingan06.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vs.lnxyls.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yz.wgjwhj.cn

Ruby: (0...10).step(2).to_a
来源：http://fa.shxzukj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://si.521024.cn

[B12] 跳出多层循环
来源：http://ip.colortex.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ay.hnjuh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://uh.lnxyls.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qt.nszjky.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ik.shxzukj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pp.9csxet.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://an.9csxet.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ew.huixiangedu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://li.newstarts.cn

[B13] 判断是否为数字
来源：http://sz.521024.cn

Py:   isinstance(x, (int, float))
来源：http://jg.szxytkj.cn

PHP:  is_numeric($x)
来源：http://vn.jctech888.com.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iu.newstarts.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bx.colortex.cn

Java: x instanceof Number
来源：http://or.gzmigu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lt.yuntaijiaju.cn

Ruby: x.is_a?(Numeric)
来源：http://ag.hahajie.cn

C#:   x is int or double or decimal
来源：http://qu.yuexingan06.cn

[B14] 判断值是否在集合内
来源：http://os.jianghongdianzi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://it.muxihuayi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mz.nszjky.cn

JS:   [1, 2, 3].includes(x)
来源：http://vg.newstarts.cn

TS:   [1, 2, 3].includes(x)
来源：http://yc.hnjuh.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hn.asd995.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://aa.muxihuayi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://de.9csxet.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zl.jianghongdianzi.cn

[B15] 布尔运算与取反
来源：http://as.jctech888.com.cn

Py:   a and b or not c
来源：http://af.panjiajie.cn

PHP:  $a && $b || !$c
来源：http://si.szsharing.cn

JS:   a && b || !c
来源：http://ds.haigaiapp.cn

TS:   a && b || !c
来源：http://jp.huixinmuqiang.cn

Java: a && b || !c
来源：http://ie.shtwfgs.cn

Go:   a && b || !c
来源：http://ym.9csxet.cn

Ruby: a && b || !c
来源：http://al.yuexingan06.cn

C#:   a && b || !c
来源：http://ac.jctech888.com.cn

[B16] 卫语句：不满足条件提前返回
来源：http://pc.lnxyls.cn

Py:   if not data: return
来源：http://wv.newstarts.cn

PHP:  if (!$data) { return; }
来源：http://vx.hahajie.cn

JS:   if (!data) return;
来源：http://id.nszjky.cn

TS:   if (!data) return;
来源：http://ao.huixiangedu.cn

Java: if (data == null) return;
来源：http://xg.bjjhwx.cn

Go:   if data == nil { return }
来源：http://ib.newstarts.cn

Ruby: return if data.nil?
来源：http://xh.yuexingan06.cn

C#:   if (data == null) return;
来源：http://in.colortex.cn

================================================================================
来源：http://ns.jctech888.com.cn

C. 函数与作用域
来源：http://sq.muxihuayi.cn

================================================================================
来源：http://cr.jctech888.com.cn

[C01] 定义函数
来源：http://qn.jianghongdianzi.cn

Py:   def add(a, b): return a + b
来源：http://zs.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ek.9csxet.cn

JS:   function add(a, b) { return a + b; }
来源：http://xt.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oy.9csxet.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hy.wgjwhj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jp.nicolike.cn

Ruby: def add(a, b); a + b; end
来源：http://ba.chemitech.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://go.nszjky.cn

[C02] 默认参数
来源：http://zx.nicolike.cn

Py:   def greet(name="World"): return name
来源：http://co.bjjhwx.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bv.szxytkj.cn

JS:   function greet(name = "World") { return name; }
来源：http://iv.colortex.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://tw.9csxet.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rw.jianghongdianzi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nq.hahajie.cn

Ruby: def greet(name = "World") = name
来源：http://na.shxzskj.cn

C#:   string Greet(string name = "World") => name;
来源：http://gn.muxihuayi.cn

[C03] 可变参数
来源：http://uv.hahajie.cn

Py:   def total(*args): return sum(args)
来源：http://po.yuexingan06.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uq.chemitech.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://em.bjjhwx.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ak.huixinmuqiang.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://or.521024.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://df.huixinmuqiang.cn

Ruby: def total(*nums); nums.sum; end
来源：http://sk.shxzukj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://uc.hnjuh.cn

[C04] 命名参数 / 关键字参数
来源：http://oq.muxihuayi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ji.lnxyls.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://js.shtwfgs.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bb.shxzskj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rw.szsharing.cn

Java: // 无：用 Builder 模式或 record
来源：http://dv.gzmigu.cn

Go:   // 无：用配置结构体参数
来源：http://oz.yuntaijiaju.cn

Ruby: f(a: 1, b: 2)
来源：http://xr.yuntaijiaju.cn

C#:   f(a: 1, b: 2)
来源：http://ka.shtwfgs.cn

[C05] 返回多个值
来源：http://ab.shxzskj.cn

Py:   return a, b
来源：http://fb.shxzukj.cn

PHP:  return [$a, $b];
来源：http://xb.huanxung.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://iw.huixinmuqiang.cn

TS:   return { a, b };
来源：http://wz.shxzukj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ij.wgjwhj.cn

Go:   return a, b
来源：http://dd.shxzukj.cn

Ruby: return a, b
来源：http://fy.shtwfgs.cn

C#:   return (a, b);              // ValueTuple
来源：http://pa.newstarts.cn

[C06] 匿名函数 / lambda
来源：http://rv.jctech888.com.cn

Py:   square = lambda x: x * x
来源：http://dm.yuexingan06.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://kt.jianghongdianzi.cn

JS:   const square = x => x * x;
来源：http://tf.chemitech.net.cn

TS:   const square = (x: number): number => x * x;
来源：http://jj.wgjwhj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ij.hnjuh.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wh.jctech888.com.cn

Ruby: square = ->(x) { x * x }
来源：http://ky.wgjwhj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://iz.jctech888.com.cn

[C07] 把函数作为参数传入
来源：http://xo.nszjky.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ln.jctech888.com.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vs.521024.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zu.newstarts.cn

TS:   arr.map(String)
来源：http://xb.nszjky.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://aw.huixiangedu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rr.bjjhwx.cn

Ruby: arr.map(&:upcase)
来源：http://uv.shxzskj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hp.nicolike.cn

[C08] 闭包
来源：http://in.huixinmuqiang.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nr.panjiajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rn.szxytkj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sp.jianghongdianzi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fi.yuexingan06.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xa.huixinmuqiang.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://he.asd995.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uk.521024.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://be.521024.cn

[C09] 递归
来源：http://ws.wgjwhj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qq.hahajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tv.colortex.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://th.muxihuayi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ic.yuexingan06.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rl.haigaiapp.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://iu.panjiajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jo.jianghongdianzi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cq.jctech888.com.cn

[C10] 变量作用域
来源：http://dh.yuntaijiaju.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vq.muxihuayi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qn.shtwfgs.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lb.jianghongdianzi.cn

TS:   同 JS
来源：http://xa.huixiangedu.cn

Java: 方法内为块级作用域
来源：http://zj.newstarts.cn

Go:   花括号块级作用域
来源：http://eu.szxytkj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wc.shxzukj.cn

C#:   块级作用域
来源：http://ey.hahajie.cn

[C11] 模块导入与导出
来源：http://bv.newstarts.cn

Py:   from module import func
来源：http://cp.shxzskj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wl.panjiajie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://di.huixiangedu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uc.521024.cn

Java: import java.util.List;
来源：http://tj.yuexingan06.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fa.jctech888.com.cn

Ruby: require "json"; require_relative "./util"
来源：http://ln.szsharing.cn

C#:   using System.Text;
来源：http://is.szxytkj.cn

[C12] 立即执行函数 IIFE
来源：http://ii.wgjwhj.cn

Py:   (lambda: print("run"))()
来源：http://ma.bjjhwx.cn

PHP:  (function () { echo "run"; })();
来源：http://id.shxzukj.cn

JS:   (() => { console.log("run"); })();
来源：http://dp.haigaiapp.cn

TS:   (() => { console.log("run"); })();
来源：http://wj.szxytkj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ji.szxytkj.cn

Go:   func() { fmt.Println("run") }()
来源：http://zu.muxihuayi.cn

Ruby: -> { puts "run" }.call
来源：http://pk.nszjky.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fl.wgjwhj.cn

[C13] 类型声明 / 类型注解
来源：http://kj.nicolike.cn


<!-- 参考信息 -->