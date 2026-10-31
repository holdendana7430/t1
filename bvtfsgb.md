代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://oi.bjjhwx.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tr.yuntaijiaju.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jq.nszjky.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ok.hnjuh.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dz.jianghongdianzi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://tr.521024.cn

[A24] 去除首尾空白
来源：http://ml.jctech888.com.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ma.jctech888.com.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rj.bjjhwx.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://py.huanxung.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ho.huixinmuqiang.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://aa.jianghongdianzi.cn

Go:   strings.TrimSpace(s)
来源：http://hc.panjiajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jl.jctech888.com.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://aw.jctech888.com.cn

[A25] 字符串比较
来源：http://dh.shxzukj.cn

Py:   s1 == s2; s1 != s2
来源：http://te.jctech888.com.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fh.huixinmuqiang.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jr.huanxung.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qv.yuexingan06.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tu.yuexingan06.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dc.haigaiapp.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ke.huixinmuqiang.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xp.gzmigu.cn

[A26] 类型转换总览
来源：http://vd.jctech888.com.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ze.9csxet.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pt.muxihuayi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bb.yuntaijiaju.cn

TS:   Number() String() Boolean() x as number
来源：http://es.haigaiapp.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://js.nicolike.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mi.nszjky.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ee.huanxung.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://iz.shxzskj.cn

================================================================================
来源：http://gh.hahajie.cn

B. 流程控制
来源：http://hs.shxzskj.cn

================================================================================
来源：http://fc.jctech888.com.cn

[B01] 条件判断 if / else
来源：http://nr.huixinmuqiang.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://nu.chemitech.net.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kp.wgjwhj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dx.lnxyls.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xu.shtwfgs.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://dm.hnjuh.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vx.asd995.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://eb.shxzskj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mi.szsharing.cn

[B02] 多分支 else if / elif
来源：http://qb.szsharing.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ti.9csxet.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xh.muxihuayi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lv.chemitech.net.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ic.huanxung.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bf.asd995.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://li.gzmigu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ni.jianghongdianzi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lw.shxzskj.cn

[B03] switch / match / case
来源：http://gd.bjjhwx.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qi.szsharing.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ml.521024.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hc.huixiangedu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fu.yuntaijiaju.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tg.nszjky.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fz.shxzskj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lg.jctech888.com.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pc.asd995.cn

[B04] for 计数循环
来源：http://bb.hahajie.cn

Py:   for i in range(10): print(i)
来源：http://kc.hnjuh.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zs.yuntaijiaju.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rg.colortex.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bj.haigaiapp.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vo.lnxyls.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://en.hahajie.cn

Ruby: 10.times { |i| puts i }
来源：http://cn.newstarts.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lw.newstarts.cn

[B05] 遍历数组 / 列表
来源：http://gi.521024.cn

Py:   for item in arr: print(item)
来源：http://nn.lnxyls.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bj.hnjuh.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://nb.bjjhwx.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://pt.jctech888.com.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://mt.huixiangedu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gf.hnjuh.cn

Ruby: arr.each { |item| puts item }
来源：http://pc.huixiangedu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ou.wgjwhj.cn

[B06] 遍历字典 / 对象
来源：http://ya.9csxet.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zy.nszjky.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hi.jctech888.com.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jv.szsharing.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vb.bjjhwx.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mu.nszjky.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ec.bjjhwx.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://db.hnjuh.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sx.521024.cn

[B07] while 循环
来源：http://oj.panjiajie.cn

Py:   while i < 10: i += 1
来源：http://cr.jctech888.com.cn

PHP:  while ($i < 10) { $i++; }
来源：http://nn.gzmigu.cn

JS:   while (i < 10) { i++; }
来源：http://jj.muxihuayi.cn

TS:   while (i < 10) { i++; }
来源：http://qv.jianghongdianzi.cn

Java: while (i < 10) { i++; }
来源：http://mw.bookmarksfly.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tb.jianghongdianzi.cn

Ruby: while i < 10; i += 1; end
来源：http://fl.huixiangedu.cn

C#:   while (i < 10) { i++; }
来源：http://ju.lnxyls.cn

[B08] do-while（至少执行一次）
来源：http://mo.hahajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://ds.jctech888.com.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://in.chemitech.net.cn

JS:   do { i++; } while (i < 10);
来源：http://yz.521024.cn

TS:   do { i++; } while (i < 10);
来源：http://pu.shxzukj.cn

Java: do { i++; } while (i < 10);
来源：http://ie.wgjwhj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://iy.jianghongdianzi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ai.huixinmuqiang.cn

C#:   do { i++; } while (i < 10);
来源：http://gc.bjjhwx.cn

