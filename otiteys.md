代发 wailian999

TS:   s.length
来源：http://cw.bjjhwx.cn

Java: s.length()
来源：http://iz.hnjuh.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ol.jianghongdianzi.cn

Ruby: s.length
来源：http://ue.jianghongdianzi.cn

C#:   s.Length
来源：http://cs.yuexingan06.cn

[A23] 大小写转换
来源：http://mw.hnjuh.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vx.bookmarksfly.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rl.bjjhwx.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yu.bookmarksfly.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vs.521024.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ie.shxzskj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zx.yuexingan06.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cw.shtwfgs.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zs.nicolike.cn

[A24] 去除首尾空白
来源：http://jg.9csxet.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ek.nszjky.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rn.9csxet.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://up.521024.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ae.shtwfgs.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ox.chemitech.net.cn

Go:   strings.TrimSpace(s)
来源：http://ju.bookmarksfly.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gi.asd995.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jb.shtwfgs.cn

[A25] 字符串比较
来源：http://zv.bjjhwx.cn

Py:   s1 == s2; s1 != s2
来源：http://py.huixiangedu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ow.hnjuh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ze.yuntaijiaju.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dh.panjiajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qd.jianghongdianzi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gj.huanxung.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://uv.huanxung.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tc.lnxyls.cn

[A26] 类型转换总览
来源：http://ui.jianghongdianzi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fq.huixiangedu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://co.yuexingan06.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gj.jianghongdianzi.cn

TS:   Number() String() Boolean() x as number
来源：http://qg.shxzskj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qf.521024.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dr.nicolike.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ar.chemitech.net.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fh.colortex.cn

================================================================================
来源：http://hr.wgjwhj.cn

B. 流程控制
来源：http://mb.521024.cn

================================================================================
来源：http://pi.nszjky.cn

[B01] 条件判断 if / else
来源：http://by.bookmarksfly.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://fx.nicolike.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zy.lnxyls.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://oe.asd995.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ji.jctech888.com.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://op.jctech888.com.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pl.bookmarksfly.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ve.colortex.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yk.jianghongdianzi.cn

[B02] 多分支 else if / elif
来源：http://vv.jctech888.com.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://db.hnjuh.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cf.szsharing.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://es.huixinmuqiang.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ss.jianghongdianzi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zi.hnjuh.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yv.hnjuh.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uj.colortex.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://im.chemitech.net.cn

[B03] switch / match / case
来源：http://ub.chemitech.net.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ql.wgjwhj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qz.colortex.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hu.haigaiapp.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gw.huixinmuqiang.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://au.lnxyls.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xg.yuntaijiaju.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://us.jctech888.com.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://of.szxytkj.cn

[B04] for 计数循环
来源：http://ij.jianghongdianzi.cn

Py:   for i in range(10): print(i)
来源：http://oc.muxihuayi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zf.wgjwhj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kk.muxihuayi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kk.hahajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.shxzskj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ug.szsharing.cn

Ruby: 10.times { |i| puts i }
来源：http://fm.huanxung.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ds.jianghongdianzi.cn

[B05] 遍历数组 / 列表
来源：http://hj.chemitech.net.cn

Py:   for item in arr: print(item)
来源：http://zg.hahajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xr.jianghongdianzi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://vw.hnjuh.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://jq.jianghongdianzi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yg.colortex.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gj.yuntaijiaju.cn

Ruby: arr.each { |item| puts item }
来源：http://xt.colortex.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://is.yuexingan06.cn

[B06] 遍历字典 / 对象
来源：http://lq.bookmarksfly.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://cz.szxytkj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ni.szxytkj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nd.shtwfgs.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nb.chemitech.net.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ii.newstarts.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tc.chemitech.net.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hb.lnxyls.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kg.9csxet.cn

[B07] while 循环
来源：http://jl.bjjhwx.cn

Py:   while i < 10: i += 1
来源：http://yj.shtwfgs.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mr.szsharing.cn

JS:   while (i < 10) { i++; }
来源：http://dl.shtwfgs.cn

TS:   while (i < 10) { i++; }
来源：http://tq.nicolike.cn

Java: while (i < 10) { i++; }
来源：http://lx.huixiangedu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ba.shxzukj.cn

Ruby: while i < 10; i += 1; end
来源：http://ee.muxihuayi.cn

C#:   while (i < 10) { i++; }
来源：http://ta.hahajie.cn

[B08] do-while（至少执行一次）
来源：http://ib.jctech888.com.cn

Py:   # 无 do-while：用 while True + break
来源：http://eg.jctech888.com.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xd.panjiajie.cn

JS:   do { i++; } while (i < 10);
来源：http://ys.asd995.cn

TS:   do { i++; } while (i < 10);
来源：http://ju.szsharing.cn

