代发 wailian999

TS:   s.length
来源：http://ln.szsharing.cn

Java: s.length()
来源：http://ee.bookmarksfly.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://je.wgjwhj.cn

Ruby: s.length
来源：http://tu.huixinmuqiang.cn

C#:   s.Length
来源：http://hi.szxytkj.cn

[A23] 大小写转换
来源：http://dy.chemitech.net.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://mp.9csxet.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dp.muxihuayi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ne.9csxet.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vw.newstarts.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pk.521024.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ue.huixiangedu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://kx.521024.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://tg.lnxyls.cn

[A24] 去除首尾空白
来源：http://ty.shtwfgs.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tz.szxytkj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dk.lnxyls.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pj.9csxet.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gy.shxzukj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pu.chemitech.net.cn

Go:   strings.TrimSpace(s)
来源：http://yl.newstarts.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bw.huixiangedu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vf.521024.cn

[A25] 字符串比较
来源：http://xi.muxihuayi.cn

Py:   s1 == s2; s1 != s2
来源：http://hn.colortex.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://px.shxzukj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vi.jctech888.com.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://uq.lnxyls.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rg.wgjwhj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://uq.wgjwhj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ba.szxytkj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wo.newstarts.cn

[A26] 类型转换总览
来源：http://ea.shxzukj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ux.huanxung.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://az.521024.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xo.9csxet.cn

TS:   Number() String() Boolean() x as number
来源：http://qg.haigaiapp.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ka.nszjky.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://uy.shxzskj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://cu.jianghongdianzi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qj.yuntaijiaju.cn

================================================================================
来源：http://dc.521024.cn

B. 流程控制
来源：http://rs.chemitech.net.cn

================================================================================
来源：http://wf.hnjuh.cn

[B01] 条件判断 if / else
来源：http://hi.huixinmuqiang.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://rq.jctech888.com.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://uc.bjjhwx.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xw.szsharing.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qv.shxzukj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bn.wgjwhj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gf.yuexingan06.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bs.hahajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://un.shxzskj.cn

[B02] 多分支 else if / elif
来源：http://xa.lnxyls.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ln.panjiajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ee.panjiajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hy.panjiajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://md.nicolike.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bw.yuntaijiaju.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jp.haigaiapp.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://co.huixiangedu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rl.newstarts.cn

[B03] switch / match / case
来源：http://sz.colortex.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://de.newstarts.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yv.huixinmuqiang.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hs.bookmarksfly.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mw.yuntaijiaju.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zg.newstarts.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gd.panjiajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ck.521024.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jv.yuexingan06.cn

[B04] for 计数循环
来源：http://ea.haigaiapp.cn

Py:   for i in range(10): print(i)
来源：http://lj.haigaiapp.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://oj.newstarts.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cg.shxzskj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ls.521024.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cz.huixiangedu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yn.huixiangedu.cn

Ruby: 10.times { |i| puts i }
来源：http://dg.bjjhwx.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rv.chemitech.net.cn

[B05] 遍历数组 / 列表
来源：http://tg.panjiajie.cn

Py:   for item in arr: print(item)
来源：http://qj.chemitech.net.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dn.chemitech.net.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fe.chemitech.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://nk.gzmigu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://mz.colortex.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hy.521024.cn

Ruby: arr.each { |item| puts item }
来源：http://ah.shxzskj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ic.hahajie.cn

[B06] 遍历字典 / 对象
来源：http://am.bookmarksfly.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ua.jctech888.com.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gk.bookmarksfly.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xn.hnjuh.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bw.wgjwhj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mg.nszjky.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gw.szxytkj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xa.9csxet.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jy.yuntaijiaju.cn

[B07] while 循环
来源：http://rg.9csxet.cn

Py:   while i < 10: i += 1
来源：http://yv.bjjhwx.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gv.shxzukj.cn

JS:   while (i < 10) { i++; }
来源：http://do.bookmarksfly.cn

TS:   while (i < 10) { i++; }
来源：http://qd.muxihuayi.cn

Java: while (i < 10) { i++; }
来源：http://qr.huixiangedu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sm.jianghongdianzi.cn

Ruby: while i < 10; i += 1; end
来源：http://ev.wgjwhj.cn

C#:   while (i < 10) { i++; }
来源：http://ls.9csxet.cn

[B08] do-while（至少执行一次）
来源：http://dz.yuntaijiaju.cn

Py:   # 无 do-while：用 while True + break
来源：http://zr.shxzskj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ot.szsharing.cn

JS:   do { i++; } while (i < 10);
来源：http://ts.huixinmuqiang.cn

TS:   do { i++; } while (i < 10);
来源：http://zz.shtwfgs.cn

