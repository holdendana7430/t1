代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://av.haigaiapp.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fj.asd995.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ka.panjiajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ub.hnjuh.cn

Go:   strings.TrimSpace(s)
来源：http://un.9csxet.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jn.shtwfgs.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pc.yuntaijiaju.cn

[A25] 字符串比较
来源：http://jn.asd995.cn

Py:   s1 == s2; s1 != s2
来源：http://gw.muxihuayi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zt.521024.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wb.newstarts.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ys.asd995.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lu.asd995.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ot.muxihuayi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rw.szxytkj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rr.asd995.cn

[A26] 类型转换总览
来源：http://vd.huixinmuqiang.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gy.muxihuayi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lz.szsharing.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tx.jianghongdianzi.cn

TS:   Number() String() Boolean() x as number
来源：http://jp.bjjhwx.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fl.shxzukj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fp.521024.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://iv.hnjuh.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pd.newstarts.cn

================================================================================
来源：http://zp.yuntaijiaju.cn

B. 流程控制
来源：http://bk.nicolike.cn

================================================================================
来源：http://op.huixiangedu.cn

[B01] 条件判断 if / else
来源：http://tl.panjiajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://nd.muxihuayi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kb.szxytkj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ym.panjiajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kc.szxytkj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://iz.9csxet.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://es.chemitech.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gj.chemitech.net.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hc.nszjky.cn

[B02] 多分支 else if / elif
来源：http://vs.yuntaijiaju.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jd.lnxyls.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gs.bookmarksfly.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fv.wgjwhj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oo.yuntaijiaju.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://my.nszjky.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xt.jctech888.com.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://aw.huixinmuqiang.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ol.nszjky.cn

[B03] switch / match / case
来源：http://hq.huanxung.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bb.jianghongdianzi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://iv.nszjky.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hs.colortex.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yl.muxihuayi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kk.wgjwhj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fv.gzmigu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mf.yuntaijiaju.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jo.hahajie.cn

[B04] for 计数循环
来源：http://ap.jctech888.com.cn

Py:   for i in range(10): print(i)
来源：http://gy.bjjhwx.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rr.shxzskj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qw.szsharing.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wm.colortex.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wl.shxzukj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yl.yuntaijiaju.cn

Ruby: 10.times { |i| puts i }
来源：http://im.gzmigu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yt.shtwfgs.cn

[B05] 遍历数组 / 列表
来源：http://gk.yuexingan06.cn

Py:   for item in arr: print(item)
来源：http://ui.hahajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qm.hahajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://od.gzmigu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://as.panjiajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yn.yuntaijiaju.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zp.jianghongdianzi.cn

Ruby: arr.each { |item| puts item }
来源：http://pi.yuntaijiaju.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://es.bookmarksfly.cn

[B06] 遍历字典 / 对象
来源：http://ml.huixiangedu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://gw.nszjky.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vn.huanxung.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qt.jctech888.com.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cv.newstarts.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nm.lnxyls.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pt.nszjky.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ew.nicolike.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kt.haigaiapp.cn

[B07] while 循环
来源：http://gm.huixiangedu.cn

Py:   while i < 10: i += 1
来源：http://yi.9csxet.cn

PHP:  while ($i < 10) { $i++; }
来源：http://nj.bjjhwx.cn

JS:   while (i < 10) { i++; }
来源：http://kv.hnjuh.cn

TS:   while (i < 10) { i++; }
来源：http://mb.panjiajie.cn

Java: while (i < 10) { i++; }
来源：http://oj.jianghongdianzi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qb.hnjuh.cn

Ruby: while i < 10; i += 1; end
来源：http://zy.shxzukj.cn

C#:   while (i < 10) { i++; }
来源：http://ou.521024.cn

[B08] do-while（至少执行一次）
来源：http://ud.bjjhwx.cn

Py:   # 无 do-while：用 while True + break
来源：http://jc.shtwfgs.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://es.newstarts.cn

JS:   do { i++; } while (i < 10);
来源：http://rw.wgjwhj.cn

TS:   do { i++; } while (i < 10);
来源：http://xi.wgjwhj.cn

Java: do { i++; } while (i < 10);
来源：http://nq.jianghongdianzi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://co.shtwfgs.cn

Ruby: begin; i += 1; end while i < 10
来源：http://sw.nszjky.cn

C#:   do { i++; } while (i < 10);
来源：http://ka.huanxung.cn

[B09] break 与 continue
来源：http://ky.hahajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ta.colortex.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ro.9csxet.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pa.panjiajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ku.gzmigu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bq.shxzskj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tr.bjjhwx.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wp.hnjuh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uu.colortex.cn

