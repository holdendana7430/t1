代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hd.shxzskj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rv.bjjhwx.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://in.wgjwhj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ti.yuexingan06.cn

Go:   strings.TrimSpace(s)
来源：http://pu.nicolike.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://iz.gzmigu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ez.newstarts.cn

[A25] 字符串比较
来源：http://ea.wgjwhj.cn

Py:   s1 == s2; s1 != s2
来源：http://sm.muxihuayi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://iv.asd995.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xg.521024.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ge.hahajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ti.shtwfgs.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fg.colortex.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://oz.bjjhwx.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dj.yuntaijiaju.cn

[A26] 类型转换总览
来源：http://uv.bookmarksfly.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://za.szxytkj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xm.newstarts.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fl.shtwfgs.cn

TS:   Number() String() Boolean() x as number
来源：http://pv.huanxung.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xu.jctech888.com.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ub.huixiangedu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://iv.bjjhwx.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ea.hnjuh.cn

================================================================================
来源：http://xg.yuexingan06.cn

B. 流程控制
来源：http://fp.muxihuayi.cn

================================================================================
来源：http://wu.jctech888.com.cn

[B01] 条件判断 if / else
来源：http://bq.gzmigu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://yg.nszjky.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bm.bookmarksfly.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xq.shxzukj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sf.bookmarksfly.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://kt.521024.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kg.nicolike.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://et.jctech888.com.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zu.muxihuayi.cn

[B02] 多分支 else if / elif
来源：http://xm.muxihuayi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bl.huixiangedu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kw.muxihuayi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yp.bjjhwx.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://of.gzmigu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://op.chemitech.net.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vb.bjjhwx.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nn.asd995.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qf.lnxyls.cn

[B03] switch / match / case
来源：http://wl.asd995.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vm.gzmigu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ct.521024.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nw.colortex.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://er.bjjhwx.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ps.lnxyls.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lk.muxihuayi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zh.nicolike.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xf.shxzukj.cn

[B04] for 计数循环
来源：http://ay.chemitech.net.cn

Py:   for i in range(10): print(i)
来源：http://gt.jctech888.com.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fs.9csxet.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://el.bjjhwx.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lv.521024.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mq.bookmarksfly.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wi.bookmarksfly.cn

Ruby: 10.times { |i| puts i }
来源：http://il.chemitech.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ud.colortex.cn

[B05] 遍历数组 / 列表
来源：http://te.haigaiapp.cn

Py:   for item in arr: print(item)
来源：http://ay.bjjhwx.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bn.wgjwhj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://de.szxytkj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gw.nszjky.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ym.shxzskj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tz.jianghongdianzi.cn

Ruby: arr.each { |item| puts item }
来源：http://ip.nszjky.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ue.bookmarksfly.cn

[B06] 遍历字典 / 对象
来源：http://mf.bookmarksfly.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qq.huixinmuqiang.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xt.lnxyls.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zt.lnxyls.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jy.shxzukj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cq.bookmarksfly.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://oi.shxzukj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rq.bookmarksfly.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tt.nszjky.cn

[B07] while 循环
来源：http://ga.szsharing.cn

Py:   while i < 10: i += 1
来源：http://fa.huanxung.cn

PHP:  while ($i < 10) { $i++; }
来源：http://sl.muxihuayi.cn

JS:   while (i < 10) { i++; }
来源：http://ok.lnxyls.cn

TS:   while (i < 10) { i++; }
来源：http://id.bookmarksfly.cn

Java: while (i < 10) { i++; }
来源：http://xr.asd995.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://in.nszjky.cn

Ruby: while i < 10; i += 1; end
来源：http://pv.bookmarksfly.cn

C#:   while (i < 10) { i++; }
来源：http://eb.521024.cn

[B08] do-while（至少执行一次）
来源：http://nt.szsharing.cn

Py:   # 无 do-while：用 while True + break
来源：http://jk.521024.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://gy.bjjhwx.cn

JS:   do { i++; } while (i < 10);
来源：http://eh.huixiangedu.cn

TS:   do { i++; } while (i < 10);
来源：http://wo.haigaiapp.cn

Java: do { i++; } while (i < 10);
来源：http://cu.panjiajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://nm.jctech888.com.cn

Ruby: begin; i += 1; end while i < 10
来源：http://iy.asd995.cn

C#:   do { i++; } while (i < 10);
来源：http://bg.shxzukj.cn

[B09] break 与 continue
来源：http://cf.bookmarksfly.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dt.chemitech.net.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xv.nszjky.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lk.szsharing.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ek.huixiangedu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ao.shxzskj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pg.szsharing.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wa.shtwfgs.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qw.lnxyls.cn

