代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ar.bookmarksfly.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://dl.asd995.cn

[A24] 去除首尾空白
来源：http://xk.huixinmuqiang.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zg.asd995.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hw.wgjwhj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hb.hahajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://li.szxytkj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qs.yuntaijiaju.cn

Go:   strings.TrimSpace(s)
来源：http://lz.huixiangedu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ou.shxzukj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fi.haigaiapp.cn

[A25] 字符串比较
来源：http://ow.szxytkj.cn

Py:   s1 == s2; s1 != s2
来源：http://my.shxzskj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ox.huanxung.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tz.shtwfgs.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gy.colortex.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://re.colortex.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dy.haigaiapp.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://lw.yuexingan06.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mv.szsharing.cn

[A26] 类型转换总览
来源：http://wg.521024.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yk.yuntaijiaju.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://du.hnjuh.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fi.jctech888.com.cn

TS:   Number() String() Boolean() x as number
来源：http://dg.shxzskj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zm.newstarts.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://az.hnjuh.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://op.yuexingan06.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hj.hnjuh.cn

================================================================================
来源：http://zd.bjjhwx.cn

B. 流程控制
来源：http://xf.muxihuayi.cn

================================================================================
来源：http://iq.haigaiapp.cn

[B01] 条件判断 if / else
来源：http://pl.521024.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dd.shxzukj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yp.jianghongdianzi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ur.bjjhwx.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://by.lnxyls.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ym.szxytkj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mb.hnjuh.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wp.muxihuayi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lx.asd995.cn

[B02] 多分支 else if / elif
来源：http://uu.szsharing.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bp.gzmigu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jz.huixinmuqiang.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://du.521024.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xf.bookmarksfly.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://em.gzmigu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bn.wgjwhj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yk.nszjky.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gh.521024.cn

[B03] switch / match / case
来源：http://cz.nszjky.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jt.chemitech.net.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sc.hahajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://os.hahajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mn.yuntaijiaju.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jh.colortex.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yd.yuntaijiaju.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qa.colortex.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sz.9csxet.cn

[B04] for 计数循环
来源：http://qn.shxzskj.cn

Py:   for i in range(10): print(i)
来源：http://fe.jctech888.com.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mc.nszjky.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lk.szxytkj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xh.haigaiapp.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ky.jianghongdianzi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wa.nicolike.cn

Ruby: 10.times { |i| puts i }
来源：http://ik.newstarts.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fq.shxzukj.cn

[B05] 遍历数组 / 列表
来源：http://ja.haigaiapp.cn

Py:   for item in arr: print(item)
来源：http://qa.hnjuh.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cx.521024.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hn.hahajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rz.yuexingan06.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xu.nicolike.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cn.lnxyls.cn

Ruby: arr.each { |item| puts item }
来源：http://wc.colortex.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bd.9csxet.cn

[B06] 遍历字典 / 对象
来源：http://ji.haigaiapp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tw.yuntaijiaju.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://br.nszjky.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oi.chemitech.net.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://do.asd995.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://be.lnxyls.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tf.asd995.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sb.bookmarksfly.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://df.newstarts.cn

[B07] while 循环
来源：http://mi.yuntaijiaju.cn

Py:   while i < 10: i += 1
来源：http://lr.colortex.cn

PHP:  while ($i < 10) { $i++; }
来源：http://dw.huixiangedu.cn

JS:   while (i < 10) { i++; }
来源：http://xg.huixinmuqiang.cn

TS:   while (i < 10) { i++; }
来源：http://ib.shxzukj.cn

Java: while (i < 10) { i++; }
来源：http://xd.hahajie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hf.wgjwhj.cn

Ruby: while i < 10; i += 1; end
来源：http://zv.nicolike.cn

C#:   while (i < 10) { i++; }
来源：http://yu.haigaiapp.cn

[B08] do-while（至少执行一次）
来源：http://ou.nszjky.cn

Py:   # 无 do-while：用 while True + break
来源：http://hu.hnjuh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ax.bookmarksfly.cn

JS:   do { i++; } while (i < 10);
来源：http://kf.colortex.cn

TS:   do { i++; } while (i < 10);
来源：http://dg.asd995.cn

Java: do { i++; } while (i < 10);
来源：http://hh.hnjuh.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://cm.muxihuayi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ji.jctech888.com.cn

C#:   do { i++; } while (i < 10);
来源：http://py.bookmarksfly.cn

[B09] break 与 continue
来源：http://gk.gzmigu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dz.gzmigu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ig.bjjhwx.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ud.jianghongdianzi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dx.newstarts.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ed.gzmigu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tb.shxzukj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rm.shxzukj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oa.bookmarksfly.cn

