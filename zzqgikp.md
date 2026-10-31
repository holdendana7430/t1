代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://js.asd995.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tt.bookmarksfly.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ok.521024.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pr.panjiajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://il.jctech888.com.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://jf.huixiangedu.cn

[A24] 去除首尾空白
来源：http://au.yuexingan06.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lm.haigaiapp.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vg.panjiajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yi.bookmarksfly.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://en.asd995.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://es.jctech888.com.cn

Go:   strings.TrimSpace(s)
来源：http://ql.haigaiapp.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ub.wgjwhj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lx.gzmigu.cn

[A25] 字符串比较
来源：http://ks.shxzukj.cn

Py:   s1 == s2; s1 != s2
来源：http://wl.9csxet.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sc.shxzskj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ht.shtwfgs.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jo.asd995.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://po.asd995.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wn.yuexingan06.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ma.bjjhwx.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zi.panjiajie.cn

[A26] 类型转换总览
来源：http://jv.muxihuayi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vk.yuntaijiaju.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://oh.yuexingan06.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://lg.nicolike.cn

TS:   Number() String() Boolean() x as number
来源：http://pi.huixinmuqiang.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tb.colortex.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cg.haigaiapp.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://sp.newstarts.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jm.yuntaijiaju.cn

================================================================================
来源：http://vh.shxzukj.cn

B. 流程控制
来源：http://sz.huixiangedu.cn

================================================================================
来源：http://ua.haigaiapp.cn

[B01] 条件判断 if / else
来源：http://vs.lnxyls.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://qh.gzmigu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bj.gzmigu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gg.lnxyls.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xy.wgjwhj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://nf.yuntaijiaju.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ja.newstarts.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fg.hnjuh.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ds.newstarts.cn

[B02] 多分支 else if / elif
来源：http://pc.hnjuh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bx.lnxyls.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wd.szxytkj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tj.chemitech.net.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nl.huanxung.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jp.bookmarksfly.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zo.jctech888.com.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nq.szxytkj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uo.bjjhwx.cn

[B03] switch / match / case
来源：http://if.newstarts.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lp.wgjwhj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xn.nszjky.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xi.wgjwhj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jo.newstarts.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zh.yuntaijiaju.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gv.colortex.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jt.shxzskj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yt.yuexingan06.cn

[B04] for 计数循环
来源：http://qx.wgjwhj.cn

Py:   for i in range(10): print(i)
来源：http://qt.9csxet.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vy.yuexingan06.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rw.jctech888.com.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zk.jctech888.com.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ci.shxzskj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ta.521024.cn

Ruby: 10.times { |i| puts i }
来源：http://az.chemitech.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ew.nszjky.cn

[B05] 遍历数组 / 列表
来源：http://wq.newstarts.cn

Py:   for item in arr: print(item)
来源：http://cl.nicolike.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cj.lnxyls.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://as.asd995.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://dh.nszjky.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://py.huixiangedu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wa.szsharing.cn

Ruby: arr.each { |item| puts item }
来源：http://qy.shtwfgs.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tj.gzmigu.cn

[B06] 遍历字典 / 对象
来源：http://yu.9csxet.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://py.gzmigu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qv.huixiangedu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ek.gzmigu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hm.9csxet.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rn.huanxung.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ij.shtwfgs.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ab.bjjhwx.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://es.yuntaijiaju.cn

[B07] while 循环
来源：http://ka.shxzskj.cn

Py:   while i < 10: i += 1
来源：http://vw.huixinmuqiang.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ww.shxzukj.cn

JS:   while (i < 10) { i++; }
来源：http://lw.521024.cn

TS:   while (i < 10) { i++; }
来源：http://vd.hahajie.cn

Java: while (i < 10) { i++; }
来源：http://iv.nicolike.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uw.huanxung.cn

Ruby: while i < 10; i += 1; end
来源：http://pq.huixinmuqiang.cn

C#:   while (i < 10) { i++; }
来源：http://nq.szsharing.cn

[B08] do-while（至少执行一次）
来源：http://ik.asd995.cn

Py:   # 无 do-while：用 while True + break
来源：http://qt.521024.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://hj.gzmigu.cn

JS:   do { i++; } while (i < 10);
来源：http://qd.szxytkj.cn

TS:   do { i++; } while (i < 10);
来源：http://tc.jctech888.com.cn

Java: do { i++; } while (i < 10);
来源：http://mt.asd995.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://nh.lnxyls.cn

Ruby: begin; i += 1; end while i < 10
来源：http://tk.panjiajie.cn

C#:   do { i++; } while (i < 10);
来源：http://tb.shxzskj.cn

