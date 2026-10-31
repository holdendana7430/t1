代发 wailian999

TS:   s.length
来源：http://zl.szsharing.cn

Java: s.length()
来源：http://bz.szxytkj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dk.jctech888.com.cn

Ruby: s.length
来源：http://eg.muxihuayi.cn

C#:   s.Length
来源：http://qu.yuexingan06.cn

[A23] 大小写转换
来源：http://ag.521024.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zp.muxihuayi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yy.nicolike.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://iz.muxihuayi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cd.hahajie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qm.hnjuh.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dc.jctech888.com.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://du.gzmigu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ug.nicolike.cn

[A24] 去除首尾空白
来源：http://dq.shxzukj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zb.newstarts.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nz.9csxet.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zc.panjiajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ym.bjjhwx.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ah.shxzukj.cn

Go:   strings.TrimSpace(s)
来源：http://ne.muxihuayi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mr.hahajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jz.szsharing.cn

[A25] 字符串比较
来源：http://pi.hnjuh.cn

Py:   s1 == s2; s1 != s2
来源：http://yb.shxzskj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://eb.nszjky.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ik.newstarts.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ma.huanxung.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://st.szxytkj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.gzmigu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vd.shxzukj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ue.hnjuh.cn

[A26] 类型转换总览
来源：http://ie.bjjhwx.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dk.yuntaijiaju.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wl.colortex.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fn.newstarts.cn

TS:   Number() String() Boolean() x as number
来源：http://iy.yuntaijiaju.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://td.hnjuh.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ty.yuexingan06.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ol.jianghongdianzi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tq.muxihuayi.cn

================================================================================
来源：http://rp.hnjuh.cn

B. 流程控制
来源：http://yr.9csxet.cn

================================================================================
来源：http://ng.yuntaijiaju.cn

[B01] 条件判断 if / else
来源：http://ya.huixinmuqiang.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://mm.muxihuayi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bi.shtwfgs.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mn.panjiajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gn.szsharing.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://gk.521024.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://sn.shtwfgs.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://iu.chemitech.net.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kj.jianghongdianzi.cn

[B02] 多分支 else if / elif
来源：http://kx.nicolike.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fp.9csxet.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nx.shxzskj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ye.panjiajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qz.haigaiapp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ms.nicolike.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hu.newstarts.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nu.shxzskj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wc.asd995.cn

[B03] switch / match / case
来源：http://tq.yuntaijiaju.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://eq.yuntaijiaju.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lj.jianghongdianzi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gm.huixinmuqiang.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rq.hnjuh.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vd.szsharing.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lk.gzmigu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qq.9csxet.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kz.shxzskj.cn

[B04] for 计数循环
来源：http://ve.haigaiapp.cn

Py:   for i in range(10): print(i)
来源：http://ad.panjiajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ts.gzmigu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jn.gzmigu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ha.huixiangedu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://on.newstarts.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wl.jctech888.com.cn

Ruby: 10.times { |i| puts i }
来源：http://re.huixiangedu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pv.chemitech.net.cn

[B05] 遍历数组 / 列表
来源：http://sz.yuntaijiaju.cn

Py:   for item in arr: print(item)
来源：http://mo.muxihuayi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ot.szsharing.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://nm.szsharing.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ok.yuexingan06.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hq.chemitech.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kz.hahajie.cn

Ruby: arr.each { |item| puts item }
来源：http://ks.muxihuayi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jm.nicolike.cn

[B06] 遍历字典 / 对象
来源：http://bu.szsharing.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tn.hahajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.wgjwhj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vc.jianghongdianzi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ib.huixiangedu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://of.wgjwhj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://oi.nszjky.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sn.hahajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nh.bjjhwx.cn

[B07] while 循环
来源：http://vr.wgjwhj.cn

Py:   while i < 10: i += 1
来源：http://lj.jianghongdianzi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ga.9csxet.cn

JS:   while (i < 10) { i++; }
来源：http://ny.haigaiapp.cn

TS:   while (i < 10) { i++; }
来源：http://ve.szsharing.cn

Java: while (i < 10) { i++; }
来源：http://kd.bookmarksfly.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bw.szxytkj.cn

Ruby: while i < 10; i += 1; end
来源：http://og.szsharing.cn

C#:   while (i < 10) { i++; }
来源：http://kh.asd995.cn

[B08] do-while（至少执行一次）
来源：http://nz.jctech888.com.cn

Py:   # 无 do-while：用 while True + break
来源：http://va.wgjwhj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://az.521024.cn

JS:   do { i++; } while (i < 10);
来源：http://dn.jianghongdianzi.cn

TS:   do { i++; } while (i < 10);
来源：http://dx.bookmarksfly.cn

