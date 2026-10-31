代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://lf.gzmigu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ql.panjiajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://we.nszjky.cn

[A25] 字符串比较
来源：http://fc.yuexingan06.cn

Py:   s1 == s2; s1 != s2
来源：http://pw.jctech888.com.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cr.chemitech.net.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gi.huixiangedu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zp.yuexingan06.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qa.nszjky.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xz.shxzskj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ng.szsharing.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cs.bjjhwx.cn

[A26] 类型转换总览
来源：http://iu.hnjuh.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ca.gzmigu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ri.asd995.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://uy.jctech888.com.cn

TS:   Number() String() Boolean() x as number
来源：http://jb.jctech888.com.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rn.wgjwhj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jo.nszjky.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://dn.521024.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://at.shxzskj.cn

================================================================================
来源：http://ca.nszjky.cn

B. 流程控制
来源：http://fg.colortex.cn

================================================================================
来源：http://kf.521024.cn

[B01] 条件判断 if / else
来源：http://vo.huixiangedu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dp.jctech888.com.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jd.szxytkj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jy.jctech888.com.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dz.jctech888.com.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://pc.chemitech.net.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cr.yuntaijiaju.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://de.nszjky.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yb.newstarts.cn

[B02] 多分支 else if / elif
来源：http://gj.shxzukj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://si.huanxung.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xj.colortex.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cm.szsharing.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gh.newstarts.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rt.szxytkj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uo.bookmarksfly.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://la.huixinmuqiang.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hw.shxzukj.cn

[B03] switch / match / case
来源：http://pu.chemitech.net.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ca.hnjuh.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vs.panjiajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://av.chemitech.net.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dg.521024.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rn.newstarts.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lq.newstarts.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ei.newstarts.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://br.chemitech.net.cn

[B04] for 计数循环
来源：http://br.hahajie.cn

Py:   for i in range(10): print(i)
来源：http://xc.newstarts.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://we.nszjky.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vj.gzmigu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nr.hahajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ay.nszjky.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pf.szsharing.cn

Ruby: 10.times { |i| puts i }
来源：http://zt.shxzukj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wk.jctech888.com.cn

[B05] 遍历数组 / 列表
来源：http://rj.panjiajie.cn

Py:   for item in arr: print(item)
来源：http://ap.yuexingan06.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://av.newstarts.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://er.nszjky.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qn.521024.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hi.nszjky.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zi.wgjwhj.cn

Ruby: arr.each { |item| puts item }
来源：http://rj.shxzukj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ic.wgjwhj.cn

[B06] 遍历字典 / 对象
来源：http://vr.hahajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://dk.newstarts.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gv.shxzskj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qy.521024.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tn.lnxyls.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://at.bookmarksfly.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://th.shtwfgs.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lt.nszjky.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yk.nicolike.cn

[B07] while 循环
来源：http://ne.shxzskj.cn

Py:   while i < 10: i += 1
来源：http://zf.panjiajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://jf.huixinmuqiang.cn

JS:   while (i < 10) { i++; }
来源：http://ra.lnxyls.cn

TS:   while (i < 10) { i++; }
来源：http://hw.haigaiapp.cn

Java: while (i < 10) { i++; }
来源：http://ek.colortex.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yq.lnxyls.cn

Ruby: while i < 10; i += 1; end
来源：http://yw.muxihuayi.cn

C#:   while (i < 10) { i++; }
来源：http://yh.hahajie.cn

[B08] do-while（至少执行一次）
来源：http://ms.chemitech.net.cn

Py:   # 无 do-while：用 while True + break
来源：http://yh.szsharing.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mn.panjiajie.cn

JS:   do { i++; } while (i < 10);
来源：http://qd.shxzukj.cn

TS:   do { i++; } while (i < 10);
来源：http://pm.nicolike.cn

Java: do { i++; } while (i < 10);
来源：http://zo.jianghongdianzi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ns.huanxung.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ki.lnxyls.cn

C#:   do { i++; } while (i < 10);
来源：http://nn.shxzukj.cn

[B09] break 与 continue
来源：http://hu.521024.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vh.gzmigu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://du.huanxung.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xm.asd995.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yd.lnxyls.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jk.bjjhwx.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://id.szxytkj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bk.newstarts.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kg.chemitech.net.cn

[B10] 遍历同时拿索引
来源：http://hg.haigaiapp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ql.jctech888.com.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://na.hahajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://if.panjiajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yd.huanxung.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lq.bjjhwx.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://js.9csxet.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qw.hnjuh.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jc.yuntaijiaju.cn

[B11] 生成数字序列 / 区间
来源：http://xh.muxihuayi.cn

Py:   list(range(0, 10, 2))
来源：http://cu.shxzukj.cn

