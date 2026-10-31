代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lr.haigaiapp.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://el.jianghongdianzi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://oy.hahajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yh.bookmarksfly.cn

[A26] 类型转换总览
来源：http://ti.huanxung.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cg.szsharing.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qo.szsharing.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ho.panjiajie.cn

TS:   Number() String() Boolean() x as number
来源：http://rv.szsharing.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jm.lnxyls.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zl.bjjhwx.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://qc.szxytkj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://em.haigaiapp.cn

================================================================================
来源：http://pd.shtwfgs.cn

B. 流程控制
来源：http://hq.gzmigu.cn

================================================================================
来源：http://bz.huixiangedu.cn

[B01] 条件判断 if / else
来源：http://vn.lnxyls.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://rc.nicolike.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://uu.bjjhwx.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://iy.gzmigu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hj.yuntaijiaju.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://tf.muxihuayi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lb.colortex.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://br.yuntaijiaju.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://th.gzmigu.cn

[B02] 多分支 else if / elif
来源：http://wj.huixiangedu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ng.panjiajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://go.szsharing.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kp.haigaiapp.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ev.szxytkj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aa.newstarts.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dn.huixiangedu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://av.colortex.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bg.asd995.cn

[B03] switch / match / case
来源：http://ny.asd995.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yg.huixinmuqiang.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hw.shxzskj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lz.gzmigu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fy.wgjwhj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ha.9csxet.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hm.lnxyls.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hc.nicolike.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gn.colortex.cn

[B04] for 计数循环
来源：http://uh.wgjwhj.cn

Py:   for i in range(10): print(i)
来源：http://lf.nicolike.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gn.shtwfgs.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zr.hahajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vb.szxytkj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xk.huixiangedu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gi.hnjuh.cn

Ruby: 10.times { |i| puts i }
来源：http://sx.bookmarksfly.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gp.huanxung.cn

[B05] 遍历数组 / 列表
来源：http://hk.panjiajie.cn

Py:   for item in arr: print(item)
来源：http://mt.nicolike.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jh.nszjky.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://al.newstarts.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tk.hahajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qa.shxzukj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gu.nszjky.cn

Ruby: arr.each { |item| puts item }
来源：http://vt.jctech888.com.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zk.huanxung.cn

[B06] 遍历字典 / 对象
来源：http://gj.lnxyls.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://kt.panjiajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ox.nicolike.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bi.jctech888.com.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xl.shtwfgs.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lx.jctech888.com.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kc.yuntaijiaju.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bx.colortex.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ps.9csxet.cn

[B07] while 循环
来源：http://gf.szxytkj.cn

Py:   while i < 10: i += 1
来源：http://ek.shxzskj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hl.huixinmuqiang.cn

JS:   while (i < 10) { i++; }
来源：http://kx.colortex.cn

TS:   while (i < 10) { i++; }
来源：http://vb.colortex.cn

Java: while (i < 10) { i++; }
来源：http://ni.lnxyls.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sl.wgjwhj.cn

Ruby: while i < 10; i += 1; end
来源：http://fh.huanxung.cn

C#:   while (i < 10) { i++; }
来源：http://vm.huixinmuqiang.cn

[B08] do-while（至少执行一次）
来源：http://bu.huixiangedu.cn

Py:   # 无 do-while：用 while True + break
来源：http://eh.9csxet.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://rb.lnxyls.cn

JS:   do { i++; } while (i < 10);
来源：http://jn.wgjwhj.cn

TS:   do { i++; } while (i < 10);
来源：http://at.nszjky.cn

Java: do { i++; } while (i < 10);
来源：http://jq.chemitech.net.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fz.bjjhwx.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wx.huanxung.cn

C#:   do { i++; } while (i < 10);
来源：http://mh.nszjky.cn

[B09] break 与 continue
来源：http://mh.lnxyls.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bf.shxzskj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://le.nicolike.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cv.szxytkj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cx.yuexingan06.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vt.yuexingan06.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wr.huixinmuqiang.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nh.szsharing.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mi.haigaiapp.cn

[B10] 遍历同时拿索引
来源：http://oi.haigaiapp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qj.lnxyls.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xc.nicolike.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mv.jctech888.com.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rz.wgjwhj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zu.szxytkj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fs.yuexingan06.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://az.shtwfgs.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sc.nicolike.cn

[B11] 生成数字序列 / 区间
来源：http://or.hahajie.cn

Py:   list(range(0, 10, 2))
来源：http://rr.colortex.cn

PHP:  range(0, 10, 2);
来源：http://es.shxzukj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ua.521024.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gv.hnjuh.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gg.haigaiapp.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://if.shtwfgs.cn

Ruby: (0...10).step(2).to_a
来源：http://zn.gzmigu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hm.yuntaijiaju.cn

