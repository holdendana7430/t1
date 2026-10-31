代发 wailian999

C#:   s.Length
来源：http://sa.panjiajie.cn

[A23] 大小写转换
来源：http://fj.hnjuh.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://hq.nicolike.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pl.huixinmuqiang.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ch.521024.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://pw.shxzukj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dj.yuntaijiaju.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bp.haigaiapp.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://sy.huixiangedu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ei.huixinmuqiang.cn

[A24] 去除首尾空白
来源：http://tk.shtwfgs.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gc.nicolike.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ha.shxzukj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gh.huixiangedu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rq.newstarts.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://oy.yuntaijiaju.cn

Go:   strings.TrimSpace(s)
来源：http://nk.hahajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ii.nszjky.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ba.bookmarksfly.cn

[A25] 字符串比较
来源：http://zo.muxihuayi.cn

Py:   s1 == s2; s1 != s2
来源：http://xp.szsharing.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bb.nicolike.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vq.huanxung.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kj.panjiajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ix.hnjuh.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fm.yuexingan06.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ce.chemitech.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ed.shtwfgs.cn

[A26] 类型转换总览
来源：http://ym.szxytkj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vd.chemitech.net.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qc.bjjhwx.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mt.newstarts.cn

TS:   Number() String() Boolean() x as number
来源：http://hl.jianghongdianzi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qp.wgjwhj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hy.szxytkj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zj.huanxung.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tn.chemitech.net.cn

================================================================================
来源：http://ml.hnjuh.cn

B. 流程控制
来源：http://rs.yuexingan06.cn

================================================================================
来源：http://bb.jianghongdianzi.cn

[B01] 条件判断 if / else
来源：http://hm.newstarts.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://pp.shxzukj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wp.szxytkj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zg.asd995.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.shtwfgs.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://sq.szxytkj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hk.9csxet.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qp.huixinmuqiang.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cu.newstarts.cn

[B02] 多分支 else if / elif
来源：http://nz.huanxung.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rq.huanxung.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://iv.gzmigu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nz.panjiajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dh.huixinmuqiang.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mm.nszjky.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dm.huixiangedu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://sv.huanxung.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cy.shxzukj.cn

[B03] switch / match / case
来源：http://lz.huixinmuqiang.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ac.huixinmuqiang.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pe.bjjhwx.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nu.lnxyls.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hf.shxzukj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dx.gzmigu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yt.bjjhwx.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uk.colortex.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kr.shxzukj.cn

[B04] for 计数循环
来源：http://sk.szsharing.cn

Py:   for i in range(10): print(i)
来源：http://yp.asd995.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cs.newstarts.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zr.huixinmuqiang.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ia.asd995.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pc.wgjwhj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nt.huixinmuqiang.cn

Ruby: 10.times { |i| puts i }
来源：http://vn.hnjuh.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ad.huixiangedu.cn

[B05] 遍历数组 / 列表
来源：http://jn.nicolike.cn

Py:   for item in arr: print(item)
来源：http://yj.panjiajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jq.hahajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://lu.yuntaijiaju.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://iz.hahajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://bz.shxzukj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ug.hahajie.cn

Ruby: arr.each { |item| puts item }
来源：http://sq.haigaiapp.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ck.nicolike.cn

[B06] 遍历字典 / 对象
来源：http://va.huixiangedu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://yw.szxytkj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://na.colortex.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dn.yuexingan06.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bn.jianghongdianzi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uq.shxzukj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pf.colortex.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lf.shxzukj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wc.szxytkj.cn

[B07] while 循环
来源：http://gr.yuexingan06.cn

Py:   while i < 10: i += 1
来源：http://hk.asd995.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qo.huixinmuqiang.cn

JS:   while (i < 10) { i++; }
来源：http://nj.bjjhwx.cn

TS:   while (i < 10) { i++; }
来源：http://ie.haigaiapp.cn

Java: while (i < 10) { i++; }
来源：http://mc.chemitech.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qo.colortex.cn

Ruby: while i < 10; i += 1; end
来源：http://yp.bjjhwx.cn

C#:   while (i < 10) { i++; }
来源：http://qe.huixiangedu.cn

[B08] do-while（至少执行一次）
来源：http://ur.lnxyls.cn

Py:   # 无 do-while：用 while True + break
来源：http://un.521024.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://hs.shtwfgs.cn

JS:   do { i++; } while (i < 10);
来源：http://kw.newstarts.cn

TS:   do { i++; } while (i < 10);
来源：http://sz.asd995.cn

Java: do { i++; } while (i < 10);
来源：http://an.521024.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://pc.hnjuh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pv.hahajie.cn

