代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qy.bookmarksfly.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://aj.panjiajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jl.hnjuh.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nq.newstarts.cn

Go:   strings.TrimSpace(s)
来源：http://dw.panjiajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rn.nszjky.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wq.nicolike.cn

[A25] 字符串比较
来源：http://qp.hnjuh.cn

Py:   s1 == s2; s1 != s2
来源：http://up.colortex.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pq.521024.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dk.521024.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lb.szxytkj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vw.hnjuh.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fl.yuntaijiaju.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vk.jctech888.com.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ro.muxihuayi.cn

[A26] 类型转换总览
来源：http://sn.panjiajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qc.bjjhwx.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://eg.panjiajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bs.yuntaijiaju.cn

TS:   Number() String() Boolean() x as number
来源：http://fm.jianghongdianzi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ny.yuntaijiaju.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cb.newstarts.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://wz.shxzskj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bu.huixinmuqiang.cn

================================================================================
来源：http://gk.521024.cn

B. 流程控制
来源：http://fr.hahajie.cn

================================================================================
来源：http://qn.colortex.cn

[B01] 条件判断 if / else
来源：http://bu.newstarts.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://up.9csxet.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qy.muxihuayi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://he.yuexingan06.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://cj.chemitech.net.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://jd.huixinmuqiang.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://sj.szsharing.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ll.nszjky.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://iz.yuexingan06.cn

[B02] 多分支 else if / elif
来源：http://mw.huixinmuqiang.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://my.9csxet.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ht.szsharing.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yl.colortex.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hx.jianghongdianzi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://un.shxzukj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ah.shxzskj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://iq.wgjwhj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wr.nszjky.cn

[B03] switch / match / case
来源：http://ts.hnjuh.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jn.bookmarksfly.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gx.panjiajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://by.panjiajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://up.asd995.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bw.hnjuh.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tp.muxihuayi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vq.muxihuayi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jt.bookmarksfly.cn

[B04] for 计数循环
来源：http://qs.hnjuh.cn

Py:   for i in range(10): print(i)
来源：http://ov.wgjwhj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rk.huixiangedu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tb.szxytkj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zd.bjjhwx.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zj.gzmigu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bm.lnxyls.cn

Ruby: 10.times { |i| puts i }
来源：http://dt.521024.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lg.jianghongdianzi.cn

[B05] 遍历数组 / 列表
来源：http://ld.jctech888.com.cn

Py:   for item in arr: print(item)
来源：http://mv.muxihuayi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gs.asd995.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://cn.bjjhwx.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ck.huixinmuqiang.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xc.jianghongdianzi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ws.gzmigu.cn

Ruby: arr.each { |item| puts item }
来源：http://hn.shtwfgs.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bi.yuexingan06.cn

[B06] 遍历字典 / 对象
来源：http://vn.huixiangedu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://de.yuntaijiaju.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pv.bookmarksfly.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nu.shxzskj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://di.yuexingan06.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gg.szsharing.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mb.shxzskj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hi.szxytkj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://aj.newstarts.cn

[B07] while 循环
来源：http://de.panjiajie.cn

Py:   while i < 10: i += 1
来源：http://ni.lnxyls.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gr.shxzskj.cn

JS:   while (i < 10) { i++; }
来源：http://ea.shxzskj.cn

TS:   while (i < 10) { i++; }
来源：http://ki.yuexingan06.cn

Java: while (i < 10) { i++; }
来源：http://jc.jctech888.com.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xa.shxzukj.cn

Ruby: while i < 10; i += 1; end
来源：http://qe.chemitech.net.cn

C#:   while (i < 10) { i++; }
来源：http://pd.asd995.cn

[B08] do-while（至少执行一次）
来源：http://we.huixinmuqiang.cn

Py:   # 无 do-while：用 while True + break
来源：http://za.521024.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jb.huanxung.cn

JS:   do { i++; } while (i < 10);
来源：http://tb.shxzukj.cn

TS:   do { i++; } while (i < 10);
来源：http://kb.szsharing.cn

Java: do { i++; } while (i < 10);
来源：http://sx.huixinmuqiang.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://oj.shtwfgs.cn

Ruby: begin; i += 1; end while i < 10
来源：http://az.szsharing.cn

C#:   do { i++; } while (i < 10);
来源：http://iv.asd995.cn

[B09] break 与 continue
来源：http://rc.huixinmuqiang.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wv.lnxyls.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jd.haigaiapp.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nb.chemitech.net.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uo.9csxet.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://we.szsharing.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vl.haigaiapp.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ou.colortex.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sv.521024.cn

[B10] 遍历同时拿索引
来源：http://cv.huixinmuqiang.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tu.muxihuayi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nb.shtwfgs.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hw.huanxung.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ys.huixinmuqiang.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nq.jctech888.com.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://se.szxytkj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uv.colortex.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mk.nicolike.cn

