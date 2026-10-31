代发 wailian999

TS:   s.length
来源：http://ke.gzmigu.cn

Java: s.length()
来源：http://zv.nszjky.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ok.szxytkj.cn

Ruby: s.length
来源：http://ng.jctech888.com.cn

C#:   s.Length
来源：http://mf.jctech888.com.cn

[A23] 大小写转换
来源：http://xb.huixiangedu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://pg.muxihuayi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mk.nicolike.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://se.bjjhwx.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tx.huixinmuqiang.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hj.shxzskj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cx.yuexingan06.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zk.bookmarksfly.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://vn.huanxung.cn

[A24] 去除首尾空白
来源：http://fd.gzmigu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pr.szxytkj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kd.yuexingan06.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qy.gzmigu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zz.yuexingan06.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wl.huanxung.cn

Go:   strings.TrimSpace(s)
来源：http://vu.bjjhwx.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gx.asd995.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ao.shxzukj.cn

[A25] 字符串比较
来源：http://to.wgjwhj.cn

Py:   s1 == s2; s1 != s2
来源：http://op.haigaiapp.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ms.shtwfgs.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lx.9csxet.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ne.nicolike.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://is.nszjky.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cv.szsharing.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://xz.nszjky.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jx.jianghongdianzi.cn

[A26] 类型转换总览
来源：http://ol.bjjhwx.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fl.shtwfgs.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vu.wgjwhj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wu.yuntaijiaju.cn

TS:   Number() String() Boolean() x as number
来源：http://oa.shxzukj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dk.muxihuayi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yn.szxytkj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://si.521024.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qo.bjjhwx.cn

================================================================================
来源：http://ra.asd995.cn

B. 流程控制
来源：http://uy.yuexingan06.cn

================================================================================
来源：http://sn.521024.cn

[B01] 条件判断 if / else
来源：http://fw.huixinmuqiang.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://iw.muxihuayi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://re.shxzskj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nh.nszjky.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hd.wgjwhj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://as.huixinmuqiang.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jj.shxzskj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ad.hnjuh.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ka.521024.cn

[B02] 多分支 else if / elif
来源：http://ua.jctech888.com.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wt.hahajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nm.szsharing.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wm.521024.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rk.huixinmuqiang.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pv.muxihuayi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zc.haigaiapp.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lz.haigaiapp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cu.lnxyls.cn

[B03] switch / match / case
来源：http://kz.bookmarksfly.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nl.newstarts.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nd.szxytkj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://de.colortex.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fw.huixiangedu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://iz.szxytkj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mi.nszjky.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hk.huixinmuqiang.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ae.hahajie.cn

[B04] for 计数循环
来源：http://gx.yuntaijiaju.cn

Py:   for i in range(10): print(i)
来源：http://rb.shxzukj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vv.huanxung.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yj.huixinmuqiang.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nc.gzmigu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ip.jianghongdianzi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mb.newstarts.cn

Ruby: 10.times { |i| puts i }
来源：http://ot.huanxung.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tp.huanxung.cn

[B05] 遍历数组 / 列表
来源：http://aw.yuntaijiaju.cn

Py:   for item in arr: print(item)
来源：http://br.shxzukj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gs.yuexingan06.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ad.yuexingan06.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mq.hahajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://tu.huixiangedu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vs.muxihuayi.cn

Ruby: arr.each { |item| puts item }
来源：http://wz.huixiangedu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qk.haigaiapp.cn

[B06] 遍历字典 / 对象
来源：http://rg.panjiajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ln.shxzukj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ee.yuexingan06.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://px.bookmarksfly.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qn.yuntaijiaju.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sf.chemitech.net.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hf.newstarts.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rj.lnxyls.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bm.nicolike.cn

[B07] while 循环
来源：http://yv.bookmarksfly.cn

Py:   while i < 10: i += 1
来源：http://sa.szsharing.cn

PHP:  while ($i < 10) { $i++; }
来源：http://yk.chemitech.net.cn

JS:   while (i < 10) { i++; }
来源：http://nj.hnjuh.cn

TS:   while (i < 10) { i++; }
来源：http://sd.shxzskj.cn

Java: while (i < 10) { i++; }
来源：http://by.lnxyls.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bl.hahajie.cn

Ruby: while i < 10; i += 1; end
来源：http://pv.jianghongdianzi.cn

C#:   while (i < 10) { i++; }
来源：http://tj.yuexingan06.cn

[B08] do-while（至少执行一次）
来源：http://jm.hnjuh.cn

Py:   # 无 do-while：用 while True + break
来源：http://ed.shxzukj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zg.shxzskj.cn

JS:   do { i++; } while (i < 10);
来源：http://zb.nszjky.cn

TS:   do { i++; } while (i < 10);
来源：http://uc.jctech888.com.cn