C#:   do { i++; } while (i < 10);
来源：http://hi.bookmarksfly.cn

[B09] break 与 continue
来源：http://pb.shxzukj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://aj.521024.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kd.jianghongdianzi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://da.huixinmuqiang.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ey.huixinmuqiang.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yg.lnxyls.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rv.huixiangedu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://te.huanxung.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yc.bjjhwx.cn

[B10] 遍历同时拿索引
来源：http://xh.asd995.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://op.chemitech.net.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jn.colortex.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kt.wgjwhj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://we.asd995.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gn.szxytkj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wl.yuexingan06.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qq.asd995.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://uy.bookmarksfly.cn

[B11] 生成数字序列 / 区间
来源：http://mi.jctech888.com.cn

Py:   list(range(0, 10, 2))
来源：http://mw.jctech888.com.cn

PHP:  range(0, 10, 2);
来源：http://gc.shxzskj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hy.panjiajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ek.shxzskj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hb.bjjhwx.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pp.nicolike.cn

Ruby: (0...10).step(2).to_a
来源：http://vv.shxzskj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lj.lnxyls.cn

[B12] 跳出多层循环
来源：http://os.muxihuayi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://lv.bjjhwx.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://nb.gzmigu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zl.shtwfgs.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nr.panjiajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lj.huanxung.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yk.jianghongdianzi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yw.asd995.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ha.haigaiapp.cn

[B13] 判断是否为数字
来源：http://kh.haigaiapp.cn

Py:   isinstance(x, (int, float))
来源：http://bh.yuntaijiaju.cn

PHP:  is_numeric($x)
来源：http://wo.huanxung.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gr.szsharing.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oq.asd995.cn

Java: x instanceof Number
来源：http://ai.hnjuh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tv.muxihuayi.cn

Ruby: x.is_a?(Numeric)
来源：http://op.yuexingan06.cn

C#:   x is int or double or decimal
来源：http://be.muxihuayi.cn

[B14] 判断值是否在集合内
来源：http://rw.asd995.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mw.asd995.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cr.yuntaijiaju.cn

JS:   [1, 2, 3].includes(x)
来源：http://kh.9csxet.cn

TS:   [1, 2, 3].includes(x)
来源：http://hv.asd995.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dh.gzmigu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://td.521024.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vy.hahajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://du.yuntaijiaju.cn

[B15] 布尔运算与取反
来源：http://gr.chemitech.net.cn

Py:   a and b or not c
来源：http://rx.jctech888.com.cn

PHP:  $a && $b || !$c
来源：http://wr.9csxet.cn

JS:   a && b || !c
来源：http://ck.shxzskj.cn

TS:   a && b || !c
来源：http://bs.panjiajie.cn

Java: a && b || !c
来源：http://vj.hnjuh.cn

Go:   a && b || !c
来源：http://qe.shxzukj.cn

Ruby: a && b || !c
来源：http://sl.colortex.cn

C#:   a && b || !c
来源：http://vi.bjjhwx.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gq.shxzskj.cn

Py:   if not data: return
来源：http://qk.haigaiapp.cn

PHP:  if (!$data) { return; }
来源：http://sp.jianghongdianzi.cn

JS:   if (!data) return;
来源：http://rq.shxzskj.cn

TS:   if (!data) return;
来源：http://qs.huanxung.cn

Java: if (data == null) return;
来源：http://ng.9csxet.cn

Go:   if data == nil { return }
来源：http://in.chemitech.net.cn

Ruby: return if data.nil?
来源：http://ct.bookmarksfly.cn

C#:   if (data == null) return;
来源：http://yy.haigaiapp.cn

================================================================================
来源：http://uh.haigaiapp.cn

C. 函数与作用域
来源：http://iq.hahajie.cn

================================================================================
来源：http://tq.hnjuh.cn

[C01] 定义函数
来源：http://tt.gzmigu.cn

Py:   def add(a, b): return a + b
来源：http://ux.shxzskj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wl.gzmigu.cn

JS:   function add(a, b) { return a + b; }
来源：http://wl.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ph.hahajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://jw.bookmarksfly.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vt.gzmigu.cn

Ruby: def add(a, b); a + b; end
来源：http://jz.shxzukj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cu.yuexingan06.cn

[C02] 默认参数
来源：http://zr.huixiangedu.cn

Py:   def greet(name="World"): return name
来源：http://dx.huanxung.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://et.chemitech.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://ub.szxytkj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ty.jianghongdianzi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cm.haigaiapp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mc.hnjuh.cn

Ruby: def greet(name = "World") = name
来源：http://zr.9csxet.cn

C#:   string Greet(string name = "World") => name;
来源：http://up.huixinmuqiang.cn

