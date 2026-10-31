代发 wailian999

C#:   s.Length
来源：http://rk.jctech888.com.cn

[A23] 大小写转换
来源：http://au.colortex.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://dz.521024.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vx.bjjhwx.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ue.chemitech.net.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bm.hnjuh.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pd.shxzukj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ch.lnxyls.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gs.nicolike.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qv.hahajie.cn

[A24] 去除首尾空白
来源：http://dp.bookmarksfly.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://om.huixiangedu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pr.muxihuayi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ke.szxytkj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rw.huixinmuqiang.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ii.nicolike.cn

Go:   strings.TrimSpace(s)
来源：http://fi.shxzukj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jl.jctech888.com.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mc.haigaiapp.cn

[A25] 字符串比较
来源：http://to.9csxet.cn

Py:   s1 == s2; s1 != s2
来源：http://gx.bjjhwx.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mw.yuntaijiaju.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gj.lnxyls.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://oa.521024.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ss.panjiajie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wf.colortex.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://bv.hnjuh.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ze.huixinmuqiang.cn

[A26] 类型转换总览
来源：http://mh.jctech888.com.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://se.panjiajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kt.szsharing.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gv.jctech888.com.cn

TS:   Number() String() Boolean() x as number
来源：http://vx.szsharing.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ho.szsharing.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ly.bookmarksfly.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.9csxet.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://md.newstarts.cn

================================================================================
来源：http://rl.huixiangedu.cn

B. 流程控制
来源：http://on.muxihuayi.cn

================================================================================
来源：http://xd.nicolike.cn

[B01] 条件判断 if / else
来源：http://iw.lnxyls.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dl.jctech888.com.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tv.huixinmuqiang.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://br.chemitech.net.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ij.wgjwhj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://lh.nicolike.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hb.521024.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xq.shtwfgs.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ma.chemitech.net.cn

[B02] 多分支 else if / elif
来源：http://oo.nszjky.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://na.szxytkj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jk.wgjwhj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yq.newstarts.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qc.bjjhwx.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kx.jianghongdianzi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://sx.colortex.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://od.colortex.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kn.bookmarksfly.cn

[B03] switch / match / case
来源：http://qv.wgjwhj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wm.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://to.shxzukj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zf.hahajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pz.muxihuayi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ag.nicolike.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kg.shxzukj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pu.lnxyls.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bn.chemitech.net.cn

[B04] for 计数循环
来源：http://uc.hnjuh.cn

Py:   for i in range(10): print(i)
来源：http://kq.bjjhwx.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mc.szsharing.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://us.colortex.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lt.jctech888.com.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://sa.newstarts.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xv.muxihuayi.cn

Ruby: 10.times { |i| puts i }
来源：http://wh.521024.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sg.szsharing.cn

[B05] 遍历数组 / 列表
来源：http://gr.shtwfgs.cn

Py:   for item in arr: print(item)
来源：http://lk.nicolike.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ep.yuexingan06.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://px.shxzskj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://jv.chemitech.net.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://bc.nicolike.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jl.521024.cn

Ruby: arr.each { |item| puts item }
来源：http://em.haigaiapp.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vz.asd995.cn

[B06] 遍历字典 / 对象
来源：http://yj.szxytkj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://dn.szsharing.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gg.asd995.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qs.lnxyls.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pd.huixiangedu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mw.chemitech.net.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zr.yuntaijiaju.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://td.wgjwhj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sx.huanxung.cn

[B07] while 循环
来源：http://qu.jianghongdianzi.cn

Py:   while i < 10: i += 1
来源：http://oe.asd995.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ac.shxzukj.cn

JS:   while (i < 10) { i++; }
来源：http://dn.szxytkj.cn

TS:   while (i < 10) { i++; }
来源：http://wg.newstarts.cn

Java: while (i < 10) { i++; }
来源：http://zi.lnxyls.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ub.9csxet.cn

Ruby: while i < 10; i += 1; end
来源：http://df.szsharing.cn

C#:   while (i < 10) { i++; }
来源：http://qi.nszjky.cn

[B08] do-while（至少执行一次）
来源：http://it.nszjky.cn

Py:   # 无 do-while：用 while True + break
来源：http://cj.gzmigu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://yo.yuntaijiaju.cn

JS:   do { i++; } while (i < 10);
来源：http://vn.panjiajie.cn

TS:   do { i++; } while (i < 10);
来源：http://fh.9csxet.cn

Java: do { i++; } while (i < 10);
来源：http://oi.haigaiapp.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xx.yuntaijiaju.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mz.lnxyls.cn

C#:   do { i++; } while (i < 10);
来源：http://qu.haigaiapp.cn

