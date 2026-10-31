代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://pa.bjjhwx.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kp.szsharing.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ju.huixinmuqiang.cn

[A25] 字符串比较
来源：http://ud.haigaiapp.cn

Py:   s1 == s2; s1 != s2
来源：http://ka.asd995.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://yc.shxzukj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://uh.bookmarksfly.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hi.huanxung.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ys.szsharing.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wj.wgjwhj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ux.newstarts.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ej.9csxet.cn

[A26] 类型转换总览
来源：http://tq.colortex.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xi.bjjhwx.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://nk.shxzskj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tf.nszjky.cn

TS:   Number() String() Boolean() x as number
来源：http://pt.bjjhwx.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rn.nszjky.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yb.huanxung.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zx.colortex.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gn.hnjuh.cn

================================================================================
来源：http://fg.chemitech.net.cn

B. 流程控制
来源：http://rq.huanxung.cn

================================================================================
来源：http://ks.newstarts.cn

[B01] 条件判断 if / else
来源：http://lt.huanxung.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hf.shxzukj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kz.jianghongdianzi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rg.panjiajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sm.shxzukj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://mu.hnjuh.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ws.nszjky.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nf.hnjuh.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wp.huixinmuqiang.cn

[B02] 多分支 else if / elif
来源：http://gi.huixinmuqiang.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wp.szsharing.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ck.szsharing.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rn.521024.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gz.szsharing.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://at.shxzskj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ft.jianghongdianzi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mm.colortex.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tk.panjiajie.cn

[B03] switch / match / case
来源：http://pc.shxzukj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xh.bookmarksfly.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nz.asd995.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xw.shtwfgs.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ng.huixinmuqiang.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cb.gzmigu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ko.shtwfgs.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://if.lnxyls.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ti.yuntaijiaju.cn

[B04] for 计数循环
来源：http://uf.jianghongdianzi.cn

Py:   for i in range(10): print(i)
来源：http://zk.jctech888.com.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sg.521024.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xv.shxzukj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tm.jianghongdianzi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ja.hahajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bn.wgjwhj.cn

Ruby: 10.times { |i| puts i }
来源：http://bf.lnxyls.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kw.colortex.cn

[B05] 遍历数组 / 列表
来源：http://dq.muxihuayi.cn

Py:   for item in arr: print(item)
来源：http://tz.hnjuh.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sj.yuexingan06.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ok.szsharing.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://wg.wgjwhj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://al.szxytkj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gb.colortex.cn

Ruby: arr.each { |item| puts item }
来源：http://aa.huixiangedu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ko.huixiangedu.cn

[B06] 遍历字典 / 对象
来源：http://ym.huanxung.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ma.huixiangedu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lo.bjjhwx.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hp.asd995.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rj.bjjhwx.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jn.wgjwhj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ih.szsharing.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://df.hnjuh.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ne.shxzskj.cn

[B07] while 循环
来源：http://qq.newstarts.cn

Py:   while i < 10: i += 1
来源：http://tw.521024.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xh.yuexingan06.cn

JS:   while (i < 10) { i++; }
来源：http://se.shtwfgs.cn

TS:   while (i < 10) { i++; }
来源：http://fi.bjjhwx.cn

Java: while (i < 10) { i++; }
来源：http://bf.huanxung.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dy.szsharing.cn

Ruby: while i < 10; i += 1; end
来源：http://ho.hahajie.cn

C#:   while (i < 10) { i++; }
来源：http://cz.chemitech.net.cn

[B08] do-while（至少执行一次）
来源：http://ig.yuntaijiaju.cn

Py:   # 无 do-while：用 while True + break
来源：http://mo.nszjky.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xx.asd995.cn

JS:   do { i++; } while (i < 10);
来源：http://ce.panjiajie.cn

TS:   do { i++; } while (i < 10);
来源：http://wn.jianghongdianzi.cn

Java: do { i++; } while (i < 10);
来源：http://ya.huixinmuqiang.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ak.yuntaijiaju.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mx.hahajie.cn

C#:   do { i++; } while (i < 10);
来源：http://fh.shtwfgs.cn

[B09] break 与 continue
来源：http://cr.chemitech.net.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kj.hnjuh.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cm.newstarts.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xl.wgjwhj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ob.huixinmuqiang.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jt.szxytkj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ov.bjjhwx.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ab.yuntaijiaju.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uo.shtwfgs.cn

[B10] 遍历同时拿索引
来源：http://wf.szsharing.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sm.lnxyls.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tg.muxihuayi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pv.newstarts.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zc.bjjhwx.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jl.huanxung.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ap.colortex.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sj.bookmarksfly.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nq.huanxung.cn

[B11] 生成数字序列 / 区间
来源：http://es.shtwfgs.cn

Py:   list(range(0, 10, 2))
来源：http://ik.szsharing.cn