[B10] 遍历同时拿索引
来源：http://az.shxzukj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dd.shxzukj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://iz.chemitech.net.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sr.hnjuh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wq.hnjuh.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uc.chemitech.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fx.gzmigu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gb.521024.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ys.shtwfgs.cn

[B11] 生成数字序列 / 区间
来源：http://mv.jianghongdianzi.cn

Py:   list(range(0, 10, 2))
来源：http://hr.chemitech.net.cn

PHP:  range(0, 10, 2);
来源：http://cv.shxzskj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fe.chemitech.net.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jf.haigaiapp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qk.jianghongdianzi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://my.bookmarksfly.cn

Ruby: (0...10).step(2).to_a
来源：http://zf.shxzskj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yn.bjjhwx.cn

[B12] 跳出多层循环
来源：http://vf.colortex.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://gv.jctech888.com.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://cb.panjiajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rg.muxihuayi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ls.lnxyls.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mr.9csxet.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ez.gzmigu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wc.jctech888.com.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://oz.nszjky.cn

[B13] 判断是否为数字
来源：http://bh.hahajie.cn

Py:   isinstance(x, (int, float))
来源：http://kx.nszjky.cn

PHP:  is_numeric($x)
来源：http://nd.shxzskj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://io.muxihuayi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gg.panjiajie.cn

Java: x instanceof Number
来源：http://wm.asd995.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ty.wgjwhj.cn

Ruby: x.is_a?(Numeric)
来源：http://rk.shtwfgs.cn

C#:   x is int or double or decimal
来源：http://aa.wgjwhj.cn

[B14] 判断值是否在集合内
来源：http://kh.nicolike.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ku.shxzukj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ol.yuexingan06.cn

JS:   [1, 2, 3].includes(x)
来源：http://ah.haigaiapp.cn

TS:   [1, 2, 3].includes(x)
来源：http://yr.huixinmuqiang.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://wg.bjjhwx.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fq.9csxet.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ml.yuntaijiaju.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://om.shxzskj.cn

[B15] 布尔运算与取反
来源：http://ek.nicolike.cn

Py:   a and b or not c
来源：http://fo.szsharing.cn

PHP:  $a && $b || !$c
来源：http://rg.lnxyls.cn

JS:   a && b || !c
来源：http://ob.wgjwhj.cn

TS:   a && b || !c
来源：http://zl.muxihuayi.cn

Java: a && b || !c
来源：http://me.yuntaijiaju.cn

Go:   a && b || !c
来源：http://bi.asd995.cn

Ruby: a && b || !c
来源：http://ot.wgjwhj.cn

C#:   a && b || !c
来源：http://mw.chemitech.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://sf.9csxet.cn

Py:   if not data: return
来源：http://jx.asd995.cn

PHP:  if (!$data) { return; }
来源：http://rc.szsharing.cn

JS:   if (!data) return;
来源：http://to.shxzskj.cn

TS:   if (!data) return;
来源：http://hy.szxytkj.cn

Java: if (data == null) return;
来源：http://sb.wgjwhj.cn

Go:   if data == nil { return }
来源：http://sd.9csxet.cn

Ruby: return if data.nil?
来源：http://en.colortex.cn

C#:   if (data == null) return;
来源：http://ji.szsharing.cn

================================================================================
来源：http://pv.jctech888.com.cn

C. 函数与作用域
来源：http://ts.wgjwhj.cn

================================================================================
来源：http://ta.wgjwhj.cn

[C01] 定义函数
来源：http://rl.chemitech.net.cn

Py:   def add(a, b): return a + b
来源：http://jm.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ar.hnjuh.cn

JS:   function add(a, b) { return a + b; }
来源：http://vl.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jj.asd995.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mk.bookmarksfly.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rk.muxihuayi.cn

Ruby: def add(a, b); a + b; end
来源：http://nq.yuexingan06.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rp.nicolike.cn

[C02] 默认参数
来源：http://su.muxihuayi.cn

Py:   def greet(name="World"): return name
来源：http://hr.9csxet.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hh.nszjky.cn

JS:   function greet(name = "World") { return name; }
来源：http://ik.szsharing.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fs.huixiangedu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://mn.szxytkj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qz.szxytkj.cn

Ruby: def greet(name = "World") = name
来源：http://ho.gzmigu.cn

C#:   string Greet(string name = "World") => name;
来源：http://ge.nicolike.cn

[C03] 可变参数
来源：http://au.muxihuayi.cn

Py:   def total(*args): return sum(args)
来源：http://ht.szsharing.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://oz.szxytkj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mg.bookmarksfly.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cg.asd995.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://by.wgjwhj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vj.muxihuayi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ep.szsharing.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ml.newstarts.cn

[C04] 命名参数 / 关键字参数
来源：http://cl.haigaiapp.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kr.yuntaijiaju.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tx.shxzskj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wm.yuntaijiaju.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qj.nicolike.cn

