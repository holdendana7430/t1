代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gc.bjjhwx.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ej.jctech888.com.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lu.huanxung.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ur.jctech888.com.cn

Go:   strings.TrimSpace(s)
来源：http://vu.bookmarksfly.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vf.nszjky.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yw.szxytkj.cn

[A25] 字符串比较
来源：http://iu.hahajie.cn

Py:   s1 == s2; s1 != s2
来源：http://qp.szsharing.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ho.9csxet.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ks.newstarts.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ve.yuexingan06.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cd.lnxyls.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vq.huixiangedu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://pb.hnjuh.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lo.jctech888.com.cn

[A26] 类型转换总览
来源：http://jm.huanxung.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pm.colortex.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bj.asd995.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rv.jctech888.com.cn

TS:   Number() String() Boolean() x as number
来源：http://io.panjiajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ge.nszjky.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zj.huanxung.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://kf.szsharing.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://so.9csxet.cn

================================================================================
来源：http://wt.panjiajie.cn

B. 流程控制
来源：http://jn.hnjuh.cn

================================================================================
来源：http://fu.jctech888.com.cn

[B01] 条件判断 if / else
来源：http://rq.jctech888.com.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://kd.szxytkj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ao.chemitech.net.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://js.szxytkj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vs.nicolike.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://em.yuexingan06.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jc.huanxung.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wy.panjiajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://eo.gzmigu.cn

[B02] 多分支 else if / elif
来源：http://ae.521024.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.shxzskj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ko.huixiangedu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://us.yuntaijiaju.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ay.jianghongdianzi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hu.bookmarksfly.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jy.lnxyls.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://db.jctech888.com.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zz.muxihuayi.cn

[B03] switch / match / case
来源：http://vm.szsharing.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://iv.jianghongdianzi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zz.bjjhwx.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://aq.yuexingan06.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gu.asd995.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.nszjky.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://sj.panjiajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xs.gzmigu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sa.bjjhwx.cn

[B04] for 计数循环
来源：http://rm.shxzukj.cn

Py:   for i in range(10): print(i)
来源：http://ok.521024.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hy.newstarts.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ak.szsharing.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zw.shxzukj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tt.shxzukj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zy.colortex.cn

Ruby: 10.times { |i| puts i }
来源：http://am.lnxyls.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xa.colortex.cn

[B05] 遍历数组 / 列表
来源：http://eb.huixinmuqiang.cn

Py:   for item in arr: print(item)
来源：http://dn.9csxet.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bo.nszjky.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://cr.shtwfgs.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gc.yuntaijiaju.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://cx.szxytkj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wp.jianghongdianzi.cn

Ruby: arr.each { |item| puts item }
来源：http://ku.yuntaijiaju.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hm.9csxet.cn

[B06] 遍历字典 / 对象
来源：http://ih.bjjhwx.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xd.jianghongdianzi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pu.lnxyls.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://il.jctech888.com.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ge.hahajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://to.panjiajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ji.shxzskj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ni.newstarts.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ch.huanxung.cn

[B07] while 循环
来源：http://ug.nicolike.cn

Py:   while i < 10: i += 1
来源：http://pa.panjiajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://sm.yuexingan06.cn

JS:   while (i < 10) { i++; }
来源：http://vn.chemitech.net.cn

TS:   while (i < 10) { i++; }
来源：http://mo.521024.cn

Java: while (i < 10) { i++; }
来源：http://ci.asd995.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dd.shxzskj.cn

Ruby: while i < 10; i += 1; end
来源：http://if.shxzskj.cn

C#:   while (i < 10) { i++; }
来源：http://jb.521024.cn

[B08] do-while（至少执行一次）
来源：http://tm.hahajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://ov.chemitech.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qr.panjiajie.cn

JS:   do { i++; } while (i < 10);
来源：http://gi.colortex.cn

TS:   do { i++; } while (i < 10);
来源：http://ph.newstarts.cn

Java: do { i++; } while (i < 10);
来源：http://sd.jctech888.com.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sq.shxzukj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://px.9csxet.cn

C#:   do { i++; } while (i < 10);
来源：http://qm.hnjuh.cn

[B09] break 与 continue
来源：http://ql.shxzukj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ft.chemitech.net.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ey.9csxet.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nq.nszjky.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bw.szxytkj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ay.huixiangedu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://na.lnxyls.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lr.shxzukj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dx.huixinmuqiang.cn

[B10] 遍历同时拿索引
来源：http://fb.521024.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ls.szsharing.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dj.szxytkj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rn.9csxet.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uz.nszjky.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vn.asd995.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ym.gzmigu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sd.bjjhwx.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kl.wgjwhj.cn

[B11] 生成数字序列 / 区间
来源：http://ba.hahajie.cn