Java: do { i++; } while (i < 10);
来源：http://ty.haigaiapp.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://yu.bjjhwx.cn

Ruby: begin; i += 1; end while i < 10
来源：http://we.muxihuayi.cn

C#:   do { i++; } while (i < 10);
来源：http://oi.haigaiapp.cn

[B09] break 与 continue
来源：http://ak.bjjhwx.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://el.nicolike.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bv.haigaiapp.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hc.bookmarksfly.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ib.yuexingan06.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ei.shxzukj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hh.9csxet.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bg.wgjwhj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ao.huanxung.cn

[B10] 遍历同时拿索引
来源：http://jj.jctech888.com.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ou.chemitech.net.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ct.lnxyls.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ei.newstarts.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ea.9csxet.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vy.gzmigu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wx.huixiangedu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://at.huixinmuqiang.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://du.521024.cn

[B11] 生成数字序列 / 区间
来源：http://kq.hahajie.cn

Py:   list(range(0, 10, 2))
来源：http://tv.hnjuh.cn

PHP:  range(0, 10, 2);
来源：http://vd.jianghongdianzi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://su.shtwfgs.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://md.panjiajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ih.yuntaijiaju.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zk.shxzukj.cn

Ruby: (0...10).step(2).to_a
来源：http://gg.521024.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://je.shxzukj.cn

[B12] 跳出多层循环
来源：http://fw.shtwfgs.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ma.yuntaijiaju.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://qm.shxzskj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ns.shtwfgs.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jk.jctech888.com.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://se.shtwfgs.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yt.lnxyls.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gc.bookmarksfly.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ln.yuntaijiaju.cn

[B13] 判断是否为数字
来源：http://ct.huixinmuqiang.cn

Py:   isinstance(x, (int, float))
来源：http://qn.521024.cn

PHP:  is_numeric($x)
来源：http://fp.shtwfgs.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hc.asd995.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://up.haigaiapp.cn

Java: x instanceof Number
来源：http://na.bjjhwx.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tt.chemitech.net.cn

Ruby: x.is_a?(Numeric)
来源：http://qw.nszjky.cn

C#:   x is int or double or decimal
来源：http://px.hahajie.cn

[B14] 判断值是否在集合内
来源：http://en.colortex.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jq.9csxet.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ns.szxytkj.cn

JS:   [1, 2, 3].includes(x)
来源：http://sq.521024.cn

TS:   [1, 2, 3].includes(x)
来源：http://qy.yuexingan06.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://lp.yuntaijiaju.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qg.huixinmuqiang.cn

Ruby: [1, 2, 3].include?(x)
来源：http://au.nicolike.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wt.bjjhwx.cn

[B15] 布尔运算与取反
来源：http://dm.wgjwhj.cn

Py:   a and b or not c
来源：http://bm.colortex.cn

PHP:  $a && $b || !$c
来源：http://ds.newstarts.cn

JS:   a && b || !c
来源：http://gt.newstarts.cn

TS:   a && b || !c
来源：http://ct.yuexingan06.cn

Java: a && b || !c
来源：http://rc.nszjky.cn

Go:   a && b || !c
来源：http://kh.chemitech.net.cn

Ruby: a && b || !c
来源：http://fg.wgjwhj.cn

C#:   a && b || !c
来源：http://ss.shxzskj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://py.shxzukj.cn

Py:   if not data: return
来源：http://fh.9csxet.cn

PHP:  if (!$data) { return; }
来源：http://is.muxihuayi.cn

JS:   if (!data) return;
来源：http://rx.haigaiapp.cn

TS:   if (!data) return;
来源：http://ok.9csxet.cn

Java: if (data == null) return;
来源：http://yy.chemitech.net.cn

Go:   if data == nil { return }
来源：http://zp.shxzskj.cn

Ruby: return if data.nil?
来源：http://ro.bjjhwx.cn

C#:   if (data == null) return;
来源：http://yj.shxzskj.cn

================================================================================
来源：http://zq.hnjuh.cn

C. 函数与作用域
来源：http://lx.521024.cn

================================================================================
来源：http://fq.hnjuh.cn

[C01] 定义函数
来源：http://in.jctech888.com.cn

Py:   def add(a, b): return a + b
来源：http://es.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jh.9csxet.cn

JS:   function add(a, b) { return a + b; }
来源：http://xi.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xp.521024.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://kq.wgjwhj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ju.colortex.cn

Ruby: def add(a, b); a + b; end
来源：http://vo.huanxung.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ry.yuntaijiaju.cn

[C02] 默认参数
来源：http://wm.shxzukj.cn

Py:   def greet(name="World"): return name
来源：http://wk.asd995.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lt.nszjky.cn

JS:   function greet(name = "World") { return name; }
来源：http://dx.shtwfgs.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://de.shtwfgs.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://er.szsharing.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://um.yuexingan06.cn

