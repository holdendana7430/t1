代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mx.gzmigu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ta.huixinmuqiang.cn

[A24] 去除首尾空白
来源：http://km.jianghongdianzi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gl.hahajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fg.yuntaijiaju.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kh.asd995.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cf.hnjuh.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ye.gzmigu.cn

Go:   strings.TrimSpace(s)
来源：http://vr.asd995.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dg.hahajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://um.jianghongdianzi.cn

[A25] 字符串比较
来源：http://ax.jctech888.com.cn

Py:   s1 == s2; s1 != s2
来源：http://ol.chemitech.net.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xo.panjiajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rz.asd995.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://le.newstarts.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xo.521024.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vg.asd995.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://sj.hnjuh.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pq.colortex.cn

[A26] 类型转换总览
来源：http://oj.521024.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hl.yuexingan06.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://iu.huixiangedu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xn.bjjhwx.cn

TS:   Number() String() Boolean() x as number
来源：http://fh.gzmigu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hg.lnxyls.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://af.haigaiapp.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://dh.shxzukj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tk.newstarts.cn

================================================================================
来源：http://vp.hnjuh.cn

B. 流程控制
来源：http://pl.jctech888.com.cn

================================================================================
来源：http://rn.colortex.cn

[B01] 条件判断 if / else
来源：http://lr.9csxet.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ed.haigaiapp.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vw.gzmigu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zv.yuexingan06.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://id.muxihuayi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://hm.gzmigu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ju.szxytkj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bx.lnxyls.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qm.huixiangedu.cn

[B02] 多分支 else if / elif
来源：http://zu.panjiajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://un.nszjky.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lw.bjjhwx.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tn.wgjwhj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jy.hnjuh.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ew.chemitech.net.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ow.wgjwhj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rh.asd995.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zu.asd995.cn

[B03] switch / match / case
来源：http://fd.yuntaijiaju.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lu.521024.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uq.yuexingan06.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://am.wgjwhj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xk.yuexingan06.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zg.lnxyls.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rc.bookmarksfly.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dc.shxzukj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pj.chemitech.net.cn

[B04] for 计数循环
来源：http://um.newstarts.cn

Py:   for i in range(10): print(i)
来源：http://kq.9csxet.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qx.hnjuh.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tx.jctech888.com.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ew.jctech888.com.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mc.nszjky.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bb.yuntaijiaju.cn

Ruby: 10.times { |i| puts i }
来源：http://jb.hahajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yc.521024.cn

[B05] 遍历数组 / 列表
来源：http://zr.muxihuayi.cn

Py:   for item in arr: print(item)
来源：http://oe.nszjky.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bt.jctech888.com.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://rn.panjiajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://kx.newstarts.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://if.jctech888.com.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ye.jctech888.com.cn

Ruby: arr.each { |item| puts item }
来源：http://aw.chemitech.net.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fo.szxytkj.cn

[B06] 遍历字典 / 对象
来源：http://uq.huixinmuqiang.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://lt.lnxyls.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hg.szsharing.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zc.gzmigu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wc.nszjky.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xs.newstarts.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nn.lnxyls.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nx.yuexingan06.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mg.huixinmuqiang.cn

[B07] while 循环
来源：http://ya.huixiangedu.cn

Py:   while i < 10: i += 1
来源：http://gj.huixinmuqiang.cn

PHP:  while ($i < 10) { $i++; }
来源：http://kp.panjiajie.cn

JS:   while (i < 10) { i++; }
来源：http://gp.newstarts.cn

TS:   while (i < 10) { i++; }
来源：http://to.gzmigu.cn

Java: while (i < 10) { i++; }
来源：http://bf.yuntaijiaju.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://oh.gzmigu.cn

Ruby: while i < 10; i += 1; end
来源：http://fs.muxihuayi.cn

C#:   while (i < 10) { i++; }
来源：http://qw.szxytkj.cn

[B08] do-while（至少执行一次）
来源：http://kl.colortex.cn

Py:   # 无 do-while：用 while True + break
来源：http://yh.nicolike.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://br.haigaiapp.cn

JS:   do { i++; } while (i < 10);
来源：http://pd.shxzskj.cn

TS:   do { i++; } while (i < 10);
来源：http://ag.panjiajie.cn

Java: do { i++; } while (i < 10);
来源：http://xk.9csxet.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://lz.jctech888.com.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xy.nszjky.cn

C#:   do { i++; } while (i < 10);
来源：http://jp.nszjky.cn

[B09] break 与 continue
来源：http://mq.jctech888.com.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sm.bjjhwx.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kx.lnxyls.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rz.gzmigu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qf.shxzskj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dz.hnjuh.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qz.wgjwhj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hb.szxytkj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://za.huanxung.cn

