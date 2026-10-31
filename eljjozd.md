代发 wailian999

TS:   s.length
来源：http://lm.haigaiapp.cn

Java: s.length()
来源：http://jh.shxzskj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zc.jctech888.com.cn

Ruby: s.length
来源：http://yl.yuntaijiaju.cn

C#:   s.Length
来源：http://lo.nicolike.cn

[A23] 大小写转换
来源：http://sa.huanxung.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wy.asd995.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qw.jctech888.com.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xt.haigaiapp.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ra.huixinmuqiang.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cs.hahajie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ds.shtwfgs.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hi.huixiangedu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://at.huanxung.cn

[A24] 去除首尾空白
来源：http://fc.szsharing.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tc.nszjky.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cl.muxihuayi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fg.bookmarksfly.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fl.hahajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zt.9csxet.cn

Go:   strings.TrimSpace(s)
来源：http://yp.huixinmuqiang.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lz.nicolike.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sy.shxzskj.cn

[A25] 字符串比较
来源：http://pq.jctech888.com.cn

Py:   s1 == s2; s1 != s2
来源：http://vy.yuntaijiaju.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://de.muxihuayi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://aq.yuexingan06.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gn.jctech888.com.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zv.muxihuayi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vs.huixiangedu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://qt.jctech888.com.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xx.hnjuh.cn

[A26] 类型转换总览
来源：http://xw.haigaiapp.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://px.huanxung.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ih.huanxung.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://eq.newstarts.cn

TS:   Number() String() Boolean() x as number
来源：http://wq.panjiajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qk.hnjuh.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sd.jctech888.com.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lr.521024.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bq.bookmarksfly.cn

================================================================================
来源：http://ja.shxzukj.cn

B. 流程控制
来源：http://qh.wgjwhj.cn

================================================================================
来源：http://er.asd995.cn

[B01] 条件判断 if / else
来源：http://zv.huixinmuqiang.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ys.yuntaijiaju.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rc.szxytkj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ei.lnxyls.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://go.yuexingan06.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://lu.hnjuh.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lv.panjiajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hl.yuexingan06.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nk.bjjhwx.cn

[B02] 多分支 else if / elif
来源：http://ra.521024.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yq.9csxet.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rt.panjiajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://id.panjiajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zx.huixinmuqiang.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ty.huanxung.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hw.jctech888.com.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cy.nszjky.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bz.asd995.cn

[B03] switch / match / case
来源：http://qk.bookmarksfly.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dq.wgjwhj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://do.jianghongdianzi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nk.shxzukj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://if.asd995.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vm.bookmarksfly.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ba.521024.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jf.huixinmuqiang.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://td.yuntaijiaju.cn

[B04] for 计数循环
来源：http://si.huixiangedu.cn

Py:   for i in range(10): print(i)
来源：http://co.haigaiapp.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sh.panjiajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tz.lnxyls.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ee.shtwfgs.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ox.yuexingan06.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kr.jctech888.com.cn

Ruby: 10.times { |i| puts i }
来源：http://my.huixiangedu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qm.huixiangedu.cn

[B05] 遍历数组 / 列表
来源：http://zf.jianghongdianzi.cn

Py:   for item in arr: print(item)
来源：http://ia.panjiajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rj.jctech888.com.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ii.asd995.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gj.huixinmuqiang.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://mz.yuntaijiaju.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wj.nszjky.cn

Ruby: arr.each { |item| puts item }
来源：http://qq.asd995.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yj.bjjhwx.cn

[B06] 遍历字典 / 对象
来源：http://xh.jianghongdianzi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tq.yuexingan06.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tl.shtwfgs.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nl.nszjky.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bq.newstarts.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vk.shxzskj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ki.huixiangedu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pv.9csxet.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ot.bookmarksfly.cn

[B07] while 循环
来源：http://zk.hnjuh.cn

Py:   while i < 10: i += 1
来源：http://mp.hahajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hb.szsharing.cn

JS:   while (i < 10) { i++; }
来源：http://ex.hahajie.cn

TS:   while (i < 10) { i++; }
来源：http://lc.bookmarksfly.cn

Java: while (i < 10) { i++; }
来源：http://sp.muxihuayi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nf.szsharing.cn

Ruby: while i < 10; i += 1; end
来源：http://zh.szxytkj.cn

C#:   while (i < 10) { i++; }
来源：http://jf.jianghongdianzi.cn

[B08] do-while（至少执行一次）
来源：http://lw.asd995.cn

Py:   # 无 do-while：用 while True + break
来源：http://rd.yuexingan06.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ly.szsharing.cn

JS:   do { i++; } while (i < 10);
来源：http://es.yuntaijiaju.cn

TS:   do { i++; } while (i < 10);
来源：http://cx.bjjhwx.cn

