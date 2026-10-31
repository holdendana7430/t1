代发 wailian999

C#:   s.Length
来源：http://uq.nszjky.cn

[A23] 大小写转换
来源：http://ng.gzmigu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://dn.nicolike.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://uy.gzmigu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://lt.szsharing.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://sm.wgjwhj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xo.9csxet.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vo.hahajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://op.shtwfgs.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ey.lnxyls.cn

[A24] 去除首尾空白
来源：http://vs.jctech888.com.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://to.szsharing.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kq.yuexingan06.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xz.muxihuayi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wx.wgjwhj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://oy.hahajie.cn

Go:   strings.TrimSpace(s)
来源：http://yd.panjiajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://am.szxytkj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sv.yuntaijiaju.cn

[A25] 字符串比较
来源：http://wq.521024.cn

Py:   s1 == s2; s1 != s2
来源：http://bc.asd995.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jh.jianghongdianzi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ed.huixinmuqiang.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zj.nszjky.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nj.chemitech.net.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mi.newstarts.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vv.9csxet.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://iz.521024.cn

[A26] 类型转换总览
来源：http://rf.wgjwhj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://le.hnjuh.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mh.gzmigu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://up.nszjky.cn

TS:   Number() String() Boolean() x as number
来源：http://ed.jctech888.com.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ez.yuexingan06.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ms.gzmigu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ma.asd995.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fm.gzmigu.cn

================================================================================
来源：http://es.wgjwhj.cn

B. 流程控制
来源：http://wl.shxzukj.cn

================================================================================
来源：http://vr.huixinmuqiang.cn

[B01] 条件判断 if / else
来源：http://ex.nszjky.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://sa.shxzskj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zv.bookmarksfly.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://az.asd995.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rd.wgjwhj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://na.hnjuh.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vk.gzmigu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://uy.jctech888.com.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jx.hnjuh.cn

[B02] 多分支 else if / elif
来源：http://hf.szxytkj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gq.newstarts.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jl.shxzukj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yd.yuexingan06.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kd.lnxyls.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qo.bookmarksfly.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mk.nszjky.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yi.haigaiapp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rb.yuexingan06.cn

[B03] switch / match / case
来源：http://xe.hahajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kw.haigaiapp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ed.nicolike.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bo.gzmigu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fg.panjiajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fs.yuntaijiaju.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pc.bjjhwx.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ne.gzmigu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wa.jianghongdianzi.cn

[B04] for 计数循环
来源：http://nd.shxzskj.cn

Py:   for i in range(10): print(i)
来源：http://pv.asd995.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://po.shxzskj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xe.shxzskj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://my.colortex.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xw.huanxung.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yy.newstarts.cn

Ruby: 10.times { |i| puts i }
来源：http://uo.szxytkj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xt.lnxyls.cn

[B05] 遍历数组 / 列表
来源：http://co.gzmigu.cn

Py:   for item in arr: print(item)
来源：http://ji.jianghongdianzi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rd.jianghongdianzi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ib.bookmarksfly.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xk.bookmarksfly.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wc.huanxung.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fx.huixiangedu.cn

Ruby: arr.each { |item| puts item }
来源：http://rw.huixinmuqiang.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wo.bookmarksfly.cn

[B06] 遍历字典 / 对象
来源：http://kw.bjjhwx.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qk.szxytkj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fd.colortex.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jq.huixiangedu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ac.panjiajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rt.nicolike.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ga.colortex.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zm.szxytkj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://eu.szxytkj.cn

[B07] while 循环
来源：http://rs.huixinmuqiang.cn

Py:   while i < 10: i += 1
来源：http://zm.wgjwhj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://td.bookmarksfly.cn

JS:   while (i < 10) { i++; }
来源：http://tp.chemitech.net.cn

TS:   while (i < 10) { i++; }
来源：http://yg.shxzukj.cn

Java: while (i < 10) { i++; }
来源：http://ym.nicolike.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ps.hahajie.cn

Ruby: while i < 10; i += 1; end
来源：http://ty.hnjuh.cn

C#:   while (i < 10) { i++; }
来源：http://ky.gzmigu.cn

[B08] do-while（至少执行一次）
来源：http://mj.nszjky.cn

Py:   # 无 do-while：用 while True + break
来源：http://ez.yuntaijiaju.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://gm.chemitech.net.cn

JS:   do { i++; } while (i < 10);
来源：http://tb.wgjwhj.cn

TS:   do { i++; } while (i < 10);
来源：http://ur.szsharing.cn

Java: do { i++; } while (i < 10);
来源：http://mv.yuntaijiaju.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sh.wgjwhj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pg.newstarts.cn

C#:   do { i++; } while (i < 10);
来源：http://af.bookmarksfly.cn

