代发 wailian999

C#:   s.Length
来源：http://wb.huixiangedu.cn

[A23] 大小写转换
来源：http://tc.shxzukj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://nc.gzmigu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ez.521024.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://eh.shxzukj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ov.shxzskj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://po.wgjwhj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ft.szxytkj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://oa.szxytkj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://kp.asd995.cn

[A24] 去除首尾空白
来源：http://xp.jianghongdianzi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://yw.szxytkj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kg.huixinmuqiang.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ls.shtwfgs.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://er.muxihuayi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dq.521024.cn

Go:   strings.TrimSpace(s)
来源：http://jy.shxzukj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qy.muxihuayi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gh.gzmigu.cn

[A25] 字符串比较
来源：http://fn.shxzskj.cn

Py:   s1 == s2; s1 != s2
来源：http://fg.huixinmuqiang.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dr.haigaiapp.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qx.chemitech.net.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wq.bjjhwx.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gp.jianghongdianzi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bq.gzmigu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://wf.shxzukj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mm.shxzskj.cn

[A26] 类型转换总览
来源：http://mm.muxihuayi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ga.newstarts.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jx.muxihuayi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jt.bookmarksfly.cn

TS:   Number() String() Boolean() x as number
来源：http://zy.bookmarksfly.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nw.hahajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wo.huixiangedu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ll.lnxyls.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lh.yuntaijiaju.cn

================================================================================
来源：http://so.bjjhwx.cn

B. 流程控制
来源：http://bt.521024.cn

================================================================================
来源：http://zy.nicolike.cn

[B01] 条件判断 if / else
来源：http://ui.yuntaijiaju.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://en.bookmarksfly.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jb.hnjuh.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rc.yuntaijiaju.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://em.colortex.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ea.bookmarksfly.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ou.hnjuh.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ei.shxzukj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://px.bookmarksfly.cn

[B02] 多分支 else if / elif
来源：http://ag.huixiangedu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sj.shtwfgs.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xy.shxzskj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tx.colortex.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nj.shtwfgs.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sy.shxzskj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lx.huixiangedu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jd.jianghongdianzi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ga.wgjwhj.cn

[B03] switch / match / case
来源：http://pk.panjiajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dx.nicolike.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tm.muxihuayi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://he.haigaiapp.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yf.bjjhwx.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ui.jctech888.com.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://or.szsharing.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qf.muxihuayi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kg.asd995.cn

[B04] for 计数循环
来源：http://vv.huanxung.cn

Py:   for i in range(10): print(i)
来源：http://kz.wgjwhj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lo.huixinmuqiang.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ur.huanxung.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bq.shxzukj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rt.asd995.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ve.shtwfgs.cn

Ruby: 10.times { |i| puts i }
来源：http://ce.hahajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sm.wgjwhj.cn

[B05] 遍历数组 / 列表
来源：http://us.shtwfgs.cn

Py:   for item in arr: print(item)
来源：http://xe.huixinmuqiang.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://io.bjjhwx.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ri.521024.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ao.hahajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ux.bookmarksfly.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lt.hnjuh.cn

Ruby: arr.each { |item| puts item }
来源：http://lv.hnjuh.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xb.hahajie.cn

[B06] 遍历字典 / 对象
来源：http://jp.haigaiapp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fd.huixiangedu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rq.huanxung.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://av.shtwfgs.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tw.bookmarksfly.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ts.hnjuh.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rf.hahajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kj.yuexingan06.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ob.wgjwhj.cn

[B07] while 循环
来源：http://qs.newstarts.cn

Py:   while i < 10: i += 1
来源：http://vb.jianghongdianzi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lx.yuexingan06.cn

JS:   while (i < 10) { i++; }
来源：http://tr.hahajie.cn

TS:   while (i < 10) { i++; }
来源：http://ck.521024.cn

Java: while (i < 10) { i++; }
来源：http://km.hnjuh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qt.szsharing.cn

Ruby: while i < 10; i += 1; end
来源：http://kb.yuntaijiaju.cn

C#:   while (i < 10) { i++; }
来源：http://lj.hnjuh.cn

[B08] do-while（至少执行一次）
来源：http://fh.jctech888.com.cn

Py:   # 无 do-while：用 while True + break
来源：http://fl.yuexingan06.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mm.huixiangedu.cn

JS:   do { i++; } while (i < 10);
来源：http://hh.szsharing.cn

TS:   do { i++; } while (i < 10);
来源：http://tj.newstarts.cn

Java: do { i++; } while (i < 10);
来源：http://mb.gzmigu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://og.shxzukj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xv.nicolike.cn

C#:   do { i++; } while (i < 10);
来源：http://jt.szxytkj.cn