[B09] break 与 continue
来源：http://lc.szxytkj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://el.jianghongdianzi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vn.szsharing.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ls.jianghongdianzi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ja.yuexingan06.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wk.hnjuh.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xq.yuntaijiaju.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bz.hnjuh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gm.9csxet.cn

[B10] 遍历同时拿索引
来源：http://am.asd995.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bd.nszjky.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://aj.shxzukj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fk.jianghongdianzi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gn.hnjuh.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hk.nszjky.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zk.haigaiapp.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zf.9csxet.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://aa.panjiajie.cn

[B11] 生成数字序列 / 区间
来源：http://nw.huanxung.cn

Py:   list(range(0, 10, 2))
来源：http://jy.asd995.cn

PHP:  range(0, 10, 2);
来源：http://vt.jianghongdianzi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xf.huixinmuqiang.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qx.yuexingan06.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://km.asd995.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ls.shtwfgs.cn

Ruby: (0...10).step(2).to_a
来源：http://nc.lnxyls.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://en.9csxet.cn

[B12] 跳出多层循环
来源：http://vr.gzmigu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yz.yuntaijiaju.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ff.shxzukj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kl.gzmigu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cv.bookmarksfly.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bu.muxihuayi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://de.huixiangedu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vv.shtwfgs.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nn.haigaiapp.cn

[B13] 判断是否为数字
来源：http://ar.colortex.cn

Py:   isinstance(x, (int, float))
来源：http://th.newstarts.cn

PHP:  is_numeric($x)
来源：http://ko.yuntaijiaju.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fl.yuntaijiaju.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wq.huixinmuqiang.cn

Java: x instanceof Number
来源：http://lc.asd995.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ie.521024.cn

Ruby: x.is_a?(Numeric)
来源：http://xv.colortex.cn

C#:   x is int or double or decimal
来源：http://jc.colortex.cn

[B14] 判断值是否在集合内
来源：http://iu.shxzskj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nu.yuexingan06.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sb.jianghongdianzi.cn

JS:   [1, 2, 3].includes(x)
来源：http://oq.asd995.cn

TS:   [1, 2, 3].includes(x)
来源：http://as.bookmarksfly.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://oz.muxihuayi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kl.bookmarksfly.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ax.panjiajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mu.yuexingan06.cn

[B15] 布尔运算与取反
来源：http://os.panjiajie.cn

Py:   a and b or not c
来源：http://pb.wgjwhj.cn

PHP:  $a && $b || !$c
来源：http://xm.szxytkj.cn

JS:   a && b || !c
来源：http://sk.huixiangedu.cn

TS:   a && b || !c
来源：http://cp.hahajie.cn

Java: a && b || !c
来源：http://db.huanxung.cn

Go:   a && b || !c
来源：http://ru.yuntaijiaju.cn

Ruby: a && b || !c
来源：http://qv.szxytkj.cn

C#:   a && b || !c
来源：http://hp.521024.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ns.shxzukj.cn

Py:   if not data: return
来源：http://tp.szxytkj.cn

PHP:  if (!$data) { return; }
来源：http://vh.haigaiapp.cn

JS:   if (!data) return;
来源：http://hf.colortex.cn

TS:   if (!data) return;
来源：http://il.hahajie.cn

Java: if (data == null) return;
来源：http://gz.gzmigu.cn

Go:   if data == nil { return }
来源：http://sj.panjiajie.cn

Ruby: return if data.nil?
来源：http://db.9csxet.cn

C#:   if (data == null) return;
来源：http://ie.shxzukj.cn

================================================================================
来源：http://iu.jctech888.com.cn

C. 函数与作用域
来源：http://ms.yuexingan06.cn

================================================================================
来源：http://rc.szxytkj.cn

[C01] 定义函数
来源：http://hx.yuexingan06.cn

Py:   def add(a, b): return a + b
来源：http://lw.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wc.panjiajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://ul.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://om.panjiajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wq.shtwfgs.cn

Go:   func add(a, b int) int { return a + b }
来源：http://it.bookmarksfly.cn

Ruby: def add(a, b); a + b; end
来源：http://xx.panjiajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pz.haigaiapp.cn

[C02] 默认参数
来源：http://ax.jianghongdianzi.cn

Py:   def greet(name="World"): return name
来源：http://wa.jianghongdianzi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cl.szsharing.cn

JS:   function greet(name = "World") { return name; }
来源：http://ek.bjjhwx.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hi.jctech888.com.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ot.colortex.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ul.szxytkj.cn

Ruby: def greet(name = "World") = name
来源：http://ut.shxzukj.cn

C#:   string Greet(string name = "World") => name;
来源：http://rw.haigaiapp.cn

[C03] 可变参数
来源：http://av.huixinmuqiang.cn

