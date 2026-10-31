代发 wailian999

TS:   s.length
来源：http://vi.shxzukj.cn

Java: s.length()
来源：http://ay.asd995.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://si.jianghongdianzi.cn

Ruby: s.length
来源：http://jm.haigaiapp.cn

C#:   s.Length
来源：http://vw.jctech888.com.cn

[A23] 大小写转换
来源：http://ud.hnjuh.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://sm.asd995.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yv.nszjky.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tc.newstarts.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ar.huanxung.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://oz.newstarts.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tc.huixiangedu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://if.asd995.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://dt.shtwfgs.cn

[A24] 去除首尾空白
来源：http://if.huixiangedu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cn.huanxung.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xi.szxytkj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fd.muxihuayi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nb.huanxung.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ge.yuntaijiaju.cn

Go:   strings.TrimSpace(s)
来源：http://fs.panjiajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://eu.hahajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lm.9csxet.cn

[A25] 字符串比较
来源：http://tn.szsharing.cn

Py:   s1 == s2; s1 != s2
来源：http://uo.jianghongdianzi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wl.szsharing.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lp.shxzskj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://sn.shtwfgs.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ch.yuntaijiaju.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ok.huanxung.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://zr.nicolike.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://px.hnjuh.cn

[A26] 类型转换总览
来源：http://jd.szsharing.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kr.lnxyls.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rb.521024.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://py.bookmarksfly.cn

TS:   Number() String() Boolean() x as number
来源：http://jd.chemitech.net.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://sg.bookmarksfly.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bu.panjiajie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://cw.shtwfgs.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://av.hnjuh.cn

================================================================================
来源：http://zs.huixiangedu.cn

B. 流程控制
来源：http://mt.huanxung.cn

================================================================================
来源：http://qb.huanxung.cn

[B01] 条件判断 if / else
来源：http://mk.chemitech.net.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wq.wgjwhj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pu.shxzukj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ep.panjiajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://om.asd995.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ow.shxzukj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jk.lnxyls.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gz.huixiangedu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ew.hahajie.cn

[B02] 多分支 else if / elif
来源：http://nl.huixinmuqiang.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nz.shxzukj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ny.yuntaijiaju.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nt.huixinmuqiang.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mw.yuexingan06.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xx.huixinmuqiang.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ps.9csxet.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yw.shtwfgs.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eh.9csxet.cn

[B03] switch / match / case
来源：http://wl.shxzskj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xc.hahajie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xi.jianghongdianzi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hs.panjiajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xh.colortex.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dn.bjjhwx.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lt.huixiangedu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rh.bookmarksfly.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zt.hahajie.cn

[B04] for 计数循环
来源：http://or.bookmarksfly.cn

Py:   for i in range(10): print(i)
来源：http://oo.nicolike.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ne.nicolike.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ly.hnjuh.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ej.gzmigu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hs.shxzskj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xc.shtwfgs.cn

Ruby: 10.times { |i| puts i }
来源：http://yt.asd995.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zp.huixinmuqiang.cn

[B05] 遍历数组 / 列表
来源：http://ls.haigaiapp.cn

Py:   for item in arr: print(item)
来源：http://qx.bookmarksfly.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jm.hnjuh.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://rp.nicolike.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ls.szxytkj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ju.jianghongdianzi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://af.nicolike.cn

Ruby: arr.each { |item| puts item }
来源：http://rn.muxihuayi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yl.chemitech.net.cn

[B06] 遍历字典 / 对象
来源：http://hp.yuntaijiaju.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://nm.szxytkj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dy.shxzukj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://in.521024.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hx.bjjhwx.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yr.gzmigu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fz.szsharing.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nm.yuntaijiaju.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sf.huixinmuqiang.cn

[B07] while 循环
来源：http://qm.panjiajie.cn

Py:   while i < 10: i += 1
来源：http://ly.bookmarksfly.cn

PHP:  while ($i < 10) { $i++; }
来源：http://nx.hahajie.cn

JS:   while (i < 10) { i++; }
来源：http://om.huixinmuqiang.cn

TS:   while (i < 10) { i++; }
来源：http://ma.hnjuh.cn

Java: while (i < 10) { i++; }
来源：http://hu.wgjwhj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wc.bookmarksfly.cn

Ruby: while i < 10; i += 1; end
来源：http://dv.shtwfgs.cn

C#:   while (i < 10) { i++; }
来源：http://ae.shxzukj.cn

[B08] do-while（至少执行一次）
来源：http://ex.yuexingan06.cn

Py:   # 无 do-while：用 while True + break
来源：http://eb.9csxet.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://uf.jianghongdianzi.cn

JS:   do { i++; } while (i < 10);
来源：http://nt.shxzukj.cn

TS:   do { i++; } while (i < 10);
来源：http://is.bjjhwx.cn

