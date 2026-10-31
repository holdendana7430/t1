代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xm.hahajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://na.newstarts.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vw.szsharing.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sj.asd995.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gv.huixinmuqiang.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://yj.haigaiapp.cn

[A24] 去除首尾空白
来源：http://xg.yuexingan06.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://kg.chemitech.net.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gy.shtwfgs.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ob.521024.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kn.jctech888.com.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ww.nicolike.cn

Go:   strings.TrimSpace(s)
来源：http://lt.521024.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xa.yuexingan06.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://oi.szsharing.cn

[A25] 字符串比较
来源：http://ca.huixinmuqiang.cn

Py:   s1 == s2; s1 != s2
来源：http://cx.bjjhwx.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://aq.yuntaijiaju.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zp.shxzukj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ik.panjiajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jd.521024.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hf.szsharing.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://bf.huixinmuqiang.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vl.muxihuayi.cn

[A26] 类型转换总览
来源：http://tk.shtwfgs.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fm.yuexingan06.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vu.yuntaijiaju.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gu.nicolike.cn

TS:   Number() String() Boolean() x as number
来源：http://bx.shxzukj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ec.haigaiapp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gv.haigaiapp.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vp.huanxung.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fz.shtwfgs.cn

================================================================================
来源：http://vx.wgjwhj.cn

B. 流程控制
来源：http://ir.hahajie.cn

================================================================================
来源：http://cx.yuntaijiaju.cn

[B01] 条件判断 if / else
来源：http://de.nszjky.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://fk.gzmigu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rb.hahajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sd.hahajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dj.hahajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ha.huanxung.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://if.wgjwhj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yi.jianghongdianzi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hq.wgjwhj.cn

[B02] 多分支 else if / elif
来源：http://bc.wgjwhj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sn.hahajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ze.nszjky.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gt.huixiangedu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zf.hnjuh.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vq.yuntaijiaju.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://se.9csxet.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lu.nicolike.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dh.jianghongdianzi.cn

[B03] switch / match / case
来源：http://pu.lnxyls.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pn.colortex.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gg.shxzskj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kw.hnjuh.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tb.bjjhwx.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bw.hahajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rq.szxytkj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fr.nszjky.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://el.shxzukj.cn

[B04] for 计数循环
来源：http://su.asd995.cn

Py:   for i in range(10): print(i)
来源：http://zz.huixinmuqiang.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ba.nicolike.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vp.hahajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yd.bookmarksfly.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ue.chemitech.net.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ay.huixiangedu.cn

Ruby: 10.times { |i| puts i }
来源：http://jk.jianghongdianzi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mh.jctech888.com.cn

[B05] 遍历数组 / 列表
来源：http://vx.wgjwhj.cn

Py:   for item in arr: print(item)
来源：http://in.haigaiapp.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nd.wgjwhj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://rl.9csxet.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ju.haigaiapp.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://mb.nicolike.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kw.szsharing.cn

Ruby: arr.each { |item| puts item }
来源：http://ix.gzmigu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ep.colortex.cn

[B06] 遍历字典 / 对象
来源：http://ir.hnjuh.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mv.yuntaijiaju.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fk.hnjuh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ar.haigaiapp.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://na.panjiajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://op.shxzukj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dm.gzmigu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mo.wgjwhj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://er.yuexingan06.cn

[B07] while 循环
来源：http://gj.huixiangedu.cn

Py:   while i < 10: i += 1
来源：http://uf.bjjhwx.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wo.huixinmuqiang.cn

JS:   while (i < 10) { i++; }
来源：http://dr.shtwfgs.cn

TS:   while (i < 10) { i++; }
来源：http://db.jctech888.com.cn

Java: while (i < 10) { i++; }
来源：http://ao.newstarts.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gw.bjjhwx.cn

Ruby: while i < 10; i += 1; end
来源：http://ct.yuexingan06.cn

C#:   while (i < 10) { i++; }
来源：http://cy.huixinmuqiang.cn

[B08] do-while（至少执行一次）
来源：http://ll.hnjuh.cn

Py:   # 无 do-while：用 while True + break
来源：http://er.shxzskj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://in.lnxyls.cn

JS:   do { i++; } while (i < 10);
来源：http://jt.haigaiapp.cn

TS:   do { i++; } while (i < 10);
来源：http://lk.muxihuayi.cn

Java: do { i++; } while (i < 10);
来源：http://ka.yuexingan06.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sm.nszjky.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fp.panjiajie.cn

C#:   do { i++; } while (i < 10);
来源：http://qt.hahajie.cn

[B09] break 与 continue
来源：http://nx.yuntaijiaju.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kz.nicolike.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qo.asd995.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gs.chemitech.net.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zz.jianghongdianzi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rv.hnjuh.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xw.yuntaijiaju.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ls.jianghongdianzi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oy.9csxet.cn

