代发 wailian999

C#:   s.Length
来源：http://ip.yuexingan06.cn

[A23] 大小写转换
来源：http://dy.shxzukj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://nh.panjiajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hb.asd995.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xz.jctech888.com.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gp.huixinmuqiang.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://po.jctech888.com.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://it.9csxet.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bg.jctech888.com.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://oc.hahajie.cn

[A24] 去除首尾空白
来源：http://pm.yuexingan06.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://yr.newstarts.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xu.yuntaijiaju.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sm.huixinmuqiang.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://me.panjiajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wh.huixiangedu.cn

Go:   strings.TrimSpace(s)
来源：http://xj.lnxyls.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://oo.yuexingan06.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vb.shxzskj.cn

[A25] 字符串比较
来源：http://dm.shxzskj.cn

Py:   s1 == s2; s1 != s2
来源：http://up.lnxyls.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dd.szxytkj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://th.panjiajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zv.lnxyls.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nt.newstarts.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vm.huanxung.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://js.colortex.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cn.521024.cn

[A26] 类型转换总览
来源：http://yi.hnjuh.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fe.szxytkj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jj.shxzukj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://oq.gzmigu.cn

TS:   Number() String() Boolean() x as number
来源：http://sw.muxihuayi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ct.haigaiapp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yg.jianghongdianzi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://qx.huixiangedu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://is.hnjuh.cn

================================================================================
来源：http://jr.jctech888.com.cn

B. 流程控制
来源：http://bz.shtwfgs.cn

================================================================================
来源：http://ix.panjiajie.cn

[B01] 条件判断 if / else
来源：http://he.shtwfgs.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ek.hnjuh.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://te.9csxet.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pa.huixiangedu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sf.bjjhwx.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://wd.wgjwhj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ss.521024.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yn.szsharing.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hf.hahajie.cn

[B02] 多分支 else if / elif
来源：http://im.huixinmuqiang.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yk.hahajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://il.hnjuh.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qp.shtwfgs.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ch.hahajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pe.bjjhwx.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bw.yuntaijiaju.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://sm.chemitech.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eh.shtwfgs.cn

[B03] switch / match / case
来源：http://fc.asd995.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ta.shtwfgs.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ih.lnxyls.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mi.hahajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qb.bjjhwx.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wk.lnxyls.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ud.nicolike.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dz.chemitech.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tx.shxzskj.cn

[B04] for 计数循环
来源：http://zb.nszjky.cn

Py:   for i in range(10): print(i)
来源：http://kr.hahajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xi.newstarts.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ku.nszjky.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rg.newstarts.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ai.chemitech.net.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zf.gzmigu.cn

Ruby: 10.times { |i| puts i }
来源：http://lr.yuntaijiaju.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wo.huanxung.cn

[B05] 遍历数组 / 列表
来源：http://dn.yuntaijiaju.cn

Py:   for item in arr: print(item)
来源：http://ab.lnxyls.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://si.yuntaijiaju.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://re.hnjuh.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rt.szsharing.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jb.nszjky.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xt.bjjhwx.cn

Ruby: arr.each { |item| puts item }
来源：http://ad.hnjuh.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xf.521024.cn

[B06] 遍历字典 / 对象
来源：http://sg.szxytkj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://uw.shtwfgs.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ol.bookmarksfly.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yq.huanxung.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ix.9csxet.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yw.shxzskj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sp.muxihuayi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nd.nicolike.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tu.chemitech.net.cn

[B07] while 循环
来源：http://xw.lnxyls.cn

Py:   while i < 10: i += 1
来源：http://lx.yuntaijiaju.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mq.haigaiapp.cn

JS:   while (i < 10) { i++; }
来源：http://ty.panjiajie.cn

TS:   while (i < 10) { i++; }
来源：http://yz.panjiajie.cn

Java: while (i < 10) { i++; }
来源：http://pe.hahajie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qz.huixiangedu.cn

Ruby: while i < 10; i += 1; end
来源：http://we.muxihuayi.cn

C#:   while (i < 10) { i++; }
来源：http://zu.huanxung.cn

[B08] do-while（至少执行一次）
来源：http://dy.haigaiapp.cn

Py:   # 无 do-while：用 while True + break
来源：http://gq.9csxet.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ya.szxytkj.cn

JS:   do { i++; } while (i < 10);
来源：http://qj.lnxyls.cn

TS:   do { i++; } while (i < 10);
来源：http://dz.hahajie.cn

Java: do { i++; } while (i < 10);
来源：http://ic.bjjhwx.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ww.9csxet.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mm.muxihuayi.cn

C#:   do { i++; } while (i < 10);
来源：http://qd.521024.cn