[B09] break 与 continue
来源：http://az.szsharing.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bj.gzmigu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zb.521024.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lg.colortex.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sn.lnxyls.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mu.hahajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fa.panjiajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qz.huanxung.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lk.huanxung.cn

[B10] 遍历同时拿索引
来源：http://cd.hahajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ud.huanxung.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pn.wgjwhj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ly.lnxyls.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wm.jctech888.com.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://aa.panjiajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cp.shxzukj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://on.nszjky.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xb.9csxet.cn

[B11] 生成数字序列 / 区间
来源：http://gu.bookmarksfly.cn

Py:   list(range(0, 10, 2))
来源：http://gy.colortex.cn

PHP:  range(0, 10, 2);
来源：http://ik.shxzukj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xj.newstarts.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jf.jctech888.com.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jj.colortex.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zj.jctech888.com.cn

Ruby: (0...10).step(2).to_a
来源：http://yu.hnjuh.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rc.9csxet.cn

[B12] 跳出多层循环
来源：http://rq.huixiangedu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hn.jianghongdianzi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://iu.yuntaijiaju.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yk.nszjky.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kh.yuexingan06.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rl.muxihuayi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dg.wgjwhj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://be.hnjuh.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dn.bjjhwx.cn

[B13] 判断是否为数字
来源：http://ls.lnxyls.cn

Py:   isinstance(x, (int, float))
来源：http://eh.jctech888.com.cn

PHP:  is_numeric($x)
来源：http://xc.newstarts.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ry.asd995.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://no.shxzukj.cn

Java: x instanceof Number
来源：http://oj.bookmarksfly.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rd.huixiangedu.cn

Ruby: x.is_a?(Numeric)
来源：http://or.szsharing.cn

C#:   x is int or double or decimal
来源：http://qd.9csxet.cn

[B14] 判断值是否在集合内
来源：http://iq.muxihuayi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://co.hahajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yd.newstarts.cn

JS:   [1, 2, 3].includes(x)
来源：http://ba.nicolike.cn

TS:   [1, 2, 3].includes(x)
来源：http://re.yuexingan06.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://nl.yuntaijiaju.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hu.huixinmuqiang.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fy.gzmigu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zq.9csxet.cn

[B15] 布尔运算与取反
来源：http://gz.colortex.cn

Py:   a and b or not c
来源：http://fy.jctech888.com.cn

PHP:  $a && $b || !$c
来源：http://ul.jianghongdianzi.cn

JS:   a && b || !c
来源：http://iq.bjjhwx.cn

TS:   a && b || !c
来源：http://ey.huanxung.cn

Java: a && b || !c
来源：http://az.jctech888.com.cn

Go:   a && b || !c
来源：http://uq.huixinmuqiang.cn

Ruby: a && b || !c
来源：http://ad.szsharing.cn

C#:   a && b || !c
来源：http://ma.shxzukj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://be.yuexingan06.cn

Py:   if not data: return
来源：http://jp.szsharing.cn

PHP:  if (!$data) { return; }
来源：http://lp.jianghongdianzi.cn

JS:   if (!data) return;
来源：http://eb.521024.cn

TS:   if (!data) return;
来源：http://xh.lnxyls.cn

Java: if (data == null) return;
来源：http://yl.chemitech.net.cn

Go:   if data == nil { return }
来源：http://ik.panjiajie.cn

Ruby: return if data.nil?
来源：http://so.haigaiapp.cn

C#:   if (data == null) return;
来源：http://cs.gzmigu.cn

================================================================================
来源：http://jo.bjjhwx.cn

C. 函数与作用域
来源：http://nd.muxihuayi.cn

================================================================================
来源：http://wd.muxihuayi.cn

[C01] 定义函数
来源：http://ri.huanxung.cn

Py:   def add(a, b): return a + b
来源：http://kr.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cj.muxihuayi.cn

JS:   function add(a, b) { return a + b; }
来源：http://xn.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pm.huanxung.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://tg.nicolike.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zc.colortex.cn

Ruby: def add(a, b); a + b; end
来源：http://yn.yuexingan06.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wc.asd995.cn

[C02] 默认参数
来源：http://ja.panjiajie.cn

Py:   def greet(name="World"): return name
来源：http://iv.jianghongdianzi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fg.muxihuayi.cn

JS:   function greet(name = "World") { return name; }
来源：http://cq.yuntaijiaju.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fm.szsharing.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ha.szxytkj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dp.521024.cn

Ruby: def greet(name = "World") = name
来源：http://gn.hnjuh.cn

C#:   string Greet(string name = "World") => name;
来源：http://nm.lnxyls.cn

[C03] 可变参数
来源：http://yf.shxzukj.cn