[B10] 遍历同时拿索引
来源：http://et.huixiangedu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zl.asd995.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lq.haigaiapp.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vx.bookmarksfly.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dj.wgjwhj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hu.colortex.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dk.yuexingan06.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fm.wgjwhj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yy.yuntaijiaju.cn

[B11] 生成数字序列 / 区间
来源：http://ga.bookmarksfly.cn

Py:   list(range(0, 10, 2))
来源：http://bz.hahajie.cn

PHP:  range(0, 10, 2);
来源：http://sq.huanxung.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vb.wgjwhj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xz.nicolike.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ke.hnjuh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://uf.bjjhwx.cn

Ruby: (0...10).step(2).to_a
来源：http://oy.asd995.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bw.szsharing.cn

[B12] 跳出多层循环
来源：http://hx.nicolike.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://lp.521024.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ln.shtwfgs.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ur.muxihuayi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ob.jctech888.com.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://id.bookmarksfly.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ye.9csxet.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qf.jianghongdianzi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hs.jctech888.com.cn

[B13] 判断是否为数字
来源：http://kc.shxzskj.cn

Py:   isinstance(x, (int, float))
来源：http://cp.lnxyls.cn

PHP:  is_numeric($x)
来源：http://qk.shxzukj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yf.nszjky.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tp.chemitech.net.cn

Java: x instanceof Number
来源：http://dm.asd995.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://su.panjiajie.cn

Ruby: x.is_a?(Numeric)
来源：http://un.nszjky.cn

C#:   x is int or double or decimal
来源：http://ab.wgjwhj.cn

[B14] 判断值是否在集合内
来源：http://ms.newstarts.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kf.szxytkj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://el.haigaiapp.cn

JS:   [1, 2, 3].includes(x)
来源：http://bv.huanxung.cn

TS:   [1, 2, 3].includes(x)
来源：http://zy.lnxyls.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://jh.newstarts.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mt.yuntaijiaju.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qy.hahajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xq.gzmigu.cn

[B15] 布尔运算与取反
来源：http://zj.chemitech.net.cn

Py:   a and b or not c
来源：http://gs.huanxung.cn

PHP:  $a && $b || !$c
来源：http://sh.wgjwhj.cn

JS:   a && b || !c
来源：http://lc.szsharing.cn

TS:   a && b || !c
来源：http://go.jctech888.com.cn

Java: a && b || !c
来源：http://yb.gzmigu.cn

Go:   a && b || !c
来源：http://ts.hnjuh.cn

Ruby: a && b || !c
来源：http://af.wgjwhj.cn

C#:   a && b || !c
来源：http://rj.shtwfgs.cn

[B16] 卫语句：不满足条件提前返回
来源：http://py.huixiangedu.cn

Py:   if not data: return
来源：http://rd.lnxyls.cn

PHP:  if (!$data) { return; }
来源：http://nv.hnjuh.cn

JS:   if (!data) return;
来源：http://rg.asd995.cn

TS:   if (!data) return;
来源：http://zb.panjiajie.cn

Java: if (data == null) return;
来源：http://wk.9csxet.cn

Go:   if data == nil { return }
来源：http://hu.chemitech.net.cn

Ruby: return if data.nil?
来源：http://sh.9csxet.cn

C#:   if (data == null) return;
来源：http://wh.muxihuayi.cn

================================================================================
来源：http://nq.nicolike.cn

C. 函数与作用域
来源：http://hs.newstarts.cn

================================================================================
来源：http://iq.chemitech.net.cn

[C01] 定义函数
来源：http://fy.shxzukj.cn

Py:   def add(a, b): return a + b
来源：http://sq.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qh.hnjuh.cn

JS:   function add(a, b) { return a + b; }
来源：http://xc.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iu.jctech888.com.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fz.nszjky.cn

Go:   func add(a, b int) int { return a + b }
来源：http://sw.yuexingan06.cn

Ruby: def add(a, b); a + b; end
来源：http://vh.hnjuh.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dz.jctech888.com.cn

[C02] 默认参数
来源：http://aq.hahajie.cn

Py:   def greet(name="World"): return name
来源：http://xw.jctech888.com.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bn.bookmarksfly.cn

JS:   function greet(name = "World") { return name; }
来源：http://ri.asd995.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qe.yuntaijiaju.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://sr.yuexingan06.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qb.huanxung.cn

Ruby: def greet(name = "World") = name
来源：http://mc.jctech888.com.cn

C#:   string Greet(string name = "World") => name;
来源：http://ts.yuntaijiaju.cn

[C03] 可变参数
来源：http://vu.colortex.cn

Py:   def total(*args): return sum(args)
来源：http://mv.haigaiapp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ay.gzmigu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://go.jctech888.com.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fx.bookmarksfly.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mq.jianghongdianzi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hv.jctech888.com.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vq.shxzukj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://te.huanxung.cn