[B09] break 与 continue
来源：http://qy.haigaiapp.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sn.huixiangedu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wm.panjiajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zt.muxihuayi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://my.huixiangedu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zh.hahajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xg.shxzskj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://at.nszjky.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cr.shtwfgs.cn

[B10] 遍历同时拿索引
来源：http://bg.bookmarksfly.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rf.gzmigu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zh.huanxung.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bj.hahajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vs.yuntaijiaju.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wd.9csxet.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cg.muxihuayi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://th.gzmigu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cf.hnjuh.cn

[B11] 生成数字序列 / 区间
来源：http://ey.colortex.cn

Py:   list(range(0, 10, 2))
来源：http://lc.szsharing.cn

PHP:  range(0, 10, 2);
来源：http://pa.shxzskj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pi.newstarts.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mq.huixiangedu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pu.newstarts.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fg.colortex.cn

Ruby: (0...10).step(2).to_a
来源：http://zh.colortex.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://at.yuntaijiaju.cn

[B12] 跳出多层循环
来源：http://lp.shtwfgs.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://be.huanxung.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://se.newstarts.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hr.jctech888.com.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mp.shxzukj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ul.hnjuh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lp.szxytkj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ji.hnjuh.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yu.wgjwhj.cn

[B13] 判断是否为数字
来源：http://nc.gzmigu.cn

Py:   isinstance(x, (int, float))
来源：http://pp.shtwfgs.cn

PHP:  is_numeric($x)
来源：http://ot.yuntaijiaju.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bk.colortex.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bf.shxzukj.cn

Java: x instanceof Number
来源：http://io.shxzskj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ab.jianghongdianzi.cn

Ruby: x.is_a?(Numeric)
来源：http://sa.haigaiapp.cn

C#:   x is int or double or decimal
来源：http://um.yuexingan06.cn

[B14] 判断值是否在集合内
来源：http://mr.szxytkj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ox.bjjhwx.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kd.szxytkj.cn

JS:   [1, 2, 3].includes(x)
来源：http://di.shxzukj.cn

TS:   [1, 2, 3].includes(x)
来源：http://ls.shxzskj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://jt.chemitech.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ji.shxzukj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://kl.szxytkj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bx.lnxyls.cn

[B15] 布尔运算与取反
来源：http://jy.haigaiapp.cn

Py:   a and b or not c
来源：http://ck.haigaiapp.cn

PHP:  $a && $b || !$c
来源：http://ii.yuexingan06.cn

JS:   a && b || !c
来源：http://pj.colortex.cn

TS:   a && b || !c
来源：http://kx.newstarts.cn

Java: a && b || !c
来源：http://hs.huixinmuqiang.cn

Go:   a && b || !c
来源：http://aq.yuexingan06.cn

Ruby: a && b || !c
来源：http://py.gzmigu.cn

C#:   a && b || !c
来源：http://po.szsharing.cn

[B16] 卫语句：不满足条件提前返回
来源：http://cz.szsharing.cn

Py:   if not data: return
来源：http://ox.szsharing.cn

PHP:  if (!$data) { return; }
来源：http://lx.szsharing.cn

JS:   if (!data) return;
来源：http://fy.nicolike.cn

TS:   if (!data) return;
来源：http://ad.jctech888.com.cn

Java: if (data == null) return;
来源：http://dp.9csxet.cn

Go:   if data == nil { return }
来源：http://qx.bookmarksfly.cn

Ruby: return if data.nil?
来源：http://os.hnjuh.cn

C#:   if (data == null) return;
来源：http://hf.colortex.cn

================================================================================
来源：http://lj.huanxung.cn

C. 函数与作用域
来源：http://mg.bookmarksfly.cn

================================================================================
来源：http://dw.asd995.cn

[C01] 定义函数
来源：http://ca.huixinmuqiang.cn

Py:   def add(a, b): return a + b
来源：http://nz.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mc.huixiangedu.cn

JS:   function add(a, b) { return a + b; }
来源：http://eo.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gd.shxzukj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://jq.huixiangedu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ur.hahajie.cn

Ruby: def add(a, b); a + b; end
来源：http://hh.huixiangedu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xa.wgjwhj.cn

[C02] 默认参数
来源：http://ob.newstarts.cn

Py:   def greet(name="World"): return name
来源：http://eo.huixinmuqiang.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://pc.bjjhwx.cn

JS:   function greet(name = "World") { return name; }
来源：http://zb.chemitech.net.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://we.9csxet.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://gp.hahajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://aa.gzmigu.cn

Ruby: def greet(name = "World") = name
来源：http://yx.wgjwhj.cn

C#:   string Greet(string name = "World") => name;
来源：http://uw.shxzukj.cn

[C03] 可变参数
来源：http://nf.yuntaijiaju.cn