[B09] break 与 continue
来源：http://pv.shxzukj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rf.szxytkj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tv.asd995.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jr.lnxyls.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xu.shxzskj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mc.huanxung.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ll.asd995.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bd.hahajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yz.szxytkj.cn

[B10] 遍历同时拿索引
来源：http://lr.colortex.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hq.shxzskj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bn.bookmarksfly.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wm.huixinmuqiang.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mt.huixinmuqiang.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dn.shtwfgs.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hf.szxytkj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ms.nszjky.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://db.shxzukj.cn

[B11] 生成数字序列 / 区间
来源：http://mq.shtwfgs.cn

Py:   list(range(0, 10, 2))
来源：http://az.nicolike.cn

PHP:  range(0, 10, 2);
来源：http://gu.nszjky.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yp.panjiajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dt.shtwfgs.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gu.yuntaijiaju.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://av.muxihuayi.cn

Ruby: (0...10).step(2).to_a
来源：http://zv.szsharing.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dp.colortex.cn

[B12] 跳出多层循环
来源：http://hi.szxytkj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://qi.panjiajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://rt.521024.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lj.jctech888.com.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qu.yuntaijiaju.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://da.panjiajie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ps.szxytkj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://oc.shtwfgs.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xr.huixinmuqiang.cn

[B13] 判断是否为数字
来源：http://xz.asd995.cn

Py:   isinstance(x, (int, float))
来源：http://xq.nicolike.cn

PHP:  is_numeric($x)
来源：http://az.521024.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xa.jianghongdianzi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gz.shtwfgs.cn

Java: x instanceof Number
来源：http://da.shxzukj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fx.haigaiapp.cn

Ruby: x.is_a?(Numeric)
来源：http://ox.nicolike.cn

C#:   x is int or double or decimal
来源：http://xa.chemitech.net.cn

[B14] 判断值是否在集合内
来源：http://eg.chemitech.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uh.lnxyls.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zx.huixiangedu.cn

JS:   [1, 2, 3].includes(x)
来源：http://yk.haigaiapp.cn

TS:   [1, 2, 3].includes(x)
来源：http://bb.shtwfgs.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://cq.gzmigu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ga.haigaiapp.cn

Ruby: [1, 2, 3].include?(x)
来源：http://pe.yuntaijiaju.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gy.chemitech.net.cn

[B15] 布尔运算与取反
来源：http://bw.bookmarksfly.cn

Py:   a and b or not c
来源：http://da.bookmarksfly.cn

PHP:  $a && $b || !$c
来源：http://to.colortex.cn

JS:   a && b || !c
来源：http://nz.asd995.cn

TS:   a && b || !c
来源：http://mz.shxzskj.cn

Java: a && b || !c
来源：http://nj.yuntaijiaju.cn

Go:   a && b || !c
来源：http://wb.szsharing.cn

Ruby: a && b || !c
来源：http://kq.newstarts.cn

C#:   a && b || !c
来源：http://ea.szxytkj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lu.colortex.cn

Py:   if not data: return
来源：http://pc.huixiangedu.cn

PHP:  if (!$data) { return; }
来源：http://ti.huanxung.cn

JS:   if (!data) return;
来源：http://kf.lnxyls.cn

TS:   if (!data) return;
来源：http://un.bjjhwx.cn

Java: if (data == null) return;
来源：http://sm.wgjwhj.cn

Go:   if data == nil { return }
来源：http://np.huixiangedu.cn

Ruby: return if data.nil?
来源：http://co.lnxyls.cn

C#:   if (data == null) return;
来源：http://sa.nszjky.cn

================================================================================
来源：http://uf.bookmarksfly.cn

C. 函数与作用域
来源：http://bf.lnxyls.cn

================================================================================
来源：http://gx.9csxet.cn

[C01] 定义函数
来源：http://om.szxytkj.cn

Py:   def add(a, b): return a + b
来源：http://yy.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qz.hnjuh.cn

JS:   function add(a, b) { return a + b; }
来源：http://iy.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ho.huixiangedu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ph.shxzukj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://be.nszjky.cn

Ruby: def add(a, b); a + b; end
来源：http://pa.huanxung.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tb.huixiangedu.cn

[C02] 默认参数
来源：http://rq.shtwfgs.cn

Py:   def greet(name="World"): return name
来源：http://ov.szsharing.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qs.szxytkj.cn

JS:   function greet(name = "World") { return name; }
来源：http://nn.muxihuayi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rz.hahajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jo.szsharing.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jt.szsharing.cn

Ruby: def greet(name = "World") = name
来源：http://pq.nicolike.cn

C#:   string Greet(string name = "World") => name;
来源：http://ni.yuntaijiaju.cn

