代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lo.nicolike.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zr.huanxung.cn

[A24] 去除首尾空白
来源：http://lj.gzmigu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fi.asd995.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ij.521024.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://as.asd995.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sv.asd995.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zj.521024.cn

Go:   strings.TrimSpace(s)
来源：http://qm.shtwfgs.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://av.nicolike.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wp.jianghongdianzi.cn

[A25] 字符串比较
来源：http://ck.yuexingan06.cn

Py:   s1 == s2; s1 != s2
来源：http://es.nszjky.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://uz.haigaiapp.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jk.chemitech.net.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ry.jianghongdianzi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://la.nicolike.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://md.asd995.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ia.newstarts.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qp.nszjky.cn

[A26] 类型转换总览
来源：http://zu.haigaiapp.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hr.lnxyls.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fb.bjjhwx.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rk.hnjuh.cn

TS:   Number() String() Boolean() x as number
来源：http://vf.shtwfgs.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gl.gzmigu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://co.nszjky.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ue.szxytkj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cp.bookmarksfly.cn

================================================================================
来源：http://om.hnjuh.cn

B. 流程控制
来源：http://tz.huanxung.cn

================================================================================
来源：http://js.huixinmuqiang.cn

[B01] 条件判断 if / else
来源：http://ur.wgjwhj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://eu.nicolike.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tp.hahajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ie.chemitech.net.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dd.shxzskj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://pl.nszjky.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ka.jianghongdianzi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ou.nicolike.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tx.nicolike.cn

[B02] 多分支 else if / elif
来源：http://tj.bjjhwx.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bb.hahajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yl.haigaiapp.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wu.9csxet.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://to.bookmarksfly.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aj.yuexingan06.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qg.hnjuh.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wx.szxytkj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ys.lnxyls.cn

[B03] switch / match / case
来源：http://rj.panjiajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://on.bookmarksfly.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sh.shtwfgs.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ux.hnjuh.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sk.szxytkj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://by.huixinmuqiang.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gq.wgjwhj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://oi.haigaiapp.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yp.521024.cn

[B04] for 计数循环
来源：http://bx.shxzukj.cn

Py:   for i in range(10): print(i)
来源：http://na.hahajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qz.bjjhwx.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zh.bookmarksfly.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cm.asd995.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hn.521024.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ox.szsharing.cn

Ruby: 10.times { |i| puts i }
来源：http://pz.chemitech.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vu.panjiajie.cn

[B05] 遍历数组 / 列表
来源：http://af.nicolike.cn

Py:   for item in arr: print(item)
来源：http://wz.shxzskj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://re.haigaiapp.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://kb.yuntaijiaju.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qv.gzmigu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ae.hahajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ox.colortex.cn

Ruby: arr.each { |item| puts item }
来源：http://fe.521024.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lj.colortex.cn

[B06] 遍历字典 / 对象
来源：http://fq.nicolike.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://nb.jctech888.com.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uq.nicolike.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jj.szsharing.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cp.nszjky.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fn.jctech888.com.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rp.hahajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ix.bjjhwx.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xh.shxzukj.cn

[B07] while 循环
来源：http://vy.muxihuayi.cn

Py:   while i < 10: i += 1
来源：http://th.newstarts.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qf.hnjuh.cn

JS:   while (i < 10) { i++; }
来源：http://tw.shtwfgs.cn

TS:   while (i < 10) { i++; }
来源：http://xb.shtwfgs.cn

Java: while (i < 10) { i++; }
来源：http://sg.gzmigu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bg.wgjwhj.cn

Ruby: while i < 10; i += 1; end
来源：http://dr.bjjhwx.cn

C#:   while (i < 10) { i++; }
来源：http://ah.nszjky.cn

[B08] do-while（至少执行一次）
来源：http://wh.yuexingan06.cn

Py:   # 无 do-while：用 while True + break
来源：http://uh.bjjhwx.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://po.yuntaijiaju.cn

JS:   do { i++; } while (i < 10);
来源：http://tv.jianghongdianzi.cn

TS:   do { i++; } while (i < 10);
来源：http://lh.shxzukj.cn

Java: do { i++; } while (i < 10);
来源：http://qg.hahajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://so.yuexingan06.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wl.huixinmuqiang.cn

C#:   do { i++; } while (i < 10);
来源：http://nf.chemitech.net.cn

[B09] break 与 continue
来源：http://md.szsharing.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dy.haigaiapp.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vy.huanxung.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://me.521024.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cd.colortex.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ry.nicolike.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wc.nicolike.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mv.lnxyls.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rp.shxzskj.cn

[B10] 遍历同时拿索引
来源：http://ab.bookmarksfly.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ax.bookmarksfly.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jx.521024.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://be.szsharing.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jm.huixinmuqiang.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qc.chemitech.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wr.gzmigu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xu.shxzskj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ts.lnxyls.cn