Java: do { i++; } while (i < 10);
来源：http://gt.newstarts.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://es.lnxyls.cn

Ruby: begin; i += 1; end while i < 10
来源：http://dq.yuexingan06.cn

C#:   do { i++; } while (i < 10);
来源：http://yv.gzmigu.cn

[B09] break 与 continue
来源：http://iv.yuexingan06.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jk.shxzukj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wo.hnjuh.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xm.colortex.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tc.bjjhwx.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xx.colortex.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gh.panjiajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nq.hahajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ez.wgjwhj.cn

[B10] 遍历同时拿索引
来源：http://vw.yuexingan06.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dp.jctech888.com.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pp.panjiajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rs.shxzukj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ab.bookmarksfly.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kc.wgjwhj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vf.nicolike.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nf.huixinmuqiang.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yn.muxihuayi.cn

[B11] 生成数字序列 / 区间
来源：http://cb.huixiangedu.cn

Py:   list(range(0, 10, 2))
来源：http://wy.huixiangedu.cn

PHP:  range(0, 10, 2);
来源：http://zk.huixiangedu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eq.huanxung.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dh.hnjuh.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ey.szxytkj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wc.jianghongdianzi.cn

Ruby: (0...10).step(2).to_a
来源：http://cj.colortex.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kz.huixinmuqiang.cn

[B12] 跳出多层循环
来源：http://se.shtwfgs.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://gh.gzmigu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://en.szxytkj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://eq.hnjuh.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ww.hahajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://du.newstarts.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zt.521024.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://io.jctech888.com.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nn.wgjwhj.cn

[B13] 判断是否为数字
来源：http://jr.huanxung.cn

Py:   isinstance(x, (int, float))
来源：http://uk.chemitech.net.cn

PHP:  is_numeric($x)
来源：http://gs.szxytkj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jc.bjjhwx.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fv.huixinmuqiang.cn

Java: x instanceof Number
来源：http://va.szxytkj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://es.nicolike.cn

Ruby: x.is_a?(Numeric)
来源：http://cl.gzmigu.cn

C#:   x is int or double or decimal
来源：http://hq.jianghongdianzi.cn

[B14] 判断值是否在集合内
来源：http://je.yuntaijiaju.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xr.chemitech.net.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yu.hahajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://bc.szxytkj.cn

TS:   [1, 2, 3].includes(x)
来源：http://td.hnjuh.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://pa.bookmarksfly.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ko.yuexingan06.cn

Ruby: [1, 2, 3].include?(x)
来源：http://bs.hahajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wy.yuntaijiaju.cn

[B15] 布尔运算与取反
来源：http://zw.hahajie.cn

Py:   a and b or not c
来源：http://it.huanxung.cn

PHP:  $a && $b || !$c
来源：http://zh.panjiajie.cn

JS:   a && b || !c
来源：http://qz.yuexingan06.cn

TS:   a && b || !c
来源：http://ju.jianghongdianzi.cn

Java: a && b || !c
来源：http://tt.yuexingan06.cn

Go:   a && b || !c
来源：http://fi.bookmarksfly.cn

Ruby: a && b || !c
来源：http://xo.nszjky.cn

C#:   a && b || !c
来源：http://jf.lnxyls.cn

[B16] 卫语句：不满足条件提前返回
来源：http://kk.haigaiapp.cn

Py:   if not data: return
来源：http://fd.huixiangedu.cn

PHP:  if (!$data) { return; }
来源：http://gp.jctech888.com.cn

JS:   if (!data) return;
来源：http://qn.chemitech.net.cn

TS:   if (!data) return;
来源：http://oa.yuntaijiaju.cn

Java: if (data == null) return;
来源：http://rh.szxytkj.cn

Go:   if data == nil { return }
来源：http://tx.haigaiapp.cn

Ruby: return if data.nil?
来源：http://us.bookmarksfly.cn

C#:   if (data == null) return;
来源：http://aa.panjiajie.cn

================================================================================
来源：http://np.nicolike.cn

C. 函数与作用域
来源：http://tz.szsharing.cn

================================================================================
来源：http://to.jianghongdianzi.cn

[C01] 定义函数
来源：http://ak.yuexingan06.cn

Py:   def add(a, b): return a + b
来源：http://op.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vz.shtwfgs.cn

JS:   function add(a, b) { return a + b; }
来源：http://ip.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ka.hnjuh.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://jt.9csxet.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mb.panjiajie.cn

Ruby: def add(a, b); a + b; end
来源：http://pt.bookmarksfly.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vs.huixinmuqiang.cn

[C02] 默认参数
来源：http://gs.lnxyls.cn

Py:   def greet(name="World"): return name
来源：http://rz.huixinmuqiang.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://oq.wgjwhj.cn

JS:   function greet(name = "World") { return name; }
来源：http://jw.shtwfgs.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rp.nicolike.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ag.huanxung.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fl.asd995.cn