[B09] break 与 continue
来源：http://jb.shtwfgs.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xk.szxytkj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lf.huixinmuqiang.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mn.9csxet.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://za.yuexingan06.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lb.szsharing.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dl.jctech888.com.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zv.jctech888.com.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vl.bjjhwx.cn

[B10] 遍历同时拿索引
来源：http://az.szxytkj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://se.huanxung.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qh.bookmarksfly.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ec.panjiajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kh.nszjky.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wk.panjiajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tv.nszjky.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uo.nszjky.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://oj.9csxet.cn

[B11] 生成数字序列 / 区间
来源：http://no.colortex.cn

Py:   list(range(0, 10, 2))
来源：http://ly.lnxyls.cn

PHP:  range(0, 10, 2);
来源：http://gu.haigaiapp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gs.jianghongdianzi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ik.521024.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sr.huanxung.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://oi.521024.cn

Ruby: (0...10).step(2).to_a
来源：http://he.colortex.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jc.jianghongdianzi.cn

[B12] 跳出多层循环
来源：http://up.yuntaijiaju.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://kd.szxytkj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://iy.huixinmuqiang.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hy.lnxyls.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lh.chemitech.net.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yc.bjjhwx.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xz.lnxyls.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hs.shtwfgs.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sx.wgjwhj.cn

[B13] 判断是否为数字
来源：http://oc.hahajie.cn

Py:   isinstance(x, (int, float))
来源：http://ui.szxytkj.cn

PHP:  is_numeric($x)
来源：http://se.chemitech.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ae.szsharing.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lp.jianghongdianzi.cn

Java: x instanceof Number
来源：http://ct.nicolike.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bz.panjiajie.cn

Ruby: x.is_a?(Numeric)
来源：http://jx.szxytkj.cn

C#:   x is int or double or decimal
来源：http://mv.haigaiapp.cn

[B14] 判断值是否在集合内
来源：http://vu.bjjhwx.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ew.bookmarksfly.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bs.jianghongdianzi.cn

JS:   [1, 2, 3].includes(x)
来源：http://xw.asd995.cn

TS:   [1, 2, 3].includes(x)
来源：http://yz.bjjhwx.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://om.newstarts.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://og.newstarts.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cz.gzmigu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://je.shtwfgs.cn

[B15] 布尔运算与取反
来源：http://jv.szsharing.cn

Py:   a and b or not c
来源：http://yb.yuntaijiaju.cn

PHP:  $a && $b || !$c
来源：http://np.shtwfgs.cn

JS:   a && b || !c
来源：http://jn.panjiajie.cn

TS:   a && b || !c
来源：http://mb.jctech888.com.cn

Java: a && b || !c
来源：http://ro.huanxung.cn

Go:   a && b || !c
来源：http://yt.szsharing.cn

Ruby: a && b || !c
来源：http://bo.hahajie.cn

C#:   a && b || !c
来源：http://et.nszjky.cn

[B16] 卫语句：不满足条件提前返回
来源：http://sx.nszjky.cn

Py:   if not data: return
来源：http://bq.jctech888.com.cn

PHP:  if (!$data) { return; }
来源：http://bx.huanxung.cn

JS:   if (!data) return;
来源：http://gn.bjjhwx.cn

TS:   if (!data) return;
来源：http://wf.shtwfgs.cn

Java: if (data == null) return;
来源：http://wq.jianghongdianzi.cn

Go:   if data == nil { return }
来源：http://ax.newstarts.cn

Ruby: return if data.nil?
来源：http://oo.jctech888.com.cn

C#:   if (data == null) return;
来源：http://vk.shxzskj.cn

================================================================================
来源：http://ki.asd995.cn

C. 函数与作用域
来源：http://kz.yuntaijiaju.cn

================================================================================
来源：http://rk.huixinmuqiang.cn

[C01] 定义函数
来源：http://qb.bookmarksfly.cn

Py:   def add(a, b): return a + b
来源：http://ds.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ce.chemitech.net.cn

JS:   function add(a, b) { return a + b; }
来源：http://sv.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tv.hnjuh.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://le.panjiajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xq.yuexingan06.cn

Ruby: def add(a, b); a + b; end
来源：http://ao.bjjhwx.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rd.nszjky.cn

[C02] 默认参数
来源：http://qw.bookmarksfly.cn

Py:   def greet(name="World"): return name
来源：http://qf.panjiajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ib.hnjuh.cn

JS:   function greet(name = "World") { return name; }
来源：http://ad.asd995.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cf.haigaiapp.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://pe.shtwfgs.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ln.szxytkj.cn

Ruby: def greet(name = "World") = name
来源：http://sv.jianghongdianzi.cn

C#:   string Greet(string name = "World") => name;
来源：http://am.huixinmuqiang.cn