Py:   def total(*args): return sum(args)
来源：http://ss.jctech888.com.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://na.gzmigu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xp.huixinmuqiang.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ib.colortex.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ju.hnjuh.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fi.colortex.cn

Ruby: def total(*nums); nums.sum; end
来源：http://cm.shtwfgs.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fe.panjiajie.cn

[C04] 命名参数 / 关键字参数
来源：http://su.shxzukj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://iq.jctech888.com.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pj.huixinmuqiang.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sx.yuexingan06.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xz.hahajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://hw.lnxyls.cn

Go:   // 无：用配置结构体参数
来源：http://gm.9csxet.cn

Ruby: f(a: 1, b: 2)
来源：http://wl.asd995.cn

C#:   f(a: 1, b: 2)
来源：http://cu.haigaiapp.cn

[C05] 返回多个值
来源：http://pf.huixinmuqiang.cn

Py:   return a, b
来源：http://hc.shxzukj.cn

PHP:  return [$a, $b];
来源：http://ry.panjiajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pr.haigaiapp.cn

TS:   return { a, b };
来源：http://vd.bookmarksfly.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kr.bookmarksfly.cn

Go:   return a, b
来源：http://wr.hnjuh.cn

Ruby: return a, b
来源：http://pi.521024.cn

C#:   return (a, b);              // ValueTuple
来源：http://vc.panjiajie.cn

[C06] 匿名函数 / lambda
来源：http://tb.jianghongdianzi.cn

Py:   square = lambda x: x * x
来源：http://of.nszjky.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://vu.jianghongdianzi.cn

JS:   const square = x => x * x;
来源：http://hu.9csxet.cn

TS:   const square = (x: number): number => x * x;
来源：http://bm.bjjhwx.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cn.jianghongdianzi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://yl.panjiajie.cn

Ruby: square = ->(x) { x * x }
来源：http://wc.colortex.cn

C#:   Func<int, int> square = x => x * x;
来源：http://nv.newstarts.cn

[C07] 把函数作为参数传入
来源：http://dk.9csxet.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qc.szsharing.cn

PHP:  array_map("strtoupper", $arr);
来源：http://rg.hahajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sw.shxzskj.cn

TS:   arr.map(String)
来源：http://kh.nszjky.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gf.chemitech.net.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://st.hnjuh.cn

Ruby: arr.map(&:upcase)
来源：http://zh.jianghongdianzi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://sx.bjjhwx.cn

[C08] 闭包
来源：http://fz.shtwfgs.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tl.nszjky.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ef.bookmarksfly.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hy.9csxet.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ks.521024.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gb.nicolike.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zm.521024.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qh.bookmarksfly.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ch.hnjuh.cn

[C09] 递归
来源：http://gd.szsharing.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vq.huixinmuqiang.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qk.jctech888.com.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gf.szsharing.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yl.szxytkj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zn.chemitech.net.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://io.colortex.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xo.lnxyls.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fx.jianghongdianzi.cn

[C10] 变量作用域
来源：http://en.muxihuayi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yq.lnxyls.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cj.gzmigu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bz.huixinmuqiang.cn

TS:   同 JS
来源：http://qt.chemitech.net.cn

Java: 方法内为块级作用域
来源：http://zg.bookmarksfly.cn

Go:   花括号块级作用域
来源：http://yi.lnxyls.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dq.bjjhwx.cn

C#:   块级作用域
来源：http://co.jctech888.com.cn

[C11] 模块导入与导出
来源：http://qe.huixinmuqiang.cn

Py:   from module import func
来源：http://vo.521024.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://aa.wgjwhj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ep.jianghongdianzi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sf.bookmarksfly.cn

Java: import java.util.List;
来源：http://rt.9csxet.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ph.jctech888.com.cn

Ruby: require "json"; require_relative "./util"
来源：http://nz.newstarts.cn

C#:   using System.Text;
来源：http://oj.521024.cn

[C12] 立即执行函数 IIFE
来源：http://oa.huixiangedu.cn

Py:   (lambda: print("run"))()
来源：http://qn.jctech888.com.cn

PHP:  (function () { echo "run"; })();
来源：http://gn.szsharing.cn

JS:   (() => { console.log("run"); })();
来源：http://ye.huanxung.cn

TS:   (() => { console.log("run"); })();
来源：http://xe.shxzukj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qs.nicolike.cn

Go:   func() { fmt.Println("run") }()
来源：http://sd.huanxung.cn

Ruby: -> { puts "run" }.call
来源：http://ty.chemitech.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://hv.hahajie.cn

[C13] 类型声明 / 类型注解
来源：http://ao.bookmarksfly.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yh.haigaiapp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gs.shxzskj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dc.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ox.lnxyls.cn


<!-- 参考信息 -->