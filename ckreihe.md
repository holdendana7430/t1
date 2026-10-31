代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nk.huanxung.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://lo.shtwfgs.cn

[A24] 去除首尾空白
来源：http://wc.yuexingan06.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fd.9csxet.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wk.gzmigu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mj.hnjuh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eq.lnxyls.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mt.chemitech.net.cn

Go:   strings.TrimSpace(s)
来源：http://zn.muxihuayi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jb.chemitech.net.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sj.521024.cn

[A25] 字符串比较
来源：http://cs.szsharing.cn

Py:   s1 == s2; s1 != s2
来源：http://td.jctech888.com.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bc.chemitech.net.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tn.colortex.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cz.9csxet.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://by.shxzskj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hj.jianghongdianzi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://gw.lnxyls.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wb.shxzukj.cn

[A26] 类型转换总览
来源：http://vm.shxzukj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ig.newstarts.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zp.colortex.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://za.jctech888.com.cn

TS:   Number() String() Boolean() x as number
来源：http://da.lnxyls.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bv.bookmarksfly.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://co.lnxyls.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://fj.nszjky.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://en.jctech888.com.cn

================================================================================
来源：http://os.newstarts.cn

B. 流程控制
来源：http://sx.asd995.cn

================================================================================
来源：http://eu.szxytkj.cn

[B01] 条件判断 if / else
来源：http://xe.huixiangedu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://qx.huixiangedu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pj.chemitech.net.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hu.panjiajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kg.jianghongdianzi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://md.asd995.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mk.nicolike.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qy.haigaiapp.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dx.yuexingan06.cn

[B02] 多分支 else if / elif
来源：http://fk.yuexingan06.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dp.nicolike.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wn.jianghongdianzi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dn.yuexingan06.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wc.colortex.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hc.haigaiapp.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cr.huanxung.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://aw.shtwfgs.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ys.huixiangedu.cn

[B03] switch / match / case
来源：http://jn.yuntaijiaju.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sa.haigaiapp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qe.yuexingan06.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lq.jianghongdianzi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://su.jctech888.com.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ai.colortex.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qg.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wa.521024.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yl.gzmigu.cn

[B04] for 计数循环
来源：http://oa.huixinmuqiang.cn

Py:   for i in range(10): print(i)
来源：http://pl.huixinmuqiang.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jy.gzmigu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ly.colortex.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://at.wgjwhj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fi.lnxyls.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lb.wgjwhj.cn

Ruby: 10.times { |i| puts i }
来源：http://lw.huanxung.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://db.gzmigu.cn

[B05] 遍历数组 / 列表
来源：http://dz.nicolike.cn

Py:   for item in arr: print(item)
来源：http://yy.haigaiapp.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fo.bookmarksfly.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dk.jianghongdianzi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://zd.panjiajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://eb.nicolike.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dg.jctech888.com.cn

Ruby: arr.each { |item| puts item }
来源：http://ze.gzmigu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jt.asd995.cn

[B06] 遍历字典 / 对象
来源：http://qu.bookmarksfly.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://au.panjiajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yw.hahajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xm.newstarts.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cm.9csxet.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://se.muxihuayi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://it.wgjwhj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bx.521024.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hn.chemitech.net.cn

[B07] while 循环
来源：http://da.gzmigu.cn

Py:   while i < 10: i += 1
来源：http://hf.huanxung.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fb.lnxyls.cn

JS:   while (i < 10) { i++; }
来源：http://jh.huixinmuqiang.cn

TS:   while (i < 10) { i++; }
来源：http://th.shtwfgs.cn

Java: while (i < 10) { i++; }
来源：http://ns.asd995.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://um.panjiajie.cn

Ruby: while i < 10; i += 1; end
来源：http://vf.jctech888.com.cn

C#:   while (i < 10) { i++; }
来源：http://rg.huanxung.cn

[B08] do-while（至少执行一次）
来源：http://om.lnxyls.cn

Py:   # 无 do-while：用 while True + break
来源：http://pr.gzmigu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://nn.hnjuh.cn

JS:   do { i++; } while (i < 10);
来源：http://te.chemitech.net.cn

TS:   do { i++; } while (i < 10);
来源：http://ll.hahajie.cn

Java: do { i++; } while (i < 10);
来源：http://wl.newstarts.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wf.huixiangedu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ei.huixinmuqiang.cn

C#:   do { i++; } while (i < 10);
来源：http://bg.hnjuh.cn

[B09] break 与 continue
来源：http://sx.jctech888.com.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dz.newstarts.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yd.jctech888.com.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lf.shtwfgs.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ia.521024.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jj.huixiangedu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ey.shtwfgs.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xm.521024.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qz.521024.cn