[B10] 遍历同时拿索引
来源：http://ru.bjjhwx.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yt.yuntaijiaju.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://un.huixiangedu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zq.hahajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nc.panjiajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sn.jianghongdianzi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ac.szxytkj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pb.haigaiapp.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kn.shtwfgs.cn

[B11] 生成数字序列 / 区间
来源：http://wb.gzmigu.cn

Py:   list(range(0, 10, 2))
来源：http://se.hahajie.cn

PHP:  range(0, 10, 2);
来源：http://nn.nicolike.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wz.shtwfgs.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://va.shtwfgs.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kt.huixiangedu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mb.yuntaijiaju.cn

Ruby: (0...10).step(2).to_a
来源：http://ew.chemitech.net.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hg.yuntaijiaju.cn

[B12] 跳出多层循环
来源：http://mv.haigaiapp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://cf.wgjwhj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://yq.asd995.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hb.chemitech.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zx.haigaiapp.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xk.yuexingan06.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ok.huixinmuqiang.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://my.shxzskj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ji.nicolike.cn

[B13] 判断是否为数字
来源：http://fm.huanxung.cn

Py:   isinstance(x, (int, float))
来源：http://bl.shtwfgs.cn

PHP:  is_numeric($x)
来源：http://cv.colortex.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://la.lnxyls.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yy.shxzukj.cn

Java: x instanceof Number
来源：http://fx.hnjuh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wb.szsharing.cn

Ruby: x.is_a?(Numeric)
来源：http://mt.9csxet.cn

C#:   x is int or double or decimal
来源：http://vh.521024.cn

[B14] 判断值是否在集合内
来源：http://zp.chemitech.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yj.jctech888.com.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dk.shxzskj.cn

JS:   [1, 2, 3].includes(x)
来源：http://xw.bjjhwx.cn

TS:   [1, 2, 3].includes(x)
来源：http://ix.9csxet.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rv.szxytkj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://eq.newstarts.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fg.jianghongdianzi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mb.gzmigu.cn

[B15] 布尔运算与取反
来源：http://sh.szsharing.cn

Py:   a and b or not c
来源：http://gx.yuexingan06.cn

PHP:  $a && $b || !$c
来源：http://lk.hnjuh.cn

JS:   a && b || !c
来源：http://zf.lnxyls.cn

TS:   a && b || !c
来源：http://yj.huixinmuqiang.cn

Java: a && b || !c
来源：http://ul.haigaiapp.cn

Go:   a && b || !c
来源：http://aa.nszjky.cn

Ruby: a && b || !c
来源：http://rb.shxzukj.cn

C#:   a && b || !c
来源：http://xe.bjjhwx.cn

[B16] 卫语句：不满足条件提前返回
来源：http://yz.nicolike.cn

Py:   if not data: return
来源：http://pc.jianghongdianzi.cn

PHP:  if (!$data) { return; }
来源：http://dp.newstarts.cn

JS:   if (!data) return;
来源：http://qq.szxytkj.cn

TS:   if (!data) return;
来源：http://po.lnxyls.cn

Java: if (data == null) return;
来源：http://iw.jctech888.com.cn

Go:   if data == nil { return }
来源：http://do.huanxung.cn

Ruby: return if data.nil?
来源：http://sw.yuntaijiaju.cn

C#:   if (data == null) return;
来源：http://gi.muxihuayi.cn

================================================================================
来源：http://to.gzmigu.cn

C. 函数与作用域
来源：http://jc.jianghongdianzi.cn

================================================================================
来源：http://fp.yuexingan06.cn

[C01] 定义函数
来源：http://ya.huixinmuqiang.cn

Py:   def add(a, b): return a + b
来源：http://pb.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ue.colortex.cn

JS:   function add(a, b) { return a + b; }
来源：http://pv.yuexingan06.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hi.521024.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://jo.bookmarksfly.cn

Go:   func add(a, b int) int { return a + b }
来源：http://fk.nicolike.cn

Ruby: def add(a, b); a + b; end
来源：http://gr.panjiajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qn.521024.cn

[C02] 默认参数
来源：http://ce.huanxung.cn

Py:   def greet(name="World"): return name
来源：http://sy.shtwfgs.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yx.jctech888.com.cn

JS:   function greet(name = "World") { return name; }
来源：http://eh.shxzukj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://he.haigaiapp.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ff.hnjuh.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xx.lnxyls.cn

Ruby: def greet(name = "World") = name
来源：http://ad.nicolike.cn

C#:   string Greet(string name = "World") => name;
来源：http://uy.shxzskj.cn

[C03] 可变参数
来源：http://nw.hnjuh.cn