Java: do { i++; } while (i < 10);
来源：http://qz.nicolike.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jq.yuexingan06.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zd.nicolike.cn

C#:   do { i++; } while (i < 10);
来源：http://nl.szsharing.cn

[B09] break 与 continue
来源：http://wh.nszjky.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ae.huixiangedu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rf.jianghongdianzi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hy.shxzukj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vq.bjjhwx.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bf.yuexingan06.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kd.shtwfgs.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://td.huixinmuqiang.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pc.521024.cn

[B10] 遍历同时拿索引
来源：http://sz.nszjky.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xo.hnjuh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hx.asd995.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ye.shxzskj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jz.newstarts.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tc.shtwfgs.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dc.bjjhwx.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wd.yuexingan06.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ks.nszjky.cn

[B11] 生成数字序列 / 区间
来源：http://km.muxihuayi.cn

Py:   list(range(0, 10, 2))
来源：http://dd.nszjky.cn

PHP:  range(0, 10, 2);
来源：http://zx.szxytkj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nj.wgjwhj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ft.yuntaijiaju.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bn.jianghongdianzi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yj.yuntaijiaju.cn

Ruby: (0...10).step(2).to_a
来源：http://ob.nicolike.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jr.wgjwhj.cn

[B12] 跳出多层循环
来源：http://fn.szxytkj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ac.colortex.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://kc.huixiangedu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qt.huixinmuqiang.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ql.panjiajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ic.muxihuayi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xm.lnxyls.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wi.hahajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wm.chemitech.net.cn

[B13] 判断是否为数字
来源：http://kz.lnxyls.cn

Py:   isinstance(x, (int, float))
来源：http://hf.9csxet.cn

PHP:  is_numeric($x)
来源：http://ml.colortex.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://as.huixiangedu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xq.jctech888.com.cn

Java: x instanceof Number
来源：http://kh.hahajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xc.bookmarksfly.cn

Ruby: x.is_a?(Numeric)
来源：http://hk.panjiajie.cn

C#:   x is int or double or decimal
来源：http://qe.jctech888.com.cn

[B14] 判断值是否在集合内
来源：http://fo.hahajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mf.hahajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qu.shxzskj.cn

JS:   [1, 2, 3].includes(x)
来源：http://mi.haigaiapp.cn

TS:   [1, 2, 3].includes(x)
来源：http://tg.9csxet.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qd.huixiangedu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lp.hnjuh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ea.muxihuayi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://af.szsharing.cn

[B15] 布尔运算与取反
来源：http://kk.hnjuh.cn

Py:   a and b or not c
来源：http://dp.szsharing.cn

PHP:  $a && $b || !$c
来源：http://jd.nicolike.cn

JS:   a && b || !c
来源：http://mb.muxihuayi.cn

TS:   a && b || !c
来源：http://ab.colortex.cn

Java: a && b || !c
来源：http://mn.lnxyls.cn

Go:   a && b || !c
来源：http://jj.bookmarksfly.cn

Ruby: a && b || !c
来源：http://fa.nszjky.cn

C#:   a && b || !c
来源：http://eb.nszjky.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bb.9csxet.cn

Py:   if not data: return
来源：http://hb.yuexingan06.cn

PHP:  if (!$data) { return; }
来源：http://rh.lnxyls.cn

JS:   if (!data) return;
来源：http://uk.szxytkj.cn

TS:   if (!data) return;
来源：http://er.hnjuh.cn

Java: if (data == null) return;
来源：http://ct.szsharing.cn

Go:   if data == nil { return }
来源：http://hs.newstarts.cn

Ruby: return if data.nil?
来源：http://my.huixinmuqiang.cn

C#:   if (data == null) return;
来源：http://ul.chemitech.net.cn

================================================================================
来源：http://qs.shxzukj.cn

C. 函数与作用域
来源：http://ml.huanxung.cn

================================================================================
来源：http://xw.gzmigu.cn

[C01] 定义函数
来源：http://ps.bjjhwx.cn

Py:   def add(a, b): return a + b
来源：http://cr.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wn.colortex.cn

JS:   function add(a, b) { return a + b; }
来源：http://uc.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bp.haigaiapp.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://br.bjjhwx.cn

Go:   func add(a, b int) int { return a + b }
来源：http://iv.shtwfgs.cn

Ruby: def add(a, b); a + b; end
来源：http://hd.521024.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uz.shxzukj.cn

[C02] 默认参数
来源：http://am.panjiajie.cn

Py:   def greet(name="World"): return name
来源：http://qn.shxzukj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://gh.yuntaijiaju.cn

JS:   function greet(name = "World") { return name; }
来源：http://lt.hahajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://mt.newstarts.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wp.bookmarksfly.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fx.huanxung.cn