[B10] 遍历同时拿索引
来源：http://bw.hahajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ip.yuexingan06.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xl.shxzskj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qm.shtwfgs.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ar.szsharing.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vp.wgjwhj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ft.bjjhwx.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kv.huanxung.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://iy.nszjky.cn

[B11] 生成数字序列 / 区间
来源：http://jy.yuexingan06.cn

Py:   list(range(0, 10, 2))
来源：http://ji.huixiangedu.cn

PHP:  range(0, 10, 2);
来源：http://ng.shxzukj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lm.szxytkj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kt.szxytkj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mo.wgjwhj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ai.chemitech.net.cn

Ruby: (0...10).step(2).to_a
来源：http://ki.nszjky.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vo.panjiajie.cn

[B12] 跳出多层循环
来源：http://xl.jctech888.com.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://th.shxzukj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mu.521024.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://op.asd995.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tr.panjiajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sd.nicolike.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xd.lnxyls.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qp.jctech888.com.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qu.huixinmuqiang.cn

[B13] 判断是否为数字
来源：http://mx.nicolike.cn

Py:   isinstance(x, (int, float))
来源：http://sy.nszjky.cn

PHP:  is_numeric($x)
来源：http://kb.chemitech.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wi.muxihuayi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nt.hnjuh.cn

Java: x instanceof Number
来源：http://lh.asd995.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xr.huixiangedu.cn

Ruby: x.is_a?(Numeric)
来源：http://xn.jianghongdianzi.cn

C#:   x is int or double or decimal
来源：http://wt.huanxung.cn

[B14] 判断值是否在集合内
来源：http://xm.yuntaijiaju.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ty.huanxung.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oq.wgjwhj.cn

JS:   [1, 2, 3].includes(x)
来源：http://ac.newstarts.cn

TS:   [1, 2, 3].includes(x)
来源：http://wd.shtwfgs.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://sw.colortex.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ge.lnxyls.cn

Ruby: [1, 2, 3].include?(x)
来源：http://hr.asd995.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jd.yuntaijiaju.cn

[B15] 布尔运算与取反
来源：http://lt.colortex.cn

Py:   a and b or not c
来源：http://xk.9csxet.cn

PHP:  $a && $b || !$c
来源：http://bt.szxytkj.cn

JS:   a && b || !c
来源：http://dr.bookmarksfly.cn

TS:   a && b || !c
来源：http://ek.huanxung.cn

Java: a && b || !c
来源：http://hg.jctech888.com.cn

Go:   a && b || !c
来源：http://cj.521024.cn

Ruby: a && b || !c
来源：http://hl.lnxyls.cn

C#:   a && b || !c
来源：http://gm.shxzukj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://mx.szxytkj.cn

Py:   if not data: return
来源：http://ua.shxzskj.cn

PHP:  if (!$data) { return; }
来源：http://ve.gzmigu.cn

JS:   if (!data) return;
来源：http://fk.shxzskj.cn

TS:   if (!data) return;
来源：http://ae.muxihuayi.cn

Java: if (data == null) return;
来源：http://oe.gzmigu.cn

Go:   if data == nil { return }
来源：http://st.huanxung.cn

Ruby: return if data.nil?
来源：http://do.haigaiapp.cn

C#:   if (data == null) return;
来源：http://us.yuexingan06.cn

================================================================================
来源：http://gw.wgjwhj.cn

C. 函数与作用域
来源：http://at.asd995.cn

================================================================================
来源：http://ui.hnjuh.cn

[C01] 定义函数
来源：http://wx.nszjky.cn

Py:   def add(a, b): return a + b
来源：http://ws.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pm.newstarts.cn

JS:   function add(a, b) { return a + b; }
来源：http://vw.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nc.yuexingan06.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://my.nszjky.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ib.bookmarksfly.cn

Ruby: def add(a, b); a + b; end
来源：http://fj.gzmigu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://eb.huixiangedu.cn

[C02] 默认参数
来源：http://sy.huanxung.cn

Py:   def greet(name="World"): return name
来源：http://vi.jianghongdianzi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lw.bjjhwx.cn

JS:   function greet(name = "World") { return name; }
来源：http://us.muxihuayi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hh.nszjky.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zj.hahajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ga.huanxung.cn

Ruby: def greet(name = "World") = name
来源：http://zf.nicolike.cn

C#:   string Greet(string name = "World") => name;
来源：http://lb.wgjwhj.cn

[C03] 可变参数
来源：http://mz.huixiangedu.cn

Py:   def total(*args): return sum(args)
来源：http://fe.shxzskj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yg.521024.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cs.huixinmuqiang.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wq.jianghongdianzi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wb.asd995.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://as.gzmigu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ck.haigaiapp.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lr.gzmigu.cn

[C04] 命名参数 / 关键字参数
来源：http://dg.521024.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kx.jctech888.com.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gx.szxytkj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ug.9csxet.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yj.gzmigu.cn

