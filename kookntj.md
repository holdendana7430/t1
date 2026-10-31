代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gi.huanxung.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://pc.shxzukj.cn

[A24] 去除首尾空白
来源：http://bz.panjiajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fw.haigaiapp.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qa.hnjuh.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vs.huixinmuqiang.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mi.szsharing.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vr.colortex.cn

Go:   strings.TrimSpace(s)
来源：http://pv.hahajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lt.newstarts.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pw.lnxyls.cn

[A25] 字符串比较
来源：http://yn.shxzukj.cn

Py:   s1 == s2; s1 != s2
来源：http://dc.lnxyls.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bc.jctech888.com.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qp.yuntaijiaju.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fs.huixinmuqiang.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ry.jianghongdianzi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jv.nicolike.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://py.hahajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://un.muxihuayi.cn

[A26] 类型转换总览
来源：http://ba.yuntaijiaju.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sb.szxytkj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://an.szxytkj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ve.huixinmuqiang.cn

TS:   Number() String() Boolean() x as number
来源：http://na.chemitech.net.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://st.gzmigu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xv.huixiangedu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ac.huixinmuqiang.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ta.szsharing.cn

================================================================================
来源：http://pq.shxzukj.cn

B. 流程控制
来源：http://hx.szsharing.cn

================================================================================
来源：http://uc.huixinmuqiang.cn

[B01] 条件判断 if / else
来源：http://yy.szxytkj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://yn.panjiajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://as.huanxung.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jk.bookmarksfly.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sa.nszjky.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vu.newstarts.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://in.nszjky.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mv.jctech888.com.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ph.huanxung.cn

[B02] 多分支 else if / elif
来源：http://vi.huixinmuqiang.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ac.lnxyls.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://an.nszjky.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ck.jianghongdianzi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wf.haigaiapp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nm.colortex.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ey.jctech888.com.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xt.shxzskj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vf.shtwfgs.cn

[B03] switch / match / case
来源：http://mq.szsharing.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sg.9csxet.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xi.newstarts.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ab.yuntaijiaju.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fw.shxzskj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fh.521024.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wl.chemitech.net.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fh.nszjky.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mb.hnjuh.cn

[B04] for 计数循环
来源：http://ej.nicolike.cn

Py:   for i in range(10): print(i)
来源：http://xg.hahajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pt.wgjwhj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ce.szxytkj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://if.hahajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mx.szsharing.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wi.panjiajie.cn

Ruby: 10.times { |i| puts i }
来源：http://it.nicolike.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cn.szxytkj.cn

[B05] 遍历数组 / 列表
来源：http://ox.521024.cn

Py:   for item in arr: print(item)
来源：http://er.shtwfgs.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gi.chemitech.net.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://co.chemitech.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://nx.shtwfgs.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://po.nicolike.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bh.newstarts.cn

Ruby: arr.each { |item| puts item }
来源：http://sv.szxytkj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dw.szsharing.cn

[B06] 遍历字典 / 对象
来源：http://hk.huanxung.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://bw.lnxyls.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gc.521024.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cl.wgjwhj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://re.newstarts.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ps.bjjhwx.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hw.jianghongdianzi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rm.huanxung.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cw.bjjhwx.cn

[B07] while 循环
来源：http://xm.huanxung.cn

Py:   while i < 10: i += 1
来源：http://wl.hahajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://om.jctech888.com.cn

JS:   while (i < 10) { i++; }
来源：http://oa.szxytkj.cn

TS:   while (i < 10) { i++; }
来源：http://al.jianghongdianzi.cn

Java: while (i < 10) { i++; }
来源：http://np.jctech888.com.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rv.nszjky.cn

Ruby: while i < 10; i += 1; end
来源：http://eg.szxytkj.cn

C#:   while (i < 10) { i++; }
来源：http://uv.szxytkj.cn

[B08] do-while（至少执行一次）
来源：http://gr.szsharing.cn

Py:   # 无 do-while：用 while True + break
来源：http://sx.hnjuh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ga.shxzukj.cn

JS:   do { i++; } while (i < 10);
来源：http://wj.colortex.cn

TS:   do { i++; } while (i < 10);
来源：http://kc.huixinmuqiang.cn

Java: do { i++; } while (i < 10);
来源：http://ce.hnjuh.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ya.muxihuayi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://lp.szsharing.cn

C#:   do { i++; } while (i < 10);
来源：http://bj.bookmarksfly.cn

[B09] break 与 continue
来源：http://yr.muxihuayi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lv.yuntaijiaju.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://up.bookmarksfly.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zk.bjjhwx.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wf.huixiangedu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gm.hnjuh.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ys.lnxyls.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dj.colortex.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lc.shxzskj.cn