[B09] break 与 continue
来源：http://rm.gzmigu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rg.shxzukj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mm.newstarts.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ht.yuexingan06.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aa.bjjhwx.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xy.nicolike.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hs.chemitech.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fv.hahajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uh.jianghongdianzi.cn

[B10] 遍历同时拿索引
来源：http://lq.chemitech.net.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bo.chemitech.net.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ex.wgjwhj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cx.huixinmuqiang.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lj.huixinmuqiang.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://df.newstarts.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kx.huixinmuqiang.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ey.nszjky.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yx.shxzskj.cn

[B11] 生成数字序列 / 区间
来源：http://ri.muxihuayi.cn

Py:   list(range(0, 10, 2))
来源：http://mn.521024.cn

PHP:  range(0, 10, 2);
来源：http://kw.shxzukj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rx.gzmigu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://le.newstarts.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wn.panjiajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sr.huixinmuqiang.cn

Ruby: (0...10).step(2).to_a
来源：http://th.jianghongdianzi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qu.bjjhwx.cn

[B12] 跳出多层循环
来源：http://ib.9csxet.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://to.panjiajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ae.gzmigu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ow.bjjhwx.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://un.panjiajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bw.muxihuayi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uu.bjjhwx.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sq.jctech888.com.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ep.wgjwhj.cn

[B13] 判断是否为数字
来源：http://vx.shxzskj.cn

Py:   isinstance(x, (int, float))
来源：http://qp.asd995.cn

PHP:  is_numeric($x)
来源：http://yq.newstarts.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://te.wgjwhj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ji.yuexingan06.cn

Java: x instanceof Number
来源：http://fs.jctech888.com.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jh.huixiangedu.cn

Ruby: x.is_a?(Numeric)
来源：http://ei.newstarts.cn

C#:   x is int or double or decimal
来源：http://qr.huixinmuqiang.cn

[B14] 判断值是否在集合内
来源：http://sg.wgjwhj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ry.bookmarksfly.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ku.shxzskj.cn

JS:   [1, 2, 3].includes(x)
来源：http://ah.shxzskj.cn

TS:   [1, 2, 3].includes(x)
来源：http://vf.521024.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://tf.jianghongdianzi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pp.nicolike.cn

Ruby: [1, 2, 3].include?(x)
来源：http://yq.gzmigu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mo.colortex.cn

[B15] 布尔运算与取反
来源：http://rz.haigaiapp.cn

Py:   a and b or not c
来源：http://op.szxytkj.cn

PHP:  $a && $b || !$c
来源：http://jp.szsharing.cn

JS:   a && b || !c
来源：http://ws.jianghongdianzi.cn

TS:   a && b || !c
来源：http://kd.huixiangedu.cn

Java: a && b || !c
来源：http://vh.jctech888.com.cn

Go:   a && b || !c
来源：http://ea.muxihuayi.cn

Ruby: a && b || !c
来源：http://fo.jctech888.com.cn

C#:   a && b || !c
来源：http://tl.colortex.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lx.haigaiapp.cn

Py:   if not data: return
来源：http://wx.yuexingan06.cn

PHP:  if (!$data) { return; }
来源：http://tp.9csxet.cn

JS:   if (!data) return;
来源：http://os.bjjhwx.cn

TS:   if (!data) return;
来源：http://aj.shxzskj.cn

Java: if (data == null) return;
来源：http://cf.haigaiapp.cn

Go:   if data == nil { return }
来源：http://kf.chemitech.net.cn

Ruby: return if data.nil?
来源：http://fa.szsharing.cn

C#:   if (data == null) return;
来源：http://ja.shxzskj.cn

================================================================================
来源：http://br.jianghongdianzi.cn

C. 函数与作用域
来源：http://vc.bjjhwx.cn

================================================================================
来源：http://rh.yuexingan06.cn

[C01] 定义函数
来源：http://cr.bookmarksfly.cn

Py:   def add(a, b): return a + b
来源：http://md.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fq.haigaiapp.cn

JS:   function add(a, b) { return a + b; }
来源：http://xd.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rd.hnjuh.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wh.jianghongdianzi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mj.hnjuh.cn

Ruby: def add(a, b); a + b; end
来源：http://tl.newstarts.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hw.panjiajie.cn

[C02] 默认参数
来源：http://to.huixiangedu.cn

Py:   def greet(name="World"): return name
来源：http://sj.yuexingan06.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xv.szsharing.cn

JS:   function greet(name = "World") { return name; }
来源：http://gc.shxzskj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://sd.nicolike.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://un.huixiangedu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wn.asd995.cn

Ruby: def greet(name = "World") = name
来源：http://zg.gzmigu.cn

C#:   string Greet(string name = "World") => name;
来源：http://ne.9csxet.cn

[C03] 可变参数
来源：http://qt.huanxung.cn