Java: // 无：用 Builder 模式或 record
来源：http://kv.colortex.cn

Go:   // 无：用配置结构体参数
来源：http://no.jctech888.com.cn

Ruby: f(a: 1, b: 2)
来源：http://ic.panjiajie.cn

C#:   f(a: 1, b: 2)
来源：http://od.asd995.cn

[C05] 返回多个值
来源：http://dx.gzmigu.cn

Py:   return a, b
来源：http://pv.shtwfgs.cn

PHP:  return [$a, $b];
来源：http://mo.szxytkj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pp.jianghongdianzi.cn

TS:   return { a, b };
来源：http://qi.jctech888.com.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jh.jianghongdianzi.cn

Go:   return a, b
来源：http://lh.hnjuh.cn

Ruby: return a, b
来源：http://pw.jctech888.com.cn

C#:   return (a, b);              // ValueTuple
来源：http://aq.lnxyls.cn

[C06] 匿名函数 / lambda
来源：http://yf.asd995.cn

Py:   square = lambda x: x * x
来源：http://wf.nicolike.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://io.jctech888.com.cn

JS:   const square = x => x * x;
来源：http://or.9csxet.cn

TS:   const square = (x: number): number => x * x;
来源：http://el.szxytkj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zn.yuntaijiaju.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jc.nicolike.cn

Ruby: square = ->(x) { x * x }
来源：http://xj.shxzskj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://sm.gzmigu.cn

[C07] 把函数作为参数传入
来源：http://oc.szxytkj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lu.bookmarksfly.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hn.newstarts.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uy.huixinmuqiang.cn

TS:   arr.map(String)
来源：http://xt.chemitech.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://to.panjiajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://at.shtwfgs.cn

Ruby: arr.map(&:upcase)
来源：http://on.newstarts.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://zi.shxzskj.cn

[C08] 闭包
来源：http://hl.muxihuayi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zs.shxzukj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://al.colortex.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ki.szxytkj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uv.haigaiapp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bc.9csxet.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sv.gzmigu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ak.521024.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://it.bookmarksfly.cn

[C09] 递归
来源：http://ax.newstarts.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xm.muxihuayi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lo.nszjky.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ic.bjjhwx.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ro.asd995.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kp.shxzukj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vy.wgjwhj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ux.szxytkj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ff.szsharing.cn

[C10] 变量作用域
来源：http://ji.chemitech.net.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zs.nicolike.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tr.nszjky.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fa.gzmigu.cn

TS:   同 JS
来源：http://sr.jctech888.com.cn

Java: 方法内为块级作用域
来源：http://ex.wgjwhj.cn

Go:   花括号块级作用域
来源：http://rb.szsharing.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://eo.haigaiapp.cn

C#:   块级作用域
来源：http://nt.newstarts.cn

[C11] 模块导入与导出
来源：http://oe.nszjky.cn

Py:   from module import func
来源：http://ku.jctech888.com.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://gp.colortex.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://xn.hahajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jz.shtwfgs.cn

Java: import java.util.List;
来源：http://lp.colortex.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wj.bookmarksfly.cn

Ruby: require "json"; require_relative "./util"
来源：http://ko.hahajie.cn

C#:   using System.Text;
来源：http://jo.nszjky.cn

[C12] 立即执行函数 IIFE
来源：http://oe.shxzukj.cn

Py:   (lambda: print("run"))()
来源：http://ol.gzmigu.cn

PHP:  (function () { echo "run"; })();
来源：http://kv.hahajie.cn

JS:   (() => { console.log("run"); })();
来源：http://dn.lnxyls.cn

TS:   (() => { console.log("run"); })();
来源：http://qa.9csxet.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ti.yuntaijiaju.cn

Go:   func() { fmt.Println("run") }()
来源：http://oa.hnjuh.cn

Ruby: -> { puts "run" }.call
来源：http://jw.hnjuh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://sf.szsharing.cn

[C13] 类型声明 / 类型注解
来源：http://lm.lnxyls.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jr.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ru.chemitech.net.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tx.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ui.nszjky.cn

Java: int add(int a, int b) { return a + b; }
来源：http://do.bjjhwx.cn

Go:   func add(a, b int) int
来源：http://jy.hahajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hb.huixiangedu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://iq.newstarts.cn

[C14] 泛型函数
来源：http://pi.muxihuayi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cp.yuexingan06.cn

PHP:  // 无泛型
来源：http://eo.jctech888.com.cn

JS:   // 无泛型
来源：http://xz.szxytkj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jn.huanxung.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://py.huanxung.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fb.lnxyls.cn

Ruby: # 无泛型
来源：http://bm.hnjuh.cn


<!-- 参考信息 -->