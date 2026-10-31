代发 wailian999

C#:   s.Length
来源：http://qw.asd995.cn

[A23] 大小写转换
来源：http://ac.bookmarksfly.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://xb.chemitech.net.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yp.nicolike.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://we.shxzukj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qh.521024.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ib.jianghongdianzi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kt.colortex.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gj.huanxung.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://yp.wgjwhj.cn

[A24] 去除首尾空白
来源：http://uj.9csxet.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://di.wgjwhj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://av.panjiajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zq.newstarts.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xs.asd995.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ic.huanxung.cn

Go:   strings.TrimSpace(s)
来源：http://iw.szsharing.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tz.newstarts.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qb.hahajie.cn

[A25] 字符串比较
来源：http://nd.lnxyls.cn

Py:   s1 == s2; s1 != s2
来源：http://wr.wgjwhj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://uo.huanxung.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wy.shxzskj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hu.bjjhwx.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xf.panjiajie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bh.yuntaijiaju.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://bk.jianghongdianzi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zi.bjjhwx.cn

[A26] 类型转换总览
来源：http://gv.nszjky.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xh.shtwfgs.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sd.muxihuayi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://br.shxzskj.cn

TS:   Number() String() Boolean() x as number
来源：http://dd.shtwfgs.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pa.szxytkj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://uj.shxzukj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vr.huixiangedu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hh.haigaiapp.cn

================================================================================
来源：http://nn.newstarts.cn

B. 流程控制
来源：http://ma.nszjky.cn

================================================================================
来源：http://hi.huanxung.cn

[B01] 条件判断 if / else
来源：http://xn.szxytkj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://sd.521024.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ae.szsharing.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ne.huixiangedu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://aa.panjiajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://me.szsharing.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ue.jctech888.com.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ky.nicolike.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dh.jianghongdianzi.cn

[B02] 多分支 else if / elif
来源：http://mn.hnjuh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zf.gzmigu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lm.nszjky.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://az.shtwfgs.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ew.yuexingan06.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ri.szsharing.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://as.newstarts.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://oe.lnxyls.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ve.yuntaijiaju.cn

[B03] switch / match / case
来源：http://ab.colortex.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lr.szxytkj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://of.huixiangedu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sx.huanxung.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sa.szxytkj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ps.colortex.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uv.muxihuayi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ld.asd995.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://az.szsharing.cn

[B04] for 计数循环
来源：http://yy.9csxet.cn

Py:   for i in range(10): print(i)
来源：http://dr.szxytkj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mp.yuntaijiaju.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://we.huixinmuqiang.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pi.lnxyls.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uq.yuexingan06.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ln.bookmarksfly.cn

Ruby: 10.times { |i| puts i }
来源：http://yo.hahajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tr.521024.cn

[B05] 遍历数组 / 列表
来源：http://uh.nicolike.cn

Py:   for item in arr: print(item)
来源：http://et.bookmarksfly.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xo.yuexingan06.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://st.haigaiapp.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://cu.nicolike.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://db.yuexingan06.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://oj.shtwfgs.cn

Ruby: arr.each { |item| puts item }
来源：http://us.huixinmuqiang.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://va.521024.cn

[B06] 遍历字典 / 对象
来源：http://ku.yuexingan06.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ry.yuexingan06.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wr.bookmarksfly.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xy.huanxung.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gi.yuntaijiaju.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xg.bjjhwx.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vn.hahajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fa.huanxung.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hl.jianghongdianzi.cn

[B07] while 循环
来源：http://ws.huanxung.cn

Py:   while i < 10: i += 1
来源：http://ca.9csxet.cn

PHP:  while ($i < 10) { $i++; }
来源：http://pj.colortex.cn

JS:   while (i < 10) { i++; }
来源：http://tt.yuntaijiaju.cn

TS:   while (i < 10) { i++; }
来源：http://gc.wgjwhj.cn

Java: while (i < 10) { i++; }
来源：http://hx.hnjuh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ps.bookmarksfly.cn

Ruby: while i < 10; i += 1; end
来源：http://vs.jianghongdianzi.cn

C#:   while (i < 10) { i++; }
来源：http://ym.wgjwhj.cn

[B08] do-while（至少执行一次）
来源：http://hv.newstarts.cn

Py:   # 无 do-while：用 while True + break
来源：http://md.shtwfgs.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vp.yuntaijiaju.cn

JS:   do { i++; } while (i < 10);
来源：http://ir.nicolike.cn

TS:   do { i++; } while (i < 10);
来源：http://fa.gzmigu.cn

Java: do { i++; } while (i < 10);
来源：http://cb.yuntaijiaju.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://qr.huanxung.cn

Ruby: begin; i += 1; end while i < 10
来源：http://uw.hahajie.cn