Py:   def total(*args): return sum(args)
来源：http://uv.haigaiapp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lw.muxihuayi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cq.hahajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://td.yuexingan06.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gr.lnxyls.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ve.9csxet.cn

Ruby: def total(*nums); nums.sum; end
来源：http://px.gzmigu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qm.muxihuayi.cn

[C04] 命名参数 / 关键字参数
来源：http://ji.muxihuayi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jp.shxzskj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kl.hnjuh.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://af.jctech888.com.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://js.panjiajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://od.chemitech.net.cn

Go:   // 无：用配置结构体参数
来源：http://fo.hahajie.cn

Ruby: f(a: 1, b: 2)
来源：http://wt.521024.cn

C#:   f(a: 1, b: 2)
来源：http://ad.chemitech.net.cn

[C05] 返回多个值
来源：http://fk.panjiajie.cn

Py:   return a, b
来源：http://jr.gzmigu.cn

PHP:  return [$a, $b];
来源：http://jb.haigaiapp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ti.9csxet.cn

TS:   return { a, b };
来源：http://rm.9csxet.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jo.lnxyls.cn

Go:   return a, b
来源：http://rk.muxihuayi.cn

Ruby: return a, b
来源：http://xt.wgjwhj.cn

C#:   return (a, b);              // ValueTuple
来源：http://lb.hnjuh.cn

[C06] 匿名函数 / lambda
来源：http://vv.nszjky.cn

Py:   square = lambda x: x * x
来源：http://mq.gzmigu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ef.521024.cn

JS:   const square = x => x * x;
来源：http://od.lnxyls.cn

TS:   const square = (x: number): number => x * x;
来源：http://qm.newstarts.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vj.yuntaijiaju.cn

Go:   sq := func(x int) int { return x * x }
来源：http://vu.haigaiapp.cn

Ruby: square = ->(x) { x * x }
来源：http://be.newstarts.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dw.asd995.cn

[C07] 把函数作为参数传入
来源：http://yo.nicolike.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dz.9csxet.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ib.9csxet.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pa.9csxet.cn

TS:   arr.map(String)
来源：http://if.asd995.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nd.bookmarksfly.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jp.asd995.cn

Ruby: arr.map(&:upcase)
来源：http://iz.shtwfgs.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ih.huixinmuqiang.cn

[C08] 闭包
来源：http://it.521024.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ph.muxihuayi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ox.hnjuh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xx.asd995.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nt.colortex.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://au.9csxet.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hk.jianghongdianzi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zy.huanxung.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pa.chemitech.net.cn

[C09] 递归
来源：http://bf.9csxet.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ga.muxihuayi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rk.wgjwhj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ul.colortex.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://az.huixinmuqiang.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rp.szsharing.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cs.nicolike.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hm.shxzskj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zc.521024.cn

[C10] 变量作用域
来源：http://eu.wgjwhj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rq.panjiajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ea.huanxung.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mx.shtwfgs.cn

TS:   同 JS
来源：http://lv.huixiangedu.cn

Java: 方法内为块级作用域
来源：http://uq.lnxyls.cn

Go:   花括号块级作用域
来源：http://rw.szsharing.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gb.chemitech.net.cn

C#:   块级作用域
来源：http://kg.gzmigu.cn

[C11] 模块导入与导出
来源：http://bj.asd995.cn

Py:   from module import func
来源：http://ll.hnjuh.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ek.muxihuayi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://sv.huanxung.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lu.panjiajie.cn

Java: import java.util.List;
来源：http://kg.9csxet.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gl.hnjuh.cn

Ruby: require "json"; require_relative "./util"
来源：http://rv.yuntaijiaju.cn

C#:   using System.Text;
来源：http://bq.shtwfgs.cn

[C12] 立即执行函数 IIFE
来源：http://vy.hahajie.cn

Py:   (lambda: print("run"))()
来源：http://lh.szsharing.cn

PHP:  (function () { echo "run"; })();
来源：http://hc.huixinmuqiang.cn

JS:   (() => { console.log("run"); })();
来源：http://jv.colortex.cn

TS:   (() => { console.log("run"); })();
来源：http://is.colortex.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wg.szxytkj.cn

Go:   func() { fmt.Println("run") }()
来源：http://db.521024.cn

Ruby: -> { puts "run" }.call
来源：http://fs.szxytkj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ar.bjjhwx.cn

[C13] 类型声明 / 类型注解
来源：http://cb.nicolike.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lv.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cw.panjiajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zs.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ap.shtwfgs.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mu.jianghongdianzi.cn

Go:   func add(a, b int) int
来源：http://nd.yuexingan06.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ma.panjiajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://dt.muxihuayi.cn


<!-- 参考信息 -->