[C03] 可变参数
来源：http://wy.haigaiapp.cn

Py:   def total(*args): return sum(args)
来源：http://jn.nszjky.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zx.shxzskj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sh.newstarts.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ot.bookmarksfly.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ek.bookmarksfly.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mk.panjiajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://kl.asd995.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://er.huanxung.cn

[C04] 命名参数 / 关键字参数
来源：http://yi.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cu.lnxyls.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://px.huixinmuqiang.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xe.nszjky.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xe.shtwfgs.cn

Java: // 无：用 Builder 模式或 record
来源：http://vh.jctech888.com.cn

Go:   // 无：用配置结构体参数
来源：http://op.shxzukj.cn

Ruby: f(a: 1, b: 2)
来源：http://bh.hnjuh.cn

C#:   f(a: 1, b: 2)
来源：http://kg.hahajie.cn

[C05] 返回多个值
来源：http://jz.9csxet.cn

Py:   return a, b
来源：http://ni.521024.cn

PHP:  return [$a, $b];
来源：http://ca.panjiajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://kn.shxzskj.cn

TS:   return { a, b };
来源：http://bu.jctech888.com.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mp.bookmarksfly.cn

Go:   return a, b
来源：http://ql.hahajie.cn

Ruby: return a, b
来源：http://xi.huanxung.cn

C#:   return (a, b);              // ValueTuple
来源：http://ay.521024.cn

[C06] 匿名函数 / lambda
来源：http://hn.huanxung.cn

Py:   square = lambda x: x * x
来源：http://hh.jianghongdianzi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://uh.panjiajie.cn

JS:   const square = x => x * x;
来源：http://rg.jctech888.com.cn

TS:   const square = (x: number): number => x * x;
来源：http://td.yuntaijiaju.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lv.bjjhwx.cn

Go:   sq := func(x int) int { return x * x }
来源：http://yi.nszjky.cn

Ruby: square = ->(x) { x * x }
来源：http://rl.asd995.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zg.asd995.cn

[C07] 把函数作为参数传入
来源：http://rd.nicolike.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zm.huixiangedu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xw.szxytkj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zy.panjiajie.cn

TS:   arr.map(String)
来源：http://bs.521024.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vz.shtwfgs.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xd.shxzskj.cn

Ruby: arr.map(&:upcase)
来源：http://cg.huixiangedu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://sj.9csxet.cn

[C08] 闭包
来源：http://fx.hahajie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cv.shtwfgs.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wj.huanxung.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sr.colortex.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://we.newstarts.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ko.muxihuayi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://no.yuntaijiaju.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vb.haigaiapp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ul.hnjuh.cn

[C09] 递归
来源：http://bj.wgjwhj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pp.shxzskj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vm.bjjhwx.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ch.nszjky.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nn.hnjuh.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hw.jianghongdianzi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ey.nicolike.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jq.szxytkj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gs.huixiangedu.cn

[C10] 变量作用域
来源：http://hd.lnxyls.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://iw.huanxung.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yd.shtwfgs.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jg.gzmigu.cn

TS:   同 JS
来源：http://te.panjiajie.cn

Java: 方法内为块级作用域
来源：http://ys.asd995.cn

Go:   花括号块级作用域
来源：http://pz.huanxung.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wg.szsharing.cn

C#:   块级作用域
来源：http://vl.nicolike.cn

[C11] 模块导入与导出
来源：http://ht.nszjky.cn

Py:   from module import func
来源：http://yl.hahajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://nw.521024.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hc.huixiangedu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rz.newstarts.cn

Java: import java.util.List;
来源：http://iy.jianghongdianzi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zi.huanxung.cn

Ruby: require "json"; require_relative "./util"
来源：http://tc.jianghongdianzi.cn

C#:   using System.Text;
来源：http://hi.haigaiapp.cn

[C12] 立即执行函数 IIFE
来源：http://fe.szxytkj.cn

Py:   (lambda: print("run"))()
来源：http://qo.yuexingan06.cn

PHP:  (function () { echo "run"; })();
来源：http://zu.jctech888.com.cn

JS:   (() => { console.log("run"); })();
来源：http://zi.szxytkj.cn

TS:   (() => { console.log("run"); })();
来源：http://sj.bjjhwx.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://uy.szxytkj.cn

Go:   func() { fmt.Println("run") }()
来源：http://jt.asd995.cn

Ruby: -> { puts "run" }.call
来源：http://ka.huanxung.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wk.shxzskj.cn

[C13] 类型声明 / 类型注解
来源：http://tf.jianghongdianzi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jp.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sv.yuntaijiaju.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kn.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://na.nszjky.cn


<!-- 参考信息 -->