Py:   def total(*args): return sum(args)
来源：http://ql.haigaiapp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vp.chemitech.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bq.szsharing.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fx.huanxung.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dm.bjjhwx.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yw.yuntaijiaju.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hl.hnjuh.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://im.panjiajie.cn

[C04] 命名参数 / 关键字参数
来源：http://sz.521024.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ir.yuntaijiaju.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ho.newstarts.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fv.szsharing.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nd.gzmigu.cn

Java: // 无：用 Builder 模式或 record
来源：http://wb.szsharing.cn

Go:   // 无：用配置结构体参数
来源：http://da.muxihuayi.cn

Ruby: f(a: 1, b: 2)
来源：http://hp.9csxet.cn

C#:   f(a: 1, b: 2)
来源：http://gx.9csxet.cn

[C05] 返回多个值
来源：http://xp.newstarts.cn

Py:   return a, b
来源：http://tu.bjjhwx.cn

PHP:  return [$a, $b];
来源：http://ww.yuexingan06.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vq.hahajie.cn

TS:   return { a, b };
来源：http://qg.bookmarksfly.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fn.jctech888.com.cn

Go:   return a, b
来源：http://kk.shtwfgs.cn

Ruby: return a, b
来源：http://mj.jctech888.com.cn

C#:   return (a, b);              // ValueTuple
来源：http://za.huixiangedu.cn

[C06] 匿名函数 / lambda
来源：http://mg.shxzskj.cn

Py:   square = lambda x: x * x
来源：http://ow.yuexingan06.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://hi.nszjky.cn

JS:   const square = x => x * x;
来源：http://jg.panjiajie.cn

TS:   const square = (x: number): number => x * x;
来源：http://dr.gzmigu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xb.shxzskj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://tl.newstarts.cn

Ruby: square = ->(x) { x * x }
来源：http://sz.szsharing.cn

C#:   Func<int, int> square = x => x * x;
来源：http://yz.bjjhwx.cn

[C07] 把函数作为参数传入
来源：http://je.lnxyls.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pv.gzmigu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://pe.yuexingan06.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vz.bjjhwx.cn

TS:   arr.map(String)
来源：http://mc.521024.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ir.huanxung.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jc.shxzskj.cn

Ruby: arr.map(&:upcase)
来源：http://cc.bookmarksfly.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://bx.gzmigu.cn

[C08] 闭包
来源：http://kr.muxihuayi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://re.nszjky.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vh.gzmigu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vg.bjjhwx.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kg.huixiangedu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bx.szsharing.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://my.wgjwhj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://il.bookmarksfly.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://on.bjjhwx.cn

[C09] 递归
来源：http://lm.bjjhwx.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fj.shtwfgs.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hg.huanxung.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vv.bookmarksfly.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kn.521024.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jd.hnjuh.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rh.asd995.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://py.shxzukj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nu.shxzskj.cn

[C10] 变量作用域
来源：http://zg.nicolike.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jw.wgjwhj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://er.panjiajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qn.yuntaijiaju.cn

TS:   同 JS
来源：http://wq.panjiajie.cn

Java: 方法内为块级作用域
来源：http://jk.shtwfgs.cn

Go:   花括号块级作用域
来源：http://sf.jianghongdianzi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ht.9csxet.cn

C#:   块级作用域
来源：http://ag.panjiajie.cn

[C11] 模块导入与导出
来源：http://qu.haigaiapp.cn

Py:   from module import func
来源：http://gg.521024.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bx.yuexingan06.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://op.gzmigu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qf.shxzukj.cn

Java: import java.util.List;
来源：http://au.yuexingan06.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qd.9csxet.cn

Ruby: require "json"; require_relative "./util"
来源：http://fy.asd995.cn

C#:   using System.Text;
来源：http://oe.szxytkj.cn

[C12] 立即执行函数 IIFE
来源：http://ir.muxihuayi.cn

Py:   (lambda: print("run"))()
来源：http://ej.gzmigu.cn

PHP:  (function () { echo "run"; })();
来源：http://jp.9csxet.cn

JS:   (() => { console.log("run"); })();
来源：http://ra.bjjhwx.cn

TS:   (() => { console.log("run"); })();
来源：http://yf.wgjwhj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gp.szsharing.cn

Go:   func() { fmt.Println("run") }()
来源：http://fv.huixiangedu.cn

Ruby: -> { puts "run" }.call
来源：http://tw.muxihuayi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fk.nicolike.cn

[C13] 类型声明 / 类型注解
来源：http://wq.newstarts.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jy.haigaiapp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lt.nicolike.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rx.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vn.muxihuayi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ap.jctech888.com.cn

Go:   func add(a, b int) int
来源：http://yq.jianghongdianzi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ql.nicolike.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cm.lnxyls.cn


<!-- 参考信息 -->