Py:   list(range(0, 10, 2))
来源：http://is.panjiajie.cn

PHP:  range(0, 10, 2);
来源：http://ld.gzmigu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://im.shxzukj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bk.lnxyls.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://us.bookmarksfly.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gu.jianghongdianzi.cn

Ruby: (0...10).step(2).to_a
来源：http://dl.colortex.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zk.bjjhwx.cn

[B12] 跳出多层循环
来源：http://lo.yuntaijiaju.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fi.yuexingan06.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://tu.haigaiapp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hs.colortex.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gh.muxihuayi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mz.shxzukj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ps.huanxung.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rr.yuntaijiaju.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tk.wgjwhj.cn

[B13] 判断是否为数字
来源：http://dq.huixinmuqiang.cn

Py:   isinstance(x, (int, float))
来源：http://yi.huixiangedu.cn

PHP:  is_numeric($x)
来源：http://nj.521024.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://af.gzmigu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mj.521024.cn

Java: x instanceof Number
来源：http://tc.shxzukj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tg.hahajie.cn

Ruby: x.is_a?(Numeric)
来源：http://ae.gzmigu.cn

C#:   x is int or double or decimal
来源：http://lc.jctech888.com.cn

[B14] 判断值是否在集合内
来源：http://op.chemitech.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nq.haigaiapp.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sn.gzmigu.cn

JS:   [1, 2, 3].includes(x)
来源：http://si.shxzskj.cn

TS:   [1, 2, 3].includes(x)
来源：http://ae.huixinmuqiang.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kt.szxytkj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xj.shxzskj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://dt.nicolike.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://of.muxihuayi.cn

[B15] 布尔运算与取反
来源：http://eo.muxihuayi.cn

Py:   a and b or not c
来源：http://qz.nszjky.cn

PHP:  $a && $b || !$c
来源：http://ia.lnxyls.cn

JS:   a && b || !c
来源：http://uq.huixinmuqiang.cn

TS:   a && b || !c
来源：http://sq.9csxet.cn

Java: a && b || !c
来源：http://co.chemitech.net.cn

Go:   a && b || !c
来源：http://tf.colortex.cn

Ruby: a && b || !c
来源：http://ds.colortex.cn

C#:   a && b || !c
来源：http://ot.panjiajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://dz.huixiangedu.cn

Py:   if not data: return
来源：http://wo.szxytkj.cn

PHP:  if (!$data) { return; }
来源：http://ck.haigaiapp.cn

JS:   if (!data) return;
来源：http://xc.jctech888.com.cn

TS:   if (!data) return;
来源：http://hf.yuexingan06.cn

Java: if (data == null) return;
来源：http://ek.muxihuayi.cn

Go:   if data == nil { return }
来源：http://ur.jianghongdianzi.cn

Ruby: return if data.nil?
来源：http://xt.asd995.cn

C#:   if (data == null) return;
来源：http://vd.chemitech.net.cn

================================================================================
来源：http://jq.yuntaijiaju.cn

C. 函数与作用域
来源：http://uz.bjjhwx.cn

================================================================================
来源：http://ri.shxzukj.cn

[C01] 定义函数
来源：http://zt.jianghongdianzi.cn

Py:   def add(a, b): return a + b
来源：http://el.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mw.gzmigu.cn

JS:   function add(a, b) { return a + b; }
来源：http://ks.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vd.nszjky.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xt.muxihuayi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dh.huanxung.cn

Ruby: def add(a, b); a + b; end
来源：http://bl.huanxung.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fp.chemitech.net.cn

[C02] 默认参数
来源：http://vx.muxihuayi.cn

Py:   def greet(name="World"): return name
来源：http://ny.jctech888.com.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wm.szxytkj.cn

JS:   function greet(name = "World") { return name; }
来源：http://cj.huanxung.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lc.muxihuayi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://us.nicolike.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ta.shtwfgs.cn

Ruby: def greet(name = "World") = name
来源：http://fx.jctech888.com.cn

C#:   string Greet(string name = "World") => name;
来源：http://fq.yuntaijiaju.cn

[C03] 可变参数
来源：http://cc.lnxyls.cn

Py:   def total(*args): return sum(args)
来源：http://ga.gzmigu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qj.jctech888.com.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ww.shxzukj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nc.huixinmuqiang.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fj.muxihuayi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ex.yuntaijiaju.cn

Ruby: def total(*nums); nums.sum; end
来源：http://mc.jctech888.com.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hr.szxytkj.cn

[C04] 命名参数 / 关键字参数
来源：http://fm.asd995.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://my.bjjhwx.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gc.jianghongdianzi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wa.szsharing.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vk.chemitech.net.cn