Java: do { i++; } while (i < 10);
来源：http://dh.asd995.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wf.wgjwhj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://tf.hnjuh.cn

C#:   do { i++; } while (i < 10);
来源：http://pi.bookmarksfly.cn

[B09] break 与 continue
来源：http://gk.shxzukj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ud.colortex.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://np.shxzukj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hw.wgjwhj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ul.szsharing.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yb.9csxet.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cr.huanxung.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ix.chemitech.net.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ta.bjjhwx.cn

[B10] 遍历同时拿索引
来源：http://gg.asd995.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://uf.asd995.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yu.yuexingan06.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://re.huixinmuqiang.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pm.nicolike.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lz.jctech888.com.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nj.9csxet.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yw.9csxet.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mh.asd995.cn

[B11] 生成数字序列 / 区间
来源：http://uc.yuexingan06.cn

Py:   list(range(0, 10, 2))
来源：http://mp.huixiangedu.cn

PHP:  range(0, 10, 2);
来源：http://oi.szsharing.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yg.chemitech.net.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ur.szxytkj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sf.chemitech.net.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hb.szsharing.cn

Ruby: (0...10).step(2).to_a
来源：http://bm.haigaiapp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xq.huanxung.cn

[B12] 跳出多层循环
来源：http://cc.haigaiapp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yf.colortex.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://lo.muxihuayi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ak.shtwfgs.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qj.jianghongdianzi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://en.jctech888.com.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dh.newstarts.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jj.lnxyls.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dv.haigaiapp.cn

[B13] 判断是否为数字
来源：http://ir.wgjwhj.cn

Py:   isinstance(x, (int, float))
来源：http://xd.hahajie.cn

PHP:  is_numeric($x)
来源：http://jj.asd995.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ev.jctech888.com.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bw.lnxyls.cn

Java: x instanceof Number
来源：http://tx.muxihuayi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://eo.shxzskj.cn

Ruby: x.is_a?(Numeric)
来源：http://dd.jctech888.com.cn

C#:   x is int or double or decimal
来源：http://qu.hahajie.cn

[B14] 判断值是否在集合内
来源：http://lp.lnxyls.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zc.nicolike.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kd.521024.cn

JS:   [1, 2, 3].includes(x)
来源：http://wd.nszjky.cn

TS:   [1, 2, 3].includes(x)
来源：http://ya.jctech888.com.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://tx.gzmigu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ji.chemitech.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cf.chemitech.net.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lk.bjjhwx.cn

[B15] 布尔运算与取反
来源：http://ow.lnxyls.cn

Py:   a and b or not c
来源：http://lu.bjjhwx.cn

PHP:  $a && $b || !$c
来源：http://ob.yuntaijiaju.cn

JS:   a && b || !c
来源：http://er.jianghongdianzi.cn

TS:   a && b || !c
来源：http://yl.lnxyls.cn

Java: a && b || !c
来源：http://ca.chemitech.net.cn

Go:   a && b || !c
来源：http://kq.wgjwhj.cn

Ruby: a && b || !c
来源：http://ur.shtwfgs.cn

C#:   a && b || !c
来源：http://kd.hnjuh.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xc.huixiangedu.cn

Py:   if not data: return
来源：http://um.9csxet.cn

PHP:  if (!$data) { return; }
来源：http://ph.huanxung.cn

JS:   if (!data) return;
来源：http://ql.9csxet.cn

TS:   if (!data) return;
来源：http://uu.huanxung.cn

Java: if (data == null) return;
来源：http://kr.muxihuayi.cn

Go:   if data == nil { return }
来源：http://vu.521024.cn

Ruby: return if data.nil?
来源：http://lf.shtwfgs.cn

C#:   if (data == null) return;
来源：http://sa.colortex.cn

================================================================================
来源：http://bt.panjiajie.cn

C. 函数与作用域
来源：http://al.yuexingan06.cn

================================================================================
来源：http://ln.colortex.cn

[C01] 定义函数
来源：http://zh.huixinmuqiang.cn

Py:   def add(a, b): return a + b
来源：http://pm.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zh.jctech888.com.cn

JS:   function add(a, b) { return a + b; }
来源：http://kz.hahajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ij.huixinmuqiang.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ct.colortex.cn

Go:   func add(a, b int) int { return a + b }
来源：http://tr.szsharing.cn

Ruby: def add(a, b); a + b; end
来源：http://hc.jianghongdianzi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qq.huixiangedu.cn

[C02] 默认参数
来源：http://ht.huixiangedu.cn

Py:   def greet(name="World"): return name
来源：http://ut.newstarts.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ud.yuexingan06.cn

JS:   function greet(name = "World") { return name; }
来源：http://jb.huixinmuqiang.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yg.wgjwhj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qe.newstarts.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lx.jianghongdianzi.cn