[B12] 跳出多层循环
来源：http://vf.jianghongdianzi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zq.jctech888.com.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ft.yuexingan06.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gu.bjjhwx.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jh.gzmigu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hr.asd995.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gt.shxzskj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://oc.newstarts.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rw.szxytkj.cn

[B13] 判断是否为数字
来源：http://uf.yuexingan06.cn

Py:   isinstance(x, (int, float))
来源：http://fb.yuntaijiaju.cn

PHP:  is_numeric($x)
来源：http://wo.asd995.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ao.panjiajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aa.gzmigu.cn

Java: x instanceof Number
来源：http://nj.szsharing.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tm.yuntaijiaju.cn

Ruby: x.is_a?(Numeric)
来源：http://ka.jctech888.com.cn

C#:   x is int or double or decimal
来源：http://cy.lnxyls.cn

[B14] 判断值是否在集合内
来源：http://bb.szxytkj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://im.shtwfgs.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vm.lnxyls.cn

JS:   [1, 2, 3].includes(x)
来源：http://wt.panjiajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://hp.9csxet.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ug.bookmarksfly.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xj.colortex.cn

Ruby: [1, 2, 3].include?(x)
来源：http://um.colortex.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lh.szxytkj.cn

[B15] 布尔运算与取反
来源：http://ca.hnjuh.cn

Py:   a and b or not c
来源：http://ng.shxzskj.cn

PHP:  $a && $b || !$c
来源：http://dd.nszjky.cn

JS:   a && b || !c
来源：http://vx.shtwfgs.cn

TS:   a && b || !c
来源：http://nh.jctech888.com.cn

Java: a && b || !c
来源：http://ud.newstarts.cn

Go:   a && b || !c
来源：http://nw.chemitech.net.cn

Ruby: a && b || !c
来源：http://qf.chemitech.net.cn

C#:   a && b || !c
来源：http://jw.muxihuayi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://st.yuexingan06.cn

Py:   if not data: return
来源：http://bt.huixinmuqiang.cn

PHP:  if (!$data) { return; }
来源：http://mh.9csxet.cn

JS:   if (!data) return;
来源：http://hj.nicolike.cn

TS:   if (!data) return;
来源：http://nk.jctech888.com.cn

Java: if (data == null) return;
来源：http://zs.shtwfgs.cn

Go:   if data == nil { return }
来源：http://fm.9csxet.cn

Ruby: return if data.nil?
来源：http://cy.gzmigu.cn

C#:   if (data == null) return;
来源：http://qy.shxzskj.cn

================================================================================
来源：http://bp.wgjwhj.cn

C. 函数与作用域
来源：http://hl.gzmigu.cn

================================================================================
来源：http://ut.nszjky.cn

[C01] 定义函数
来源：http://js.lnxyls.cn

Py:   def add(a, b): return a + b
来源：http://ja.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yp.colortex.cn

JS:   function add(a, b) { return a + b; }
来源：http://uo.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bx.panjiajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ku.shtwfgs.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ia.shtwfgs.cn

Ruby: def add(a, b); a + b; end
来源：http://px.bjjhwx.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rx.huixiangedu.cn

[C02] 默认参数
来源：http://wy.gzmigu.cn

Py:   def greet(name="World"): return name
来源：http://ym.wgjwhj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://nh.yuntaijiaju.cn

JS:   function greet(name = "World") { return name; }
来源：http://fd.jctech888.com.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gv.yuntaijiaju.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dv.521024.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lf.wgjwhj.cn

Ruby: def greet(name = "World") = name
来源：http://uz.huixinmuqiang.cn

C#:   string Greet(string name = "World") => name;
来源：http://rr.yuntaijiaju.cn

[C03] 可变参数
来源：http://lm.gzmigu.cn

Py:   def total(*args): return sum(args)
来源：http://jn.panjiajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zz.nicolike.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nq.bjjhwx.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kf.asd995.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://df.jianghongdianzi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nd.huixinmuqiang.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fy.jctech888.com.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dn.wgjwhj.cn

[C04] 命名参数 / 关键字参数
来源：http://vi.haigaiapp.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wn.nicolike.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hr.chemitech.net.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://oz.shxzukj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://da.huanxung.cn

Java: // 无：用 Builder 模式或 record
来源：http://hk.gzmigu.cn

Go:   // 无：用配置结构体参数
来源：http://bw.szxytkj.cn

Ruby: f(a: 1, b: 2)
来源：http://wx.hahajie.cn

C#:   f(a: 1, b: 2)
来源：http://yf.jianghongdianzi.cn

[C05] 返回多个值
来源：http://pm.shtwfgs.cn

Py:   return a, b
来源：http://nt.wgjwhj.cn

PHP:  return [$a, $b];
来源：http://cg.bookmarksfly.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://cw.newstarts.cn

