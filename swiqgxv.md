代发 wailian999

C#:   s.Length
来源：http://sq.jianghongdianzi.cn

[A23] 大小写转换
来源：http://dy.hahajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://io.521024.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ys.nicolike.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://oy.bookmarksfly.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://we.asd995.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ji.jctech888.com.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gh.lnxyls.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wu.shtwfgs.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://jr.jctech888.com.cn

[A24] 去除首尾空白
来源：http://ra.shxzukj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bf.szxytkj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dh.jianghongdianzi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vj.lnxyls.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ih.szsharing.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ns.szxytkj.cn

Go:   strings.TrimSpace(s)
来源：http://kk.huanxung.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mf.colortex.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://iu.szsharing.cn

[A25] 字符串比较
来源：http://rg.nszjky.cn

Py:   s1 == s2; s1 != s2
来源：http://tu.jctech888.com.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pv.shxzskj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xi.shxzskj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lw.jianghongdianzi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ka.nszjky.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ce.shxzukj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rd.hnjuh.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fy.521024.cn

[A26] 类型转换总览
来源：http://un.huixiangedu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zp.huixinmuqiang.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://do.wgjwhj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ka.shxzskj.cn

TS:   Number() String() Boolean() x as number
来源：http://ow.huixinmuqiang.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kx.gzmigu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://at.shxzskj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://el.yuexingan06.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xu.jianghongdianzi.cn

================================================================================
来源：http://vg.shtwfgs.cn

B. 流程控制
来源：http://ud.bookmarksfly.cn

================================================================================
来源：http://oq.gzmigu.cn

[B01] 条件判断 if / else
来源：http://gn.nszjky.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dk.colortex.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wn.szxytkj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mn.shxzskj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://es.colortex.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://wg.gzmigu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kt.szxytkj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sb.colortex.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://uk.lnxyls.cn

[B02] 多分支 else if / elif
来源：http://km.gzmigu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vw.521024.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ti.colortex.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ha.bjjhwx.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rc.yuntaijiaju.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gz.muxihuayi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fa.shxzukj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fv.panjiajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ma.muxihuayi.cn

[B03] switch / match / case
来源：http://sw.yuntaijiaju.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vp.asd995.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hh.huanxung.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cp.szsharing.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pg.huanxung.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nq.gzmigu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kr.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dg.9csxet.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bu.nszjky.cn

[B04] for 计数循环
来源：http://fi.jctech888.com.cn

Py:   for i in range(10): print(i)
来源：http://vn.muxihuayi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ro.huixinmuqiang.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.nicolike.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fd.szxytkj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bx.jctech888.com.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://uh.shtwfgs.cn

Ruby: 10.times { |i| puts i }
来源：http://wf.shxzukj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://oo.szxytkj.cn

[B05] 遍历数组 / 列表
来源：http://oh.521024.cn

Py:   for item in arr: print(item)
来源：http://wz.gzmigu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ku.gzmigu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://go.shtwfgs.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xa.huixiangedu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://iq.huixinmuqiang.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ym.shtwfgs.cn

Ruby: arr.each { |item| puts item }
来源：http://uu.huanxung.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ad.chemitech.net.cn

[B06] 遍历字典 / 对象
来源：http://js.huixiangedu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://bw.bookmarksfly.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pf.haigaiapp.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dq.panjiajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sn.shxzskj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xz.panjiajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mj.bookmarksfly.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://if.hahajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ub.jctech888.com.cn

[B07] while 循环
来源：http://kh.huanxung.cn

Py:   while i < 10: i += 1
来源：http://jd.wgjwhj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fl.hahajie.cn

JS:   while (i < 10) { i++; }
来源：http://ob.shtwfgs.cn

TS:   while (i < 10) { i++; }
来源：http://ea.yuntaijiaju.cn

Java: while (i < 10) { i++; }
来源：http://wt.panjiajie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ok.lnxyls.cn

Ruby: while i < 10; i += 1; end
来源：http://fk.lnxyls.cn

C#:   while (i < 10) { i++; }
来源：http://jq.chemitech.net.cn

[B08] do-while（至少执行一次）
来源：http://yw.szsharing.cn

Py:   # 无 do-while：用 while True + break
来源：http://ax.huixiangedu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vo.haigaiapp.cn

JS:   do { i++; } while (i < 10);
来源：http://sb.hnjuh.cn

TS:   do { i++; } while (i < 10);
来源：http://kh.jctech888.com.cn

Java: do { i++; } while (i < 10);
来源：http://wa.nszjky.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xx.nszjky.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hp.asd995.cn

C#:   do { i++; } while (i < 10);
来源：http://tr.lnxyls.cn