[C04] 命名参数 / 关键字参数
来源：http://jv.szsharing.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pj.chemitech.net.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jg.9csxet.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wr.huixiangedu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kr.yuntaijiaju.cn

Java: // 无：用 Builder 模式或 record
来源：http://xj.huanxung.cn

Go:   // 无：用配置结构体参数
来源：http://iy.colortex.cn

Ruby: f(a: 1, b: 2)
来源：http://fq.9csxet.cn

C#:   f(a: 1, b: 2)
来源：http://rw.colortex.cn

[C05] 返回多个值
来源：http://dj.jctech888.com.cn

Py:   return a, b
来源：http://ep.shtwfgs.cn

PHP:  return [$a, $b];
来源：http://js.hahajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zz.jianghongdianzi.cn

TS:   return { a, b };
来源：http://um.chemitech.net.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fg.yuexingan06.cn

Go:   return a, b
来源：http://xz.shxzskj.cn

Ruby: return a, b
来源：http://md.nicolike.cn

C#:   return (a, b);              // ValueTuple
来源：http://mg.gzmigu.cn

[C06] 匿名函数 / lambda
来源：http://qr.nicolike.cn

Py:   square = lambda x: x * x
来源：http://rv.haigaiapp.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bq.521024.cn

JS:   const square = x => x * x;
来源：http://ep.huanxung.cn

TS:   const square = (x: number): number => x * x;
来源：http://yy.521024.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ea.yuexingan06.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ej.newstarts.cn

Ruby: square = ->(x) { x * x }
来源：http://zj.yuntaijiaju.cn

C#:   Func<int, int> square = x => x * x;
来源：http://iq.bookmarksfly.cn

[C07] 把函数作为参数传入
来源：http://bg.muxihuayi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vb.9csxet.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kt.shxzskj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ju.panjiajie.cn

TS:   arr.map(String)
来源：http://zy.haigaiapp.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ai.huanxung.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yd.yuntaijiaju.cn

Ruby: arr.map(&:upcase)
来源：http://kh.yuntaijiaju.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jw.bjjhwx.cn

[C08] 闭包
来源：http://gu.lnxyls.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wr.colortex.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ch.jctech888.com.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ve.jctech888.com.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ha.9csxet.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ll.hnjuh.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qw.bjjhwx.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gc.lnxyls.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dd.jctech888.com.cn

[C09] 递归
来源：http://so.521024.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wy.bjjhwx.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ny.shxzskj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dz.asd995.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ow.huixiangedu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://co.gzmigu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ul.haigaiapp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wt.shxzskj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jp.huixiangedu.cn

[C10] 变量作用域
来源：http://jr.shxzskj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ug.szxytkj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xf.colortex.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fn.9csxet.cn

TS:   同 JS
来源：http://ys.jianghongdianzi.cn

Java: 方法内为块级作用域
来源：http://il.9csxet.cn

Go:   花括号块级作用域
来源：http://cf.jctech888.com.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ix.haigaiapp.cn

C#:   块级作用域
来源：http://jl.nszjky.cn

[C11] 模块导入与导出
来源：http://bi.newstarts.cn

Py:   from module import func
来源：http://br.huanxung.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bt.huanxung.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vc.colortex.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://au.jianghongdianzi.cn

Java: import java.util.List;
来源：http://pr.yuexingan06.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sd.9csxet.cn

Ruby: require "json"; require_relative "./util"
来源：http://mb.jctech888.com.cn

C#:   using System.Text;
来源：http://dp.bookmarksfly.cn

[C12] 立即执行函数 IIFE
来源：http://os.nicolike.cn

Py:   (lambda: print("run"))()
来源：http://ky.haigaiapp.cn

PHP:  (function () { echo "run"; })();
来源：http://nw.szxytkj.cn

JS:   (() => { console.log("run"); })();
来源：http://kc.colortex.cn

TS:   (() => { console.log("run"); })();
来源：http://vv.huanxung.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pg.yuntaijiaju.cn

Go:   func() { fmt.Println("run") }()
来源：http://ej.muxihuayi.cn

Ruby: -> { puts "run" }.call
来源：http://tb.shxzskj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ls.jianghongdianzi.cn

[C13] 类型声明 / 类型注解
来源：http://qg.newstarts.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wp.hahajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dw.lnxyls.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vw.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xk.jctech888.com.cn

Java: int add(int a, int b) { return a + b; }
来源：http://sw.chemitech.net.cn

Go:   func add(a, b int) int
来源：http://yz.jianghongdianzi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ng.wgjwhj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cv.521024.cn

[C14] 泛型函数
来源：http://ie.colortex.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ee.bjjhwx.cn

PHP:  // 无泛型
来源：http://ku.bookmarksfly.cn

JS:   // 无泛型
来源：http://lb.jctech888.com.cn


<!-- 参考信息 -->