[B11] 生成数字序列 / 区间
来源：http://om.hahajie.cn

Py:   list(range(0, 10, 2))
来源：http://vl.jctech888.com.cn

PHP:  range(0, 10, 2);
来源：http://ok.szxytkj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ec.wgjwhj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wm.newstarts.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xl.nszjky.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wk.wgjwhj.cn

Ruby: (0...10).step(2).to_a
来源：http://my.nszjky.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ps.lnxyls.cn

[B12] 跳出多层循环
来源：http://qf.szsharing.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://qn.colortex.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ar.yuntaijiaju.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cj.szxytkj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ej.huixiangedu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gv.szsharing.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pe.jianghongdianzi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xc.panjiajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://oe.shxzukj.cn

[B13] 判断是否为数字
来源：http://wh.521024.cn

Py:   isinstance(x, (int, float))
来源：http://ms.bjjhwx.cn

PHP:  is_numeric($x)
来源：http://dd.jctech888.com.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pt.shtwfgs.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fm.chemitech.net.cn

Java: x instanceof Number
来源：http://jl.huanxung.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ok.gzmigu.cn

Ruby: x.is_a?(Numeric)
来源：http://aa.huixinmuqiang.cn

C#:   x is int or double or decimal
来源：http://du.gzmigu.cn

[B14] 判断值是否在集合内
来源：http://tp.gzmigu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gp.colortex.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://du.muxihuayi.cn

JS:   [1, 2, 3].includes(x)
来源：http://rg.521024.cn

TS:   [1, 2, 3].includes(x)
来源：http://tt.panjiajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qr.lnxyls.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pq.521024.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ay.huixiangedu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://iy.yuntaijiaju.cn

[B15] 布尔运算与取反
来源：http://oo.panjiajie.cn

Py:   a and b or not c
来源：http://jt.shxzskj.cn

PHP:  $a && $b || !$c
来源：http://rb.huixiangedu.cn

JS:   a && b || !c
来源：http://sd.hnjuh.cn

TS:   a && b || !c
来源：http://vg.9csxet.cn

Java: a && b || !c
来源：http://kn.9csxet.cn

Go:   a && b || !c
来源：http://aq.521024.cn

Ruby: a && b || !c
来源：http://iq.yuntaijiaju.cn

C#:   a && b || !c
来源：http://pq.haigaiapp.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xd.wgjwhj.cn

Py:   if not data: return
来源：http://le.bjjhwx.cn

PHP:  if (!$data) { return; }
来源：http://sr.panjiajie.cn

JS:   if (!data) return;
来源：http://ql.asd995.cn

TS:   if (!data) return;
来源：http://hh.panjiajie.cn

Java: if (data == null) return;
来源：http://ay.9csxet.cn

Go:   if data == nil { return }
来源：http://hb.huixiangedu.cn

Ruby: return if data.nil?
来源：http://uz.szxytkj.cn

C#:   if (data == null) return;
来源：http://il.haigaiapp.cn

================================================================================
来源：http://lo.huixiangedu.cn

C. 函数与作用域
来源：http://wf.huanxung.cn

================================================================================
来源：http://qg.shxzukj.cn

[C01] 定义函数
来源：http://yt.jianghongdianzi.cn

Py:   def add(a, b): return a + b
来源：http://fy.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sz.bjjhwx.cn

JS:   function add(a, b) { return a + b; }
来源：http://lr.yuexingan06.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kp.nicolike.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://za.huixiangedu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://lq.szxytkj.cn

Ruby: def add(a, b); a + b; end
来源：http://bm.muxihuayi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://we.panjiajie.cn

[C02] 默认参数
来源：http://ft.wgjwhj.cn

Py:   def greet(name="World"): return name
来源：http://eu.huixinmuqiang.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lc.nicolike.cn

JS:   function greet(name = "World") { return name; }
来源：http://qu.huanxung.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://mu.yuntaijiaju.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://if.szsharing.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ig.muxihuayi.cn

Ruby: def greet(name = "World") = name
来源：http://so.jianghongdianzi.cn

C#:   string Greet(string name = "World") => name;
来源：http://ys.jianghongdianzi.cn

[C03] 可变参数
来源：http://zg.jctech888.com.cn

Py:   def total(*args): return sum(args)
来源：http://ks.haigaiapp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hq.shxzskj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ft.521024.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bn.colortex.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pm.lnxyls.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zl.hnjuh.cn

Ruby: def total(*nums); nums.sum; end
来源：http://aq.szsharing.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zw.bookmarksfly.cn