[B10] 遍历同时拿索引
来源：http://sm.colortex.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tk.hahajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ig.hahajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ia.chemitech.net.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vi.gzmigu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sb.jianghongdianzi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bf.jctech888.com.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pr.shtwfgs.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sx.szxytkj.cn

[B11] 生成数字序列 / 区间
来源：http://dk.shxzukj.cn

Py:   list(range(0, 10, 2))
来源：http://xx.szxytkj.cn

PHP:  range(0, 10, 2);
来源：http://xg.gzmigu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uj.shxzukj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ir.asd995.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cy.chemitech.net.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kl.muxihuayi.cn

Ruby: (0...10).step(2).to_a
来源：http://pm.colortex.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cp.gzmigu.cn

[B12] 跳出多层循环
来源：http://db.colortex.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://nh.shtwfgs.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://oj.newstarts.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uh.shxzukj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lb.yuntaijiaju.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hk.chemitech.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hx.yuntaijiaju.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zo.muxihuayi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gf.huixinmuqiang.cn

[B13] 判断是否为数字
来源：http://rb.muxihuayi.cn

Py:   isinstance(x, (int, float))
来源：http://te.yuexingan06.cn

PHP:  is_numeric($x)
来源：http://ai.yuntaijiaju.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pm.lnxyls.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gs.yuntaijiaju.cn

Java: x instanceof Number
来源：http://gy.newstarts.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hu.bookmarksfly.cn

Ruby: x.is_a?(Numeric)
来源：http://bg.shxzskj.cn

C#:   x is int or double or decimal
来源：http://bb.bookmarksfly.cn

[B14] 判断值是否在集合内
来源：http://io.hahajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://sr.bjjhwx.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://id.yuexingan06.cn

JS:   [1, 2, 3].includes(x)
来源：http://tv.nicolike.cn

TS:   [1, 2, 3].includes(x)
来源：http://wx.chemitech.net.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ur.colortex.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sa.szsharing.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zt.yuntaijiaju.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bq.szsharing.cn

[B15] 布尔运算与取反
来源：http://di.asd995.cn

Py:   a and b or not c
来源：http://ks.9csxet.cn

PHP:  $a && $b || !$c
来源：http://dq.panjiajie.cn

JS:   a && b || !c
来源：http://vk.jianghongdianzi.cn

TS:   a && b || !c
来源：http://op.shxzskj.cn

Java: a && b || !c
来源：http://pt.muxihuayi.cn

Go:   a && b || !c
来源：http://vh.gzmigu.cn

Ruby: a && b || !c
来源：http://vs.9csxet.cn

C#:   a && b || !c
来源：http://kk.colortex.cn

[B16] 卫语句：不满足条件提前返回
来源：http://th.yuntaijiaju.cn

Py:   if not data: return
来源：http://ge.lnxyls.cn

PHP:  if (!$data) { return; }
来源：http://md.bjjhwx.cn

JS:   if (!data) return;
来源：http://og.yuntaijiaju.cn

TS:   if (!data) return;
来源：http://gj.gzmigu.cn

Java: if (data == null) return;
来源：http://rf.yuntaijiaju.cn

Go:   if data == nil { return }
来源：http://in.nszjky.cn

Ruby: return if data.nil?
来源：http://bo.chemitech.net.cn

C#:   if (data == null) return;
来源：http://cc.gzmigu.cn

================================================================================
来源：http://wx.shtwfgs.cn

C. 函数与作用域
来源：http://gg.yuntaijiaju.cn

================================================================================
来源：http://ja.wgjwhj.cn

[C01] 定义函数
来源：http://iq.hnjuh.cn

Py:   def add(a, b): return a + b
来源：http://nz.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kt.huixiangedu.cn

JS:   function add(a, b) { return a + b; }
来源：http://ed.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nx.shxzukj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vq.jctech888.com.cn

Go:   func add(a, b int) int { return a + b }
来源：http://gf.wgjwhj.cn

Ruby: def add(a, b); a + b; end
来源：http://ij.panjiajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wz.shtwfgs.cn

[C02] 默认参数
来源：http://mh.gzmigu.cn

Py:   def greet(name="World"): return name
来源：http://hj.nszjky.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://jp.hahajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://pf.shtwfgs.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://eo.lnxyls.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://xj.lnxyls.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dc.wgjwhj.cn

Ruby: def greet(name = "World") = name
来源：http://vr.jctech888.com.cn

C#:   string Greet(string name = "World") => name;
来源：http://ak.gzmigu.cn

[C03] 可变参数
来源：http://ue.shtwfgs.cn

Py:   def total(*args): return sum(args)
来源：http://pw.lnxyls.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pc.chemitech.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tt.bookmarksfly.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hj.asd995.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://oe.hnjuh.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ys.muxihuayi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rd.panjiajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wo.wgjwhj.cn