Ruby: def greet(name = "World") = name
来源：http://vm.huixiangedu.cn

C#:   string Greet(string name = "World") => name;
来源：http://ip.jianghongdianzi.cn

[C03] 可变参数
来源：http://go.nszjky.cn

Py:   def total(*args): return sum(args)
来源：http://ha.huanxung.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yu.huixiangedu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://il.bookmarksfly.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lf.jctech888.com.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rv.szxytkj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://px.wgjwhj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://lf.chemitech.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hi.shtwfgs.cn

[C04] 命名参数 / 关键字参数
来源：http://ry.yuntaijiaju.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://te.hnjuh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sz.lnxyls.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jz.nszjky.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vo.shxzskj.cn

Java: // 无：用 Builder 模式或 record
来源：http://mx.asd995.cn

Go:   // 无：用配置结构体参数
来源：http://fn.nicolike.cn

Ruby: f(a: 1, b: 2)
来源：http://oy.szsharing.cn

C#:   f(a: 1, b: 2)
来源：http://dy.huanxung.cn

[C05] 返回多个值
来源：http://ce.muxihuayi.cn

Py:   return a, b
来源：http://mb.nszjky.cn

PHP:  return [$a, $b];
来源：http://ag.szxytkj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zd.nszjky.cn

TS:   return { a, b };
来源：http://nu.shxzukj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yr.huanxung.cn

Go:   return a, b
来源：http://bj.yuntaijiaju.cn

Ruby: return a, b
来源：http://ee.panjiajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://pb.hahajie.cn

[C06] 匿名函数 / lambda
来源：http://cs.yuexingan06.cn

Py:   square = lambda x: x * x
来源：http://uy.newstarts.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ko.szsharing.cn

JS:   const square = x => x * x;
来源：http://uu.9csxet.cn

TS:   const square = (x: number): number => x * x;
来源：http://pj.bjjhwx.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ng.bookmarksfly.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rd.bookmarksfly.cn

Ruby: square = ->(x) { x * x }
来源：http://cb.lnxyls.cn

C#:   Func<int, int> square = x => x * x;
来源：http://li.chemitech.net.cn

[C07] 把函数作为参数传入
来源：http://dp.huixiangedu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dr.hnjuh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://tz.haigaiapp.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ek.hahajie.cn

TS:   arr.map(String)
来源：http://zh.521024.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hr.szsharing.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ni.shxzukj.cn

Ruby: arr.map(&:upcase)
来源：http://gc.shtwfgs.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fw.lnxyls.cn

[C08] 闭包
来源：http://sj.szsharing.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wl.bjjhwx.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zo.newstarts.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://op.muxihuayi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qj.jctech888.com.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://eb.lnxyls.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ky.9csxet.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jm.huixinmuqiang.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://te.szsharing.cn

[C09] 递归
来源：http://bo.wgjwhj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dv.asd995.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mp.nszjky.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bx.shxzukj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qr.yuexingan06.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vu.haigaiapp.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qt.jianghongdianzi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dp.jctech888.com.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zc.szsharing.cn

[C10] 变量作用域
来源：http://ks.nicolike.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://uv.yuexingan06.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vb.hahajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ce.jianghongdianzi.cn

TS:   同 JS
来源：http://ds.jctech888.com.cn

Java: 方法内为块级作用域
来源：http://cm.nicolike.cn

Go:   花括号块级作用域
来源：http://bv.huixinmuqiang.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mx.jianghongdianzi.cn

C#:   块级作用域
来源：http://bv.shtwfgs.cn

[C11] 模块导入与导出
来源：http://iw.bjjhwx.cn

Py:   from module import func
来源：http://qr.shtwfgs.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hq.huanxung.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zv.hnjuh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xu.9csxet.cn

Java: import java.util.List;
来源：http://os.shxzukj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ma.szxytkj.cn

Ruby: require "json"; require_relative "./util"
来源：http://ao.jianghongdianzi.cn

C#:   using System.Text;
来源：http://bu.szsharing.cn

[C12] 立即执行函数 IIFE
来源：http://ol.szsharing.cn

Py:   (lambda: print("run"))()
来源：http://bm.bookmarksfly.cn

PHP:  (function () { echo "run"; })();
来源：http://wj.wgjwhj.cn

JS:   (() => { console.log("run"); })();
来源：http://is.colortex.cn

TS:   (() => { console.log("run"); })();
来源：http://ep.chemitech.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hi.muxihuayi.cn

Go:   func() { fmt.Println("run") }()
来源：http://sh.szsharing.cn

Ruby: -> { puts "run" }.call
来源：http://fp.newstarts.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://km.bookmarksfly.cn

[C13] 类型声明 / 类型注解
来源：http://en.gzmigu.cn


<!-- 参考信息 -->