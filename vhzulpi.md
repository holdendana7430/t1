代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://st.huixinmuqiang.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rl.muxihuayi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://to.wgjwhj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ce.colortex.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://av.szxytkj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://bu.yuexingan06.cn

[A24] 去除首尾空白
来源：http://mk.shtwfgs.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xn.huixiangedu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cf.shxzukj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jk.huixinmuqiang.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vw.yuexingan06.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mr.panjiajie.cn

Go:   strings.TrimSpace(s)
来源：http://ud.haigaiapp.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hg.shxzskj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wk.szsharing.cn

[A25] 字符串比较
来源：http://oo.yuntaijiaju.cn

Py:   s1 == s2; s1 != s2
来源：http://vt.asd995.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sa.wgjwhj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qa.colortex.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kn.huixiangedu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ea.gzmigu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yb.szsharing.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://je.newstarts.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kq.jianghongdianzi.cn

[A26] 类型转换总览
来源：http://an.bjjhwx.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zr.yuexingan06.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vr.chemitech.net.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ep.szsharing.cn

TS:   Number() String() Boolean() x as number
来源：http://cn.yuexingan06.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lt.bookmarksfly.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jf.yuntaijiaju.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://bz.jianghongdianzi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wc.yuntaijiaju.cn

================================================================================
来源：http://xv.shxzskj.cn

B. 流程控制
来源：http://mp.panjiajie.cn

================================================================================
来源：http://zj.yuntaijiaju.cn

[B01] 条件判断 if / else
来源：http://lq.gzmigu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://om.shxzukj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ev.nszjky.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jk.521024.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fb.yuexingan06.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://of.nicolike.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zj.haigaiapp.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://og.bookmarksfly.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fo.yuexingan06.cn

[B02] 多分支 else if / elif
来源：http://bi.9csxet.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dt.szxytkj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ck.9csxet.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lp.521024.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zn.bookmarksfly.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tf.huanxung.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tv.haigaiapp.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hn.9csxet.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pn.jctech888.com.cn

[B03] switch / match / case
来源：http://mg.wgjwhj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tt.bjjhwx.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zc.wgjwhj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xd.szxytkj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zs.yuexingan06.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ve.hnjuh.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://eg.panjiajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uw.huanxung.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://be.shxzukj.cn

[B04] for 计数循环
来源：http://qw.asd995.cn

Py:   for i in range(10): print(i)
来源：http://jc.shtwfgs.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://id.gzmigu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nv.muxihuayi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wo.wgjwhj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ne.huixiangedu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qr.panjiajie.cn

Ruby: 10.times { |i| puts i }
来源：http://hd.huixiangedu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://px.newstarts.cn

[B05] 遍历数组 / 列表
来源：http://zo.521024.cn

Py:   for item in arr: print(item)
来源：http://yg.chemitech.net.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://to.9csxet.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://mm.yuexingan06.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://jg.nszjky.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ch.yuntaijiaju.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zu.nszjky.cn

Ruby: arr.each { |item| puts item }
来源：http://vz.huixiangedu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kz.haigaiapp.cn

[B06] 遍历字典 / 对象
来源：http://gv.asd995.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://oq.jianghongdianzi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://iw.lnxyls.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hr.chemitech.net.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gm.hahajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dc.hahajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://by.9csxet.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yr.wgjwhj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://oo.lnxyls.cn

[B07] while 循环
来源：http://eo.nicolike.cn

Py:   while i < 10: i += 1
来源：http://mh.haigaiapp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zh.haigaiapp.cn

JS:   while (i < 10) { i++; }
来源：http://mo.yuexingan06.cn

TS:   while (i < 10) { i++; }
来源：http://qw.jianghongdianzi.cn

Java: while (i < 10) { i++; }
来源：http://qa.haigaiapp.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sa.panjiajie.cn

Ruby: while i < 10; i += 1; end
来源：http://wb.colortex.cn

C#:   while (i < 10) { i++; }
来源：http://mx.yuexingan06.cn

[B08] do-while（至少执行一次）
来源：http://da.shxzskj.cn

Py:   # 无 do-while：用 while True + break
来源：http://hs.szxytkj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://fi.521024.cn

JS:   do { i++; } while (i < 10);
来源：http://gs.yuntaijiaju.cn

TS:   do { i++; } while (i < 10);
来源：http://ya.huixinmuqiang.cn

Java: do { i++; } while (i < 10);
来源：http://nr.gzmigu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wb.haigaiapp.cn

Ruby: begin; i += 1; end while i < 10
来源：http://af.hahajie.cn

C#:   do { i++; } while (i < 10);
来源：http://ln.gzmigu.cn