[B09] break 与 continue
来源：http://he.lnxyls.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ms.bookmarksfly.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hs.huanxung.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mb.jianghongdianzi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tm.9csxet.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bz.muxihuayi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://km.yuexingan06.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ne.9csxet.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qn.haigaiapp.cn

[B10] 遍历同时拿索引
来源：http://ay.panjiajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://eh.9csxet.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kn.hnjuh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ou.bjjhwx.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lc.nszjky.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vd.shxzukj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cu.yuntaijiaju.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dr.szsharing.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gw.521024.cn

[B11] 生成数字序列 / 区间
来源：http://hk.jctech888.com.cn

Py:   list(range(0, 10, 2))
来源：http://zv.shtwfgs.cn

PHP:  range(0, 10, 2);
来源：http://wk.colortex.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qw.521024.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ub.huixinmuqiang.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ht.huixinmuqiang.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sp.jianghongdianzi.cn

Ruby: (0...10).step(2).to_a
来源：http://gq.newstarts.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yv.gzmigu.cn

[B12] 跳出多层循环
来源：http://bq.asd995.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://rk.yuntaijiaju.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://tf.yuexingan06.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ft.bookmarksfly.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gk.huixinmuqiang.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pj.gzmigu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://af.chemitech.net.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://de.nicolike.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bi.hahajie.cn

[B13] 判断是否为数字
来源：http://hj.9csxet.cn

Py:   isinstance(x, (int, float))
来源：http://mk.hahajie.cn

PHP:  is_numeric($x)
来源：http://cs.panjiajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hs.hahajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://as.haigaiapp.cn

Java: x instanceof Number
来源：http://sf.9csxet.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ab.huixinmuqiang.cn

Ruby: x.is_a?(Numeric)
来源：http://an.asd995.cn

C#:   x is int or double or decimal
来源：http://xy.521024.cn

[B14] 判断值是否在集合内
来源：http://kz.szsharing.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ns.521024.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kb.lnxyls.cn

JS:   [1, 2, 3].includes(x)
来源：http://tm.chemitech.net.cn

TS:   [1, 2, 3].includes(x)
来源：http://hf.haigaiapp.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qj.jctech888.com.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pm.muxihuayi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://au.hnjuh.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ny.wgjwhj.cn

[B15] 布尔运算与取反
来源：http://kp.lnxyls.cn

Py:   a and b or not c
来源：http://jf.bookmarksfly.cn

PHP:  $a && $b || !$c
来源：http://kl.asd995.cn

JS:   a && b || !c
来源：http://ql.panjiajie.cn

TS:   a && b || !c
来源：http://za.yuexingan06.cn

Java: a && b || !c
来源：http://fn.shxzukj.cn

Go:   a && b || !c
来源：http://nu.huixinmuqiang.cn

Ruby: a && b || !c
来源：http://uy.muxihuayi.cn

C#:   a && b || !c
来源：http://gl.wgjwhj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xw.huixinmuqiang.cn

Py:   if not data: return
来源：http://um.521024.cn

PHP:  if (!$data) { return; }
来源：http://uv.shxzukj.cn

JS:   if (!data) return;
来源：http://uh.szsharing.cn

TS:   if (!data) return;
来源：http://ci.yuntaijiaju.cn

Java: if (data == null) return;
来源：http://ar.newstarts.cn

Go:   if data == nil { return }
来源：http://qo.bookmarksfly.cn

Ruby: return if data.nil?
来源：http://ds.haigaiapp.cn

C#:   if (data == null) return;
来源：http://da.muxihuayi.cn

================================================================================
来源：http://zg.9csxet.cn

C. 函数与作用域
来源：http://ca.bookmarksfly.cn

================================================================================
来源：http://uq.newstarts.cn

[C01] 定义函数
来源：http://be.haigaiapp.cn

Py:   def add(a, b): return a + b
来源：http://dd.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hk.521024.cn

JS:   function add(a, b) { return a + b; }
来源：http://sf.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hg.521024.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gl.jianghongdianzi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zi.bookmarksfly.cn

Ruby: def add(a, b); a + b; end
来源：http://sj.huanxung.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yi.panjiajie.cn

[C02] 默认参数
来源：http://br.wgjwhj.cn

Py:   def greet(name="World"): return name
来源：http://oa.shxzskj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hc.panjiajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://ri.shxzskj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://op.wgjwhj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qi.bookmarksfly.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://oo.chemitech.net.cn

Ruby: def greet(name = "World") = name
来源：http://cl.huixiangedu.cn

C#:   string Greet(string name = "World") => name;
来源：http://pb.haigaiapp.cn

[C03] 可变参数
来源：http://hy.muxihuayi.cn