[B10] 遍历同时拿索引
来源：http://nv.yuexingan06.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ck.muxihuayi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kp.yuexingan06.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ib.huixinmuqiang.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ae.jctech888.com.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://un.hahajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mw.muxihuayi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ed.bookmarksfly.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ue.521024.cn

[B11] 生成数字序列 / 区间
来源：http://qn.colortex.cn

Py:   list(range(0, 10, 2))
来源：http://tq.shtwfgs.cn

PHP:  range(0, 10, 2);
来源：http://eh.nicolike.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kh.jctech888.com.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gy.haigaiapp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rd.hahajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lk.huixinmuqiang.cn

Ruby: (0...10).step(2).to_a
来源：http://vp.huanxung.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rs.yuexingan06.cn

[B12] 跳出多层循环
来源：http://wx.jctech888.com.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bf.jctech888.com.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gu.chemitech.net.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gh.nszjky.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dt.shtwfgs.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ng.huixiangedu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://up.wgjwhj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ot.shxzukj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qt.huixiangedu.cn

[B13] 判断是否为数字
来源：http://qw.haigaiapp.cn

Py:   isinstance(x, (int, float))
来源：http://ip.haigaiapp.cn

PHP:  is_numeric($x)
来源：http://ix.wgjwhj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://re.wgjwhj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cy.szxytkj.cn

Java: x instanceof Number
来源：http://ta.huanxung.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://id.huixinmuqiang.cn

Ruby: x.is_a?(Numeric)
来源：http://ru.bookmarksfly.cn

C#:   x is int or double or decimal
来源：http://er.9csxet.cn

[B14] 判断值是否在集合内
来源：http://cc.shxzukj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://al.szxytkj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://li.lnxyls.cn

JS:   [1, 2, 3].includes(x)
来源：http://ia.nszjky.cn

TS:   [1, 2, 3].includes(x)
来源：http://at.huixiangedu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://lq.shxzskj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qx.nicolike.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ev.bjjhwx.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ew.haigaiapp.cn

[B15] 布尔运算与取反
来源：http://nw.nicolike.cn

Py:   a and b or not c
来源：http://qe.colortex.cn

PHP:  $a && $b || !$c
来源：http://pc.huixiangedu.cn

JS:   a && b || !c
来源：http://ln.hahajie.cn

TS:   a && b || !c
来源：http://in.jctech888.com.cn

Java: a && b || !c
来源：http://ny.muxihuayi.cn

Go:   a && b || !c
来源：http://ju.hahajie.cn

Ruby: a && b || !c
来源：http://bh.colortex.cn

C#:   a && b || !c
来源：http://io.muxihuayi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gw.huixinmuqiang.cn

Py:   if not data: return
来源：http://sp.9csxet.cn

PHP:  if (!$data) { return; }
来源：http://sh.muxihuayi.cn

JS:   if (!data) return;
来源：http://gh.colortex.cn

TS:   if (!data) return;
来源：http://mg.colortex.cn

Java: if (data == null) return;
来源：http://gt.nszjky.cn

Go:   if data == nil { return }
来源：http://op.9csxet.cn

Ruby: return if data.nil?
来源：http://te.bjjhwx.cn

C#:   if (data == null) return;
来源：http://wo.haigaiapp.cn

================================================================================
来源：http://xf.wgjwhj.cn

C. 函数与作用域
来源：http://pb.jctech888.com.cn

================================================================================
来源：http://ad.szxytkj.cn

[C01] 定义函数
来源：http://mk.colortex.cn

Py:   def add(a, b): return a + b
来源：http://gh.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kz.9csxet.cn

JS:   function add(a, b) { return a + b; }
来源：http://hf.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uq.shxzukj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qs.panjiajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hr.panjiajie.cn

Ruby: def add(a, b); a + b; end
来源：http://dn.huixinmuqiang.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pd.newstarts.cn

[C02] 默认参数
来源：http://vj.hahajie.cn

Py:   def greet(name="World"): return name
来源：http://mu.yuntaijiaju.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zo.lnxyls.cn

JS:   function greet(name = "World") { return name; }
来源：http://wy.hahajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://nv.nicolike.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qh.asd995.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fz.shxzukj.cn

Ruby: def greet(name = "World") = name
来源：http://xl.shxzukj.cn

C#:   string Greet(string name = "World") => name;
来源：http://hg.huixiangedu.cn

[C03] 可变参数
来源：http://ij.haigaiapp.cn

Py:   def total(*args): return sum(args)
来源：http://dt.hahajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mg.jianghongdianzi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yf.shtwfgs.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://aq.yuntaijiaju.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pu.bookmarksfly.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lt.huixiangedu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yx.shtwfgs.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cn.haigaiapp.cn

[C04] 命名参数 / 关键字参数
来源：http://ck.nszjky.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gs.bjjhwx.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ng.newstarts.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qi.huixinmuqiang.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nn.gzmigu.cn

