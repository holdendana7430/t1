代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cq.szsharing.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ql.haigaiapp.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ex.jianghongdianzi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gv.hahajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mp.panjiajie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://no.hahajie.cn

[A24] 去除首尾空白
来源：http://ff.panjiajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bo.huanxung.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xb.yuntaijiaju.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sw.haigaiapp.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dx.huixiangedu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zp.jianghongdianzi.cn

Go:   strings.TrimSpace(s)
来源：http://hw.szsharing.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bx.haigaiapp.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jq.wgjwhj.cn

[A25] 字符串比较
来源：http://kr.bookmarksfly.cn

Py:   s1 == s2; s1 != s2
来源：http://cj.shxzukj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gg.szxytkj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zm.huanxung.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gi.bookmarksfly.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dz.jctech888.com.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lj.huixinmuqiang.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ke.szxytkj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jx.shxzskj.cn

[A26] 类型转换总览
来源：http://lo.yuntaijiaju.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lq.bjjhwx.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zf.muxihuayi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bo.lnxyls.cn

TS:   Number() String() Boolean() x as number
来源：http://xm.huixiangedu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://me.panjiajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tm.huanxung.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://fe.9csxet.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tl.shxzukj.cn

================================================================================
来源：http://vm.muxihuayi.cn

B. 流程控制
来源：http://wm.szxytkj.cn

================================================================================
来源：http://qq.jctech888.com.cn

[B01] 条件判断 if / else
来源：http://fa.panjiajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://up.szxytkj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fq.newstarts.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://km.huixiangedu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yt.521024.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://oj.shtwfgs.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nz.shxzskj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qd.panjiajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dt.521024.cn

[B02] 多分支 else if / elif
来源：http://yq.colortex.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sw.panjiajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://uc.yuexingan06.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ai.nicolike.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zf.huanxung.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qo.hahajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tx.yuntaijiaju.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gd.521024.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xp.hahajie.cn

[B03] switch / match / case
来源：http://dm.gzmigu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://na.lnxyls.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yo.hahajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hd.hahajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oj.jianghongdianzi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zt.521024.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vw.9csxet.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tq.panjiajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://aj.szsharing.cn

[B04] for 计数循环
来源：http://ze.jianghongdianzi.cn

Py:   for i in range(10): print(i)
来源：http://wh.huixinmuqiang.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ku.shxzukj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vr.chemitech.net.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://km.yuntaijiaju.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mb.szxytkj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ri.chemitech.net.cn

Ruby: 10.times { |i| puts i }
来源：http://ly.gzmigu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mo.colortex.cn

[B05] 遍历数组 / 列表
来源：http://ao.9csxet.cn

Py:   for item in arr: print(item)
来源：http://lc.chemitech.net.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ip.jianghongdianzi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fg.szxytkj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ix.nszjky.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yv.yuntaijiaju.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://na.bookmarksfly.cn

Ruby: arr.each { |item| puts item }
来源：http://fs.jianghongdianzi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://eu.jctech888.com.cn

[B06] 遍历字典 / 对象
来源：http://rh.szxytkj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ld.shxzukj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ty.521024.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oj.hnjuh.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://it.lnxyls.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xn.hnjuh.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dr.shtwfgs.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qy.huixinmuqiang.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://is.yuntaijiaju.cn

[B07] while 循环
来源：http://af.muxihuayi.cn

Py:   while i < 10: i += 1
来源：http://aw.huixiangedu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://rl.newstarts.cn

JS:   while (i < 10) { i++; }
来源：http://tu.panjiajie.cn

TS:   while (i < 10) { i++; }
来源：http://yo.gzmigu.cn

Java: while (i < 10) { i++; }
来源：http://mc.szsharing.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xk.shxzskj.cn

Ruby: while i < 10; i += 1; end
来源：http://mo.yuntaijiaju.cn

C#:   while (i < 10) { i++; }
来源：http://cf.bjjhwx.cn

[B08] do-while（至少执行一次）
来源：http://eo.jianghongdianzi.cn

Py:   # 无 do-while：用 while True + break
来源：http://vo.haigaiapp.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cy.shxzskj.cn

JS:   do { i++; } while (i < 10);
来源：http://nf.shxzukj.cn

TS:   do { i++; } while (i < 10);
来源：http://gl.9csxet.cn

Java: do { i++; } while (i < 10);
来源：http://rj.jianghongdianzi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mb.bjjhwx.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ts.colortex.cn

C#:   do { i++; } while (i < 10);
来源：http://ze.521024.cn

[B09] break 与 continue
来源：http://ne.colortex.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nr.shtwfgs.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mc.bookmarksfly.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rd.hnjuh.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lw.hnjuh.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ow.shtwfgs.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kz.huixiangedu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hi.muxihuayi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qd.colortex.cn

