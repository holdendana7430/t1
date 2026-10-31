代发 wailian999

C#:   s.Length
来源：http://iu.wgjwhj.cn

[A23] 大小写转换
来源：http://lv.gzmigu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://na.muxihuayi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jz.newstarts.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ox.haigaiapp.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fn.hnjuh.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ci.nicolike.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dl.haigaiapp.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mr.521024.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://df.hahajie.cn

[A24] 去除首尾空白
来源：http://ub.chemitech.net.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xn.hahajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dc.jctech888.com.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jl.nicolike.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tu.szxytkj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://sy.gzmigu.cn

Go:   strings.TrimSpace(s)
来源：http://dt.asd995.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rf.huanxung.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jj.panjiajie.cn

[A25] 字符串比较
来源：http://kp.yuexingan06.cn

Py:   s1 == s2; s1 != s2
来源：http://wd.szxytkj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ev.nicolike.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xk.szsharing.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://za.nszjky.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xm.shtwfgs.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fh.colortex.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://oz.huixiangedu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ee.shxzskj.cn

[A26] 类型转换总览
来源：http://fe.gzmigu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mi.yuexingan06.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vu.jctech888.com.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jo.jctech888.com.cn

TS:   Number() String() Boolean() x as number
来源：http://rc.bjjhwx.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pf.szxytkj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bv.muxihuayi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://jw.asd995.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nd.shtwfgs.cn

================================================================================
来源：http://vs.gzmigu.cn

B. 流程控制
来源：http://wa.colortex.cn

================================================================================
来源：http://ck.szxytkj.cn

[B01] 条件判断 if / else
来源：http://av.haigaiapp.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://qd.gzmigu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wc.shxzukj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kx.huanxung.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://au.hnjuh.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://pq.muxihuayi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://re.bookmarksfly.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lx.szsharing.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://do.haigaiapp.cn

[B02] 多分支 else if / elif
来源：http://uu.bookmarksfly.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pa.panjiajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xk.lnxyls.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dh.wgjwhj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zd.bjjhwx.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://de.chemitech.net.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://oj.haigaiapp.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fx.szsharing.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xt.shxzskj.cn

[B03] switch / match / case
来源：http://rp.panjiajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fz.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wz.asd995.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mx.szxytkj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wb.haigaiapp.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sv.szsharing.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wt.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://id.huixinmuqiang.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ev.shtwfgs.cn

[B04] for 计数循环
来源：http://it.lnxyls.cn

Py:   for i in range(10): print(i)
来源：http://em.bookmarksfly.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pm.nicolike.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mf.9csxet.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sj.9csxet.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ja.jianghongdianzi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wc.huanxung.cn

Ruby: 10.times { |i| puts i }
来源：http://ar.chemitech.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://li.bjjhwx.cn

[B05] 遍历数组 / 列表
来源：http://gy.huanxung.cn

Py:   for item in arr: print(item)
来源：http://gp.9csxet.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rl.yuexingan06.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zm.chemitech.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://cs.9csxet.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ax.szsharing.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://uc.szsharing.cn

Ruby: arr.each { |item| puts item }
来源：http://nk.lnxyls.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://md.hahajie.cn

[B06] 遍历字典 / 对象
来源：http://bk.muxihuayi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://eo.lnxyls.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://am.panjiajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hh.asd995.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://an.521024.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vf.wgjwhj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gp.asd995.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xi.muxihuayi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bg.lnxyls.cn

[B07] while 循环
来源：http://ar.nicolike.cn

Py:   while i < 10: i += 1
来源：http://ly.521024.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ui.nszjky.cn

JS:   while (i < 10) { i++; }
来源：http://tm.nicolike.cn

TS:   while (i < 10) { i++; }
来源：http://qy.bookmarksfly.cn

Java: while (i < 10) { i++; }
来源：http://sy.shxzskj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://en.huanxung.cn

Ruby: while i < 10; i += 1; end
来源：http://tz.szsharing.cn

C#:   while (i < 10) { i++; }
来源：http://le.shxzukj.cn

[B08] do-while（至少执行一次）
来源：http://sr.haigaiapp.cn

Py:   # 无 do-while：用 while True + break
来源：http://bp.huixiangedu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zu.szxytkj.cn

JS:   do { i++; } while (i < 10);
来源：http://oq.hahajie.cn

TS:   do { i++; } while (i < 10);
来源：http://xj.wgjwhj.cn

Java: do { i++; } while (i < 10);
来源：http://ws.newstarts.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://af.shxzukj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rk.panjiajie.cn

C#:   do { i++; } while (i < 10);
来源：http://ju.hnjuh.cn

