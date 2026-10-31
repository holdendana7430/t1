代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bc.yuntaijiaju.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sf.bookmarksfly.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sf.hnjuh.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cv.hahajie.cn

Go:   strings.TrimSpace(s)
来源：http://ic.muxihuayi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ra.hnjuh.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jj.huixinmuqiang.cn

[A25] 字符串比较
来源：http://fc.jianghongdianzi.cn

Py:   s1 == s2; s1 != s2
来源：http://dm.haigaiapp.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gx.jctech888.com.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lv.chemitech.net.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nx.lnxyls.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://le.chemitech.net.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fj.521024.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://gp.bookmarksfly.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hl.521024.cn

[A26] 类型转换总览
来源：http://ju.bjjhwx.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fn.gzmigu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pe.shxzukj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rk.newstarts.cn

TS:   Number() String() Boolean() x as number
来源：http://ui.muxihuayi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://od.szxytkj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wq.nszjky.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://sh.szxytkj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vm.haigaiapp.cn

================================================================================
来源：http://ni.bookmarksfly.cn

B. 流程控制
来源：http://qo.huixiangedu.cn

================================================================================
来源：http://sg.nicolike.cn

[B01] 条件判断 if / else
来源：http://fv.yuntaijiaju.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://tr.colortex.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xx.bookmarksfly.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gu.hahajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pe.gzmigu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ru.chemitech.net.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xx.chemitech.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://as.szxytkj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qm.yuntaijiaju.cn

[B02] 多分支 else if / elif
来源：http://tr.chemitech.net.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://if.huixiangedu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://iq.colortex.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mt.panjiajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qy.shtwfgs.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lf.chemitech.net.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bh.yuntaijiaju.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ku.chemitech.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ea.newstarts.cn

[B03] switch / match / case
来源：http://fm.shtwfgs.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yx.yuexingan06.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://oo.newstarts.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://he.shxzukj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ui.yuexingan06.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://yd.haigaiapp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://er.gzmigu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wn.szxytkj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gg.bjjhwx.cn

[B04] for 计数循环
来源：http://im.jianghongdianzi.cn

Py:   for i in range(10): print(i)
来源：http://qd.nicolike.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wt.haigaiapp.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://id.521024.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dh.hnjuh.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://eg.huixinmuqiang.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ga.bjjhwx.cn

Ruby: 10.times { |i| puts i }
来源：http://vv.shxzukj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ld.bjjhwx.cn

[B05] 遍历数组 / 列表
来源：http://uc.szxytkj.cn

Py:   for item in arr: print(item)
来源：http://tm.9csxet.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vb.521024.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://cg.bjjhwx.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xy.colortex.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fh.huanxung.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://us.nicolike.cn

Ruby: arr.each { |item| puts item }
来源：http://bu.shxzukj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ym.haigaiapp.cn

[B06] 遍历字典 / 对象
来源：http://hp.shxzskj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zn.hnjuh.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uk.hahajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iq.lnxyls.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://by.newstarts.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ax.521024.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mb.gzmigu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ho.nszjky.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://os.nicolike.cn

[B07] while 循环
来源：http://ep.bjjhwx.cn

Py:   while i < 10: i += 1
来源：http://wu.bookmarksfly.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bz.nszjky.cn

JS:   while (i < 10) { i++; }
来源：http://wx.newstarts.cn

TS:   while (i < 10) { i++; }
来源：http://pd.chemitech.net.cn

Java: while (i < 10) { i++; }
来源：http://nh.szsharing.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nx.muxihuayi.cn

Ruby: while i < 10; i += 1; end
来源：http://vp.colortex.cn

C#:   while (i < 10) { i++; }
来源：http://lb.yuntaijiaju.cn

[B08] do-while（至少执行一次）
来源：http://vo.gzmigu.cn

Py:   # 无 do-while：用 while True + break
来源：http://at.nszjky.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qo.shtwfgs.cn

JS:   do { i++; } while (i < 10);
来源：http://sq.wgjwhj.cn

TS:   do { i++; } while (i < 10);
来源：http://gg.wgjwhj.cn

Java: do { i++; } while (i < 10);
来源：http://eg.wgjwhj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vq.szxytkj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fr.shxzukj.cn

C#:   do { i++; } while (i < 10);
来源：http://jn.szsharing.cn

[B09] break 与 continue
来源：http://bl.shxzukj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mt.asd995.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nm.hnjuh.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cg.hahajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cl.shtwfgs.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wh.newstarts.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ne.panjiajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tz.shxzskj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.521024.cn

[B10] 遍历同时拿索引
来源：http://zz.panjiajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vz.gzmigu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ud.huixinmuqiang.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jn.newstarts.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bj.bookmarksfly.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://si.wgjwhj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xg.yuntaijiaju.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jr.huixinmuqiang.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ff.shxzskj.cn