Java: // 无：用 Builder 模式或 record
来源：http://rq.gzmigu.cn

Go:   // 无：用配置结构体参数
来源：http://qz.panjiajie.cn

Ruby: f(a: 1, b: 2)
来源：http://oq.521024.cn

C#:   f(a: 1, b: 2)
来源：http://ha.newstarts.cn

[C05] 返回多个值
来源：http://aq.jctech888.com.cn

Py:   return a, b
来源：http://rg.nszjky.cn

PHP:  return [$a, $b];
来源：http://ec.bookmarksfly.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ui.shtwfgs.cn

TS:   return { a, b };
来源：http://ic.panjiajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bu.huixinmuqiang.cn

Go:   return a, b
来源：http://at.521024.cn

Ruby: return a, b
来源：http://rx.colortex.cn

C#:   return (a, b);              // ValueTuple
来源：http://pp.hnjuh.cn

[C06] 匿名函数 / lambda
来源：http://sl.shtwfgs.cn

Py:   square = lambda x: x * x
来源：http://jj.huixinmuqiang.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://hw.nszjky.cn

JS:   const square = x => x * x;
来源：http://nv.shxzskj.cn

TS:   const square = (x: number): number => x * x;
来源：http://bv.lnxyls.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qo.panjiajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://iu.szsharing.cn

Ruby: square = ->(x) { x * x }
来源：http://bo.szsharing.cn

C#:   Func<int, int> square = x => x * x;
来源：http://jk.shtwfgs.cn

[C07] 把函数作为参数传入
来源：http://zz.chemitech.net.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gn.huixinmuqiang.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ra.haigaiapp.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jr.chemitech.net.cn

TS:   arr.map(String)
来源：http://zl.huixiangedu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gg.huanxung.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kt.huanxung.cn

Ruby: arr.map(&:upcase)
来源：http://hp.bookmarksfly.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pv.haigaiapp.cn

[C08] 闭包
来源：http://im.szsharing.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ho.bjjhwx.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qg.bookmarksfly.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hd.bjjhwx.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ku.muxihuayi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sr.yuntaijiaju.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vq.yuntaijiaju.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://as.huixiangedu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ms.yuntaijiaju.cn

[C09] 递归
来源：http://xl.shtwfgs.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nl.colortex.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pt.nicolike.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bk.hahajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wr.wgjwhj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wg.jctech888.com.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mv.shxzukj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ig.jctech888.com.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vo.jctech888.com.cn

[C10] 变量作用域
来源：http://vh.gzmigu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wt.nszjky.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ev.huixinmuqiang.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fs.muxihuayi.cn

TS:   同 JS
来源：http://oj.huanxung.cn

Java: 方法内为块级作用域
来源：http://iu.shxzskj.cn

Go:   花括号块级作用域
来源：http://ri.yuntaijiaju.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hx.haigaiapp.cn

C#:   块级作用域
来源：http://qx.nszjky.cn

[C11] 模块导入与导出
来源：http://vj.huanxung.cn

Py:   from module import func
来源：http://as.asd995.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bt.jianghongdianzi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://wu.hahajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lj.shxzukj.cn

Java: import java.util.List;
来源：http://eq.nicolike.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bb.yuntaijiaju.cn

Ruby: require "json"; require_relative "./util"
来源：http://qj.521024.cn

C#:   using System.Text;
来源：http://in.jctech888.com.cn

[C12] 立即执行函数 IIFE
来源：http://qk.jctech888.com.cn

Py:   (lambda: print("run"))()
来源：http://li.bjjhwx.cn

PHP:  (function () { echo "run"; })();
来源：http://vs.panjiajie.cn

JS:   (() => { console.log("run"); })();
来源：http://ob.jianghongdianzi.cn

TS:   (() => { console.log("run"); })();
来源：http://ip.shtwfgs.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://og.shxzukj.cn

Go:   func() { fmt.Println("run") }()
来源：http://xz.szsharing.cn

Ruby: -> { puts "run" }.call
来源：http://la.521024.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zu.shxzukj.cn

[C13] 类型声明 / 类型注解
来源：http://bb.yuntaijiaju.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jz.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zj.shxzskj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gr.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://et.shxzskj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://yw.jctech888.com.cn

Go:   func add(a, b int) int
来源：http://eg.521024.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ec.hahajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://el.wgjwhj.cn

[C14] 泛型函数
来源：http://tl.szsharing.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://oz.szxytkj.cn

PHP:  // 无泛型
来源：http://fp.chemitech.net.cn

JS:   // 无泛型
来源：http://mk.bjjhwx.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://li.gzmigu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sr.haigaiapp.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://og.521024.cn

Ruby: # 无泛型
来源：http://wv.huixiangedu.cn


<!-- 参考信息 -->