C#:   do { i++; } while (i < 10);
来源：http://zc.wgjwhj.cn

[B09] break 与 continue
来源：http://ud.yuntaijiaju.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ph.521024.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jh.panjiajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qc.szsharing.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kx.shxzukj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ys.muxihuayi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://li.shxzskj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ov.huanxung.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xx.hahajie.cn

[B10] 遍历同时拿索引
来源：http://yg.muxihuayi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jp.nszjky.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cf.szxytkj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ks.muxihuayi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://oc.lnxyls.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hh.yuexingan06.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dq.jianghongdianzi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sz.shxzskj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bn.huixiangedu.cn

[B11] 生成数字序列 / 区间
来源：http://ox.nicolike.cn

Py:   list(range(0, 10, 2))
来源：http://it.haigaiapp.cn

PHP:  range(0, 10, 2);
来源：http://mv.jctech888.com.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rh.wgjwhj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ho.nicolike.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://br.nicolike.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rf.bjjhwx.cn

Ruby: (0...10).step(2).to_a
来源：http://av.521024.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://js.huixinmuqiang.cn

[B12] 跳出多层循环
来源：http://vc.shtwfgs.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://gi.hnjuh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://lk.huanxung.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://eo.newstarts.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://at.shxzskj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://up.chemitech.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://om.hahajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wc.shtwfgs.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://oh.shxzskj.cn

[B13] 判断是否为数字
来源：http://kk.jianghongdianzi.cn

Py:   isinstance(x, (int, float))
来源：http://aj.hnjuh.cn

PHP:  is_numeric($x)
来源：http://nk.panjiajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ov.chemitech.net.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cb.jctech888.com.cn

Java: x instanceof Number
来源：http://qw.nicolike.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wz.yuntaijiaju.cn

Ruby: x.is_a?(Numeric)
来源：http://nc.jctech888.com.cn

C#:   x is int or double or decimal
来源：http://pk.shxzukj.cn

[B14] 判断值是否在集合内
来源：http://qn.muxihuayi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zs.jctech888.com.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fx.szxytkj.cn

JS:   [1, 2, 3].includes(x)
来源：http://al.newstarts.cn

TS:   [1, 2, 3].includes(x)
来源：http://jj.shxzukj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://wp.wgjwhj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yk.jctech888.com.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mf.haigaiapp.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mc.bjjhwx.cn

[B15] 布尔运算与取反
来源：http://hz.wgjwhj.cn

Py:   a and b or not c
来源：http://gv.haigaiapp.cn

PHP:  $a && $b || !$c
来源：http://mo.newstarts.cn

JS:   a && b || !c
来源：http://tu.asd995.cn

TS:   a && b || !c
来源：http://fu.nszjky.cn

Java: a && b || !c
来源：http://sd.hahajie.cn

Go:   a && b || !c
来源：http://cn.huanxung.cn

Ruby: a && b || !c
来源：http://yr.szxytkj.cn

C#:   a && b || !c
来源：http://vk.jianghongdianzi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jc.521024.cn

Py:   if not data: return
来源：http://zk.nicolike.cn

PHP:  if (!$data) { return; }
来源：http://gr.gzmigu.cn

JS:   if (!data) return;
来源：http://wv.shxzskj.cn

TS:   if (!data) return;
来源：http://nj.haigaiapp.cn

Java: if (data == null) return;
来源：http://fh.lnxyls.cn

Go:   if data == nil { return }
来源：http://be.shtwfgs.cn

Ruby: return if data.nil?
来源：http://gg.shxzukj.cn

C#:   if (data == null) return;
来源：http://fv.521024.cn

================================================================================
来源：http://ll.jianghongdianzi.cn

C. 函数与作用域
来源：http://ue.nszjky.cn

================================================================================
来源：http://nb.shxzukj.cn

[C01] 定义函数
来源：http://fs.chemitech.net.cn

Py:   def add(a, b): return a + b
来源：http://ra.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pm.bjjhwx.cn

JS:   function add(a, b) { return a + b; }
来源：http://wp.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xp.hahajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xx.bjjhwx.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rz.panjiajie.cn

Ruby: def add(a, b); a + b; end
来源：http://fp.asd995.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qi.shtwfgs.cn

[C02] 默认参数
来源：http://iy.nicolike.cn

Py:   def greet(name="World"): return name
来源：http://vw.nicolike.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qz.wgjwhj.cn

JS:   function greet(name = "World") { return name; }
来源：http://qp.gzmigu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://un.nszjky.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vp.huixiangedu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://op.hahajie.cn

Ruby: def greet(name = "World") = name
来源：http://bt.gzmigu.cn

C#:   string Greet(string name = "World") => name;
来源：http://ac.haigaiapp.cn