Java: do { i++; } while (i < 10);
来源：http://gp.wgjwhj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ba.yuntaijiaju.cn

Ruby: begin; i += 1; end while i < 10
来源：http://bq.jianghongdianzi.cn

C#:   do { i++; } while (i < 10);
来源：http://lw.9csxet.cn

[B09] break 与 continue
来源：http://rh.gzmigu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xg.shxzskj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ir.bjjhwx.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://es.bjjhwx.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cg.asd995.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hl.haigaiapp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nm.shxzskj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zy.nicolike.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ts.huanxung.cn

[B10] 遍历同时拿索引
来源：http://df.yuntaijiaju.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jt.hnjuh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ea.shxzukj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://do.nszjky.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tu.hnjuh.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ea.haigaiapp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fu.huixinmuqiang.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wz.nicolike.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qw.nszjky.cn

[B11] 生成数字序列 / 区间
来源：http://rz.szxytkj.cn

Py:   list(range(0, 10, 2))
来源：http://qp.asd995.cn

PHP:  range(0, 10, 2);
来源：http://tc.bookmarksfly.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mu.gzmigu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://va.colortex.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lz.yuexingan06.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ue.szxytkj.cn

Ruby: (0...10).step(2).to_a
来源：http://tr.szsharing.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kp.panjiajie.cn

[B12] 跳出多层循环
来源：http://up.szxytkj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://vt.jctech888.com.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://kc.szsharing.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zu.colortex.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xb.asd995.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hc.shxzukj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rn.shxzskj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ct.yuexingan06.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lh.haigaiapp.cn

[B13] 判断是否为数字
来源：http://ov.bookmarksfly.cn

Py:   isinstance(x, (int, float))
来源：http://zz.gzmigu.cn

PHP:  is_numeric($x)
来源：http://ge.bookmarksfly.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gh.colortex.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aj.jianghongdianzi.cn

Java: x instanceof Number
来源：http://fn.huanxung.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://go.gzmigu.cn

Ruby: x.is_a?(Numeric)
来源：http://yc.hnjuh.cn

C#:   x is int or double or decimal
来源：http://sb.yuntaijiaju.cn

[B14] 判断值是否在集合内
来源：http://vy.shxzukj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cb.bjjhwx.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rk.lnxyls.cn

JS:   [1, 2, 3].includes(x)
来源：http://gw.nicolike.cn

TS:   [1, 2, 3].includes(x)
来源：http://nx.shxzskj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://eu.huixinmuqiang.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kc.wgjwhj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://iu.newstarts.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mg.huanxung.cn

[B15] 布尔运算与取反
来源：http://lz.bookmarksfly.cn

Py:   a and b or not c
来源：http://xo.jianghongdianzi.cn

PHP:  $a && $b || !$c
来源：http://ir.wgjwhj.cn

JS:   a && b || !c
来源：http://lu.bookmarksfly.cn

TS:   a && b || !c
来源：http://bg.shxzskj.cn

Java: a && b || !c
来源：http://xq.9csxet.cn

Go:   a && b || !c
来源：http://lb.shxzukj.cn

Ruby: a && b || !c
来源：http://mc.szxytkj.cn

C#:   a && b || !c
来源：http://ag.521024.cn

[B16] 卫语句：不满足条件提前返回
来源：http://dl.huanxung.cn

Py:   if not data: return
来源：http://qg.521024.cn

PHP:  if (!$data) { return; }
来源：http://px.nicolike.cn

JS:   if (!data) return;
来源：http://fm.521024.cn

TS:   if (!data) return;
来源：http://fw.muxihuayi.cn

Java: if (data == null) return;
来源：http://ar.9csxet.cn

Go:   if data == nil { return }
来源：http://ao.hnjuh.cn

Ruby: return if data.nil?
来源：http://kv.shxzukj.cn

C#:   if (data == null) return;
来源：http://kj.jctech888.com.cn

================================================================================
来源：http://gt.shxzukj.cn

C. 函数与作用域
来源：http://de.huanxung.cn

================================================================================
来源：http://jv.jctech888.com.cn

[C01] 定义函数
来源：http://qx.gzmigu.cn

Py:   def add(a, b): return a + b
来源：http://uq.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ij.yuexingan06.cn

JS:   function add(a, b) { return a + b; }
来源：http://ns.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wo.panjiajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qb.haigaiapp.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ne.szxytkj.cn

Ruby: def add(a, b); a + b; end
来源：http://vy.9csxet.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tm.haigaiapp.cn

[C02] 默认参数
来源：http://cs.jctech888.com.cn

Py:   def greet(name="World"): return name
来源：http://fn.nicolike.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ct.colortex.cn

JS:   function greet(name = "World") { return name; }
来源：http://ox.gzmigu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cl.jianghongdianzi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://kr.huixiangedu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yn.jianghongdianzi.cn