[C04] 命名参数 / 关键字参数
来源：http://tu.shxzskj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cy.gzmigu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://iu.bjjhwx.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dh.panjiajie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://br.bookmarksfly.cn

Java: // 无：用 Builder 模式或 record
来源：http://rk.nszjky.cn

Go:   // 无：用配置结构体参数
来源：http://mo.gzmigu.cn

Ruby: f(a: 1, b: 2)
来源：http://fo.chemitech.net.cn

C#:   f(a: 1, b: 2)
来源：http://wp.muxihuayi.cn

[C05] 返回多个值
来源：http://ac.huanxung.cn

Py:   return a, b
来源：http://bp.colortex.cn

PHP:  return [$a, $b];
来源：http://zh.521024.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zz.gzmigu.cn

TS:   return { a, b };
来源：http://lh.nszjky.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sh.nszjky.cn

Go:   return a, b
来源：http://ib.asd995.cn

Ruby: return a, b
来源：http://yv.hnjuh.cn

C#:   return (a, b);              // ValueTuple
来源：http://oh.bookmarksfly.cn

[C06] 匿名函数 / lambda
来源：http://sb.jctech888.com.cn

Py:   square = lambda x: x * x
来源：http://dc.haigaiapp.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://gt.hnjuh.cn

JS:   const square = x => x * x;
来源：http://nz.shtwfgs.cn

TS:   const square = (x: number): number => x * x;
来源：http://wm.newstarts.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kp.hnjuh.cn

Go:   sq := func(x int) int { return x * x }
来源：http://mr.chemitech.net.cn

Ruby: square = ->(x) { x * x }
来源：http://ak.huanxung.cn

C#:   Func<int, int> square = x => x * x;
来源：http://oi.yuntaijiaju.cn

[C07] 把函数作为参数传入
来源：http://dr.newstarts.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://iu.szxytkj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bk.shxzukj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pg.newstarts.cn

TS:   arr.map(String)
来源：http://io.jianghongdianzi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kw.shxzskj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mq.asd995.cn

Ruby: arr.map(&:upcase)
来源：http://jg.yuntaijiaju.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pm.haigaiapp.cn

[C08] 闭包
来源：http://vt.nicolike.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gr.asd995.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ja.asd995.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sq.gzmigu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kw.haigaiapp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fl.szsharing.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dq.lnxyls.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yg.chemitech.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vy.newstarts.cn

[C09] 递归
来源：http://qn.nicolike.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dg.huanxung.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uv.panjiajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://es.huixinmuqiang.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ab.szsharing.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://js.asd995.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ys.wgjwhj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hk.shxzskj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yv.asd995.cn

[C10] 变量作用域
来源：http://fj.jianghongdianzi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://py.szsharing.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zo.huixiangedu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gh.yuntaijiaju.cn

TS:   同 JS
来源：http://dd.asd995.cn

Java: 方法内为块级作用域
来源：http://zf.nszjky.cn

Go:   花括号块级作用域
来源：http://rf.panjiajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uh.huixinmuqiang.cn

C#:   块级作用域
来源：http://ke.szxytkj.cn

[C11] 模块导入与导出
来源：http://sc.nszjky.cn

Py:   from module import func
来源：http://ps.yuexingan06.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://iz.hahajie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://lc.chemitech.net.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qe.jianghongdianzi.cn

Java: import java.util.List;
来源：http://im.wgjwhj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ne.shxzskj.cn

Ruby: require "json"; require_relative "./util"
来源：http://to.hnjuh.cn

C#:   using System.Text;
来源：http://hx.haigaiapp.cn

[C12] 立即执行函数 IIFE
来源：http://ce.nicolike.cn

Py:   (lambda: print("run"))()
来源：http://hl.muxihuayi.cn

PHP:  (function () { echo "run"; })();
来源：http://jh.huixinmuqiang.cn

JS:   (() => { console.log("run"); })();
来源：http://lk.521024.cn

TS:   (() => { console.log("run"); })();
来源：http://gg.panjiajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gf.newstarts.cn

Go:   func() { fmt.Println("run") }()
来源：http://df.shtwfgs.cn

Ruby: -> { puts "run" }.call
来源：http://pa.lnxyls.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://bb.newstarts.cn

[C13] 类型声明 / 类型注解
来源：http://ym.huixinmuqiang.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cs.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xd.hnjuh.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cq.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zd.hahajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://dn.chemitech.net.cn

Go:   func add(a, b int) int
来源：http://gg.521024.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pz.bookmarksfly.cn

C#:   int Add(int a, int b) => a + b;
来源：http://sm.asd995.cn

[C14] 泛型函数
来源：http://ms.huanxung.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ql.jianghongdianzi.cn

PHP:  // 无泛型
来源：http://fk.newstarts.cn

JS:   // 无泛型
来源：http://zo.hnjuh.cn


<!-- 参考信息 -->