[B09] break 与 continue
来源：http://rk.hahajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://oe.chemitech.net.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wm.bookmarksfly.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ol.colortex.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ee.muxihuayi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mq.yuntaijiaju.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ay.hnjuh.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dh.haigaiapp.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://po.bjjhwx.cn

[B10] 遍历同时拿索引
来源：http://ek.szxytkj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vx.newstarts.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tw.huixinmuqiang.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hv.colortex.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tg.colortex.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ym.shxzskj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fg.szxytkj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lj.szsharing.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://im.szxytkj.cn

[B11] 生成数字序列 / 区间
来源：http://kj.szsharing.cn

Py:   list(range(0, 10, 2))
来源：http://xo.yuexingan06.cn

PHP:  range(0, 10, 2);
来源：http://hv.nszjky.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uj.nszjky.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ks.yuntaijiaju.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cs.yuntaijiaju.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dj.jctech888.com.cn

Ruby: (0...10).step(2).to_a
来源：http://vw.lnxyls.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://db.hnjuh.cn

[B12] 跳出多层循环
来源：http://as.huixiangedu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://on.szxytkj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://qx.panjiajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fu.jctech888.com.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ja.bjjhwx.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sg.hahajie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vb.shtwfgs.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zj.szxytkj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bv.shxzskj.cn

[B13] 判断是否为数字
来源：http://ob.gzmigu.cn

Py:   isinstance(x, (int, float))
来源：http://yc.bjjhwx.cn

PHP:  is_numeric($x)
来源：http://gp.yuexingan06.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://as.szxytkj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://af.huanxung.cn

Java: x instanceof Number
来源：http://dm.panjiajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zx.haigaiapp.cn

Ruby: x.is_a?(Numeric)
来源：http://zj.muxihuayi.cn

C#:   x is int or double or decimal
来源：http://yp.huanxung.cn

[B14] 判断值是否在集合内
来源：http://oj.haigaiapp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qa.hnjuh.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xk.wgjwhj.cn

JS:   [1, 2, 3].includes(x)
来源：http://zi.gzmigu.cn

TS:   [1, 2, 3].includes(x)
来源：http://dm.lnxyls.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://tx.shxzukj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zq.huixinmuqiang.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ig.wgjwhj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qq.shxzukj.cn

[B15] 布尔运算与取反
来源：http://dz.haigaiapp.cn

Py:   a and b or not c
来源：http://wu.szsharing.cn

PHP:  $a && $b || !$c
来源：http://re.newstarts.cn

JS:   a && b || !c
来源：http://cz.yuexingan06.cn

TS:   a && b || !c
来源：http://ln.521024.cn

Java: a && b || !c
来源：http://pz.muxihuayi.cn

Go:   a && b || !c
来源：http://xl.nszjky.cn

Ruby: a && b || !c
来源：http://fh.lnxyls.cn

C#:   a && b || !c
来源：http://zp.hahajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://cr.jctech888.com.cn

Py:   if not data: return
来源：http://me.9csxet.cn

PHP:  if (!$data) { return; }
来源：http://kj.hahajie.cn

JS:   if (!data) return;
来源：http://ek.9csxet.cn

TS:   if (!data) return;
来源：http://rz.yuexingan06.cn

Java: if (data == null) return;
来源：http://ru.wgjwhj.cn

Go:   if data == nil { return }
来源：http://hs.9csxet.cn

Ruby: return if data.nil?
来源：http://sf.lnxyls.cn

C#:   if (data == null) return;
来源：http://iw.wgjwhj.cn

================================================================================
来源：http://yo.szxytkj.cn

C. 函数与作用域
来源：http://zb.521024.cn

================================================================================
来源：http://wx.haigaiapp.cn

[C01] 定义函数
来源：http://dn.colortex.cn

Py:   def add(a, b): return a + b
来源：http://ek.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zc.asd995.cn

JS:   function add(a, b) { return a + b; }
来源：http://je.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vg.shxzukj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xa.huanxung.cn

Go:   func add(a, b int) int { return a + b }
来源：http://if.nszjky.cn

Ruby: def add(a, b); a + b; end
来源：http://km.521024.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mi.jianghongdianzi.cn

[C02] 默认参数
来源：http://is.colortex.cn

Py:   def greet(name="World"): return name
来源：http://tk.9csxet.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://kh.yuexingan06.cn

JS:   function greet(name = "World") { return name; }
来源：http://rt.jianghongdianzi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vt.shtwfgs.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://iw.wgjwhj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ez.jianghongdianzi.cn

Ruby: def greet(name = "World") = name
来源：http://ho.huixiangedu.cn

C#:   string Greet(string name = "World") => name;
来源：http://tg.chemitech.net.cn