Ruby: def greet(name = "World") = name
来源：http://op.huixinmuqiang.cn

C#:   string Greet(string name = "World") => name;
来源：http://ky.9csxet.cn

[C03] 可变参数
来源：http://tp.bjjhwx.cn

Py:   def total(*args): return sum(args)
来源：http://nl.yuexingan06.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kf.haigaiapp.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ac.panjiajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xy.huixiangedu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ez.huixiangedu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dr.nszjky.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pf.panjiajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://op.yuexingan06.cn

[C04] 命名参数 / 关键字参数
来源：http://ov.nicolike.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ps.yuntaijiaju.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nd.lnxyls.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://id.9csxet.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wb.szsharing.cn

Java: // 无：用 Builder 模式或 record
来源：http://cl.jctech888.com.cn

Go:   // 无：用配置结构体参数
来源：http://go.huanxung.cn

Ruby: f(a: 1, b: 2)
来源：http://kj.bjjhwx.cn

C#:   f(a: 1, b: 2)
来源：http://xm.asd995.cn

[C05] 返回多个值
来源：http://qb.nicolike.cn

Py:   return a, b
来源：http://fg.asd995.cn

PHP:  return [$a, $b];
来源：http://nn.chemitech.net.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://tb.muxihuayi.cn

TS:   return { a, b };
来源：http://jb.asd995.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dd.muxihuayi.cn

Go:   return a, b
来源：http://mk.nszjky.cn

Ruby: return a, b
来源：http://ai.yuntaijiaju.cn

C#:   return (a, b);              // ValueTuple
来源：http://sa.szsharing.cn

[C06] 匿名函数 / lambda
来源：http://dm.gzmigu.cn

Py:   square = lambda x: x * x
来源：http://zn.bjjhwx.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://sb.haigaiapp.cn

JS:   const square = x => x * x;
来源：http://ls.521024.cn

TS:   const square = (x: number): number => x * x;
来源：http://lf.shtwfgs.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tf.lnxyls.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ss.huanxung.cn

Ruby: square = ->(x) { x * x }
来源：http://pl.newstarts.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ch.huixiangedu.cn

[C07] 把函数作为参数传入
来源：http://au.yuntaijiaju.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ry.521024.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jj.asd995.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uw.asd995.cn

TS:   arr.map(String)
来源：http://pl.gzmigu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ol.nszjky.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ox.lnxyls.cn

Ruby: arr.map(&:upcase)
来源：http://mw.szxytkj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ty.panjiajie.cn

[C08] 闭包
来源：http://kh.jianghongdianzi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ey.9csxet.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vy.shxzskj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://go.jctech888.com.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kq.bjjhwx.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sw.lnxyls.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://go.hahajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qg.shxzskj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tb.gzmigu.cn

[C09] 递归
来源：http://de.521024.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ps.szsharing.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nl.huixinmuqiang.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pt.haigaiapp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fm.nszjky.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bm.asd995.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xs.muxihuayi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rk.panjiajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ig.huixiangedu.cn

[C10] 变量作用域
来源：http://mt.huixinmuqiang.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://on.bookmarksfly.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qj.muxihuayi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vg.9csxet.cn

TS:   同 JS
来源：http://jw.huixiangedu.cn

Java: 方法内为块级作用域
来源：http://ie.gzmigu.cn

Go:   花括号块级作用域
来源：http://ww.huanxung.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tp.521024.cn

C#:   块级作用域
来源：http://bs.jctech888.com.cn

[C11] 模块导入与导出
来源：http://vw.lnxyls.cn

Py:   from module import func
来源：http://lk.hahajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pw.shxzskj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ky.shxzukj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://df.huanxung.cn

Java: import java.util.List;
来源：http://xm.asd995.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fb.huixiangedu.cn

Ruby: require "json"; require_relative "./util"
来源：http://ps.chemitech.net.cn

C#:   using System.Text;
来源：http://ha.jctech888.com.cn

[C12] 立即执行函数 IIFE
来源：http://it.newstarts.cn

Py:   (lambda: print("run"))()
来源：http://zp.nicolike.cn

PHP:  (function () { echo "run"; })();
来源：http://ol.nicolike.cn

JS:   (() => { console.log("run"); })();
来源：http://gx.wgjwhj.cn

TS:   (() => { console.log("run"); })();
来源：http://cv.9csxet.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ix.haigaiapp.cn

Go:   func() { fmt.Println("run") }()
来源：http://ha.bookmarksfly.cn

Ruby: -> { puts "run" }.call
来源：http://je.shxzukj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://cw.shxzskj.cn

[C13] 类型声明 / 类型注解
来源：http://ki.newstarts.cn


<!-- 参考信息 -->