Java: // 无：用 Builder 模式或 record
来源：http://sb.521024.cn

Go:   // 无：用配置结构体参数
来源：http://qa.lnxyls.cn

Ruby: f(a: 1, b: 2)
来源：http://hz.szxytkj.cn

C#:   f(a: 1, b: 2)
来源：http://ot.9csxet.cn

[C05] 返回多个值
来源：http://up.jctech888.com.cn

Py:   return a, b
来源：http://ub.nszjky.cn

PHP:  return [$a, $b];
来源：http://ht.hahajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fm.haigaiapp.cn

TS:   return { a, b };
来源：http://vv.newstarts.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pc.shxzskj.cn

Go:   return a, b
来源：http://qx.jctech888.com.cn

Ruby: return a, b
来源：http://yx.chemitech.net.cn

C#:   return (a, b);              // ValueTuple
来源：http://wc.wgjwhj.cn

[C06] 匿名函数 / lambda
来源：http://xg.521024.cn

Py:   square = lambda x: x * x
来源：http://su.lnxyls.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ez.colortex.cn

JS:   const square = x => x * x;
来源：http://gc.lnxyls.cn

TS:   const square = (x: number): number => x * x;
来源：http://eo.yuexingan06.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vp.gzmigu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wx.huixiangedu.cn

Ruby: square = ->(x) { x * x }
来源：http://uj.yuexingan06.cn

C#:   Func<int, int> square = x => x * x;
来源：http://rs.huixinmuqiang.cn

[C07] 把函数作为参数传入
来源：http://wo.shtwfgs.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gf.shxzskj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://mx.hnjuh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ck.shxzukj.cn

TS:   arr.map(String)
来源：http://mg.colortex.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ia.chemitech.net.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ky.nszjky.cn

Ruby: arr.map(&:upcase)
来源：http://vk.chemitech.net.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://oc.9csxet.cn

[C08] 闭包
来源：http://ui.hahajie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mu.yuexingan06.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lu.hahajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qt.huixiangedu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ey.9csxet.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ul.newstarts.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jx.asd995.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yi.bjjhwx.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hw.jianghongdianzi.cn

[C09] 递归
来源：http://hb.9csxet.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hm.huixiangedu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qg.haigaiapp.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ih.hahajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jv.jianghongdianzi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mb.yuexingan06.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ue.huixinmuqiang.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yv.panjiajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xg.asd995.cn

[C10] 变量作用域
来源：http://om.9csxet.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qv.lnxyls.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gw.huixiangedu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bv.shxzskj.cn

TS:   同 JS
来源：http://hx.521024.cn

Java: 方法内为块级作用域
来源：http://cy.jianghongdianzi.cn

Go:   花括号块级作用域
来源：http://gb.huixinmuqiang.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ba.hahajie.cn

C#:   块级作用域
来源：http://rw.shxzukj.cn

[C11] 模块导入与导出
来源：http://ik.newstarts.cn

Py:   from module import func
来源：http://zl.shtwfgs.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pm.huixiangedu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://lq.nszjky.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ts.bjjhwx.cn

Java: import java.util.List;
来源：http://ba.hahajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tc.nicolike.cn

Ruby: require "json"; require_relative "./util"
来源：http://ce.521024.cn

C#:   using System.Text;
来源：http://ly.yuexingan06.cn

[C12] 立即执行函数 IIFE
来源：http://ri.huixinmuqiang.cn

Py:   (lambda: print("run"))()
来源：http://ed.shtwfgs.cn

PHP:  (function () { echo "run"; })();
来源：http://vb.huanxung.cn

JS:   (() => { console.log("run"); })();
来源：http://aw.huixiangedu.cn

TS:   (() => { console.log("run"); })();
来源：http://qn.haigaiapp.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ke.gzmigu.cn

Go:   func() { fmt.Println("run") }()
来源：http://tf.hnjuh.cn

Ruby: -> { puts "run" }.call
来源：http://uy.szxytkj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wz.newstarts.cn

[C13] 类型声明 / 类型注解
来源：http://he.huanxung.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pc.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uw.9csxet.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kx.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ka.panjiajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jh.huanxung.cn

Go:   func add(a, b int) int
来源：http://xt.huanxung.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cf.yuexingan06.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bf.yuexingan06.cn

[C14] 泛型函数
来源：http://bu.szsharing.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rr.muxihuayi.cn

PHP:  // 无泛型
来源：http://yo.asd995.cn

JS:   // 无泛型
来源：http://mj.nicolike.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ow.shxzukj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uv.haigaiapp.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vo.wgjwhj.cn

Ruby: # 无泛型
来源：http://cw.colortex.cn


<!-- 参考信息 -->