PHP:  range(0, 10, 2);
来源：http://nl.szxytkj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gc.lnxyls.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ki.hahajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uu.asd995.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://uf.521024.cn

Ruby: (0...10).step(2).to_a
来源：http://jq.bookmarksfly.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://et.yuexingan06.cn

[B12] 跳出多层循环
来源：http://sm.shxzukj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://qn.asd995.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://qt.shxzskj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ri.shxzskj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://be.huanxung.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hd.shxzskj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ia.panjiajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sf.haigaiapp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lx.huixiangedu.cn

[B13] 判断是否为数字
来源：http://bq.szxytkj.cn

Py:   isinstance(x, (int, float))
来源：http://fc.lnxyls.cn

PHP:  is_numeric($x)
来源：http://xp.haigaiapp.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xl.521024.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yi.hahajie.cn

Java: x instanceof Number
来源：http://yz.bookmarksfly.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sc.521024.cn

Ruby: x.is_a?(Numeric)
来源：http://bg.asd995.cn

C#:   x is int or double or decimal
来源：http://el.wgjwhj.cn

[B14] 判断值是否在集合内
来源：http://yq.asd995.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hw.bjjhwx.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xh.bookmarksfly.cn

JS:   [1, 2, 3].includes(x)
来源：http://fm.lnxyls.cn

TS:   [1, 2, 3].includes(x)
来源：http://zi.gzmigu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ra.yuexingan06.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ad.muxihuayi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ny.9csxet.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ht.asd995.cn

[B15] 布尔运算与取反
来源：http://vr.wgjwhj.cn

Py:   a and b or not c
来源：http://sv.haigaiapp.cn

PHP:  $a && $b || !$c
来源：http://wl.hnjuh.cn

JS:   a && b || !c
来源：http://vh.wgjwhj.cn

TS:   a && b || !c
来源：http://hn.szsharing.cn

Java: a && b || !c
来源：http://qi.shxzskj.cn

Go:   a && b || !c
来源：http://jw.bjjhwx.cn

Ruby: a && b || !c
来源：http://hz.hahajie.cn

C#:   a && b || !c
来源：http://em.jctech888.com.cn

[B16] 卫语句：不满足条件提前返回
来源：http://on.newstarts.cn

Py:   if not data: return
来源：http://ta.muxihuayi.cn

PHP:  if (!$data) { return; }
来源：http://tq.huanxung.cn

JS:   if (!data) return;
来源：http://px.hahajie.cn

TS:   if (!data) return;
来源：http://bh.shtwfgs.cn

Java: if (data == null) return;
来源：http://zu.asd995.cn

Go:   if data == nil { return }
来源：http://po.wgjwhj.cn

Ruby: return if data.nil?
来源：http://cx.nszjky.cn

C#:   if (data == null) return;
来源：http://lw.haigaiapp.cn

================================================================================
来源：http://dq.muxihuayi.cn

C. 函数与作用域
来源：http://fk.wgjwhj.cn

================================================================================
来源：http://mt.huanxung.cn

[C01] 定义函数
来源：http://qg.jianghongdianzi.cn

Py:   def add(a, b): return a + b
来源：http://vt.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jz.chemitech.net.cn

JS:   function add(a, b) { return a + b; }
来源：http://gv.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qs.yuexingan06.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fa.huixinmuqiang.cn

Go:   func add(a, b int) int { return a + b }
来源：http://yl.nicolike.cn

Ruby: def add(a, b); a + b; end
来源：http://tz.haigaiapp.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uq.szxytkj.cn

[C02] 默认参数
来源：http://ef.yuexingan06.cn

Py:   def greet(name="World"): return name
来源：http://ux.szsharing.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wg.jianghongdianzi.cn

JS:   function greet(name = "World") { return name; }
来源：http://rw.nicolike.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fi.huanxung.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://be.shxzukj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mh.szsharing.cn

Ruby: def greet(name = "World") = name
来源：http://cz.chemitech.net.cn

C#:   string Greet(string name = "World") => name;
来源：http://xy.521024.cn

[C03] 可变参数
来源：http://wu.bjjhwx.cn

Py:   def total(*args): return sum(args)
来源：http://cd.muxihuayi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xm.hahajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ec.jctech888.com.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wd.chemitech.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ri.muxihuayi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cy.gzmigu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wh.huanxung.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://db.asd995.cn

[C04] 命名参数 / 关键字参数
来源：http://mi.9csxet.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://iq.colortex.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kz.gzmigu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://or.hnjuh.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jx.hnjuh.cn

Java: // 无：用 Builder 模式或 record
来源：http://ir.jctech888.com.cn

Go:   // 无：用配置结构体参数
来源：http://lm.jianghongdianzi.cn

Ruby: f(a: 1, b: 2)
来源：http://ra.shxzukj.cn