[C03] 可变参数
来源：http://fy.hahajie.cn

Py:   def total(*args): return sum(args)
来源：http://gp.yuexingan06.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jz.hnjuh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nc.asd995.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ct.shtwfgs.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://li.colortex.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cm.shtwfgs.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hj.wgjwhj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fc.wgjwhj.cn

[C04] 命名参数 / 关键字参数
来源：http://vg.gzmigu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bj.huanxung.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bs.lnxyls.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://eh.szxytkj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xd.bookmarksfly.cn

Java: // 无：用 Builder 模式或 record
来源：http://qc.nszjky.cn

Go:   // 无：用配置结构体参数
来源：http://lr.newstarts.cn

Ruby: f(a: 1, b: 2)
来源：http://gw.wgjwhj.cn

C#:   f(a: 1, b: 2)
来源：http://ul.shtwfgs.cn

[C05] 返回多个值
来源：http://gc.yuntaijiaju.cn

Py:   return a, b
来源：http://xy.shxzukj.cn

PHP:  return [$a, $b];
来源：http://ux.asd995.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yt.9csxet.cn

TS:   return { a, b };
来源：http://ij.huanxung.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://th.gzmigu.cn

Go:   return a, b
来源：http://yo.muxihuayi.cn

Ruby: return a, b
来源：http://vy.muxihuayi.cn

C#:   return (a, b);              // ValueTuple
来源：http://wz.muxihuayi.cn

[C06] 匿名函数 / lambda
来源：http://pp.nszjky.cn

Py:   square = lambda x: x * x
来源：http://rj.chemitech.net.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://cf.asd995.cn

JS:   const square = x => x * x;
来源：http://ft.shtwfgs.cn

TS:   const square = (x: number): number => x * x;
来源：http://aa.chemitech.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://uw.jianghongdianzi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://vh.huixinmuqiang.cn

Ruby: square = ->(x) { x * x }
来源：http://az.shxzskj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://gd.haigaiapp.cn

[C07] 把函数作为参数传入
来源：http://cv.yuexingan06.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wc.jianghongdianzi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://fo.huixinmuqiang.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mv.panjiajie.cn

TS:   arr.map(String)
来源：http://bk.gzmigu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lk.gzmigu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kl.jianghongdianzi.cn

Ruby: arr.map(&:upcase)
来源：http://fe.haigaiapp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://yv.haigaiapp.cn

[C08] 闭包
来源：http://uv.hnjuh.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yg.jctech888.com.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dw.521024.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jt.szsharing.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mz.chemitech.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://va.nszjky.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jl.yuntaijiaju.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qb.shxzskj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://np.9csxet.cn

[C09] 递归
来源：http://qm.lnxyls.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fx.521024.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fs.shxzskj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rr.521024.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kj.muxihuayi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rd.lnxyls.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zr.haigaiapp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sy.wgjwhj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wr.nszjky.cn

[C10] 变量作用域
来源：http://lb.shtwfgs.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sb.nszjky.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zy.bjjhwx.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zz.hahajie.cn

TS:   同 JS
来源：http://pv.huanxung.cn

Java: 方法内为块级作用域
来源：http://jz.szxytkj.cn

Go:   花括号块级作用域
来源：http://hf.lnxyls.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nh.nicolike.cn

C#:   块级作用域
来源：http://km.szsharing.cn

[C11] 模块导入与导出
来源：http://lu.521024.cn

Py:   from module import func
来源：http://fc.jctech888.com.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://uh.nicolike.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zc.haigaiapp.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://my.asd995.cn

Java: import java.util.List;
来源：http://lp.huixiangedu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gh.gzmigu.cn

Ruby: require "json"; require_relative "./util"
来源：http://gr.huixinmuqiang.cn

C#:   using System.Text;
来源：http://wn.shtwfgs.cn

[C12] 立即执行函数 IIFE
来源：http://bl.nicolike.cn

Py:   (lambda: print("run"))()
来源：http://gs.nicolike.cn

PHP:  (function () { echo "run"; })();
来源：http://zr.hnjuh.cn

JS:   (() => { console.log("run"); })();
来源：http://fo.gzmigu.cn

TS:   (() => { console.log("run"); })();
来源：http://wi.521024.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ci.newstarts.cn

Go:   func() { fmt.Println("run") }()
来源：http://fc.haigaiapp.cn

Ruby: -> { puts "run" }.call
来源：http://tb.nicolike.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gq.szxytkj.cn

[C13] 类型声明 / 类型注解
来源：http://tp.yuntaijiaju.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xc.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gq.newstarts.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://as.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vs.szsharing.cn


<!-- 参考信息 -->