[B10] 遍历同时拿索引
来源：http://eo.wgjwhj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ga.jctech888.com.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://da.nszjky.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://em.haigaiapp.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://az.panjiajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mx.colortex.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ax.panjiajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pw.huixiangedu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fa.szxytkj.cn

[B11] 生成数字序列 / 区间
来源：http://fu.panjiajie.cn

Py:   list(range(0, 10, 2))
来源：http://yp.shxzskj.cn

PHP:  range(0, 10, 2);
来源：http://mu.lnxyls.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eu.haigaiapp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wa.jianghongdianzi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pf.bookmarksfly.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ny.jctech888.com.cn

Ruby: (0...10).step(2).to_a
来源：http://lc.huanxung.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://iy.bookmarksfly.cn

[B12] 跳出多层循环
来源：http://ac.huixiangedu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://cu.521024.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ay.bjjhwx.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bs.shxzskj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rp.jianghongdianzi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://le.gzmigu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ue.huixinmuqiang.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ff.haigaiapp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xj.9csxet.cn

[B13] 判断是否为数字
来源：http://jr.nszjky.cn

Py:   isinstance(x, (int, float))
来源：http://mi.hnjuh.cn

PHP:  is_numeric($x)
来源：http://ud.newstarts.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vd.chemitech.net.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://le.muxihuayi.cn

Java: x instanceof Number
来源：http://ai.shxzskj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://iz.szsharing.cn

Ruby: x.is_a?(Numeric)
来源：http://dp.521024.cn

C#:   x is int or double or decimal
来源：http://uu.nszjky.cn

[B14] 判断值是否在集合内
来源：http://yr.chemitech.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bm.jianghongdianzi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fv.huixiangedu.cn

JS:   [1, 2, 3].includes(x)
来源：http://vw.nszjky.cn

TS:   [1, 2, 3].includes(x)
来源：http://wa.shtwfgs.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kv.521024.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ck.shtwfgs.cn

Ruby: [1, 2, 3].include?(x)
来源：http://yp.colortex.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ge.hahajie.cn

[B15] 布尔运算与取反
来源：http://vj.huixiangedu.cn

Py:   a and b or not c
来源：http://mz.yuexingan06.cn

PHP:  $a && $b || !$c
来源：http://kp.haigaiapp.cn

JS:   a && b || !c
来源：http://ew.wgjwhj.cn

TS:   a && b || !c
来源：http://yn.nicolike.cn

Java: a && b || !c
来源：http://el.521024.cn

Go:   a && b || !c
来源：http://sa.shxzukj.cn

Ruby: a && b || !c
来源：http://ic.muxihuayi.cn

C#:   a && b || !c
来源：http://iv.yuexingan06.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hv.bjjhwx.cn

Py:   if not data: return
来源：http://vx.shtwfgs.cn

PHP:  if (!$data) { return; }
来源：http://kg.shxzukj.cn

JS:   if (!data) return;
来源：http://kp.521024.cn

TS:   if (!data) return;
来源：http://zi.panjiajie.cn

Java: if (data == null) return;
来源：http://wj.521024.cn

Go:   if data == nil { return }
来源：http://ax.szxytkj.cn

Ruby: return if data.nil?
来源：http://iy.yuexingan06.cn

C#:   if (data == null) return;
来源：http://lw.bjjhwx.cn

================================================================================
来源：http://yj.lnxyls.cn

C. 函数与作用域
来源：http://nu.huanxung.cn

================================================================================
来源：http://xh.521024.cn

[C01] 定义函数
来源：http://le.wgjwhj.cn

Py:   def add(a, b): return a + b
来源：http://dp.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sx.bookmarksfly.cn

JS:   function add(a, b) { return a + b; }
来源：http://ih.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gg.nszjky.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ck.jctech888.com.cn

Go:   func add(a, b int) int { return a + b }
来源：http://kt.muxihuayi.cn

Ruby: def add(a, b); a + b; end
来源：http://me.bjjhwx.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sf.nszjky.cn

[C02] 默认参数
来源：http://rv.huixiangedu.cn

Py:   def greet(name="World"): return name
来源：http://ap.panjiajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tu.bjjhwx.cn

JS:   function greet(name = "World") { return name; }
来源：http://zj.szxytkj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wp.huanxung.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://uf.huixiangedu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ff.huanxung.cn

Ruby: def greet(name = "World") = name
来源：http://wj.9csxet.cn

C#:   string Greet(string name = "World") => name;
来源：http://am.wgjwhj.cn

[C03] 可变参数
来源：http://zq.hnjuh.cn

Py:   def total(*args): return sum(args)
来源：http://mu.huixiangedu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ua.newstarts.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ka.gzmigu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yl.huixiangedu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xg.huanxung.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rh.newstarts.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ro.nicolike.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zy.panjiajie.cn