Ruby: def greet(name = "World") = name
来源：http://im.shxzukj.cn

C#:   string Greet(string name = "World") => name;
来源：http://lt.muxihuayi.cn

[C03] 可变参数
来源：http://pm.yuntaijiaju.cn

Py:   def total(*args): return sum(args)
来源：http://uq.chemitech.net.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qi.huanxung.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cb.asd995.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jr.muxihuayi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rk.hahajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ma.muxihuayi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://iy.nicolike.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rb.szsharing.cn

[C04] 命名参数 / 关键字参数
来源：http://kf.yuntaijiaju.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nh.jctech888.com.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rl.bookmarksfly.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nx.9csxet.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qy.bookmarksfly.cn

Java: // 无：用 Builder 模式或 record
来源：http://rg.bookmarksfly.cn

Go:   // 无：用配置结构体参数
来源：http://ql.chemitech.net.cn

Ruby: f(a: 1, b: 2)
来源：http://hd.yuexingan06.cn

C#:   f(a: 1, b: 2)
来源：http://fv.shtwfgs.cn

[C05] 返回多个值
来源：http://ug.hnjuh.cn

Py:   return a, b
来源：http://yq.yuntaijiaju.cn

PHP:  return [$a, $b];
来源：http://ju.hnjuh.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xd.panjiajie.cn

TS:   return { a, b };
来源：http://ks.nszjky.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sk.szsharing.cn

Go:   return a, b
来源：http://iy.nszjky.cn

Ruby: return a, b
来源：http://yv.hahajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://bt.huixinmuqiang.cn

[C06] 匿名函数 / lambda
来源：http://eg.yuntaijiaju.cn

Py:   square = lambda x: x * x
来源：http://no.nicolike.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ed.shxzskj.cn

JS:   const square = x => x * x;
来源：http://rd.huixiangedu.cn

TS:   const square = (x: number): number => x * x;
来源：http://ls.asd995.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tp.hahajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ve.wgjwhj.cn

Ruby: square = ->(x) { x * x }
来源：http://xc.shxzskj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zg.yuexingan06.cn

[C07] 把函数作为参数传入
来源：http://ti.nicolike.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lv.newstarts.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vo.huanxung.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ba.hahajie.cn

TS:   arr.map(String)
来源：http://gi.huixinmuqiang.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bs.chemitech.net.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vq.shtwfgs.cn

Ruby: arr.map(&:upcase)
来源：http://xr.lnxyls.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ci.9csxet.cn

[C08] 闭包
来源：http://xy.shxzskj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rq.shxzukj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://th.9csxet.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ww.nszjky.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qz.yuexingan06.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vr.lnxyls.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nt.haigaiapp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mf.521024.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mb.wgjwhj.cn

[C09] 递归
来源：http://ow.shtwfgs.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ri.nszjky.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fn.huanxung.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qs.shxzskj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wi.haigaiapp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tp.huixiangedu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uv.hnjuh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cc.szxytkj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ku.szxytkj.cn

[C10] 变量作用域
来源：http://sn.521024.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vi.shtwfgs.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ly.muxihuayi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cx.colortex.cn

TS:   同 JS
来源：http://jk.asd995.cn

Java: 方法内为块级作用域
来源：http://ru.hahajie.cn

Go:   花括号块级作用域
来源：http://ky.colortex.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ix.yuexingan06.cn

C#:   块级作用域
来源：http://pg.muxihuayi.cn

[C11] 模块导入与导出
来源：http://tt.shxzskj.cn

Py:   from module import func
来源：http://vx.colortex.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://lw.muxihuayi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://pa.nicolike.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ft.shtwfgs.cn

Java: import java.util.List;
来源：http://jc.szxytkj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ee.bookmarksfly.cn

Ruby: require "json"; require_relative "./util"
来源：http://fe.wgjwhj.cn

C#:   using System.Text;
来源：http://aj.asd995.cn

[C12] 立即执行函数 IIFE
来源：http://lb.haigaiapp.cn

Py:   (lambda: print("run"))()
来源：http://cq.gzmigu.cn

PHP:  (function () { echo "run"; })();
来源：http://ey.newstarts.cn

JS:   (() => { console.log("run"); })();
来源：http://mi.nicolike.cn

TS:   (() => { console.log("run"); })();
来源：http://tp.521024.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://po.shxzskj.cn

Go:   func() { fmt.Println("run") }()
来源：http://nh.jctech888.com.cn

Ruby: -> { puts "run" }.call
来源：http://oo.yuexingan06.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pq.jctech888.com.cn

[C13] 类型声明 / 类型注解
来源：http://ne.newstarts.cn


<!-- 参考信息 -->