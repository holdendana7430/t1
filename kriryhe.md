代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://xo.gzmigu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://am.muxihuayi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rw.nszjky.cn

[A25] 字符串比较
来源：http://wm.chemitech.net.cn

Py:   s1 == s2; s1 != s2
来源：http://na.chemitech.net.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wr.yuntaijiaju.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://iu.szxytkj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kw.wgjwhj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fd.yuexingan06.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qz.panjiajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://od.bjjhwx.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wn.shxzukj.cn

[A26] 类型转换总览
来源：http://gq.9csxet.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ib.chemitech.net.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xn.newstarts.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bd.521024.cn

TS:   Number() String() Boolean() x as number
来源：http://ww.hnjuh.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://px.yuexingan06.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xh.521024.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://yi.huixiangedu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zc.panjiajie.cn

================================================================================
来源：http://hh.shxzukj.cn

B. 流程控制
来源：http://vz.newstarts.cn

================================================================================
来源：http://wx.gzmigu.cn

[B01] 条件判断 if / else
来源：http://wf.shtwfgs.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://kj.521024.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://js.jianghongdianzi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ln.bookmarksfly.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gw.chemitech.net.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://rn.chemitech.net.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zz.huixiangedu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://uh.bjjhwx.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ju.szsharing.cn

[B02] 多分支 else if / elif
来源：http://om.huixinmuqiang.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dg.huanxung.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fn.bookmarksfly.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nv.colortex.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dl.huixiangedu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bq.chemitech.net.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zy.lnxyls.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ka.nszjky.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rr.shtwfgs.cn

[B03] switch / match / case
来源：http://ut.chemitech.net.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sd.wgjwhj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ux.muxihuayi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rp.haigaiapp.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zq.szsharing.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vp.chemitech.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zz.szxytkj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cg.nicolike.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pt.panjiajie.cn

[B04] for 计数循环
来源：http://cb.9csxet.cn

Py:   for i in range(10): print(i)
来源：http://bt.hnjuh.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kz.panjiajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://aa.haigaiapp.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dp.nicolike.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zz.shxzukj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://he.hnjuh.cn

Ruby: 10.times { |i| puts i }
来源：http://bs.shtwfgs.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xg.shtwfgs.cn

[B05] 遍历数组 / 列表
来源：http://qs.chemitech.net.cn

Py:   for item in arr: print(item)
来源：http://kl.szsharing.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xv.9csxet.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ii.yuexingan06.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yf.chemitech.net.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yr.szxytkj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yi.colortex.cn

Ruby: arr.each { |item| puts item }
来源：http://vc.shtwfgs.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ny.shtwfgs.cn

[B06] 遍历字典 / 对象
来源：http://jz.hahajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://uq.521024.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://eu.wgjwhj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xz.huanxung.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://db.jctech888.com.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bb.wgjwhj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://um.szsharing.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xd.huanxung.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kz.asd995.cn

[B07] while 循环
来源：http://hc.yuexingan06.cn

Py:   while i < 10: i += 1
来源：http://qp.szxytkj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://jq.huixiangedu.cn

JS:   while (i < 10) { i++; }
来源：http://ac.9csxet.cn

TS:   while (i < 10) { i++; }
来源：http://oj.huixinmuqiang.cn

Java: while (i < 10) { i++; }
来源：http://ox.colortex.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://oq.yuexingan06.cn

Ruby: while i < 10; i += 1; end
来源：http://ug.nicolike.cn

C#:   while (i < 10) { i++; }
来源：http://hq.9csxet.cn

[B08] do-while（至少执行一次）
来源：http://dc.hahajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://bx.shtwfgs.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://af.huixinmuqiang.cn

JS:   do { i++; } while (i < 10);
来源：http://wk.jianghongdianzi.cn

TS:   do { i++; } while (i < 10);
来源：http://dn.huixiangedu.cn

Java: do { i++; } while (i < 10);
来源：http://ls.bookmarksfly.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://oi.hahajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://if.hahajie.cn

C#:   do { i++; } while (i < 10);
来源：http://py.szsharing.cn

[B09] break 与 continue
来源：http://iw.nszjky.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ij.hnjuh.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vt.yuexingan06.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cg.hnjuh.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mw.chemitech.net.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xv.hahajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gw.panjiajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nj.colortex.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xm.szsharing.cn

[B10] 遍历同时拿索引
来源：http://ql.asd995.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nr.colortex.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xo.hnjuh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pp.huixinmuqiang.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xy.wgjwhj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ge.szxytkj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kz.jctech888.com.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gf.jianghongdianzi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gz.wgjwhj.cn

[B11] 生成数字序列 / 区间
来源：http://lg.muxihuayi.cn

Py:   list(range(0, 10, 2))
来源：http://qp.nszjky.cn