C#:   f(a: 1, b: 2)
来源：http://my.hahajie.cn

[C05] 返回多个值
来源：http://kt.jctech888.com.cn

Py:   return a, b
来源：http://xb.yuexingan06.cn

PHP:  return [$a, $b];
来源：http://be.huixiangedu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zq.panjiajie.cn

TS:   return { a, b };
来源：http://bu.jianghongdianzi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kg.bookmarksfly.cn

Go:   return a, b
来源：http://fc.gzmigu.cn

Ruby: return a, b
来源：http://if.huixinmuqiang.cn

C#:   return (a, b);              // ValueTuple
来源：http://rw.jctech888.com.cn

[C06] 匿名函数 / lambda
来源：http://fd.shxzukj.cn

Py:   square = lambda x: x * x
来源：http://lf.newstarts.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wz.panjiajie.cn

JS:   const square = x => x * x;
来源：http://vp.colortex.cn

TS:   const square = (x: number): number => x * x;
来源：http://os.haigaiapp.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ad.hnjuh.cn

Go:   sq := func(x int) int { return x * x }
来源：http://do.bookmarksfly.cn

Ruby: square = ->(x) { x * x }
来源：http://ki.szsharing.cn

C#:   Func<int, int> square = x => x * x;
来源：http://oa.huixiangedu.cn

[C07] 把函数作为参数传入
来源：http://be.muxihuayi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dd.newstarts.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wj.wgjwhj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qb.yuntaijiaju.cn

TS:   arr.map(String)
来源：http://rl.colortex.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ax.huixiangedu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ao.huanxung.cn

Ruby: arr.map(&:upcase)
来源：http://xh.hahajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://nk.asd995.cn

[C08] 闭包
来源：http://df.9csxet.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fh.shxzukj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xw.colortex.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ro.wgjwhj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nq.bjjhwx.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gm.huanxung.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nj.hnjuh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zt.newstarts.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://to.shxzukj.cn

[C09] 递归
来源：http://zt.yuntaijiaju.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://eb.huixiangedu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lw.bookmarksfly.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ml.lnxyls.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://io.huixiangedu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yt.bookmarksfly.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zk.jianghongdianzi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nd.colortex.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uj.shtwfgs.cn

[C10] 变量作用域
来源：http://xw.hnjuh.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ls.newstarts.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ou.yuntaijiaju.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ex.9csxet.cn

TS:   同 JS
来源：http://qw.panjiajie.cn

Java: 方法内为块级作用域
来源：http://nz.jianghongdianzi.cn

Go:   花括号块级作用域
来源：http://uu.newstarts.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fp.newstarts.cn

C#:   块级作用域
来源：http://cq.szxytkj.cn

[C11] 模块导入与导出
来源：http://wp.bjjhwx.cn

Py:   from module import func
来源：http://bd.gzmigu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hu.gzmigu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://an.shxzskj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hx.muxihuayi.cn

Java: import java.util.List;
来源：http://en.yuntaijiaju.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dg.gzmigu.cn

Ruby: require "json"; require_relative "./util"
来源：http://sj.colortex.cn

C#:   using System.Text;
来源：http://da.szxytkj.cn

[C12] 立即执行函数 IIFE
来源：http://nl.nicolike.cn

Py:   (lambda: print("run"))()
来源：http://ip.szsharing.cn

PHP:  (function () { echo "run"; })();
来源：http://xl.jianghongdianzi.cn

JS:   (() => { console.log("run"); })();
来源：http://ke.huixiangedu.cn

TS:   (() => { console.log("run"); })();
来源：http://pd.jctech888.com.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xl.yuexingan06.cn

Go:   func() { fmt.Println("run") }()
来源：http://yb.colortex.cn

Ruby: -> { puts "run" }.call
来源：http://iz.szsharing.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ko.yuexingan06.cn

[C13] 类型声明 / 类型注解
来源：http://mw.szxytkj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dw.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sx.bjjhwx.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://je.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ha.9csxet.cn

Java: int add(int a, int b) { return a + b; }
来源：http://va.yuntaijiaju.cn

Go:   func add(a, b int) int
来源：http://sh.haigaiapp.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ur.newstarts.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wc.shtwfgs.cn

[C14] 泛型函数
来源：http://vu.521024.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gm.huixinmuqiang.cn

PHP:  // 无泛型
来源：http://oz.jianghongdianzi.cn

JS:   // 无泛型
来源：http://ot.huanxung.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://aw.huixinmuqiang.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sj.jianghongdianzi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cj.shxzskj.cn

Ruby: # 无泛型
来源：http://cl.shxzskj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ed.huixiangedu.cn

[C15] 解构 / 展开参数
来源：http://bt.gzmigu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vx.panjiajie.cn

PHP:  [$a, $b] = $pair;
来源：http://df.jianghongdianzi.cn


<!-- 参考信息 -->