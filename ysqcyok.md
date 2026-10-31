代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://cm.hnjuh.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zd.lnxyls.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hc.newstarts.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://is.shxzskj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rg.szsharing.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cm.bookmarksfly.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://oe.szsharing.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xm.panjiajie.cn

[A26] 类型转换总览
来源：http://ex.szsharing.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xj.newstarts.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ji.hnjuh.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kw.szxytkj.cn

TS:   Number() String() Boolean() x as number
来源：http://vj.nicolike.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gp.shxzukj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ao.szsharing.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://va.haigaiapp.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ov.yuntaijiaju.cn

================================================================================
来源：http://rp.huixinmuqiang.cn

B. 流程控制
来源：http://ji.panjiajie.cn

================================================================================
来源：http://uz.shtwfgs.cn

[B01] 条件判断 if / else
来源：http://rd.shxzskj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dp.muxihuayi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ge.nszjky.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tg.hnjuh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gv.huanxung.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://hb.shxzukj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cl.jianghongdianzi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qc.shtwfgs.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nq.jctech888.com.cn

[B02] 多分支 else if / elif
来源：http://af.colortex.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ny.521024.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ut.shtwfgs.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sg.huanxung.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rh.shtwfgs.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hn.nicolike.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://sm.shxzukj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hu.huixiangedu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wq.huanxung.cn

[B03] switch / match / case
来源：http://to.colortex.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ht.asd995.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zw.jctech888.com.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xn.gzmigu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hd.huanxung.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sv.bjjhwx.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wg.yuexingan06.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://oh.bookmarksfly.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://oo.newstarts.cn

[B04] for 计数循环
来源：http://jh.huanxung.cn

Py:   for i in range(10): print(i)
来源：http://qq.wgjwhj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://at.shtwfgs.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ur.shxzukj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ch.jctech888.com.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tl.shtwfgs.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lt.colortex.cn

Ruby: 10.times { |i| puts i }
来源：http://ts.newstarts.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pk.gzmigu.cn

[B05] 遍历数组 / 列表
来源：http://bv.wgjwhj.cn

Py:   for item in arr: print(item)
来源：http://ye.gzmigu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ls.shtwfgs.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ds.nicolike.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fn.chemitech.net.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://rb.haigaiapp.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cy.colortex.cn

Ruby: arr.each { |item| puts item }
来源：http://fe.wgjwhj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wk.huanxung.cn

[B06] 遍历字典 / 对象
来源：http://nq.newstarts.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ll.muxihuayi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jw.jctech888.com.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ou.szxytkj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dz.9csxet.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yu.jctech888.com.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bs.nszjky.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ir.muxihuayi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dz.szxytkj.cn

[B07] while 循环
来源：http://jz.wgjwhj.cn

Py:   while i < 10: i += 1
来源：http://zx.jctech888.com.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ml.jctech888.com.cn

JS:   while (i < 10) { i++; }
来源：http://dt.szxytkj.cn

TS:   while (i < 10) { i++; }
来源：http://wp.huanxung.cn

Java: while (i < 10) { i++; }
来源：http://iz.nszjky.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ll.colortex.cn

Ruby: while i < 10; i += 1; end
来源：http://ig.shxzskj.cn

C#:   while (i < 10) { i++; }
来源：http://sb.szsharing.cn

[B08] do-while（至少执行一次）
来源：http://hw.szsharing.cn

Py:   # 无 do-while：用 while True + break
来源：http://nr.muxihuayi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://kd.shxzskj.cn

JS:   do { i++; } while (i < 10);
来源：http://wo.yuexingan06.cn

TS:   do { i++; } while (i < 10);
来源：http://ws.bookmarksfly.cn

Java: do { i++; } while (i < 10);
来源：http://vw.521024.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xw.huanxung.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rf.shtwfgs.cn

C#:   do { i++; } while (i < 10);
来源：http://rk.yuexingan06.cn

[B09] break 与 continue
来源：http://tc.gzmigu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://np.hahajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fu.jctech888.com.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ww.shtwfgs.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tw.szxytkj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vy.shxzukj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lf.521024.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yt.jianghongdianzi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xj.szxytkj.cn

[B10] 遍历同时拿索引
来源：http://mi.muxihuayi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ny.hahajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ud.jianghongdianzi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://om.shtwfgs.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://af.szsharing.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kl.newstarts.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xk.hahajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jb.huixiangedu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qq.haigaiapp.cn

[B11] 生成数字序列 / 区间
来源：http://zw.lnxyls.cn

Py:   list(range(0, 10, 2))
来源：http://qc.bjjhwx.cn

PHP:  range(0, 10, 2);
来源：http://os.hnjuh.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ew.hahajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hw.shxzskj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://df.hnjuh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ga.9csxet.cn