Java: do { i++; } while (i < 10);
来源：http://iz.521024.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ki.shtwfgs.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fc.shxzukj.cn

C#:   do { i++; } while (i < 10);
来源：http://bt.muxihuayi.cn

[B09] break 与 continue
来源：http://ao.nicolike.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rm.521024.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qw.chemitech.net.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jx.wgjwhj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ic.nszjky.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tg.huanxung.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://oa.huixiangedu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yn.newstarts.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://el.bookmarksfly.cn

[B10] 遍历同时拿索引
来源：http://un.521024.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cp.szsharing.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://iu.chemitech.net.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xq.yuexingan06.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zl.szxytkj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nf.chemitech.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ij.9csxet.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kx.huixinmuqiang.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jc.yuexingan06.cn

[B11] 生成数字序列 / 区间
来源：http://xr.szsharing.cn

Py:   list(range(0, 10, 2))
来源：http://co.haigaiapp.cn

PHP:  range(0, 10, 2);
来源：http://pi.lnxyls.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pv.9csxet.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jy.chemitech.net.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vp.gzmigu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://su.asd995.cn

Ruby: (0...10).step(2).to_a
来源：http://ql.bookmarksfly.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dt.hnjuh.cn

[B12] 跳出多层循环
来源：http://un.szsharing.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ke.nicolike.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://db.panjiajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sh.szsharing.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yf.shtwfgs.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://un.yuntaijiaju.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dy.bjjhwx.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sa.muxihuayi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sc.colortex.cn

[B13] 判断是否为数字
来源：http://ym.521024.cn

Py:   isinstance(x, (int, float))
来源：http://mm.yuexingan06.cn

PHP:  is_numeric($x)
来源：http://pu.huanxung.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fa.chemitech.net.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://co.asd995.cn

Java: x instanceof Number
来源：http://cl.huixinmuqiang.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rd.nicolike.cn

Ruby: x.is_a?(Numeric)
来源：http://xa.szxytkj.cn

C#:   x is int or double or decimal
来源：http://dr.wgjwhj.cn

[B14] 判断值是否在集合内
来源：http://ka.bookmarksfly.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cs.newstarts.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wm.newstarts.cn

JS:   [1, 2, 3].includes(x)
来源：http://as.shxzskj.cn

TS:   [1, 2, 3].includes(x)
来源：http://jg.szsharing.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ax.nicolike.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ye.chemitech.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://lg.yuexingan06.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cf.newstarts.cn

[B15] 布尔运算与取反
来源：http://xq.haigaiapp.cn

Py:   a and b or not c
来源：http://zi.asd995.cn

PHP:  $a && $b || !$c
来源：http://qb.wgjwhj.cn

JS:   a && b || !c
来源：http://id.huanxung.cn

TS:   a && b || !c
来源：http://qb.jctech888.com.cn

Java: a && b || !c
来源：http://pl.huixiangedu.cn

Go:   a && b || !c
来源：http://wp.szsharing.cn

Ruby: a && b || !c
来源：http://yx.bookmarksfly.cn

C#:   a && b || !c
来源：http://cz.yuntaijiaju.cn

[B16] 卫语句：不满足条件提前返回
来源：http://kp.shxzukj.cn

Py:   if not data: return
来源：http://dw.lnxyls.cn

PHP:  if (!$data) { return; }
来源：http://sl.asd995.cn

JS:   if (!data) return;
来源：http://kj.szsharing.cn

TS:   if (!data) return;
来源：http://jn.nszjky.cn

Java: if (data == null) return;
来源：http://ub.lnxyls.cn

Go:   if data == nil { return }
来源：http://ik.huanxung.cn

Ruby: return if data.nil?
来源：http://pm.huixiangedu.cn

C#:   if (data == null) return;
来源：http://ma.hahajie.cn

================================================================================
来源：http://gj.haigaiapp.cn

C. 函数与作用域
来源：http://xv.521024.cn

================================================================================
来源：http://tg.bjjhwx.cn

[C01] 定义函数
来源：http://af.yuexingan06.cn

Py:   def add(a, b): return a + b
来源：http://ji.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sx.newstarts.cn

JS:   function add(a, b) { return a + b; }
来源：http://hw.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fr.haigaiapp.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://jk.bjjhwx.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qx.nszjky.cn

Ruby: def add(a, b); a + b; end
来源：http://jz.jctech888.com.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yp.yuntaijiaju.cn

[C02] 默认参数
来源：http://rh.wgjwhj.cn

Py:   def greet(name="World"): return name
来源：http://qo.jctech888.com.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://nn.muxihuayi.cn

JS:   function greet(name = "World") { return name; }
来源：http://lu.colortex.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cf.szsharing.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jl.hahajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yz.521024.cn