[C03] 可变参数
来源：http://vc.yuntaijiaju.cn

Py:   def total(*args): return sum(args)
来源：http://mo.shxzukj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tt.huixiangedu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nh.wgjwhj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ks.wgjwhj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fj.lnxyls.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qf.hahajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wi.chemitech.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xi.yuexingan06.cn

[C04] 命名参数 / 关键字参数
来源：http://qp.hahajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lv.szsharing.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://eu.haigaiapp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ug.jctech888.com.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ld.shxzskj.cn

Java: // 无：用 Builder 模式或 record
来源：http://an.nicolike.cn

Go:   // 无：用配置结构体参数
来源：http://af.hahajie.cn

Ruby: f(a: 1, b: 2)
来源：http://et.muxihuayi.cn

C#:   f(a: 1, b: 2)
来源：http://mv.nicolike.cn

[C05] 返回多个值
来源：http://pa.shxzukj.cn

Py:   return a, b
来源：http://gh.asd995.cn

PHP:  return [$a, $b];
来源：http://ab.lnxyls.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://cx.haigaiapp.cn

TS:   return { a, b };
来源：http://rb.nszjky.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hh.shxzskj.cn

Go:   return a, b
来源：http://zc.hnjuh.cn

Ruby: return a, b
来源：http://kp.hahajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://cw.shxzskj.cn

[C06] 匿名函数 / lambda
来源：http://zf.hahajie.cn

Py:   square = lambda x: x * x
来源：http://nu.huixiangedu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xj.gzmigu.cn

JS:   const square = x => x * x;
来源：http://jp.huixiangedu.cn

TS:   const square = (x: number): number => x * x;
来源：http://dy.shtwfgs.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xc.asd995.cn

Go:   sq := func(x int) int { return x * x }
来源：http://nt.asd995.cn

Ruby: square = ->(x) { x * x }
来源：http://cc.newstarts.cn

C#:   Func<int, int> square = x => x * x;
来源：http://um.wgjwhj.cn

[C07] 把函数作为参数传入
来源：http://wr.muxihuayi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rp.shtwfgs.cn

PHP:  array_map("strtoupper", $arr);
来源：http://sb.colortex.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://oa.wgjwhj.cn

TS:   arr.map(String)
来源：http://xs.nicolike.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rb.bookmarksfly.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wn.huixiangedu.cn

Ruby: arr.map(&:upcase)
来源：http://tn.chemitech.net.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://kq.szxytkj.cn

[C08] 闭包
来源：http://dd.shxzukj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rj.panjiajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ri.huixiangedu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ff.bookmarksfly.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cz.muxihuayi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cj.huanxung.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://we.haigaiapp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mk.521024.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://es.521024.cn

[C09] 递归
来源：http://wd.huanxung.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rc.jctech888.com.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ta.hnjuh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ae.huanxung.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ix.lnxyls.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://of.hahajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mk.yuntaijiaju.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kp.muxihuayi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mk.nszjky.cn

[C10] 变量作用域
来源：http://wo.lnxyls.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ok.newstarts.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cd.shxzukj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://af.nszjky.cn

TS:   同 JS
来源：http://os.lnxyls.cn

Java: 方法内为块级作用域
来源：http://jt.hahajie.cn

Go:   花括号块级作用域
来源：http://nf.huixiangedu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yr.newstarts.cn

C#:   块级作用域
来源：http://vj.asd995.cn

[C11] 模块导入与导出
来源：http://vy.szsharing.cn

Py:   from module import func
来源：http://xo.haigaiapp.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ql.nszjky.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rw.yuexingan06.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yv.521024.cn

Java: import java.util.List;
来源：http://fe.shxzukj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cy.gzmigu.cn

Ruby: require "json"; require_relative "./util"
来源：http://os.huixiangedu.cn

C#:   using System.Text;
来源：http://ov.huixinmuqiang.cn

[C12] 立即执行函数 IIFE
来源：http://xs.shtwfgs.cn

Py:   (lambda: print("run"))()
来源：http://fr.huanxung.cn

PHP:  (function () { echo "run"; })();
来源：http://am.gzmigu.cn

JS:   (() => { console.log("run"); })();
来源：http://sr.hahajie.cn

TS:   (() => { console.log("run"); })();
来源：http://cw.yuexingan06.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://oh.nicolike.cn

Go:   func() { fmt.Println("run") }()
来源：http://ua.shxzukj.cn

Ruby: -> { puts "run" }.call
来源：http://ei.lnxyls.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://lq.szxytkj.cn

[C13] 类型声明 / 类型注解
来源：http://vw.jctech888.com.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://my.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://po.shxzskj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ul.yuexingan06.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wr.jianghongdianzi.cn


<!-- 参考信息 -->