[C04] 命名参数 / 关键字参数
来源：http://rh.lnxyls.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://el.panjiajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dp.nszjky.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rd.bookmarksfly.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uz.yuexingan06.cn

Java: // 无：用 Builder 模式或 record
来源：http://zu.huixinmuqiang.cn

Go:   // 无：用配置结构体参数
来源：http://cc.szsharing.cn

Ruby: f(a: 1, b: 2)
来源：http://ki.lnxyls.cn

C#:   f(a: 1, b: 2)
来源：http://px.panjiajie.cn

[C05] 返回多个值
来源：http://ru.nicolike.cn

Py:   return a, b
来源：http://sy.hnjuh.cn

PHP:  return [$a, $b];
来源：http://uv.muxihuayi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://gg.lnxyls.cn

TS:   return { a, b };
来源：http://cj.yuexingan06.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xu.yuntaijiaju.cn

Go:   return a, b
来源：http://po.huixinmuqiang.cn

Ruby: return a, b
来源：http://cs.521024.cn

C#:   return (a, b);              // ValueTuple
来源：http://mp.shxzukj.cn

[C06] 匿名函数 / lambda
来源：http://jz.nszjky.cn

Py:   square = lambda x: x * x
来源：http://hj.huanxung.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pd.hnjuh.cn

JS:   const square = x => x * x;
来源：http://ea.yuexingan06.cn

TS:   const square = (x: number): number => x * x;
来源：http://iu.wgjwhj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gz.haigaiapp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://mm.jianghongdianzi.cn

Ruby: square = ->(x) { x * x }
来源：http://pm.szsharing.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ck.chemitech.net.cn

[C07] 把函数作为参数传入
来源：http://bs.lnxyls.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cx.newstarts.cn

PHP:  array_map("strtoupper", $arr);
来源：http://pk.bjjhwx.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://on.gzmigu.cn

TS:   arr.map(String)
来源：http://cw.nszjky.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sj.chemitech.net.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ap.huixiangedu.cn

Ruby: arr.map(&:upcase)
来源：http://on.jctech888.com.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fs.szsharing.cn

[C08] 闭包
来源：http://ij.panjiajie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pa.bjjhwx.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wf.szsharing.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dg.huixinmuqiang.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qk.chemitech.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wt.lnxyls.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://th.521024.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ts.lnxyls.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lr.lnxyls.cn

[C09] 递归
来源：http://gb.nszjky.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rj.jctech888.com.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jw.nicolike.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xc.hnjuh.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://is.yuexingan06.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wr.9csxet.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dh.hahajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://je.haigaiapp.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fm.newstarts.cn

[C10] 变量作用域
来源：http://xe.asd995.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xk.lnxyls.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://io.bookmarksfly.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ub.shxzukj.cn

TS:   同 JS
来源：http://zu.nszjky.cn

Java: 方法内为块级作用域
来源：http://cu.jctech888.com.cn

Go:   花括号块级作用域
来源：http://tj.chemitech.net.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rh.asd995.cn

C#:   块级作用域
来源：http://dg.jctech888.com.cn

[C11] 模块导入与导出
来源：http://wi.yuexingan06.cn

Py:   from module import func
来源：http://rq.bookmarksfly.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qg.shxzskj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ae.szsharing.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rj.yuexingan06.cn

Java: import java.util.List;
来源：http://fd.haigaiapp.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pp.muxihuayi.cn

Ruby: require "json"; require_relative "./util"
来源：http://vv.asd995.cn

C#:   using System.Text;
来源：http://ac.yuexingan06.cn

[C12] 立即执行函数 IIFE
来源：http://ik.yuexingan06.cn

Py:   (lambda: print("run"))()
来源：http://ia.shxzukj.cn

PHP:  (function () { echo "run"; })();
来源：http://df.panjiajie.cn

JS:   (() => { console.log("run"); })();
来源：http://yp.jianghongdianzi.cn

TS:   (() => { console.log("run"); })();
来源：http://gm.9csxet.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://aj.jctech888.com.cn

Go:   func() { fmt.Println("run") }()
来源：http://dg.hahajie.cn

Ruby: -> { puts "run" }.call
来源：http://eq.hnjuh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ow.muxihuayi.cn

[C13] 类型声明 / 类型注解
来源：http://vi.shtwfgs.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dg.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ee.huixinmuqiang.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qz.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rn.shxzukj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cp.huixiangedu.cn

Go:   func add(a, b int) int
来源：http://zj.haigaiapp.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ga.jctech888.com.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fz.shxzskj.cn

[C14] 泛型函数
来源：http://uh.nicolike.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ee.jianghongdianzi.cn

PHP:  // 无泛型
来源：http://ua.newstarts.cn

JS:   // 无泛型
来源：http://jh.huanxung.cn


<!-- 参考信息 -->