Ruby: def greet(name = "World") = name
来源：http://xd.nicolike.cn

C#:   string Greet(string name = "World") => name;
来源：http://kw.szxytkj.cn

[C03] 可变参数
来源：http://xr.521024.cn

Py:   def total(*args): return sum(args)
来源：http://wy.yuntaijiaju.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bk.yuexingan06.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yl.szsharing.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qq.muxihuayi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pa.szxytkj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rl.panjiajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hc.wgjwhj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://uy.jianghongdianzi.cn

[C04] 命名参数 / 关键字参数
来源：http://ur.shtwfgs.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cm.wgjwhj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://my.shxzskj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rv.yuntaijiaju.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gy.jctech888.com.cn

Java: // 无：用 Builder 模式或 record
来源：http://yh.newstarts.cn

Go:   // 无：用配置结构体参数
来源：http://ev.521024.cn

Ruby: f(a: 1, b: 2)
来源：http://tf.lnxyls.cn

C#:   f(a: 1, b: 2)
来源：http://ma.jctech888.com.cn

[C05] 返回多个值
来源：http://kp.shxzukj.cn

Py:   return a, b
来源：http://ej.gzmigu.cn

PHP:  return [$a, $b];
来源：http://ew.521024.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pz.shxzskj.cn

TS:   return { a, b };
来源：http://wp.bookmarksfly.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mu.yuntaijiaju.cn

Go:   return a, b
来源：http://uk.asd995.cn

Ruby: return a, b
来源：http://kr.huanxung.cn

C#:   return (a, b);              // ValueTuple
来源：http://iu.panjiajie.cn

[C06] 匿名函数 / lambda
来源：http://vt.panjiajie.cn

Py:   square = lambda x: x * x
来源：http://eq.colortex.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://be.nszjky.cn

JS:   const square = x => x * x;
来源：http://id.shxzukj.cn

TS:   const square = (x: number): number => x * x;
来源：http://yo.nszjky.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://at.huixiangedu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jx.huanxung.cn

Ruby: square = ->(x) { x * x }
来源：http://wb.yuexingan06.cn

C#:   Func<int, int> square = x => x * x;
来源：http://eq.newstarts.cn

[C07] 把函数作为参数传入
来源：http://ml.chemitech.net.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gj.bookmarksfly.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kh.hnjuh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nd.szsharing.cn

TS:   arr.map(String)
来源：http://nv.yuexingan06.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hp.nszjky.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ls.huanxung.cn

Ruby: arr.map(&:upcase)
来源：http://we.szxytkj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wn.521024.cn

[C08] 闭包
来源：http://mo.bjjhwx.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tg.yuexingan06.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dn.huixiangedu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cg.jianghongdianzi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vr.gzmigu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vc.colortex.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rw.hahajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tz.jctech888.com.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wz.gzmigu.cn

[C09] 递归
来源：http://cz.jctech888.com.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zb.asd995.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lv.shxzskj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hu.bjjhwx.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qf.hnjuh.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ct.haigaiapp.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xf.shxzukj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mp.chemitech.net.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xz.huanxung.cn

[C10] 变量作用域
来源：http://bw.colortex.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qw.jctech888.com.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fi.haigaiapp.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://og.nszjky.cn

TS:   同 JS
来源：http://ak.colortex.cn

Java: 方法内为块级作用域
来源：http://gb.huanxung.cn

Go:   花括号块级作用域
来源：http://zi.szxytkj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xt.huanxung.cn

C#:   块级作用域
来源：http://nd.szxytkj.cn

[C11] 模块导入与导出
来源：http://hg.newstarts.cn

Py:   from module import func
来源：http://ut.yuntaijiaju.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zb.bookmarksfly.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://nw.chemitech.net.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gf.jianghongdianzi.cn

Java: import java.util.List;
来源：http://do.newstarts.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://en.nszjky.cn

Ruby: require "json"; require_relative "./util"
来源：http://ta.chemitech.net.cn

C#:   using System.Text;
来源：http://bl.muxihuayi.cn

[C12] 立即执行函数 IIFE
来源：http://yt.colortex.cn

Py:   (lambda: print("run"))()
来源：http://je.newstarts.cn

PHP:  (function () { echo "run"; })();
来源：http://su.bookmarksfly.cn

JS:   (() => { console.log("run"); })();
来源：http://cs.yuexingan06.cn

TS:   (() => { console.log("run"); })();
来源：http://dv.shxzukj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ow.jctech888.com.cn

Go:   func() { fmt.Println("run") }()
来源：http://gd.shtwfgs.cn

Ruby: -> { puts "run" }.call
来源：http://lk.asd995.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://rv.huixinmuqiang.cn

[C13] 类型声明 / 类型注解
来源：http://zp.521024.cn


<!-- 参考信息 -->