[B10] 遍历同时拿索引
来源：http://fy.bjjhwx.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://js.nszjky.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qe.jctech888.com.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://he.asd995.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ch.lnxyls.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pi.gzmigu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jv.huixinmuqiang.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xv.chemitech.net.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qr.wgjwhj.cn

[B11] 生成数字序列 / 区间
来源：http://pn.nszjky.cn

Py:   list(range(0, 10, 2))
来源：http://ye.asd995.cn

PHP:  range(0, 10, 2);
来源：http://uw.shtwfgs.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dy.colortex.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ot.shtwfgs.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fu.wgjwhj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ul.huanxung.cn

Ruby: (0...10).step(2).to_a
来源：http://mz.yuntaijiaju.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vf.bjjhwx.cn

[B12] 跳出多层循环
来源：http://hj.huanxung.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ql.gzmigu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://bk.gzmigu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ix.huixinmuqiang.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://by.bjjhwx.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ad.yuexingan06.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://oo.chemitech.net.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mx.panjiajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nf.521024.cn

[B13] 判断是否为数字
来源：http://zb.huixiangedu.cn

Py:   isinstance(x, (int, float))
来源：http://kr.asd995.cn

PHP:  is_numeric($x)
来源：http://cq.colortex.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://el.shxzukj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bl.jctech888.com.cn

Java: x instanceof Number
来源：http://jk.nicolike.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cj.nicolike.cn

Ruby: x.is_a?(Numeric)
来源：http://bh.haigaiapp.cn

C#:   x is int or double or decimal
来源：http://qg.521024.cn

[B14] 判断值是否在集合内
来源：http://yu.shtwfgs.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qf.jctech888.com.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cx.asd995.cn

JS:   [1, 2, 3].includes(x)
来源：http://ev.yuntaijiaju.cn

TS:   [1, 2, 3].includes(x)
来源：http://az.panjiajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://pm.jctech888.com.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://by.nszjky.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ba.yuntaijiaju.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ao.yuntaijiaju.cn

[B15] 布尔运算与取反
来源：http://th.asd995.cn

Py:   a and b or not c
来源：http://jc.muxihuayi.cn

PHP:  $a && $b || !$c
来源：http://ef.bjjhwx.cn

JS:   a && b || !c
来源：http://ch.newstarts.cn

TS:   a && b || !c
来源：http://uk.yuexingan06.cn

Java: a && b || !c
来源：http://wi.9csxet.cn

Go:   a && b || !c
来源：http://sp.huixiangedu.cn

Ruby: a && b || !c
来源：http://vi.hnjuh.cn

C#:   a && b || !c
来源：http://tj.gzmigu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jv.shtwfgs.cn

Py:   if not data: return
来源：http://ei.bjjhwx.cn

PHP:  if (!$data) { return; }
来源：http://am.jctech888.com.cn

JS:   if (!data) return;
来源：http://db.huixiangedu.cn

TS:   if (!data) return;
来源：http://gp.chemitech.net.cn

Java: if (data == null) return;
来源：http://pg.gzmigu.cn

Go:   if data == nil { return }
来源：http://cw.chemitech.net.cn

Ruby: return if data.nil?
来源：http://vp.panjiajie.cn

C#:   if (data == null) return;
来源：http://wk.huixiangedu.cn

================================================================================
来源：http://vm.lnxyls.cn

C. 函数与作用域
来源：http://co.chemitech.net.cn

================================================================================
来源：http://eu.521024.cn

[C01] 定义函数
来源：http://jr.shxzukj.cn

Py:   def add(a, b): return a + b
来源：http://bq.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pg.shxzskj.cn

JS:   function add(a, b) { return a + b; }
来源：http://ix.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ml.nszjky.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://tk.shxzskj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://gl.newstarts.cn

Ruby: def add(a, b); a + b; end
来源：http://qm.yuntaijiaju.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tt.newstarts.cn

[C02] 默认参数
来源：http://fr.9csxet.cn

Py:   def greet(name="World"): return name
来源：http://ll.gzmigu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hl.shtwfgs.cn

JS:   function greet(name = "World") { return name; }
来源：http://uj.asd995.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lm.muxihuayi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://et.lnxyls.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gu.yuexingan06.cn

Ruby: def greet(name = "World") = name
来源：http://yx.haigaiapp.cn

C#:   string Greet(string name = "World") => name;
来源：http://jg.jianghongdianzi.cn

[C03] 可变参数
来源：http://rb.lnxyls.cn

Py:   def total(*args): return sum(args)
来源：http://ht.jctech888.com.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dz.newstarts.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qq.muxihuayi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ja.jianghongdianzi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dv.huixinmuqiang.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uu.wgjwhj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://cu.shtwfgs.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mk.shxzskj.cn

