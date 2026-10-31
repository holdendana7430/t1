代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dd.yuexingan06.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mj.jctech888.com.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mx.jianghongdianzi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://eb.jctech888.com.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zn.haigaiapp.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://sv.hahajie.cn

[A24] 去除首尾空白
来源：http://oi.yuexingan06.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gn.jianghongdianzi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ao.nicolike.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yh.chemitech.net.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gm.szxytkj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mi.yuntaijiaju.cn

Go:   strings.TrimSpace(s)
来源：http://wk.colortex.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nq.9csxet.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://bx.shxzskj.cn

[A25] 字符串比较
来源：http://gk.chemitech.net.cn

Py:   s1 == s2; s1 != s2
来源：http://li.shxzskj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://im.shxzukj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pn.szsharing.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zj.yuntaijiaju.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://iv.wgjwhj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tx.haigaiapp.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://gg.nicolike.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://uh.shxzukj.cn

[A26] 类型转换总览
来源：http://rg.muxihuayi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bv.hnjuh.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sb.szxytkj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cz.9csxet.cn

TS:   Number() String() Boolean() x as number
来源：http://wz.hnjuh.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tc.lnxyls.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fn.haigaiapp.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://nq.wgjwhj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mq.bjjhwx.cn

================================================================================
来源：http://io.hahajie.cn

B. 流程控制
来源：http://ti.521024.cn

================================================================================
来源：http://sp.521024.cn

[B01] 条件判断 if / else
来源：http://vr.521024.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://gs.huixinmuqiang.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mb.yuntaijiaju.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gs.nicolike.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wa.asd995.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://oq.shtwfgs.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kk.asd995.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ln.panjiajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bh.lnxyls.cn

[B02] 多分支 else if / elif
来源：http://dr.nszjky.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://me.bjjhwx.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zm.jianghongdianzi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ld.szsharing.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cx.bookmarksfly.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://az.shtwfgs.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ky.jianghongdianzi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qy.colortex.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pp.nicolike.cn

[B03] switch / match / case
来源：http://fl.asd995.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jb.bookmarksfly.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jd.colortex.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rb.gzmigu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://no.521024.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://oj.shxzukj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://am.huanxung.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uh.newstarts.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fh.9csxet.cn

[B04] for 计数循环
来源：http://xc.haigaiapp.cn

Py:   for i in range(10): print(i)
来源：http://bj.gzmigu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ic.jianghongdianzi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hf.chemitech.net.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ng.hahajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nb.asd995.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zh.lnxyls.cn

Ruby: 10.times { |i| puts i }
来源：http://yj.lnxyls.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nu.muxihuayi.cn

[B05] 遍历数组 / 列表
来源：http://al.bookmarksfly.cn

Py:   for item in arr: print(item)
来源：http://km.shxzukj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hn.szxytkj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dq.lnxyls.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xa.lnxyls.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ob.szsharing.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vt.wgjwhj.cn

Ruby: arr.each { |item| puts item }
来源：http://gt.nicolike.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sb.bjjhwx.cn

[B06] 遍历字典 / 对象
来源：http://ax.shxzukj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mw.gzmigu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lq.szsharing.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wj.huixinmuqiang.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ky.shtwfgs.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://oh.shxzskj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jk.asd995.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ea.hahajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://if.shtwfgs.cn

[B07] while 循环
来源：http://us.muxihuayi.cn

Py:   while i < 10: i += 1
来源：http://jk.huixinmuqiang.cn

PHP:  while ($i < 10) { $i++; }
来源：http://uo.huixiangedu.cn

JS:   while (i < 10) { i++; }
来源：http://zp.huanxung.cn

TS:   while (i < 10) { i++; }
来源：http://ur.wgjwhj.cn

Java: while (i < 10) { i++; }
来源：http://gz.bookmarksfly.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qz.9csxet.cn

Ruby: while i < 10; i += 1; end
来源：http://dr.huixiangedu.cn

C#:   while (i < 10) { i++; }
来源：http://ge.huanxung.cn

[B08] do-while（至少执行一次）
来源：http://xw.yuexingan06.cn

Py:   # 无 do-while：用 while True + break
来源：http://ao.chemitech.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://rj.hnjuh.cn

JS:   do { i++; } while (i < 10);
来源：http://ep.gzmigu.cn

TS:   do { i++; } while (i < 10);
来源：http://sb.asd995.cn

Java: do { i++; } while (i < 10);
来源：http://bd.gzmigu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ai.bookmarksfly.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rh.hnjuh.cn

C#:   do { i++; } while (i < 10);
来源：http://zz.yuexingan06.cn

[B09] break 与 continue
来源：http://nf.hahajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fe.wgjwhj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ly.yuexingan06.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jb.haigaiapp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ku.shtwfgs.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wr.newstarts.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xt.shxzskj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fz.521024.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://og.huixiangedu.cn