[B09] break 与 continue
来源：http://km.shxzukj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yh.yuntaijiaju.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lb.huanxung.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uy.jctech888.com.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ry.nszjky.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lk.chemitech.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jp.gzmigu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://eh.shxzskj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lw.panjiajie.cn

[B10] 遍历同时拿索引
来源：http://bq.521024.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mx.huanxung.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mp.bookmarksfly.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ck.panjiajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ya.gzmigu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fq.jianghongdianzi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rm.9csxet.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wz.hnjuh.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://io.shxzukj.cn

[B11] 生成数字序列 / 区间
来源：http://zy.shxzukj.cn

Py:   list(range(0, 10, 2))
来源：http://pp.bjjhwx.cn

PHP:  range(0, 10, 2);
来源：http://hr.muxihuayi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yc.szxytkj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tt.muxihuayi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rw.521024.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://oi.shtwfgs.cn

Ruby: (0...10).step(2).to_a
来源：http://uk.huixiangedu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vh.521024.cn

[B12] 跳出多层循环
来源：http://ak.nszjky.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://oj.wgjwhj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://dq.yuexingan06.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wa.bookmarksfly.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pm.bjjhwx.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xi.hnjuh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fc.jianghongdianzi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ms.panjiajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nr.521024.cn

[B13] 判断是否为数字
来源：http://qx.huanxung.cn

Py:   isinstance(x, (int, float))
来源：http://lf.szsharing.cn

PHP:  is_numeric($x)
来源：http://au.asd995.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xy.yuexingan06.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bl.hahajie.cn

Java: x instanceof Number
来源：http://uw.wgjwhj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kw.panjiajie.cn

Ruby: x.is_a?(Numeric)
来源：http://vk.haigaiapp.cn

C#:   x is int or double or decimal
来源：http://oy.wgjwhj.cn

[B14] 判断值是否在集合内
来源：http://fy.nicolike.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pu.bookmarksfly.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://br.9csxet.cn

JS:   [1, 2, 3].includes(x)
来源：http://ts.wgjwhj.cn

TS:   [1, 2, 3].includes(x)
来源：http://aa.hahajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ux.szxytkj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sp.chemitech.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://tl.jianghongdianzi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ah.muxihuayi.cn

[B15] 布尔运算与取反
来源：http://xs.jctech888.com.cn

Py:   a and b or not c
来源：http://eg.shtwfgs.cn

PHP:  $a && $b || !$c
来源：http://by.bookmarksfly.cn

JS:   a && b || !c
来源：http://kc.colortex.cn

TS:   a && b || !c
来源：http://mb.521024.cn

Java: a && b || !c
来源：http://gl.jctech888.com.cn

Go:   a && b || !c
来源：http://es.bjjhwx.cn

Ruby: a && b || !c
来源：http://zn.gzmigu.cn

C#:   a && b || !c
来源：http://sm.hahajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fn.nicolike.cn

Py:   if not data: return
来源：http://ag.shxzskj.cn

PHP:  if (!$data) { return; }
来源：http://xu.asd995.cn

JS:   if (!data) return;
来源：http://nn.shxzskj.cn

TS:   if (!data) return;
来源：http://lc.bookmarksfly.cn

Java: if (data == null) return;
来源：http://dc.huixinmuqiang.cn

Go:   if data == nil { return }
来源：http://gp.hahajie.cn

Ruby: return if data.nil?
来源：http://ba.shxzukj.cn

C#:   if (data == null) return;
来源：http://jh.shxzukj.cn

================================================================================
来源：http://ly.asd995.cn

C. 函数与作用域
来源：http://hb.bookmarksfly.cn

================================================================================
来源：http://up.yuntaijiaju.cn

[C01] 定义函数
来源：http://ig.wgjwhj.cn

Py:   def add(a, b): return a + b
来源：http://hk.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vz.521024.cn

JS:   function add(a, b) { return a + b; }
来源：http://nz.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ov.muxihuayi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ez.yuntaijiaju.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xq.521024.cn

Ruby: def add(a, b); a + b; end
来源：http://wf.huixinmuqiang.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jc.yuexingan06.cn

[C02] 默认参数
来源：http://kr.szsharing.cn

Py:   def greet(name="World"): return name
来源：http://fj.szsharing.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ao.shxzskj.cn

JS:   function greet(name = "World") { return name; }
来源：http://df.chemitech.net.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xk.shtwfgs.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ns.huixiangedu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qb.bookmarksfly.cn

Ruby: def greet(name = "World") = name
来源：http://fl.hahajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://ys.szxytkj.cn

[C03] 可变参数
来源：http://ja.szxytkj.cn