[C04] 命名参数 / 关键字参数
来源：http://rx.gzmigu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://of.gzmigu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xu.hahajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ju.jianghongdianzi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ms.jianghongdianzi.cn

Java: // 无：用 Builder 模式或 record
来源：http://oi.wgjwhj.cn

Go:   // 无：用配置结构体参数
来源：http://bg.gzmigu.cn

Ruby: f(a: 1, b: 2)
来源：http://bv.jianghongdianzi.cn

C#:   f(a: 1, b: 2)
来源：http://js.jctech888.com.cn

[C05] 返回多个值
来源：http://zi.newstarts.cn

Py:   return a, b
来源：http://gk.panjiajie.cn

PHP:  return [$a, $b];
来源：http://wv.wgjwhj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ah.nicolike.cn

TS:   return { a, b };
来源：http://hq.szxytkj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wc.bjjhwx.cn

Go:   return a, b
来源：http://xi.wgjwhj.cn

Ruby: return a, b
来源：http://op.nszjky.cn

C#:   return (a, b);              // ValueTuple
来源：http://js.bookmarksfly.cn

[C06] 匿名函数 / lambda
来源：http://gd.colortex.cn

Py:   square = lambda x: x * x
来源：http://bt.shxzskj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://jh.bookmarksfly.cn

JS:   const square = x => x * x;
来源：http://dj.huixiangedu.cn

TS:   const square = (x: number): number => x * x;
来源：http://gl.bjjhwx.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pk.huixinmuqiang.cn

Go:   sq := func(x int) int { return x * x }
来源：http://us.shxzskj.cn

Ruby: square = ->(x) { x * x }
来源：http://dq.jctech888.com.cn

C#:   Func<int, int> square = x => x * x;
来源：http://eh.nszjky.cn

[C07] 把函数作为参数传入
来源：http://fz.gzmigu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yx.huixinmuqiang.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xl.colortex.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yk.szxytkj.cn

TS:   arr.map(String)
来源：http://en.newstarts.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fe.shxzskj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xs.521024.cn

Ruby: arr.map(&:upcase)
来源：http://ai.huanxung.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fc.chemitech.net.cn

[C08] 闭包
来源：http://ot.bookmarksfly.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hk.jianghongdianzi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ta.gzmigu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yy.nicolike.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vu.haigaiapp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ri.jianghongdianzi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jq.521024.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://md.szsharing.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://oa.shxzukj.cn

[C09] 递归
来源：http://vw.bjjhwx.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://es.szxytkj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://il.yuntaijiaju.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yp.chemitech.net.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aj.colortex.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uj.newstarts.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gc.wgjwhj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tk.nicolike.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hr.huanxung.cn

[C10] 变量作用域
来源：http://zf.bjjhwx.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xo.yuexingan06.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wk.szsharing.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ed.shxzskj.cn

TS:   同 JS
来源：http://op.yuntaijiaju.cn

Java: 方法内为块级作用域
来源：http://ib.shxzskj.cn

Go:   花括号块级作用域
来源：http://ap.nszjky.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zv.szxytkj.cn

C#:   块级作用域
来源：http://hw.colortex.cn

[C11] 模块导入与导出
来源：http://yj.shxzukj.cn

Py:   from module import func
来源：http://vd.yuexingan06.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://eo.bookmarksfly.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jw.haigaiapp.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wz.bookmarksfly.cn

Java: import java.util.List;
来源：http://df.huanxung.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://go.shxzskj.cn

Ruby: require "json"; require_relative "./util"
来源：http://xe.jianghongdianzi.cn

C#:   using System.Text;
来源：http://pj.521024.cn

[C12] 立即执行函数 IIFE
来源：http://gb.szxytkj.cn

Py:   (lambda: print("run"))()
来源：http://ul.huixiangedu.cn

PHP:  (function () { echo "run"; })();
来源：http://ot.bookmarksfly.cn

JS:   (() => { console.log("run"); })();
来源：http://oh.shxzukj.cn

TS:   (() => { console.log("run"); })();
来源：http://xx.bookmarksfly.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://av.nszjky.cn

Go:   func() { fmt.Println("run") }()
来源：http://ud.shxzukj.cn

Ruby: -> { puts "run" }.call
来源：http://ko.yuexingan06.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wq.huixinmuqiang.cn

[C13] 类型声明 / 类型注解
来源：http://xi.hnjuh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qx.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oe.9csxet.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sn.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dg.lnxyls.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xf.shxzukj.cn

Go:   func add(a, b int) int
来源：http://po.asd995.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yx.asd995.cn

C#:   int Add(int a, int b) => a + b;
来源：http://it.haigaiapp.cn


<!-- 参考信息 -->