TS:   return { a, b };
来源：http://qa.lnxyls.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dm.521024.cn

Go:   return a, b
来源：http://lv.lnxyls.cn

Ruby: return a, b
来源：http://yx.shxzukj.cn

C#:   return (a, b);              // ValueTuple
来源：http://aj.nicolike.cn

[C06] 匿名函数 / lambda
来源：http://pp.9csxet.cn

Py:   square = lambda x: x * x
来源：http://mx.hahajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://nm.yuexingan06.cn

JS:   const square = x => x * x;
来源：http://qg.bjjhwx.cn

TS:   const square = (x: number): number => x * x;
来源：http://va.huixiangedu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vi.bookmarksfly.cn

Go:   sq := func(x int) int { return x * x }
来源：http://oe.wgjwhj.cn

Ruby: square = ->(x) { x * x }
来源：http://gr.newstarts.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ma.shtwfgs.cn

[C07] 把函数作为参数传入
来源：http://hc.hahajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ef.szxytkj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://dc.shxzukj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://oa.hnjuh.cn

TS:   arr.map(String)
来源：http://ag.yuexingan06.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gp.bjjhwx.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ni.gzmigu.cn

Ruby: arr.map(&:upcase)
来源：http://qj.gzmigu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://sg.hnjuh.cn

[C08] 闭包
来源：http://yf.newstarts.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://co.lnxyls.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xf.haigaiapp.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pk.nszjky.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://em.szsharing.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gu.huixinmuqiang.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qk.yuexingan06.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qs.hahajie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ng.521024.cn

[C09] 递归
来源：http://ba.newstarts.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vr.shxzskj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://no.huixiangedu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oi.szsharing.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eh.huixiangedu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lk.szsharing.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tl.nszjky.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xf.szxytkj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tw.nicolike.cn

[C10] 变量作用域
来源：http://rq.asd995.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://si.asd995.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ns.colortex.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ic.jctech888.com.cn

TS:   同 JS
来源：http://ib.haigaiapp.cn

Java: 方法内为块级作用域
来源：http://zz.bjjhwx.cn

Go:   花括号块级作用域
来源：http://td.panjiajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sz.szsharing.cn

C#:   块级作用域
来源：http://dl.lnxyls.cn

[C11] 模块导入与导出
来源：http://cg.bookmarksfly.cn

Py:   from module import func
来源：http://mm.newstarts.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://va.hnjuh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kg.chemitech.net.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qk.huixiangedu.cn

Java: import java.util.List;
来源：http://su.jianghongdianzi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jk.jctech888.com.cn

Ruby: require "json"; require_relative "./util"
来源：http://ab.bookmarksfly.cn

C#:   using System.Text;
来源：http://pm.asd995.cn

[C12] 立即执行函数 IIFE
来源：http://yq.hnjuh.cn

Py:   (lambda: print("run"))()
来源：http://pu.szxytkj.cn

PHP:  (function () { echo "run"; })();
来源：http://ix.shxzukj.cn

JS:   (() => { console.log("run"); })();
来源：http://ed.shxzukj.cn

TS:   (() => { console.log("run"); })();
来源：http://qz.bjjhwx.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cy.chemitech.net.cn

Go:   func() { fmt.Println("run") }()
来源：http://om.panjiajie.cn

Ruby: -> { puts "run" }.call
来源：http://ck.colortex.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gh.hahajie.cn

[C13] 类型声明 / 类型注解
来源：http://ne.gzmigu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sw.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zg.muxihuayi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cm.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yf.521024.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tq.wgjwhj.cn

Go:   func add(a, b int) int
来源：http://yt.haigaiapp.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jg.szsharing.cn

C#:   int Add(int a, int b) => a + b;
来源：http://hm.jianghongdianzi.cn

[C14] 泛型函数
来源：http://ha.shxzskj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ib.huixinmuqiang.cn

PHP:  // 无泛型
来源：http://rd.hnjuh.cn

JS:   // 无泛型
来源：http://vd.asd995.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sz.szxytkj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cr.panjiajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dc.521024.cn

Ruby: # 无泛型
来源：http://oz.lnxyls.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dv.nicolike.cn

[C15] 解构 / 展开参数
来源：http://uk.muxihuayi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ne.haigaiapp.cn

PHP:  [$a, $b] = $pair;
来源：http://dw.newstarts.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://oo.panjiajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yt.bookmarksfly.cn

Java: // 无解构
来源：http://un.jctech888.com.cn

Go:   // 无解构
来源：http://lw.chemitech.net.cn

Ruby: a, b = pair
来源：http://jv.nicolike.cn

C#:   var (a, b) = pair;
来源：http://uo.panjiajie.cn

[C16] 函数 / 方法重载
来源：http://pz.huanxung.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mj.chemitech.net.cn


<!-- 参考信息 -->