[C03] 可变参数
来源：http://tz.shtwfgs.cn

Py:   def total(*args): return sum(args)
来源：http://gs.shtwfgs.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gm.gzmigu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yr.nicolike.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ui.huanxung.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cd.jianghongdianzi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lu.asd995.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qo.jctech888.com.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ky.colortex.cn

[C04] 命名参数 / 关键字参数
来源：http://cf.asd995.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ty.bjjhwx.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ju.yuexingan06.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lq.huixiangedu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lk.huixiangedu.cn

Java: // 无：用 Builder 模式或 record
来源：http://ii.gzmigu.cn

Go:   // 无：用配置结构体参数
来源：http://lk.nszjky.cn

Ruby: f(a: 1, b: 2)
来源：http://sq.szxytkj.cn

C#:   f(a: 1, b: 2)
来源：http://wu.chemitech.net.cn

[C05] 返回多个值
来源：http://mb.gzmigu.cn

Py:   return a, b
来源：http://as.haigaiapp.cn

PHP:  return [$a, $b];
来源：http://bh.huanxung.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://nc.huixinmuqiang.cn

TS:   return { a, b };
来源：http://dg.shxzskj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xo.huixiangedu.cn

Go:   return a, b
来源：http://sg.lnxyls.cn

Ruby: return a, b
来源：http://ov.jctech888.com.cn

C#:   return (a, b);              // ValueTuple
来源：http://je.wgjwhj.cn

[C06] 匿名函数 / lambda
来源：http://jd.bookmarksfly.cn

Py:   square = lambda x: x * x
来源：http://tv.newstarts.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://jq.hahajie.cn

JS:   const square = x => x * x;
来源：http://kb.gzmigu.cn

TS:   const square = (x: number): number => x * x;
来源：http://ss.newstarts.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sp.gzmigu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ln.shxzskj.cn

Ruby: square = ->(x) { x * x }
来源：http://nb.chemitech.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ic.chemitech.net.cn

[C07] 把函数作为参数传入
来源：http://ul.jctech888.com.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ut.jctech888.com.cn

PHP:  array_map("strtoupper", $arr);
来源：http://qs.asd995.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uw.9csxet.cn

TS:   arr.map(String)
来源：http://wg.hnjuh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://oe.newstarts.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qy.colortex.cn

Ruby: arr.map(&:upcase)
来源：http://uz.jctech888.com.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gt.panjiajie.cn

[C08] 闭包
来源：http://re.shxzskj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ma.nicolike.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nj.haigaiapp.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vh.shxzskj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ek.huixiangedu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fo.haigaiapp.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vt.panjiajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uc.shtwfgs.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://my.jctech888.com.cn

[C09] 递归
来源：http://kc.chemitech.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://di.nicolike.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hc.nszjky.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wo.shtwfgs.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tl.hnjuh.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xq.asd995.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dv.nszjky.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://md.shtwfgs.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xv.hahajie.cn

[C10] 变量作用域
来源：http://tk.muxihuayi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hw.wgjwhj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rd.asd995.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zu.lnxyls.cn

TS:   同 JS
来源：http://qj.chemitech.net.cn

Java: 方法内为块级作用域
来源：http://wf.521024.cn

Go:   花括号块级作用域
来源：http://te.chemitech.net.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://th.bjjhwx.cn

C#:   块级作用域
来源：http://qd.nszjky.cn

[C11] 模块导入与导出
来源：http://az.shxzskj.cn

Py:   from module import func
来源：http://sf.bjjhwx.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://st.haigaiapp.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ts.lnxyls.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kh.9csxet.cn

Java: import java.util.List;
来源：http://al.gzmigu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ne.521024.cn

Ruby: require "json"; require_relative "./util"
来源：http://vb.szxytkj.cn

C#:   using System.Text;
来源：http://gb.nszjky.cn

[C12] 立即执行函数 IIFE
来源：http://gu.newstarts.cn

Py:   (lambda: print("run"))()
来源：http://qh.shxzskj.cn

PHP:  (function () { echo "run"; })();
来源：http://vi.jianghongdianzi.cn

JS:   (() => { console.log("run"); })();
来源：http://bd.chemitech.net.cn

TS:   (() => { console.log("run"); })();
来源：http://oy.nicolike.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://er.lnxyls.cn

Go:   func() { fmt.Println("run") }()
来源：http://hs.nicolike.cn

Ruby: -> { puts "run" }.call
来源：http://ol.huixiangedu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://hi.newstarts.cn

[C13] 类型声明 / 类型注解
来源：http://pu.hahajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xt.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vo.nszjky.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cb.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ri.huixiangedu.cn


<!-- 参考信息 -->