[C03] 可变参数
来源：http://wx.panjiajie.cn

Py:   def total(*args): return sum(args)
来源：http://cv.lnxyls.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bv.gzmigu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://za.jctech888.com.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wx.panjiajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rx.gzmigu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ud.muxihuayi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://eh.jctech888.com.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bz.shxzskj.cn

[C04] 命名参数 / 关键字参数
来源：http://ba.panjiajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bq.asd995.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pl.hahajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://km.9csxet.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fa.haigaiapp.cn

Java: // 无：用 Builder 模式或 record
来源：http://uu.panjiajie.cn

Go:   // 无：用配置结构体参数
来源：http://gl.yuntaijiaju.cn

Ruby: f(a: 1, b: 2)
来源：http://di.shxzukj.cn

C#:   f(a: 1, b: 2)
来源：http://nj.haigaiapp.cn

[C05] 返回多个值
来源：http://yd.szsharing.cn

Py:   return a, b
来源：http://xd.asd995.cn

PHP:  return [$a, $b];
来源：http://as.yuexingan06.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jx.yuexingan06.cn

TS:   return { a, b };
来源：http://gr.jianghongdianzi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ll.szsharing.cn

Go:   return a, b
来源：http://ti.muxihuayi.cn

Ruby: return a, b
来源：http://zi.nicolike.cn

C#:   return (a, b);              // ValueTuple
来源：http://vz.muxihuayi.cn

[C06] 匿名函数 / lambda
来源：http://bj.jctech888.com.cn

Py:   square = lambda x: x * x
来源：http://tm.bjjhwx.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://av.wgjwhj.cn

JS:   const square = x => x * x;
来源：http://bw.huanxung.cn

TS:   const square = (x: number): number => x * x;
来源：http://qs.jianghongdianzi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ec.yuntaijiaju.cn

Go:   sq := func(x int) int { return x * x }
来源：http://pl.bookmarksfly.cn

Ruby: square = ->(x) { x * x }
来源：http://kf.hnjuh.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ew.newstarts.cn

[C07] 把函数作为参数传入
来源：http://ab.hnjuh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bu.panjiajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ll.panjiajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tf.bjjhwx.cn

TS:   arr.map(String)
来源：http://jx.jctech888.com.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ob.lnxyls.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zj.yuntaijiaju.cn

Ruby: arr.map(&:upcase)
来源：http://mj.hnjuh.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://py.panjiajie.cn

[C08] 闭包
来源：http://bx.huixiangedu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yj.jctech888.com.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://we.wgjwhj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xi.szxytkj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rj.jctech888.com.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fn.jianghongdianzi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xz.9csxet.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mk.colortex.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zc.nicolike.cn

[C09] 递归
来源：http://df.yuexingan06.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rb.huixiangedu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pw.szsharing.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lf.newstarts.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://io.haigaiapp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fn.colortex.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://th.huanxung.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wa.jianghongdianzi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zn.9csxet.cn

[C10] 变量作用域
来源：http://on.panjiajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://al.szxytkj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mv.huixiangedu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nx.jctech888.com.cn

TS:   同 JS
来源：http://ip.bjjhwx.cn

Java: 方法内为块级作用域
来源：http://fd.shxzskj.cn

Go:   花括号块级作用域
来源：http://mj.colortex.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rx.yuntaijiaju.cn

C#:   块级作用域
来源：http://ib.jctech888.com.cn

[C11] 模块导入与导出
来源：http://rk.521024.cn

Py:   from module import func
来源：http://nv.bjjhwx.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vz.asd995.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hl.jianghongdianzi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nu.asd995.cn

Java: import java.util.List;
来源：http://ux.szxytkj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://at.yuntaijiaju.cn

Ruby: require "json"; require_relative "./util"
来源：http://zk.asd995.cn

C#:   using System.Text;
来源：http://pi.colortex.cn

[C12] 立即执行函数 IIFE
来源：http://lg.wgjwhj.cn

Py:   (lambda: print("run"))()
来源：http://jw.nicolike.cn

PHP:  (function () { echo "run"; })();
来源：http://qd.hnjuh.cn

JS:   (() => { console.log("run"); })();
来源：http://ho.muxihuayi.cn

TS:   (() => { console.log("run"); })();
来源：http://vj.hnjuh.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ea.bjjhwx.cn

Go:   func() { fmt.Println("run") }()
来源：http://sf.lnxyls.cn

Ruby: -> { puts "run" }.call
来源：http://qz.wgjwhj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zr.521024.cn

[C13] 类型声明 / 类型注解
来源：http://tq.yuntaijiaju.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hd.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gd.bjjhwx.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://go.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pe.szsharing.cn


<!-- 参考信息 -->