[C04] 命名参数 / 关键字参数
来源：http://vm.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vq.huixiangedu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lf.521024.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yi.szxytkj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cs.hnjuh.cn

Java: // 无：用 Builder 模式或 record
来源：http://fo.chemitech.net.cn

Go:   // 无：用配置结构体参数
来源：http://zw.yuexingan06.cn

Ruby: f(a: 1, b: 2)
来源：http://zq.shxzskj.cn

C#:   f(a: 1, b: 2)
来源：http://ua.shtwfgs.cn

[C05] 返回多个值
来源：http://ox.bookmarksfly.cn

Py:   return a, b
来源：http://qw.shxzukj.cn

PHP:  return [$a, $b];
来源：http://md.nicolike.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jp.panjiajie.cn

TS:   return { a, b };
来源：http://et.panjiajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jj.haigaiapp.cn

Go:   return a, b
来源：http://nf.shxzukj.cn

Ruby: return a, b
来源：http://ai.bjjhwx.cn

C#:   return (a, b);              // ValueTuple
来源：http://it.gzmigu.cn

[C06] 匿名函数 / lambda
来源：http://jw.szxytkj.cn

Py:   square = lambda x: x * x
来源：http://cd.szxytkj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://vp.szsharing.cn

JS:   const square = x => x * x;
来源：http://mr.panjiajie.cn

TS:   const square = (x: number): number => x * x;
来源：http://uv.huanxung.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vd.colortex.cn

Go:   sq := func(x int) int { return x * x }
来源：http://og.huixiangedu.cn

Ruby: square = ->(x) { x * x }
来源：http://ms.hnjuh.cn

C#:   Func<int, int> square = x => x * x;
来源：http://gd.jctech888.com.cn

[C07] 把函数作为参数传入
来源：http://om.jctech888.com.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vg.lnxyls.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bk.asd995.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gl.colortex.cn

TS:   arr.map(String)
来源：http://ae.bjjhwx.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vq.shtwfgs.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mt.jctech888.com.cn

Ruby: arr.map(&:upcase)
来源：http://xm.jctech888.com.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://oi.huanxung.cn

[C08] 闭包
来源：http://bb.asd995.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://no.shxzukj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ur.szxytkj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vi.9csxet.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lx.521024.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fh.hnjuh.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ug.bjjhwx.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rq.gzmigu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jv.521024.cn

[C09] 递归
来源：http://wt.shxzukj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cg.panjiajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://px.asd995.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jw.lnxyls.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ph.hnjuh.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bn.521024.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mb.chemitech.net.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kz.jianghongdianzi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qx.nszjky.cn

[C10] 变量作用域
来源：http://wy.szsharing.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sc.shxzskj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lk.haigaiapp.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://iw.yuntaijiaju.cn

TS:   同 JS
来源：http://ur.shxzskj.cn

Java: 方法内为块级作用域
来源：http://lz.shtwfgs.cn

Go:   花括号块级作用域
来源：http://gx.hnjuh.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pg.wgjwhj.cn

C#:   块级作用域
来源：http://aj.bjjhwx.cn

[C11] 模块导入与导出
来源：http://se.panjiajie.cn

Py:   from module import func
来源：http://mm.colortex.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xs.wgjwhj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kn.szxytkj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wb.nicolike.cn

Java: import java.util.List;
来源：http://ng.asd995.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mp.szsharing.cn

Ruby: require "json"; require_relative "./util"
来源：http://jy.szsharing.cn

C#:   using System.Text;
来源：http://lx.szxytkj.cn

[C12] 立即执行函数 IIFE
来源：http://jt.huanxung.cn

Py:   (lambda: print("run"))()
来源：http://az.lnxyls.cn

PHP:  (function () { echo "run"; })();
来源：http://oo.muxihuayi.cn

JS:   (() => { console.log("run"); })();
来源：http://ef.wgjwhj.cn

TS:   (() => { console.log("run"); })();
来源：http://hk.shxzskj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://is.jianghongdianzi.cn

Go:   func() { fmt.Println("run") }()
来源：http://zx.jctech888.com.cn

Ruby: -> { puts "run" }.call
来源：http://ik.bookmarksfly.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mj.newstarts.cn

[C13] 类型声明 / 类型注解
来源：http://bo.szsharing.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ad.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://if.jianghongdianzi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xp.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://en.hnjuh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://rj.shtwfgs.cn

Go:   func add(a, b int) int
来源：http://qg.huixiangedu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xy.jianghongdianzi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nk.jianghongdianzi.cn

[C14] 泛型函数
来源：http://pa.9csxet.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dx.newstarts.cn

PHP:  // 无泛型
来源：http://na.newstarts.cn

JS:   // 无泛型
来源：http://mo.panjiajie.cn


<!-- 参考信息 -->