[B11] 生成数字序列 / 区间
来源：http://wq.huixiangedu.cn

Py:   list(range(0, 10, 2))
来源：http://jy.huixiangedu.cn

PHP:  range(0, 10, 2);
来源：http://lm.wgjwhj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dm.yuexingan06.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qi.chemitech.net.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rc.chemitech.net.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pi.gzmigu.cn

Ruby: (0...10).step(2).to_a
来源：http://na.chemitech.net.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ve.nszjky.cn

[B12] 跳出多层循环
来源：http://rx.asd995.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zo.muxihuayi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://kp.nicolike.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://id.shxzukj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ap.muxihuayi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lk.chemitech.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pm.panjiajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://of.hnjuh.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qd.muxihuayi.cn

[B13] 判断是否为数字
来源：http://mi.asd995.cn

Py:   isinstance(x, (int, float))
来源：http://sg.nszjky.cn

PHP:  is_numeric($x)
来源：http://nk.yuntaijiaju.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gw.bjjhwx.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://je.asd995.cn

Java: x instanceof Number
来源：http://ea.shxzukj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qp.521024.cn

Ruby: x.is_a?(Numeric)
来源：http://uo.huixinmuqiang.cn

C#:   x is int or double or decimal
来源：http://kf.colortex.cn

[B14] 判断值是否在集合内
来源：http://pw.yuexingan06.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jk.hnjuh.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jc.szsharing.cn

JS:   [1, 2, 3].includes(x)
来源：http://wi.yuntaijiaju.cn

TS:   [1, 2, 3].includes(x)
来源：http://ss.9csxet.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://zi.shtwfgs.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hf.panjiajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://kd.bookmarksfly.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mu.nszjky.cn

[B15] 布尔运算与取反
来源：http://dc.hahajie.cn

Py:   a and b or not c
来源：http://cb.yuntaijiaju.cn

PHP:  $a && $b || !$c
来源：http://dm.shxzskj.cn

JS:   a && b || !c
来源：http://lv.asd995.cn

TS:   a && b || !c
来源：http://qt.szxytkj.cn

Java: a && b || !c
来源：http://ts.newstarts.cn

Go:   a && b || !c
来源：http://fy.gzmigu.cn

Ruby: a && b || !c
来源：http://ak.asd995.cn

C#:   a && b || !c
来源：http://ok.newstarts.cn

[B16] 卫语句：不满足条件提前返回
来源：http://aq.lnxyls.cn

Py:   if not data: return
来源：http://xz.yuntaijiaju.cn

PHP:  if (!$data) { return; }
来源：http://fu.hnjuh.cn

JS:   if (!data) return;
来源：http://dz.huixinmuqiang.cn

TS:   if (!data) return;
来源：http://wh.jianghongdianzi.cn

Java: if (data == null) return;
来源：http://zm.haigaiapp.cn

Go:   if data == nil { return }
来源：http://dz.hnjuh.cn

Ruby: return if data.nil?
来源：http://cq.nszjky.cn

C#:   if (data == null) return;
来源：http://ay.newstarts.cn

================================================================================
来源：http://di.huixiangedu.cn

C. 函数与作用域
来源：http://ny.shxzskj.cn

================================================================================
来源：http://zz.shtwfgs.cn

[C01] 定义函数
来源：http://oq.colortex.cn

Py:   def add(a, b): return a + b
来源：http://ia.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tm.9csxet.cn

JS:   function add(a, b) { return a + b; }
来源：http://lg.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kq.shxzskj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://tq.huanxung.cn

Go:   func add(a, b int) int { return a + b }
来源：http://la.yuntaijiaju.cn

Ruby: def add(a, b); a + b; end
来源：http://ju.jianghongdianzi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://el.chemitech.net.cn

[C02] 默认参数
来源：http://ba.colortex.cn

Py:   def greet(name="World"): return name
来源：http://al.shtwfgs.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://si.szsharing.cn

JS:   function greet(name = "World") { return name; }
来源：http://sx.nszjky.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://kq.bjjhwx.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bu.huanxung.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ki.9csxet.cn

Ruby: def greet(name = "World") = name
来源：http://zx.bjjhwx.cn

C#:   string Greet(string name = "World") => name;
来源：http://lp.szxytkj.cn

[C03] 可变参数
来源：http://np.asd995.cn

Py:   def total(*args): return sum(args)
来源：http://wo.newstarts.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fh.521024.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bl.yuntaijiaju.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fn.jianghongdianzi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gq.muxihuayi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ko.shxzukj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gg.nicolike.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://re.nszjky.cn