Py:   def total(*args): return sum(args)
来源：http://rk.asd995.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://da.hnjuh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ln.9csxet.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://aj.jctech888.com.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vo.wgjwhj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://on.gzmigu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vm.panjiajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ch.asd995.cn

[C04] 命名参数 / 关键字参数
来源：http://vj.9csxet.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yp.szxytkj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gp.shtwfgs.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rf.jianghongdianzi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jj.colortex.cn

Java: // 无：用 Builder 模式或 record
来源：http://jp.shxzskj.cn

Go:   // 无：用配置结构体参数
来源：http://ts.huanxung.cn

Ruby: f(a: 1, b: 2)
来源：http://qs.colortex.cn

C#:   f(a: 1, b: 2)
来源：http://ku.szxytkj.cn

[C05] 返回多个值
来源：http://vl.9csxet.cn

Py:   return a, b
来源：http://to.szxytkj.cn

PHP:  return [$a, $b];
来源：http://eg.yuexingan06.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ip.shxzskj.cn

TS:   return { a, b };
来源：http://tv.huixiangedu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bi.asd995.cn

Go:   return a, b
来源：http://lu.huixinmuqiang.cn

Ruby: return a, b
来源：http://tc.shxzukj.cn

C#:   return (a, b);              // ValueTuple
来源：http://hn.shxzukj.cn

[C06] 匿名函数 / lambda
来源：http://hb.haigaiapp.cn

Py:   square = lambda x: x * x
来源：http://fd.hahajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://gw.9csxet.cn

JS:   const square = x => x * x;
来源：http://xt.9csxet.cn

TS:   const square = (x: number): number => x * x;
来源：http://ec.lnxyls.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mx.lnxyls.cn

Go:   sq := func(x int) int { return x * x }
来源：http://nd.huixiangedu.cn

Ruby: square = ->(x) { x * x }
来源：http://kk.huixiangedu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hb.huixiangedu.cn

[C07] 把函数作为参数传入
来源：http://cj.jianghongdianzi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ac.shxzskj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://nk.colortex.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://su.jianghongdianzi.cn

TS:   arr.map(String)
来源：http://wh.szxytkj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kv.huixinmuqiang.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://du.chemitech.net.cn

Ruby: arr.map(&:upcase)
来源：http://cr.521024.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://op.huixiangedu.cn

[C08] 闭包
来源：http://sv.hahajie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yc.panjiajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ju.colortex.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sm.huixiangedu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ly.nszjky.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ss.521024.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vq.bookmarksfly.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yv.yuexingan06.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kx.szsharing.cn

[C09] 递归
来源：http://dv.bjjhwx.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bw.gzmigu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mh.nszjky.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vh.yuexingan06.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hl.haigaiapp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://du.wgjwhj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xl.szsharing.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vh.lnxyls.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://al.wgjwhj.cn

[C10] 变量作用域
来源：http://wh.asd995.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tb.huanxung.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rs.szsharing.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://co.nicolike.cn

TS:   同 JS
来源：http://ls.asd995.cn

Java: 方法内为块级作用域
来源：http://zv.jianghongdianzi.cn

Go:   花括号块级作用域
来源：http://jo.jctech888.com.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wx.szxytkj.cn

C#:   块级作用域
来源：http://hs.szxytkj.cn

[C11] 模块导入与导出
来源：http://or.shtwfgs.cn

Py:   from module import func
来源：http://ui.hahajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://dx.bjjhwx.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ie.huixinmuqiang.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yz.9csxet.cn

Java: import java.util.List;
来源：http://vp.gzmigu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zl.gzmigu.cn

Ruby: require "json"; require_relative "./util"
来源：http://qg.chemitech.net.cn

C#:   using System.Text;
来源：http://ov.panjiajie.cn

[C12] 立即执行函数 IIFE
来源：http://ds.nicolike.cn

Py:   (lambda: print("run"))()
来源：http://mb.jctech888.com.cn

PHP:  (function () { echo "run"; })();
来源：http://gt.huixinmuqiang.cn

JS:   (() => { console.log("run"); })();
来源：http://tn.bjjhwx.cn

TS:   (() => { console.log("run"); })();
来源：http://nx.bookmarksfly.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bt.szxytkj.cn

Go:   func() { fmt.Println("run") }()
来源：http://cy.shxzskj.cn

Ruby: -> { puts "run" }.call
来源：http://ez.hnjuh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qx.szxytkj.cn

[C13] 类型声明 / 类型注解
来源：http://ya.wgjwhj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jz.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mr.huixiangedu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jc.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jo.9csxet.cn

Java: int add(int a, int b) { return a + b; }
来源：http://un.bjjhwx.cn

Go:   func add(a, b int) int
来源：http://ns.haigaiapp.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gq.newstarts.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gd.chemitech.net.cn


<!-- 参考信息 -->