PHP:  range(0, 10, 2);
来源：http://fp.hnjuh.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cu.nszjky.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ji.hnjuh.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yu.lnxyls.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xf.nicolike.cn

Ruby: (0...10).step(2).to_a
来源：http://fn.yuexingan06.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yr.szxytkj.cn

[B12] 跳出多层循环
来源：http://es.hahajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zr.gzmigu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://bv.huanxung.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yd.jctech888.com.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vo.bjjhwx.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://up.wgjwhj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ui.shxzskj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jq.hnjuh.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nt.chemitech.net.cn

[B13] 判断是否为数字
来源：http://nl.shtwfgs.cn

Py:   isinstance(x, (int, float))
来源：http://dl.jctech888.com.cn

PHP:  is_numeric($x)
来源：http://hv.haigaiapp.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lg.chemitech.net.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rn.haigaiapp.cn

Java: x instanceof Number
来源：http://yc.lnxyls.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ml.haigaiapp.cn

Ruby: x.is_a?(Numeric)
来源：http://kk.haigaiapp.cn

C#:   x is int or double or decimal
来源：http://dx.hnjuh.cn

[B14] 判断值是否在集合内
来源：http://vo.nszjky.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qs.szxytkj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oo.huixiangedu.cn

JS:   [1, 2, 3].includes(x)
来源：http://ec.9csxet.cn

TS:   [1, 2, 3].includes(x)
来源：http://vu.huanxung.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gu.haigaiapp.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ja.shtwfgs.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ad.newstarts.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sp.panjiajie.cn

[B15] 布尔运算与取反
来源：http://zx.panjiajie.cn

Py:   a and b or not c
来源：http://wx.shxzukj.cn

PHP:  $a && $b || !$c
来源：http://ov.shtwfgs.cn

JS:   a && b || !c
来源：http://nt.lnxyls.cn

TS:   a && b || !c
来源：http://dl.newstarts.cn

Java: a && b || !c
来源：http://js.shxzskj.cn

Go:   a && b || !c
来源：http://vj.bookmarksfly.cn

Ruby: a && b || !c
来源：http://bj.szxytkj.cn

C#:   a && b || !c
来源：http://rv.szxytkj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://uf.nszjky.cn

Py:   if not data: return
来源：http://aa.hnjuh.cn

PHP:  if (!$data) { return; }
来源：http://ws.jctech888.com.cn

JS:   if (!data) return;
来源：http://eu.shxzskj.cn

TS:   if (!data) return;
来源：http://wb.shtwfgs.cn

Java: if (data == null) return;
来源：http://xg.bjjhwx.cn

Go:   if data == nil { return }
来源：http://is.yuntaijiaju.cn

Ruby: return if data.nil?
来源：http://mf.9csxet.cn

C#:   if (data == null) return;
来源：http://yr.gzmigu.cn

================================================================================
来源：http://vm.yuntaijiaju.cn

C. 函数与作用域
来源：http://oj.szsharing.cn

================================================================================
来源：http://aw.shxzskj.cn

[C01] 定义函数
来源：http://ir.wgjwhj.cn

Py:   def add(a, b): return a + b
来源：http://hp.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lh.wgjwhj.cn

JS:   function add(a, b) { return a + b; }
来源：http://dl.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yr.huanxung.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gy.huixinmuqiang.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qp.jianghongdianzi.cn

Ruby: def add(a, b); a + b; end
来源：http://bp.panjiajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ip.9csxet.cn

[C02] 默认参数
来源：http://ea.newstarts.cn

Py:   def greet(name="World"): return name
来源：http://mu.521024.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://uk.9csxet.cn

JS:   function greet(name = "World") { return name; }
来源：http://kg.9csxet.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://nj.jianghongdianzi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://tc.szsharing.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nf.chemitech.net.cn

Ruby: def greet(name = "World") = name
来源：http://rz.szsharing.cn

C#:   string Greet(string name = "World") => name;
来源：http://gp.chemitech.net.cn

[C03] 可变参数
来源：http://rd.jianghongdianzi.cn

Py:   def total(*args): return sum(args)
来源：http://dm.nicolike.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://by.huixinmuqiang.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://do.shxzukj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yuntaijiaju.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ep.colortex.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yb.hnjuh.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yp.chemitech.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://th.haigaiapp.cn

[C04] 命名参数 / 关键字参数
来源：http://zt.bookmarksfly.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zz.newstarts.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yu.huixinmuqiang.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fy.9csxet.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bw.newstarts.cn

Java: // 无：用 Builder 模式或 record
来源：http://rh.yuntaijiaju.cn

Go:   // 无：用配置结构体参数
来源：http://wy.huixiangedu.cn

Ruby: f(a: 1, b: 2)
来源：http://ea.gzmigu.cn