Py:   def total(*args): return sum(args)
来源：http://pi.newstarts.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yc.yuntaijiaju.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ym.szxytkj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bi.huixiangedu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sa.lnxyls.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tt.bjjhwx.cn

Ruby: def total(*nums); nums.sum; end
来源：http://op.huixiangedu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://px.szsharing.cn

[C04] 命名参数 / 关键字参数
来源：http://my.jianghongdianzi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tk.muxihuayi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rj.bookmarksfly.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ds.szxytkj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://di.521024.cn

Java: // 无：用 Builder 模式或 record
来源：http://ps.bjjhwx.cn

Go:   // 无：用配置结构体参数
来源：http://oa.hahajie.cn

Ruby: f(a: 1, b: 2)
来源：http://fw.521024.cn

C#:   f(a: 1, b: 2)
来源：http://kx.bjjhwx.cn

[C05] 返回多个值
来源：http://xa.shxzukj.cn

Py:   return a, b
来源：http://ax.huanxung.cn

PHP:  return [$a, $b];
来源：http://fz.nicolike.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://cb.szxytkj.cn

TS:   return { a, b };
来源：http://iu.gzmigu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dr.muxihuayi.cn

Go:   return a, b
来源：http://kn.colortex.cn

Ruby: return a, b
来源：http://vj.nicolike.cn

C#:   return (a, b);              // ValueTuple
来源：http://pc.shtwfgs.cn

[C06] 匿名函数 / lambda
来源：http://ly.huixiangedu.cn

Py:   square = lambda x: x * x
来源：http://hs.szxytkj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ui.asd995.cn

JS:   const square = x => x * x;
来源：http://mf.asd995.cn

TS:   const square = (x: number): number => x * x;
来源：http://np.huanxung.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gj.shxzskj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qt.huanxung.cn

Ruby: square = ->(x) { x * x }
来源：http://lm.bjjhwx.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dv.huixiangedu.cn

[C07] 把函数作为参数传入
来源：http://mm.wgjwhj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ol.yuntaijiaju.cn

PHP:  array_map("strtoupper", $arr);
来源：http://mf.yuntaijiaju.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://au.asd995.cn

TS:   arr.map(String)
来源：http://ok.shxzukj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ky.muxihuayi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ab.wgjwhj.cn

Ruby: arr.map(&:upcase)
来源：http://pm.panjiajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qb.huixinmuqiang.cn

[C08] 闭包
来源：http://dh.huanxung.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wa.yuexingan06.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://it.lnxyls.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tb.bookmarksfly.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rr.huixinmuqiang.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ju.shxzskj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ks.jianghongdianzi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mv.521024.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://au.bookmarksfly.cn

[C09] 递归
来源：http://fa.gzmigu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xn.hahajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://oi.haigaiapp.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yh.hahajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zx.521024.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rx.gzmigu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fh.huanxung.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zz.jianghongdianzi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lk.huixiangedu.cn

[C10] 变量作用域
来源：http://jl.panjiajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yg.chemitech.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ny.muxihuayi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tb.huanxung.cn

TS:   同 JS
来源：http://ed.huixiangedu.cn

Java: 方法内为块级作用域
来源：http://ew.nszjky.cn

Go:   花括号块级作用域
来源：http://vc.hahajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ey.shxzskj.cn

C#:   块级作用域
来源：http://uw.szsharing.cn

[C11] 模块导入与导出
来源：http://mw.huanxung.cn

Py:   from module import func
来源：http://rn.jianghongdianzi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bm.wgjwhj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jv.muxihuayi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yk.9csxet.cn

Java: import java.util.List;
来源：http://fp.bjjhwx.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ur.9csxet.cn

Ruby: require "json"; require_relative "./util"
来源：http://ne.gzmigu.cn

C#:   using System.Text;
来源：http://ud.gzmigu.cn

[C12] 立即执行函数 IIFE
来源：http://os.newstarts.cn

Py:   (lambda: print("run"))()
来源：http://xp.jctech888.com.cn

PHP:  (function () { echo "run"; })();
来源：http://xc.gzmigu.cn

JS:   (() => { console.log("run"); })();
来源：http://il.nszjky.cn

TS:   (() => { console.log("run"); })();
来源：http://tv.nicolike.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ne.huixinmuqiang.cn

Go:   func() { fmt.Println("run") }()
来源：http://vv.asd995.cn

Ruby: -> { puts "run" }.call
来源：http://zx.nicolike.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jh.asd995.cn

[C13] 类型声明 / 类型注解
来源：http://ti.hnjuh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://za.shxzskj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cm.colortex.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://at.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ob.shtwfgs.cn


<!-- 参考信息 -->