[B10] 遍历同时拿索引
来源：http://mt.haigaiapp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qu.yuntaijiaju.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qh.shxzukj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nf.9csxet.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ul.panjiajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dr.muxihuayi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mp.shxzukj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://je.asd995.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bj.huixiangedu.cn

[B11] 生成数字序列 / 区间
来源：http://bu.lnxyls.cn

Py:   list(range(0, 10, 2))
来源：http://ly.hahajie.cn

PHP:  range(0, 10, 2);
来源：http://kv.jianghongdianzi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://by.gzmigu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://js.nicolike.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qb.wgjwhj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fv.bookmarksfly.cn

Ruby: (0...10).step(2).to_a
来源：http://cf.jctech888.com.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fr.huanxung.cn

[B12] 跳出多层循环
来源：http://sc.huixinmuqiang.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ld.shtwfgs.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://nu.shtwfgs.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vm.colortex.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rd.521024.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ik.yuntaijiaju.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bm.newstarts.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mp.colortex.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hl.shtwfgs.cn

[B13] 判断是否为数字
来源：http://gm.gzmigu.cn

Py:   isinstance(x, (int, float))
来源：http://tg.asd995.cn

PHP:  is_numeric($x)
来源：http://tw.colortex.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qb.panjiajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oh.shtwfgs.cn

Java: x instanceof Number
来源：http://ps.szsharing.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tk.asd995.cn

Ruby: x.is_a?(Numeric)
来源：http://si.szsharing.cn

C#:   x is int or double or decimal
来源：http://fn.lnxyls.cn

[B14] 判断值是否在集合内
来源：http://po.wgjwhj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pf.521024.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pb.szsharing.cn

JS:   [1, 2, 3].includes(x)
来源：http://kd.chemitech.net.cn

TS:   [1, 2, 3].includes(x)
来源：http://ji.yuntaijiaju.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://nz.bjjhwx.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zl.jianghongdianzi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://bc.nicolike.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dn.jctech888.com.cn

[B15] 布尔运算与取反
来源：http://rp.hahajie.cn

Py:   a and b or not c
来源：http://sy.jctech888.com.cn

PHP:  $a && $b || !$c
来源：http://ps.newstarts.cn

JS:   a && b || !c
来源：http://mm.colortex.cn

TS:   a && b || !c
来源：http://ee.hnjuh.cn

Java: a && b || !c
来源：http://of.wgjwhj.cn

Go:   a && b || !c
来源：http://us.521024.cn

Ruby: a && b || !c
来源：http://ut.haigaiapp.cn

C#:   a && b || !c
来源：http://gj.nszjky.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lp.jctech888.com.cn

Py:   if not data: return
来源：http://wc.huixinmuqiang.cn

PHP:  if (!$data) { return; }
来源：http://yi.asd995.cn

JS:   if (!data) return;
来源：http://sv.nszjky.cn

TS:   if (!data) return;
来源：http://us.szxytkj.cn

Java: if (data == null) return;
来源：http://zw.szsharing.cn

Go:   if data == nil { return }
来源：http://de.jianghongdianzi.cn

Ruby: return if data.nil?
来源：http://mv.nszjky.cn

C#:   if (data == null) return;
来源：http://ip.chemitech.net.cn

================================================================================
来源：http://ip.panjiajie.cn

C. 函数与作用域
来源：http://ql.hahajie.cn

================================================================================
来源：http://uy.yuntaijiaju.cn

[C01] 定义函数
来源：http://pj.nicolike.cn

Py:   def add(a, b): return a + b
来源：http://cp.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qc.huanxung.cn

JS:   function add(a, b) { return a + b; }
来源：http://qu.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vh.jianghongdianzi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ml.shxzskj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://px.lnxyls.cn

Ruby: def add(a, b); a + b; end
来源：http://vn.colortex.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://st.chemitech.net.cn

[C02] 默认参数
来源：http://va.szsharing.cn

Py:   def greet(name="World"): return name
来源：http://ql.huixinmuqiang.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bw.nicolike.cn

JS:   function greet(name = "World") { return name; }
来源：http://iw.gzmigu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://jo.yuexingan06.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fy.lnxyls.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cd.jctech888.com.cn

Ruby: def greet(name = "World") = name
来源：http://ip.gzmigu.cn

C#:   string Greet(string name = "World") => name;
来源：http://sv.szxytkj.cn

[C03] 可变参数
来源：http://gw.yuexingan06.cn

Py:   def total(*args): return sum(args)
来源：http://lt.lnxyls.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ok.muxihuayi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ng.hnjuh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ok.huixiangedu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nd.yuexingan06.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jo.chemitech.net.cn