[C04] 命名参数 / 关键字参数
来源：http://cd.huixinmuqiang.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lh.newstarts.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dy.haigaiapp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://be.yuexingan06.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kk.jctech888.com.cn

Java: // 无：用 Builder 模式或 record
来源：http://hh.bjjhwx.cn

Go:   // 无：用配置结构体参数
来源：http://vx.jctech888.com.cn

Ruby: f(a: 1, b: 2)
来源：http://vv.huanxung.cn

C#:   f(a: 1, b: 2)
来源：http://kj.shxzukj.cn

[C05] 返回多个值
来源：http://jt.shxzskj.cn

Py:   return a, b
来源：http://zl.yuntaijiaju.cn

PHP:  return [$a, $b];
来源：http://ig.huixinmuqiang.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://sb.shtwfgs.cn

TS:   return { a, b };
来源：http://ae.bjjhwx.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ab.nszjky.cn

Go:   return a, b
来源：http://ga.wgjwhj.cn

Ruby: return a, b
来源：http://qd.haigaiapp.cn

C#:   return (a, b);              // ValueTuple
来源：http://ci.newstarts.cn

[C06] 匿名函数 / lambda
来源：http://bg.huanxung.cn

Py:   square = lambda x: x * x
来源：http://wz.jianghongdianzi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://yk.lnxyls.cn

JS:   const square = x => x * x;
来源：http://rk.muxihuayi.cn

TS:   const square = (x: number): number => x * x;
来源：http://vj.muxihuayi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cp.hnjuh.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xo.szsharing.cn

Ruby: square = ->(x) { x * x }
来源：http://xx.panjiajie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zc.haigaiapp.cn

[C07] 把函数作为参数传入
来源：http://wd.shtwfgs.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ju.asd995.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ue.asd995.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://oe.yuntaijiaju.cn

TS:   arr.map(String)
来源：http://fd.muxihuayi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zr.newstarts.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tl.szxytkj.cn

Ruby: arr.map(&:upcase)
来源：http://jm.hahajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://md.shtwfgs.cn

[C08] 闭包
来源：http://lw.9csxet.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://of.shxzskj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zq.yuexingan06.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wq.shxzukj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://te.yuexingan06.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vi.nicolike.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hq.colortex.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ea.bookmarksfly.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ym.hahajie.cn

[C09] 递归
来源：http://jq.nszjky.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ie.nszjky.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gm.wgjwhj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zv.bookmarksfly.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pe.lnxyls.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://of.colortex.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sr.hahajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ks.nicolike.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nx.hnjuh.cn

[C10] 变量作用域
来源：http://bo.chemitech.net.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jx.colortex.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dq.panjiajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ea.lnxyls.cn

TS:   同 JS
来源：http://kz.shxzskj.cn

Java: 方法内为块级作用域
来源：http://ir.huanxung.cn

Go:   花括号块级作用域
来源：http://zx.gzmigu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kr.szxytkj.cn

C#:   块级作用域
来源：http://mk.colortex.cn

[C11] 模块导入与导出
来源：http://li.yuntaijiaju.cn

Py:   from module import func
来源：http://up.chemitech.net.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pz.wgjwhj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://pe.newstarts.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zn.szsharing.cn

Java: import java.util.List;
来源：http://rq.shxzukj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sz.hahajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://xl.nszjky.cn

C#:   using System.Text;
来源：http://is.yuntaijiaju.cn

[C12] 立即执行函数 IIFE
来源：http://ph.asd995.cn

Py:   (lambda: print("run"))()
来源：http://wh.bookmarksfly.cn

PHP:  (function () { echo "run"; })();
来源：http://ub.szxytkj.cn

JS:   (() => { console.log("run"); })();
来源：http://co.hahajie.cn

TS:   (() => { console.log("run"); })();
来源：http://zq.asd995.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nn.shxzskj.cn

Go:   func() { fmt.Println("run") }()
来源：http://zv.yuntaijiaju.cn

Ruby: -> { puts "run" }.call
来源：http://nd.hnjuh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fk.jctech888.com.cn

[C13] 类型声明 / 类型注解
来源：http://eu.muxihuayi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://md.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://og.haigaiapp.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pv.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://to.lnxyls.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xp.bookmarksfly.cn

Go:   func add(a, b int) int
来源：http://db.jctech888.com.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ga.yuexingan06.cn

C#:   int Add(int a, int b) => a + b;
来源：http://az.chemitech.net.cn

[C14] 泛型函数
来源：http://mo.huanxung.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qh.szxytkj.cn

PHP:  // 无泛型
来源：http://pu.shxzskj.cn

JS:   // 无泛型
来源：http://ij.shtwfgs.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tx.huanxung.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cu.lnxyls.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rl.huixinmuqiang.cn

Ruby: # 无泛型
来源：http://sb.521024.cn


<!-- 参考信息 -->