Ruby: def greet(name = "World") = name
来源：http://ky.haigaiapp.cn

C#:   string Greet(string name = "World") => name;
来源：http://xr.gzmigu.cn

[C03] 可变参数
来源：http://sn.yuntaijiaju.cn

Py:   def total(*args): return sum(args)
来源：http://fy.jctech888.com.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://co.panjiajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://uq.huixiangedu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ti.jianghongdianzi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nv.shxzskj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://da.gzmigu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ic.hahajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ye.asd995.cn

[C04] 命名参数 / 关键字参数
来源：http://ym.hahajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yc.yuexingan06.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cs.hahajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ev.yuexingan06.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qo.yuntaijiaju.cn

Java: // 无：用 Builder 模式或 record
来源：http://oc.521024.cn

Go:   // 无：用配置结构体参数
来源：http://gr.huixinmuqiang.cn

Ruby: f(a: 1, b: 2)
来源：http://yw.9csxet.cn

C#:   f(a: 1, b: 2)
来源：http://ye.colortex.cn

[C05] 返回多个值
来源：http://it.shtwfgs.cn

Py:   return a, b
来源：http://ow.huixiangedu.cn

PHP:  return [$a, $b];
来源：http://wq.shxzskj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://cq.huixiangedu.cn

TS:   return { a, b };
来源：http://rb.hahajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ve.haigaiapp.cn

Go:   return a, b
来源：http://nt.colortex.cn

Ruby: return a, b
来源：http://cx.yuntaijiaju.cn

C#:   return (a, b);              // ValueTuple
来源：http://mc.yuexingan06.cn

[C06] 匿名函数 / lambda
来源：http://pv.huixiangedu.cn

Py:   square = lambda x: x * x
来源：http://zl.colortex.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qe.haigaiapp.cn

JS:   const square = x => x * x;
来源：http://sc.gzmigu.cn

TS:   const square = (x: number): number => x * x;
来源：http://xp.huanxung.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gd.shxzskj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wf.nicolike.cn

Ruby: square = ->(x) { x * x }
来源：http://if.wgjwhj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wg.hnjuh.cn

[C07] 把函数作为参数传入
来源：http://lo.panjiajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://px.szsharing.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vy.huixiangedu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dd.lnxyls.cn

TS:   arr.map(String)
来源：http://we.yuntaijiaju.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hr.hnjuh.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://se.yuntaijiaju.cn

Ruby: arr.map(&:upcase)
来源：http://ie.nszjky.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://yb.huixinmuqiang.cn

[C08] 闭包
来源：http://zv.newstarts.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fq.lnxyls.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nl.muxihuayi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uj.bjjhwx.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wg.shxzukj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lx.colortex.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://iq.newstarts.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fr.asd995.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ib.gzmigu.cn

[C09] 递归
来源：http://wr.jctech888.com.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nk.521024.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fg.shtwfgs.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uv.szsharing.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tp.wgjwhj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bw.shxzskj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cm.shxzukj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hp.huanxung.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ax.bookmarksfly.cn

[C10] 变量作用域
来源：http://zf.shxzukj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cr.panjiajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gx.nszjky.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vb.yuexingan06.cn

TS:   同 JS
来源：http://lr.nicolike.cn

Java: 方法内为块级作用域
来源：http://ip.colortex.cn

Go:   花括号块级作用域
来源：http://cb.bookmarksfly.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://he.shxzukj.cn

C#:   块级作用域
来源：http://oi.huixiangedu.cn

[C11] 模块导入与导出
来源：http://kc.chemitech.net.cn

Py:   from module import func
来源：http://hh.szxytkj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://lq.huanxung.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ui.shxzskj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://eq.szsharing.cn

Java: import java.util.List;
来源：http://lo.huixiangedu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ro.haigaiapp.cn

Ruby: require "json"; require_relative "./util"
来源：http://kz.bjjhwx.cn

C#:   using System.Text;
来源：http://nb.shtwfgs.cn

[C12] 立即执行函数 IIFE
来源：http://gr.shtwfgs.cn

Py:   (lambda: print("run"))()
来源：http://vp.shxzukj.cn

PHP:  (function () { echo "run"; })();
来源：http://pd.asd995.cn

JS:   (() => { console.log("run"); })();
来源：http://gk.9csxet.cn

TS:   (() => { console.log("run"); })();
来源：http://ol.colortex.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vd.newstarts.cn

Go:   func() { fmt.Println("run") }()
来源：http://id.huixinmuqiang.cn

Ruby: -> { puts "run" }.call
来源：http://jk.jianghongdianzi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wo.9csxet.cn

[C13] 类型声明 / 类型注解
来源：http://aq.huanxung.cn


<!-- 参考信息 -->