[B11] 生成数字序列 / 区间
来源：http://qn.asd995.cn

Py:   list(range(0, 10, 2))
来源：http://fi.shtwfgs.cn

PHP:  range(0, 10, 2);
来源：http://cu.newstarts.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mz.shtwfgs.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ff.bookmarksfly.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ue.9csxet.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://oc.szsharing.cn

Ruby: (0...10).step(2).to_a
来源：http://uc.huixiangedu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fz.hahajie.cn

[B12] 跳出多层循环
来源：http://xb.shxzukj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://nu.jianghongdianzi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hr.huixiangedu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://je.wgjwhj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ft.wgjwhj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ap.colortex.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://aq.521024.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://oa.hnjuh.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yp.hnjuh.cn

[B13] 判断是否为数字
来源：http://tx.szsharing.cn

Py:   isinstance(x, (int, float))
来源：http://zl.521024.cn

PHP:  is_numeric($x)
来源：http://xg.hahajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uq.hahajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lh.szsharing.cn

Java: x instanceof Number
来源：http://rk.yuntaijiaju.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xa.huixinmuqiang.cn

Ruby: x.is_a?(Numeric)
来源：http://fe.huixiangedu.cn

C#:   x is int or double or decimal
来源：http://yd.huanxung.cn

[B14] 判断值是否在集合内
来源：http://vn.panjiajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://df.jianghongdianzi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jz.hahajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://ep.chemitech.net.cn

TS:   [1, 2, 3].includes(x)
来源：http://yy.jianghongdianzi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://tu.nszjky.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qq.yuntaijiaju.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gq.nicolike.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ij.nszjky.cn

[B15] 布尔运算与取反
来源：http://aa.muxihuayi.cn

Py:   a and b or not c
来源：http://qj.colortex.cn

PHP:  $a && $b || !$c
来源：http://hc.gzmigu.cn

JS:   a && b || !c
来源：http://ae.nszjky.cn

TS:   a && b || !c
来源：http://vp.huixiangedu.cn

Java: a && b || !c
来源：http://fk.asd995.cn

Go:   a && b || !c
来源：http://mo.yuexingan06.cn

Ruby: a && b || !c
来源：http://ar.bjjhwx.cn

C#:   a && b || !c
来源：http://ct.nicolike.cn

[B16] 卫语句：不满足条件提前返回
来源：http://pz.huanxung.cn

Py:   if not data: return
来源：http://eo.panjiajie.cn

PHP:  if (!$data) { return; }
来源：http://zl.szsharing.cn

JS:   if (!data) return;
来源：http://sk.muxihuayi.cn

TS:   if (!data) return;
来源：http://bi.jianghongdianzi.cn

Java: if (data == null) return;
来源：http://gn.newstarts.cn

Go:   if data == nil { return }
来源：http://uv.yuexingan06.cn

Ruby: return if data.nil?
来源：http://qa.yuntaijiaju.cn

C#:   if (data == null) return;
来源：http://bf.asd995.cn

================================================================================
来源：http://bd.jianghongdianzi.cn

C. 函数与作用域
来源：http://au.yuexingan06.cn

================================================================================
来源：http://mv.bjjhwx.cn

[C01] 定义函数
来源：http://hy.shxzukj.cn

Py:   def add(a, b): return a + b
来源：http://ux.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rt.9csxet.cn

JS:   function add(a, b) { return a + b; }
来源：http://xk.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gw.bookmarksfly.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://pj.shxzskj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://wx.asd995.cn

Ruby: def add(a, b); a + b; end
来源：http://rq.nicolike.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pz.panjiajie.cn

[C02] 默认参数
来源：http://lz.huanxung.cn

Py:   def greet(name="World"): return name
来源：http://hk.shtwfgs.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hv.gzmigu.cn

JS:   function greet(name = "World") { return name; }
来源：http://fr.hahajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ru.panjiajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ux.wgjwhj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://he.nicolike.cn

Ruby: def greet(name = "World") = name
来源：http://lk.hahajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://uq.szsharing.cn

[C03] 可变参数
来源：http://oy.shxzskj.cn

Py:   def total(*args): return sum(args)
来源：http://ua.huixiangedu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vw.hahajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://td.9csxet.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xy.szsharing.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pn.huanxung.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yuexingan06.cn

Ruby: def total(*nums); nums.sum; end
来源：http://db.bookmarksfly.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mb.huixiangedu.cn

[C04] 命名参数 / 关键字参数
来源：http://ep.jianghongdianzi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uy.jianghongdianzi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kf.shxzskj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ip.jctech888.com.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wr.yuexingan06.cn