Ruby: (0...10).step(2).to_a
来源：http://lx.yuntaijiaju.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ac.nicolike.cn

[B12] 跳出多层循环
来源：http://fq.huanxung.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ae.chemitech.net.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://qc.nszjky.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://oc.panjiajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gl.9csxet.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ul.nszjky.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uu.huanxung.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://si.9csxet.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mu.wgjwhj.cn

[B13] 判断是否为数字
来源：http://cg.jianghongdianzi.cn

Py:   isinstance(x, (int, float))
来源：http://yj.hnjuh.cn

PHP:  is_numeric($x)
来源：http://vh.szxytkj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ep.jctech888.com.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rv.wgjwhj.cn

Java: x instanceof Number
来源：http://ok.wgjwhj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mq.muxihuayi.cn

Ruby: x.is_a?(Numeric)
来源：http://gn.newstarts.cn

C#:   x is int or double or decimal
来源：http://pb.huixinmuqiang.cn

[B14] 判断值是否在集合内
来源：http://lk.hahajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yw.gzmigu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ld.muxihuayi.cn

JS:   [1, 2, 3].includes(x)
来源：http://zg.panjiajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://yl.colortex.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ns.huixiangedu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://id.nszjky.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ji.yuexingan06.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pq.shxzukj.cn

[B15] 布尔运算与取反
来源：http://gh.shtwfgs.cn

Py:   a and b or not c
来源：http://ly.hahajie.cn

PHP:  $a && $b || !$c
来源：http://nz.huixiangedu.cn

JS:   a && b || !c
来源：http://xi.shxzukj.cn

TS:   a && b || !c
来源：http://do.jctech888.com.cn

Java: a && b || !c
来源：http://pq.szxytkj.cn

Go:   a && b || !c
来源：http://fk.shtwfgs.cn

Ruby: a && b || !c
来源：http://tq.huixinmuqiang.cn

C#:   a && b || !c
来源：http://xd.shxzukj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gn.hahajie.cn

Py:   if not data: return
来源：http://vv.haigaiapp.cn

PHP:  if (!$data) { return; }
来源：http://yd.lnxyls.cn

JS:   if (!data) return;
来源：http://wv.newstarts.cn

TS:   if (!data) return;
来源：http://uc.shtwfgs.cn

Java: if (data == null) return;
来源：http://yo.gzmigu.cn

Go:   if data == nil { return }
来源：http://og.panjiajie.cn

Ruby: return if data.nil?
来源：http://rb.nicolike.cn

C#:   if (data == null) return;
来源：http://cf.shtwfgs.cn

================================================================================
来源：http://ni.bjjhwx.cn

C. 函数与作用域
来源：http://cq.9csxet.cn

================================================================================
来源：http://hh.nicolike.cn

[C01] 定义函数
来源：http://lw.gzmigu.cn

Py:   def add(a, b): return a + b
来源：http://wc.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yi.jctech888.com.cn

JS:   function add(a, b) { return a + b; }
来源：http://bv.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fh.bjjhwx.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lf.huixiangedu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jm.521024.cn

Ruby: def add(a, b); a + b; end
来源：http://sa.bjjhwx.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tw.szsharing.cn

[C02] 默认参数
来源：http://mk.gzmigu.cn

Py:   def greet(name="World"): return name
来源：http://hl.521024.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://gq.nszjky.cn

JS:   function greet(name = "World") { return name; }
来源：http://kq.bookmarksfly.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ya.shtwfgs.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hk.asd995.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ee.haigaiapp.cn

Ruby: def greet(name = "World") = name
来源：http://bg.muxihuayi.cn

C#:   string Greet(string name = "World") => name;
来源：http://bj.huixiangedu.cn

[C03] 可变参数
来源：http://et.9csxet.cn

Py:   def total(*args): return sum(args)
来源：http://my.huanxung.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jr.jianghongdianzi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ls.shxzskj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zc.chemitech.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qv.szxytkj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sy.wgjwhj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gb.huanxung.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fi.chemitech.net.cn

[C04] 命名参数 / 关键字参数
来源：http://xn.shtwfgs.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cs.huixinmuqiang.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bu.yuntaijiaju.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cu.nszjky.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://st.szsharing.cn

Java: // 无：用 Builder 模式或 record
来源：http://qn.bookmarksfly.cn

Go:   // 无：用配置结构体参数
来源：http://nc.wgjwhj.cn

Ruby: f(a: 1, b: 2)
来源：http://cj.bookmarksfly.cn

C#:   f(a: 1, b: 2)
来源：http://io.yuexingan06.cn

[C05] 返回多个值
来源：http://oz.panjiajie.cn