PHP:  range(0, 10, 2);
来源：http://bs.yuexingan06.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://su.jianghongdianzi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kb.9csxet.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ho.shxzskj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jm.panjiajie.cn

Ruby: (0...10).step(2).to_a
来源：http://rm.yuntaijiaju.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sw.lnxyls.cn

[B12] 跳出多层循环
来源：http://gl.wgjwhj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://vy.haigaiapp.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wr.9csxet.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tg.colortex.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mu.szsharing.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zb.yuntaijiaju.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sf.haigaiapp.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://uo.haigaiapp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nh.nszjky.cn

[B13] 判断是否为数字
来源：http://wa.szsharing.cn

Py:   isinstance(x, (int, float))
来源：http://we.bjjhwx.cn

PHP:  is_numeric($x)
来源：http://ld.szxytkj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qg.newstarts.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gu.hahajie.cn

Java: x instanceof Number
来源：http://pu.yuexingan06.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mc.huanxung.cn

Ruby: x.is_a?(Numeric)
来源：http://uo.lnxyls.cn

C#:   x is int or double or decimal
来源：http://us.wgjwhj.cn

[B14] 判断值是否在集合内
来源：http://nt.asd995.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gj.newstarts.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ip.shxzskj.cn

JS:   [1, 2, 3].includes(x)
来源：http://cg.yuntaijiaju.cn

TS:   [1, 2, 3].includes(x)
来源：http://xw.9csxet.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ql.huixiangedu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bc.haigaiapp.cn

Ruby: [1, 2, 3].include?(x)
来源：http://wd.shxzukj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wt.yuexingan06.cn

[B15] 布尔运算与取反
来源：http://op.asd995.cn

Py:   a and b or not c
来源：http://rh.szsharing.cn

PHP:  $a && $b || !$c
来源：http://vw.nszjky.cn

JS:   a && b || !c
来源：http://he.shxzskj.cn

TS:   a && b || !c
来源：http://hl.lnxyls.cn

Java: a && b || !c
来源：http://cb.9csxet.cn

Go:   a && b || !c
来源：http://df.hnjuh.cn

Ruby: a && b || !c
来源：http://zt.bookmarksfly.cn

C#:   a && b || !c
来源：http://xo.szsharing.cn

[B16] 卫语句：不满足条件提前返回
来源：http://km.szxytkj.cn

Py:   if not data: return
来源：http://tk.yuntaijiaju.cn

PHP:  if (!$data) { return; }
来源：http://zg.shtwfgs.cn

JS:   if (!data) return;
来源：http://ye.muxihuayi.cn

TS:   if (!data) return;
来源：http://ga.nszjky.cn

Java: if (data == null) return;
来源：http://vi.bookmarksfly.cn

Go:   if data == nil { return }
来源：http://gu.yuntaijiaju.cn

Ruby: return if data.nil?
来源：http://al.nicolike.cn

C#:   if (data == null) return;
来源：http://jm.huanxung.cn

================================================================================
来源：http://wr.muxihuayi.cn

C. 函数与作用域
来源：http://tl.hahajie.cn

================================================================================
来源：http://pv.nicolike.cn

[C01] 定义函数
来源：http://gw.jianghongdianzi.cn

Py:   def add(a, b): return a + b
来源：http://qg.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jb.shxzskj.cn

JS:   function add(a, b) { return a + b; }
来源：http://im.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://og.szxytkj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://kx.bookmarksfly.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jv.chemitech.net.cn

Ruby: def add(a, b); a + b; end
来源：http://mq.muxihuayi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uj.yuntaijiaju.cn

[C02] 默认参数
来源：http://xd.nszjky.cn

Py:   def greet(name="World"): return name
来源：http://cg.shxzukj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://uc.jianghongdianzi.cn

JS:   function greet(name = "World") { return name; }
来源：http://qw.gzmigu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ew.nicolike.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://kt.panjiajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qj.huixiangedu.cn

Ruby: def greet(name = "World") = name
来源：http://ea.shxzskj.cn

C#:   string Greet(string name = "World") => name;
来源：http://kq.shxzskj.cn

[C03] 可变参数
来源：http://va.nszjky.cn

Py:   def total(*args): return sum(args)
来源：http://ql.huanxung.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lr.szsharing.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qo.shxzskj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wt.shxzukj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hs.nszjky.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lj.panjiajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rf.shxzskj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://oh.shxzskj.cn

[C04] 命名参数 / 关键字参数
来源：http://xk.huixiangedu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ri.nicolike.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ak.jianghongdianzi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vv.colortex.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://me.shtwfgs.cn

Java: // 无：用 Builder 模式或 record
来源：http://vi.bjjhwx.cn

Go:   // 无：用配置结构体参数
来源：http://fe.jctech888.com.cn