Ruby: def total(*nums); nums.sum; end
来源：http://sz.huanxung.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://up.muxihuayi.cn

[C04] 命名参数 / 关键字参数
来源：http://du.shxzskj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sl.jianghongdianzi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://um.haigaiapp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gj.chemitech.net.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wr.bookmarksfly.cn

Java: // 无：用 Builder 模式或 record
来源：http://wr.shxzskj.cn

Go:   // 无：用配置结构体参数
来源：http://yi.521024.cn

Ruby: f(a: 1, b: 2)
来源：http://aq.yuexingan06.cn

C#:   f(a: 1, b: 2)
来源：http://rr.muxihuayi.cn

[C05] 返回多个值
来源：http://vk.shxzukj.cn

Py:   return a, b
来源：http://ci.521024.cn

PHP:  return [$a, $b];
来源：http://hf.huixiangedu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://uh.huixinmuqiang.cn

TS:   return { a, b };
来源：http://cu.huixinmuqiang.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zv.huanxung.cn

Go:   return a, b
来源：http://on.newstarts.cn

Ruby: return a, b
来源：http://it.521024.cn

C#:   return (a, b);              // ValueTuple
来源：http://js.nicolike.cn

[C06] 匿名函数 / lambda
来源：http://bx.wgjwhj.cn

Py:   square = lambda x: x * x
来源：http://pu.521024.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://is.521024.cn

JS:   const square = x => x * x;
来源：http://vg.jianghongdianzi.cn

TS:   const square = (x: number): number => x * x;
来源：http://te.jianghongdianzi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ru.yuntaijiaju.cn

Go:   sq := func(x int) int { return x * x }
来源：http://us.hnjuh.cn

Ruby: square = ->(x) { x * x }
来源：http://xw.521024.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qn.shxzskj.cn

[C07] 把函数作为参数传入
来源：http://zc.panjiajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bh.wgjwhj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ea.shxzskj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yn.gzmigu.cn

TS:   arr.map(String)
来源：http://lf.huanxung.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ez.nszjky.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gs.szxytkj.cn

Ruby: arr.map(&:upcase)
来源：http://ry.colortex.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mv.colortex.cn

[C08] 闭包
来源：http://gp.nszjky.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://te.bookmarksfly.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cw.nicolike.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xj.huixiangedu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kn.huixiangedu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://to.jianghongdianzi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ow.colortex.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dp.yuexingan06.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://iw.9csxet.cn

[C09] 递归
来源：http://ot.yuexingan06.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nx.shxzukj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gq.yuexingan06.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://op.haigaiapp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xl.muxihuayi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wz.panjiajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qh.hnjuh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vk.huanxung.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hg.bookmarksfly.cn

[C10] 变量作用域
来源：http://xq.nicolike.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://oj.nicolike.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mj.szxytkj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://np.nszjky.cn

TS:   同 JS
来源：http://dl.gzmigu.cn

Java: 方法内为块级作用域
来源：http://ra.haigaiapp.cn

Go:   花括号块级作用域
来源：http://gq.wgjwhj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gx.colortex.cn

C#:   块级作用域
来源：http://kr.panjiajie.cn

[C11] 模块导入与导出
来源：http://gl.jctech888.com.cn

Py:   from module import func
来源：http://nu.szsharing.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://fv.yuntaijiaju.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://nn.yuexingan06.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://te.yuexingan06.cn

Java: import java.util.List;
来源：http://yr.colortex.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sb.colortex.cn

Ruby: require "json"; require_relative "./util"
来源：http://ct.nicolike.cn

C#:   using System.Text;
来源：http://xk.muxihuayi.cn

[C12] 立即执行函数 IIFE
来源：http://px.bjjhwx.cn

Py:   (lambda: print("run"))()
来源：http://ol.shtwfgs.cn

PHP:  (function () { echo "run"; })();
来源：http://rb.wgjwhj.cn

JS:   (() => { console.log("run"); })();
来源：http://eo.yuexingan06.cn

TS:   (() => { console.log("run"); })();
来源：http://zf.haigaiapp.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://uc.nszjky.cn

Go:   func() { fmt.Println("run") }()
来源：http://yl.chemitech.net.cn

Ruby: -> { puts "run" }.call
来源：http://dy.bjjhwx.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ez.panjiajie.cn

[C13] 类型声明 / 类型注解
来源：http://dc.nszjky.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://en.muxihuayi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://au.colortex.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wn.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nb.yuexingan06.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ts.colortex.cn

Go:   func add(a, b int) int
来源：http://vq.panjiajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://no.yuexingan06.cn

C#:   int Add(int a, int b) => a + b;
来源：http://af.9csxet.cn


<!-- 参考信息 -->