Ruby: def greet(name = "World") = name
来源：http://vg.9csxet.cn

C#:   string Greet(string name = "World") => name;
来源：http://ot.hnjuh.cn

[C03] 可变参数
来源：http://qe.nicolike.cn

Py:   def total(*args): return sum(args)
来源：http://hs.yuntaijiaju.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ez.szxytkj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yk.haigaiapp.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gq.huixiangedu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bs.panjiajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mu.szxytkj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://td.hahajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vm.huixiangedu.cn

[C04] 命名参数 / 关键字参数
来源：http://ql.yuexingan06.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mg.hnjuh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hp.gzmigu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nt.shtwfgs.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vw.bjjhwx.cn

Java: // 无：用 Builder 模式或 record
来源：http://yj.hnjuh.cn

Go:   // 无：用配置结构体参数
来源：http://yv.shxzskj.cn

Ruby: f(a: 1, b: 2)
来源：http://dj.shtwfgs.cn

C#:   f(a: 1, b: 2)
来源：http://fp.muxihuayi.cn

[C05] 返回多个值
来源：http://jp.gzmigu.cn

Py:   return a, b
来源：http://ta.huixiangedu.cn

PHP:  return [$a, $b];
来源：http://is.hahajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://of.panjiajie.cn

TS:   return { a, b };
来源：http://jp.newstarts.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ph.jctech888.com.cn

Go:   return a, b
来源：http://ms.chemitech.net.cn

Ruby: return a, b
来源：http://jf.shxzskj.cn

C#:   return (a, b);              // ValueTuple
来源：http://xp.panjiajie.cn

[C06] 匿名函数 / lambda
来源：http://zq.shxzukj.cn

Py:   square = lambda x: x * x
来源：http://wh.szxytkj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://us.lnxyls.cn

JS:   const square = x => x * x;
来源：http://im.nicolike.cn

TS:   const square = (x: number): number => x * x;
来源：http://qp.newstarts.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gc.shtwfgs.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ah.haigaiapp.cn

Ruby: square = ->(x) { x * x }
来源：http://gi.shtwfgs.cn

C#:   Func<int, int> square = x => x * x;
来源：http://nj.nszjky.cn

[C07] 把函数作为参数传入
来源：http://ck.yuexingan06.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bt.bjjhwx.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ug.bjjhwx.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qo.hahajie.cn

TS:   arr.map(String)
来源：http://mn.hnjuh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qi.shxzskj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xg.newstarts.cn

Ruby: arr.map(&:upcase)
来源：http://tb.yuntaijiaju.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://dl.shtwfgs.cn

[C08] 闭包
来源：http://kz.szsharing.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wb.jctech888.com.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qg.jianghongdianzi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fg.huixinmuqiang.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uu.panjiajie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ic.panjiajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cx.szxytkj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pb.hnjuh.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cp.szsharing.cn

[C09] 递归
来源：http://rd.asd995.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hv.hahajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ft.9csxet.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zs.shxzukj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hk.newstarts.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://eg.wgjwhj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zt.szxytkj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ob.colortex.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yz.wgjwhj.cn

[C10] 变量作用域
来源：http://ki.szxytkj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hh.yuexingan06.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.nicolike.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://or.shxzskj.cn

TS:   同 JS
来源：http://fp.yuexingan06.cn

Java: 方法内为块级作用域
来源：http://mq.gzmigu.cn

Go:   花括号块级作用域
来源：http://ko.chemitech.net.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cj.haigaiapp.cn

C#:   块级作用域
来源：http://do.szsharing.cn

[C11] 模块导入与导出
来源：http://rh.bjjhwx.cn

Py:   from module import func
来源：http://px.colortex.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hy.huixinmuqiang.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://pg.nszjky.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mm.newstarts.cn

Java: import java.util.List;
来源：http://dq.yuntaijiaju.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bt.shxzskj.cn

Ruby: require "json"; require_relative "./util"
来源：http://sm.newstarts.cn

C#:   using System.Text;
来源：http://yf.szsharing.cn

[C12] 立即执行函数 IIFE
来源：http://iw.colortex.cn

Py:   (lambda: print("run"))()
来源：http://nh.yuexingan06.cn

PHP:  (function () { echo "run"; })();
来源：http://qn.wgjwhj.cn

JS:   (() => { console.log("run"); })();
来源：http://xu.hahajie.cn

TS:   (() => { console.log("run"); })();
来源：http://zw.yuntaijiaju.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://or.haigaiapp.cn

Go:   func() { fmt.Println("run") }()
来源：http://kf.yuexingan06.cn

Ruby: -> { puts "run" }.call
来源：http://ut.chemitech.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pz.newstarts.cn

[C13] 类型声明 / 类型注解
来源：http://kd.huixiangedu.cn


<!-- 参考信息 -->