Py:   def total(*args): return sum(args)
来源：http://hh.huanxung.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pu.nicolike.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hl.huixiangedu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://oo.huixiangedu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cc.gzmigu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zi.huixiangedu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fv.asd995.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fq.huixiangedu.cn

[C04] 命名参数 / 关键字参数
来源：http://eo.asd995.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://aa.bjjhwx.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wy.jctech888.com.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://eg.shxzskj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kn.asd995.cn

Java: // 无：用 Builder 模式或 record
来源：http://dd.huanxung.cn

Go:   // 无：用配置结构体参数
来源：http://xo.panjiajie.cn

Ruby: f(a: 1, b: 2)
来源：http://me.jctech888.com.cn

C#:   f(a: 1, b: 2)
来源：http://qc.jianghongdianzi.cn

[C05] 返回多个值
来源：http://un.lnxyls.cn

Py:   return a, b
来源：http://pk.szsharing.cn

PHP:  return [$a, $b];
来源：http://ro.newstarts.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://rx.hnjuh.cn

TS:   return { a, b };
来源：http://fl.gzmigu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://di.bookmarksfly.cn

Go:   return a, b
来源：http://uz.shxzukj.cn

Ruby: return a, b
来源：http://mc.bjjhwx.cn

C#:   return (a, b);              // ValueTuple
来源：http://xj.bjjhwx.cn

[C06] 匿名函数 / lambda
来源：http://zc.nszjky.cn

Py:   square = lambda x: x * x
来源：http://bq.wgjwhj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://gt.nszjky.cn

JS:   const square = x => x * x;
来源：http://de.gzmigu.cn

TS:   const square = (x: number): number => x * x;
来源：http://ya.haigaiapp.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://no.shxzskj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ok.521024.cn

Ruby: square = ->(x) { x * x }
来源：http://mq.haigaiapp.cn

C#:   Func<int, int> square = x => x * x;
来源：http://jc.haigaiapp.cn

[C07] 把函数作为参数传入
来源：http://fw.9csxet.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://no.colortex.cn

PHP:  array_map("strtoupper", $arr);
来源：http://sf.yuntaijiaju.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jy.bjjhwx.cn

TS:   arr.map(String)
来源：http://ei.9csxet.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://na.panjiajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://oq.jctech888.com.cn

Ruby: arr.map(&:upcase)
来源：http://qv.shtwfgs.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://zk.nszjky.cn

[C08] 闭包
来源：http://lc.chemitech.net.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://by.yuntaijiaju.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ft.huanxung.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yx.nicolike.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ix.yuexingan06.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mp.gzmigu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ec.szsharing.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ig.muxihuayi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qq.chemitech.net.cn

[C09] 递归
来源：http://py.hahajie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ze.9csxet.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bw.9csxet.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://st.wgjwhj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wu.shxzskj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ej.hahajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fn.jctech888.com.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pe.521024.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ga.bjjhwx.cn

[C10] 变量作用域
来源：http://xx.szsharing.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ag.shtwfgs.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zg.nicolike.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rf.wgjwhj.cn

TS:   同 JS
来源：http://si.panjiajie.cn

Java: 方法内为块级作用域
来源：http://lk.huixiangedu.cn

Go:   花括号块级作用域
来源：http://xh.jianghongdianzi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xr.haigaiapp.cn

C#:   块级作用域
来源：http://gp.szxytkj.cn

[C11] 模块导入与导出
来源：http://xu.shtwfgs.cn

Py:   from module import func
来源：http://hc.huixiangedu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xe.colortex.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gk.jianghongdianzi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dy.nszjky.cn

Java: import java.util.List;
来源：http://eg.chemitech.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vu.gzmigu.cn

Ruby: require "json"; require_relative "./util"
来源：http://db.szsharing.cn

C#:   using System.Text;
来源：http://ap.colortex.cn

[C12] 立即执行函数 IIFE
来源：http://aq.yuntaijiaju.cn

Py:   (lambda: print("run"))()
来源：http://mj.asd995.cn

PHP:  (function () { echo "run"; })();
来源：http://up.shtwfgs.cn

JS:   (() => { console.log("run"); })();
来源：http://bk.panjiajie.cn

TS:   (() => { console.log("run"); })();
来源：http://jw.haigaiapp.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pb.nszjky.cn

Go:   func() { fmt.Println("run") }()
来源：http://rn.haigaiapp.cn

Ruby: -> { puts "run" }.call
来源：http://bp.huixinmuqiang.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://oq.huanxung.cn

[C13] 类型声明 / 类型注解
来源：http://ig.huixiangedu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xh.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ur.newstarts.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xa.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ej.huixiangedu.cn


<!-- 参考信息 -->