Java: // 无：用 Builder 模式或 record
来源：http://zl.bookmarksfly.cn

Go:   // 无：用配置结构体参数
来源：http://aq.jianghongdianzi.cn

Ruby: f(a: 1, b: 2)
来源：http://py.huixinmuqiang.cn

C#:   f(a: 1, b: 2)
来源：http://qp.newstarts.cn

[C05] 返回多个值
来源：http://ho.shtwfgs.cn

Py:   return a, b
来源：http://sb.huixiangedu.cn

PHP:  return [$a, $b];
来源：http://dc.wgjwhj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://if.szsharing.cn

TS:   return { a, b };
来源：http://ov.huanxung.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dd.panjiajie.cn

Go:   return a, b
来源：http://xm.asd995.cn

Ruby: return a, b
来源：http://ts.muxihuayi.cn

C#:   return (a, b);              // ValueTuple
来源：http://xf.shtwfgs.cn

[C06] 匿名函数 / lambda
来源：http://ki.gzmigu.cn

Py:   square = lambda x: x * x
来源：http://ed.9csxet.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://vt.shtwfgs.cn

JS:   const square = x => x * x;
来源：http://ig.newstarts.cn

TS:   const square = (x: number): number => x * x;
来源：http://ye.yuntaijiaju.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zz.huixinmuqiang.cn

Go:   sq := func(x int) int { return x * x }
来源：http://eb.shxzukj.cn

Ruby: square = ->(x) { x * x }
来源：http://jh.hahajie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://lk.szxytkj.cn

[C07] 把函数作为参数传入
来源：http://gl.521024.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rr.jianghongdianzi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kr.asd995.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wf.yuexingan06.cn

TS:   arr.map(String)
来源：http://fp.521024.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jj.wgjwhj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zd.haigaiapp.cn

Ruby: arr.map(&:upcase)
来源：http://bu.521024.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hx.chemitech.net.cn

[C08] 闭包
来源：http://po.bjjhwx.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rl.huixinmuqiang.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ye.muxihuayi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wu.shxzukj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mr.haigaiapp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mb.bookmarksfly.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://iu.nicolike.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://id.jctech888.com.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://eb.haigaiapp.cn

[C09] 递归
来源：http://hd.nicolike.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pn.shxzukj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bi.szsharing.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fx.chemitech.net.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sx.szsharing.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gs.shxzukj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ll.bjjhwx.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dx.yuntaijiaju.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://la.lnxyls.cn

[C10] 变量作用域
来源：http://hd.newstarts.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cf.gzmigu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pv.nszjky.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://le.muxihuayi.cn

TS:   同 JS
来源：http://be.shxzskj.cn

Java: 方法内为块级作用域
来源：http://rq.wgjwhj.cn

Go:   花括号块级作用域
来源：http://kr.chemitech.net.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nb.chemitech.net.cn

C#:   块级作用域
来源：http://gp.szxytkj.cn

[C11] 模块导入与导出
来源：http://sq.huanxung.cn

Py:   from module import func
来源：http://zy.9csxet.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bj.huixiangedu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qd.huixiangedu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ug.shtwfgs.cn

Java: import java.util.List;
来源：http://nu.asd995.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rs.hahajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://vq.bjjhwx.cn

C#:   using System.Text;
来源：http://rc.newstarts.cn

[C12] 立即执行函数 IIFE
来源：http://ow.huixiangedu.cn

Py:   (lambda: print("run"))()
来源：http://pr.yuntaijiaju.cn

PHP:  (function () { echo "run"; })();
来源：http://zt.panjiajie.cn

JS:   (() => { console.log("run"); })();
来源：http://mh.shxzukj.cn

TS:   (() => { console.log("run"); })();
来源：http://mu.shxzukj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kx.jctech888.com.cn

Go:   func() { fmt.Println("run") }()
来源：http://mz.yuexingan06.cn

Ruby: -> { puts "run" }.call
来源：http://nj.gzmigu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://sk.huanxung.cn

[C13] 类型声明 / 类型注解
来源：http://yz.panjiajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wa.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ti.haigaiapp.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://js.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://aq.yuntaijiaju.cn

Java: int add(int a, int b) { return a + b; }
来源：http://im.bjjhwx.cn

Go:   func add(a, b int) int
来源：http://ej.nicolike.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sp.nicolike.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ob.yuexingan06.cn

[C14] 泛型函数
来源：http://mv.yuntaijiaju.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ev.lnxyls.cn

PHP:  // 无泛型
来源：http://vw.huixiangedu.cn

JS:   // 无泛型
来源：http://hq.hahajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ya.yuntaijiaju.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ne.huixinmuqiang.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dy.521024.cn

Ruby: # 无泛型
来源：http://xt.colortex.cn


<!-- 参考信息 -->