Py:   def total(*args): return sum(args)
来源：http://gz.jianghongdianzi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ah.huanxung.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rf.jctech888.com.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jl.hahajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://br.jctech888.com.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fo.gzmigu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fo.hahajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://eb.nicolike.cn

[C04] 命名参数 / 关键字参数
来源：http://tb.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://my.szsharing.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lg.newstarts.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ak.bjjhwx.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ou.shxzskj.cn

Java: // 无：用 Builder 模式或 record
来源：http://vq.bookmarksfly.cn

Go:   // 无：用配置结构体参数
来源：http://sx.nicolike.cn

Ruby: f(a: 1, b: 2)
来源：http://fd.jianghongdianzi.cn

C#:   f(a: 1, b: 2)
来源：http://oo.colortex.cn

[C05] 返回多个值
来源：http://tc.colortex.cn

Py:   return a, b
来源：http://na.huanxung.cn

PHP:  return [$a, $b];
来源：http://oj.9csxet.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ts.muxihuayi.cn

TS:   return { a, b };
来源：http://ld.haigaiapp.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://iz.nicolike.cn

Go:   return a, b
来源：http://mn.lnxyls.cn

Ruby: return a, b
来源：http://kd.521024.cn

C#:   return (a, b);              // ValueTuple
来源：http://kk.huixiangedu.cn

[C06] 匿名函数 / lambda
来源：http://ud.bookmarksfly.cn

Py:   square = lambda x: x * x
来源：http://nz.colortex.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://jg.huixiangedu.cn

JS:   const square = x => x * x;
来源：http://eb.shtwfgs.cn

TS:   const square = (x: number): number => x * x;
来源：http://al.lnxyls.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://er.jianghongdianzi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zl.9csxet.cn

Ruby: square = ->(x) { x * x }
来源：http://nr.yuexingan06.cn

C#:   Func<int, int> square = x => x * x;
来源：http://eb.bjjhwx.cn

[C07] 把函数作为参数传入
来源：http://fa.shxzskj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://un.muxihuayi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ms.lnxyls.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vi.huixinmuqiang.cn

TS:   arr.map(String)
来源：http://gr.jctech888.com.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lv.colortex.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://oj.jianghongdianzi.cn

Ruby: arr.map(&:upcase)
来源：http://ou.huixiangedu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jc.jianghongdianzi.cn

[C08] 闭包
来源：http://pv.shtwfgs.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ao.nicolike.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bg.jctech888.com.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sn.huanxung.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ow.panjiajie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://np.gzmigu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mh.jianghongdianzi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lc.shxzukj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ru.jctech888.com.cn

[C09] 递归
来源：http://kc.jctech888.com.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sn.yuntaijiaju.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ls.hnjuh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ed.haigaiapp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pm.hnjuh.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ks.9csxet.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bl.jianghongdianzi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://us.hahajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zl.huixiangedu.cn

[C10] 变量作用域
来源：http://cy.muxihuayi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gl.panjiajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lt.nszjky.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nc.huanxung.cn

TS:   同 JS
来源：http://yg.panjiajie.cn

Java: 方法内为块级作用域
来源：http://lw.jianghongdianzi.cn

Go:   花括号块级作用域
来源：http://mr.huixinmuqiang.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xr.huixinmuqiang.cn

C#:   块级作用域
来源：http://bi.hahajie.cn

[C11] 模块导入与导出
来源：http://ka.chemitech.net.cn

Py:   from module import func
来源：http://wj.yuexingan06.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://cu.huanxung.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://aw.gzmigu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ss.muxihuayi.cn

Java: import java.util.List;
来源：http://jf.lnxyls.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pk.shxzskj.cn

Ruby: require "json"; require_relative "./util"
来源：http://gk.nszjky.cn

C#:   using System.Text;
来源：http://ss.jianghongdianzi.cn

[C12] 立即执行函数 IIFE
来源：http://sy.gzmigu.cn

Py:   (lambda: print("run"))()
来源：http://tt.jctech888.com.cn

PHP:  (function () { echo "run"; })();
来源：http://jl.shxzukj.cn

JS:   (() => { console.log("run"); })();
来源：http://mk.lnxyls.cn

TS:   (() => { console.log("run"); })();
来源：http://uq.shxzukj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ib.shxzskj.cn

Go:   func() { fmt.Println("run") }()
来源：http://vd.hnjuh.cn

Ruby: -> { puts "run" }.call
来源：http://fv.shxzukj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://na.nicolike.cn

[C13] 类型声明 / 类型注解
来源：http://qv.muxihuayi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cl.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gv.huixinmuqiang.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gx.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jg.newstarts.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fe.haigaiapp.cn

Go:   func add(a, b int) int
来源：http://ha.muxihuayi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mq.hnjuh.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fo.colortex.cn


<!-- 参考信息 -->