Py:   return a, b
来源：http://az.nicolike.cn

PHP:  return [$a, $b];
来源：http://if.huixiangedu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fs.jianghongdianzi.cn

TS:   return { a, b };
来源：http://pw.yuexingan06.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hi.szxytkj.cn

Go:   return a, b
来源：http://xc.szsharing.cn

Ruby: return a, b
来源：http://rr.asd995.cn

C#:   return (a, b);              // ValueTuple
来源：http://qh.huixiangedu.cn

[C06] 匿名函数 / lambda
来源：http://ay.hahajie.cn

Py:   square = lambda x: x * x
来源：http://tp.jctech888.com.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://us.panjiajie.cn

JS:   const square = x => x * x;
来源：http://qq.shtwfgs.cn

TS:   const square = (x: number): number => x * x;
来源：http://er.asd995.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fc.huixiangedu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://od.wgjwhj.cn

Ruby: square = ->(x) { x * x }
来源：http://qx.asd995.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ys.huixiangedu.cn

[C07] 把函数作为参数传入
来源：http://jq.jctech888.com.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kl.chemitech.net.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bu.asd995.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zv.hahajie.cn

TS:   arr.map(String)
来源：http://oh.asd995.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rl.huanxung.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ea.yuexingan06.cn

Ruby: arr.map(&:upcase)
来源：http://ay.huixiangedu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://us.huixiangedu.cn

[C08] 闭包
来源：http://xy.haigaiapp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ox.bookmarksfly.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dr.szxytkj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tc.nszjky.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xa.jianghongdianzi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tm.huanxung.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dm.nicolike.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lv.lnxyls.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kx.huixiangedu.cn

[C09] 递归
来源：http://up.huixinmuqiang.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vj.huixinmuqiang.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ib.shxzskj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ub.nicolike.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://om.muxihuayi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nw.bookmarksfly.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hl.9csxet.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cc.huixinmuqiang.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wo.colortex.cn

[C10] 变量作用域
来源：http://qy.muxihuayi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ee.panjiajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ir.bookmarksfly.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://aj.nszjky.cn

TS:   同 JS
来源：http://ks.9csxet.cn

Java: 方法内为块级作用域
来源：http://wt.lnxyls.cn

Go:   花括号块级作用域
来源：http://lw.shxzskj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xn.shxzukj.cn

C#:   块级作用域
来源：http://ax.hnjuh.cn

[C11] 模块导入与导出
来源：http://pw.lnxyls.cn

Py:   from module import func
来源：http://dl.hnjuh.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://re.jianghongdianzi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://dl.9csxet.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nq.jctech888.com.cn

Java: import java.util.List;
来源：http://pk.shxzskj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://px.chemitech.net.cn

Ruby: require "json"; require_relative "./util"
来源：http://vp.9csxet.cn

C#:   using System.Text;
来源：http://ih.9csxet.cn

[C12] 立即执行函数 IIFE
来源：http://bp.colortex.cn

Py:   (lambda: print("run"))()
来源：http://wu.colortex.cn

PHP:  (function () { echo "run"; })();
来源：http://ds.hahajie.cn

JS:   (() => { console.log("run"); })();
来源：http://ou.haigaiapp.cn

TS:   (() => { console.log("run"); })();
来源：http://dm.huanxung.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pp.hnjuh.cn

Go:   func() { fmt.Println("run") }()
来源：http://mb.nicolike.cn

Ruby: -> { puts "run" }.call
来源：http://wv.jctech888.com.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://km.nszjky.cn

[C13] 类型声明 / 类型注解
来源：http://xx.shxzskj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sd.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ul.hahajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tr.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mf.chemitech.net.cn

Java: int add(int a, int b) { return a + b; }
来源：http://nv.yuexingan06.cn

Go:   func add(a, b int) int
来源：http://wq.bjjhwx.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://de.shxzskj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qt.szsharing.cn

[C14] 泛型函数
来源：http://os.colortex.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://at.shtwfgs.cn

PHP:  // 无泛型
来源：http://xl.haigaiapp.cn

JS:   // 无泛型
来源：http://pw.521024.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gh.9csxet.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rb.yuexingan06.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lb.muxihuayi.cn

Ruby: # 无泛型
来源：http://rh.huixiangedu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pk.jctech888.com.cn

[C15] 解构 / 展开参数
来源：http://yr.shxzukj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jt.nszjky.cn

PHP:  [$a, $b] = $pair;
来源：http://tu.huixinmuqiang.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fc.szxytkj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kb.huixinmuqiang.cn

Java: // 无解构
来源：http://st.shxzskj.cn

Go:   // 无解构
来源：http://mm.lnxyls.cn


<!-- 参考信息 -->