Java: // 无：用 Builder 模式或 record
来源：http://wg.lnxyls.cn

Go:   // 无：用配置结构体参数
来源：http://sb.wgjwhj.cn

Ruby: f(a: 1, b: 2)
来源：http://eh.newstarts.cn

C#:   f(a: 1, b: 2)
来源：http://ks.szxytkj.cn

[C05] 返回多个值
来源：http://zp.9csxet.cn

Py:   return a, b
来源：http://nj.haigaiapp.cn

PHP:  return [$a, $b];
来源：http://nx.nicolike.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://de.wgjwhj.cn

TS:   return { a, b };
来源：http://nh.gzmigu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jc.wgjwhj.cn

Go:   return a, b
来源：http://jh.wgjwhj.cn

Ruby: return a, b
来源：http://fq.bjjhwx.cn

C#:   return (a, b);              // ValueTuple
来源：http://oe.9csxet.cn

[C06] 匿名函数 / lambda
来源：http://ab.asd995.cn

Py:   square = lambda x: x * x
来源：http://pg.chemitech.net.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wa.szxytkj.cn

JS:   const square = x => x * x;
来源：http://zd.haigaiapp.cn

TS:   const square = (x: number): number => x * x;
来源：http://fx.wgjwhj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hj.shxzukj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fu.huanxung.cn

Ruby: square = ->(x) { x * x }
来源：http://bd.wgjwhj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://kt.panjiajie.cn

[C07] 把函数作为参数传入
来源：http://tj.hahajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bz.huixiangedu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://no.asd995.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gp.huanxung.cn

TS:   arr.map(String)
来源：http://wn.huanxung.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cg.nicolike.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dl.asd995.cn

Ruby: arr.map(&:upcase)
来源：http://mc.muxihuayi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://yo.chemitech.net.cn

[C08] 闭包
来源：http://wq.lnxyls.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kc.panjiajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ms.jianghongdianzi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jk.bookmarksfly.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ub.szsharing.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lf.muxihuayi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gf.hnjuh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://oj.jctech888.com.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yr.shtwfgs.cn

[C09] 递归
来源：http://tk.yuntaijiaju.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kj.panjiajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wa.nicolike.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xn.asd995.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wt.huixinmuqiang.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zn.yuntaijiaju.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://md.lnxyls.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ho.asd995.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zd.panjiajie.cn

[C10] 变量作用域
来源：http://sd.asd995.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kh.panjiajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pq.asd995.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ge.bjjhwx.cn

TS:   同 JS
来源：http://kf.huanxung.cn

Java: 方法内为块级作用域
来源：http://gn.wgjwhj.cn

Go:   花括号块级作用域
来源：http://uw.yuntaijiaju.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lr.bookmarksfly.cn

C#:   块级作用域
来源：http://ch.hahajie.cn

[C11] 模块导入与导出
来源：http://xt.hahajie.cn

Py:   from module import func
来源：http://tg.huixiangedu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hv.shxzukj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jx.asd995.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bn.shtwfgs.cn

Java: import java.util.List;
来源：http://jr.jianghongdianzi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://eg.wgjwhj.cn

Ruby: require "json"; require_relative "./util"
来源：http://vk.521024.cn

C#:   using System.Text;
来源：http://kt.asd995.cn

[C12] 立即执行函数 IIFE
来源：http://qy.huixinmuqiang.cn

Py:   (lambda: print("run"))()
来源：http://zz.shxzskj.cn

PHP:  (function () { echo "run"; })();
来源：http://wr.haigaiapp.cn

JS:   (() => { console.log("run"); })();
来源：http://xu.yuntaijiaju.cn

TS:   (() => { console.log("run"); })();
来源：http://nh.chemitech.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xh.shxzskj.cn

Go:   func() { fmt.Println("run") }()
来源：http://zd.shxzskj.cn

Ruby: -> { puts "run" }.call
来源：http://lp.huixiangedu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zl.shxzskj.cn

[C13] 类型声明 / 类型注解
来源：http://tw.chemitech.net.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ab.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yi.panjiajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ef.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ik.haigaiapp.cn

Java: int add(int a, int b) { return a + b; }
来源：http://kd.muxihuayi.cn

Go:   func add(a, b int) int
来源：http://xb.jianghongdianzi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yb.szsharing.cn

C#:   int Add(int a, int b) => a + b;
来源：http://le.hnjuh.cn

[C14] 泛型函数
来源：http://ay.gzmigu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bo.szxytkj.cn

PHP:  // 无泛型
来源：http://pq.jctech888.com.cn

JS:   // 无泛型
来源：http://fr.haigaiapp.cn


<!-- 参考信息 -->