C#:   f(a: 1, b: 2)
来源：http://kx.yuntaijiaju.cn

[C05] 返回多个值
来源：http://qa.jianghongdianzi.cn

Py:   return a, b
来源：http://cg.huanxung.cn

PHP:  return [$a, $b];
来源：http://cq.szxytkj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wc.huanxung.cn

TS:   return { a, b };
来源：http://jk.szsharing.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dw.hnjuh.cn

Go:   return a, b
来源：http://hy.9csxet.cn

Ruby: return a, b
来源：http://sd.hnjuh.cn

C#:   return (a, b);              // ValueTuple
来源：http://eo.shtwfgs.cn

[C06] 匿名函数 / lambda
来源：http://re.shxzskj.cn

Py:   square = lambda x: x * x
来源：http://pm.9csxet.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ti.szsharing.cn

JS:   const square = x => x * x;
来源：http://nd.muxihuayi.cn

TS:   const square = (x: number): number => x * x;
来源：http://df.huixiangedu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wn.huanxung.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dz.lnxyls.cn

Ruby: square = ->(x) { x * x }
来源：http://wp.colortex.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ro.muxihuayi.cn

[C07] 把函数作为参数传入
来源：http://fp.huixiangedu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ph.colortex.cn

PHP:  array_map("strtoupper", $arr);
来源：http://cu.haigaiapp.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bt.huixiangedu.cn

TS:   arr.map(String)
来源：http://vl.nicolike.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ss.gzmigu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dl.bjjhwx.cn

Ruby: arr.map(&:upcase)
来源：http://ni.bjjhwx.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ax.nszjky.cn

[C08] 闭包
来源：http://km.9csxet.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://sd.yuntaijiaju.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zp.colortex.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sv.huixinmuqiang.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gq.bjjhwx.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wi.szxytkj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ez.lnxyls.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qj.nicolike.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pw.hnjuh.cn

[C09] 递归
来源：http://fw.wgjwhj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rh.szsharing.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ow.huixinmuqiang.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://of.shxzukj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qw.bookmarksfly.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sn.muxihuayi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://au.huixiangedu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kb.hahajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mk.haigaiapp.cn

[C10] 变量作用域
来源：http://ij.huixinmuqiang.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jl.hahajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pl.521024.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qe.colortex.cn

TS:   同 JS
来源：http://xn.shxzskj.cn

Java: 方法内为块级作用域
来源：http://ah.yuntaijiaju.cn

Go:   花括号块级作用域
来源：http://rt.shtwfgs.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://iu.bjjhwx.cn

C#:   块级作用域
来源：http://ih.bjjhwx.cn

[C11] 模块导入与导出
来源：http://ix.newstarts.cn

Py:   from module import func
来源：http://xp.panjiajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pz.shxzukj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gw.newstarts.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hf.muxihuayi.cn

Java: import java.util.List;
来源：http://da.bjjhwx.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jt.nszjky.cn

Ruby: require "json"; require_relative "./util"
来源：http://fe.panjiajie.cn

C#:   using System.Text;
来源：http://gf.gzmigu.cn

[C12] 立即执行函数 IIFE
来源：http://ij.newstarts.cn

Py:   (lambda: print("run"))()
来源：http://kt.muxihuayi.cn

PHP:  (function () { echo "run"; })();
来源：http://za.nszjky.cn

JS:   (() => { console.log("run"); })();
来源：http://lm.jianghongdianzi.cn

TS:   (() => { console.log("run"); })();
来源：http://yw.yuexingan06.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dq.colortex.cn

Go:   func() { fmt.Println("run") }()
来源：http://rm.muxihuayi.cn

Ruby: -> { puts "run" }.call
来源：http://pi.9csxet.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://yv.yuexingan06.cn

[C13] 类型声明 / 类型注解
来源：http://ng.szsharing.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xe.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qk.huixinmuqiang.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xw.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ab.521024.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wv.gzmigu.cn

Go:   func add(a, b int) int
来源：http://hm.szsharing.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://he.bookmarksfly.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wt.huixiangedu.cn

[C14] 泛型函数
来源：http://zm.yuntaijiaju.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ql.szsharing.cn

PHP:  // 无泛型
来源：http://di.asd995.cn

JS:   // 无泛型
来源：http://mv.nicolike.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ac.lnxyls.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jh.szsharing.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ds.hnjuh.cn

Ruby: # 无泛型
来源：http://un.huixiangedu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wa.muxihuayi.cn

[C15] 解构 / 展开参数
来源：http://ns.yuntaijiaju.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tc.nszjky.cn

PHP:  [$a, $b] = $pair;
来源：http://gy.panjiajie.cn


<!-- 参考信息 -->