Ruby: f(a: 1, b: 2)
来源：http://py.chemitech.net.cn

C#:   f(a: 1, b: 2)
来源：http://hl.yuntaijiaju.cn

[C05] 返回多个值
来源：http://bo.colortex.cn

Py:   return a, b
来源：http://cg.huixiangedu.cn

PHP:  return [$a, $b];
来源：http://et.colortex.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dp.yuntaijiaju.cn

TS:   return { a, b };
来源：http://me.newstarts.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ct.hnjuh.cn

Go:   return a, b
来源：http://lw.haigaiapp.cn

Ruby: return a, b
来源：http://iw.newstarts.cn

C#:   return (a, b);              // ValueTuple
来源：http://lf.huixinmuqiang.cn

[C06] 匿名函数 / lambda
来源：http://co.colortex.cn

Py:   square = lambda x: x * x
来源：http://yc.jianghongdianzi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://vi.colortex.cn

JS:   const square = x => x * x;
来源：http://kd.szxytkj.cn

TS:   const square = (x: number): number => x * x;
来源：http://fj.bookmarksfly.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jh.haigaiapp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://pk.hahajie.cn

Ruby: square = ->(x) { x * x }
来源：http://jz.muxihuayi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://nf.nszjky.cn

[C07] 把函数作为参数传入
来源：http://vm.9csxet.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://je.shxzukj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://mr.shxzukj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gz.bookmarksfly.cn

TS:   arr.map(String)
来源：http://rf.jianghongdianzi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ug.chemitech.net.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hg.szxytkj.cn

Ruby: arr.map(&:upcase)
来源：http://jy.shxzukj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wz.jctech888.com.cn

[C08] 闭包
来源：http://ks.bookmarksfly.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mi.gzmigu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mq.9csxet.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ug.lnxyls.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ci.nicolike.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://el.huixinmuqiang.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rv.huixiangedu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tt.shxzskj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://og.gzmigu.cn

[C09] 递归
来源：http://sf.newstarts.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xs.newstarts.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hs.nicolike.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://do.huanxung.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://br.colortex.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mw.colortex.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bu.hnjuh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dj.jianghongdianzi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sq.haigaiapp.cn

[C10] 变量作用域
来源：http://cq.szsharing.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yo.huixinmuqiang.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hx.bookmarksfly.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jt.yuexingan06.cn

TS:   同 JS
来源：http://ny.gzmigu.cn

Java: 方法内为块级作用域
来源：http://qj.521024.cn

Go:   花括号块级作用域
来源：http://zr.nszjky.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zp.521024.cn

C#:   块级作用域
来源：http://rc.gzmigu.cn

[C11] 模块导入与导出
来源：http://xw.yuntaijiaju.cn

Py:   from module import func
来源：http://dk.jianghongdianzi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pg.shxzukj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://xv.szxytkj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yn.lnxyls.cn

Java: import java.util.List;
来源：http://tm.bjjhwx.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rv.nicolike.cn

Ruby: require "json"; require_relative "./util"
来源：http://kt.newstarts.cn

C#:   using System.Text;
来源：http://fb.lnxyls.cn

[C12] 立即执行函数 IIFE
来源：http://jf.hahajie.cn

Py:   (lambda: print("run"))()
来源：http://bo.chemitech.net.cn

PHP:  (function () { echo "run"; })();
来源：http://ja.jianghongdianzi.cn

JS:   (() => { console.log("run"); })();
来源：http://xc.lnxyls.cn

TS:   (() => { console.log("run"); })();
来源：http://xi.huixinmuqiang.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://va.chemitech.net.cn

Go:   func() { fmt.Println("run") }()
来源：http://ly.shxzskj.cn

Ruby: -> { puts "run" }.call
来源：http://qi.shxzukj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xe.9csxet.cn

[C13] 类型声明 / 类型注解
来源：http://dl.nicolike.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hr.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bu.hnjuh.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ax.yuexingan06.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qz.chemitech.net.cn

Java: int add(int a, int b) { return a + b; }
来源：http://hp.yuntaijiaju.cn

Go:   func add(a, b int) int
来源：http://oz.shxzskj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fs.jianghongdianzi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://uq.szsharing.cn

[C14] 泛型函数
来源：http://xp.jctech888.com.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hh.muxihuayi.cn

PHP:  // 无泛型
来源：http://tx.hahajie.cn

JS:   // 无泛型
来源：http://ga.yuexingan06.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vv.521024.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ds.shxzukj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://oa.nszjky.cn

Ruby: # 无泛型
来源：http://qt.shxzukj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://te.newstarts.cn

[C15] 解构 / 展开参数
来源：http://vr.szxytkj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sh.lnxyls.cn

PHP:  [$a, $b] = $pair;
来源：http://zd.colortex.cn


<!-- 参考信息 -->