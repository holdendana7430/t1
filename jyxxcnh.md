代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ko.panjiajie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://lc.hahajie.cn

[A24] 去除首尾空白
来源：http://qo.muxihuayi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://as.yuntaijiaju.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xm.colortex.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yq.haigaiapp.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fy.bookmarksfly.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://op.jctech888.com.cn

Go:   strings.TrimSpace(s)
来源：http://xo.yuntaijiaju.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mm.haigaiapp.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qd.hnjuh.cn

[A25] 字符串比较
来源：http://zn.yuexingan06.cn

Py:   s1 == s2; s1 != s2
来源：http://mb.shxzukj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://eh.nicolike.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hq.yuexingan06.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kr.colortex.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zw.hahajie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://uh.hnjuh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://tz.hahajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sx.shxzukj.cn

[A26] 类型转换总览
来源：http://rn.gzmigu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ja.szsharing.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lw.9csxet.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ee.wgjwhj.cn

TS:   Number() String() Boolean() x as number
来源：http://oh.jianghongdianzi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yi.panjiajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nd.szsharing.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://dn.shxzskj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bg.521024.cn

================================================================================
来源：http://zh.lnxyls.cn

B. 流程控制
来源：http://kx.bjjhwx.cn

================================================================================
来源：http://pr.jctech888.com.cn

[B01] 条件判断 if / else
来源：http://fj.panjiajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://nb.jctech888.com.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://th.hahajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://eb.hahajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://re.haigaiapp.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://gs.asd995.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xx.shtwfgs.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qk.jianghongdianzi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ve.shtwfgs.cn

[B02] 多分支 else if / elif
来源：http://nh.jianghongdianzi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nu.panjiajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fy.hahajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tv.bjjhwx.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vn.wgjwhj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ju.521024.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uv.yuexingan06.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zw.jctech888.com.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fi.jianghongdianzi.cn

[B03] switch / match / case
来源：http://zq.huanxung.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kw.hnjuh.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ou.9csxet.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://iq.huanxung.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://il.shxzukj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ee.shxzskj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://sx.521024.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hl.hnjuh.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pk.huanxung.cn

[B04] for 计数循环
来源：http://tw.huixiangedu.cn

Py:   for i in range(10): print(i)
来源：http://dv.huanxung.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ti.jctech888.com.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mj.nicolike.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://di.asd995.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fa.bjjhwx.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xb.9csxet.cn

Ruby: 10.times { |i| puts i }
来源：http://ce.nszjky.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ca.panjiajie.cn

[B05] 遍历数组 / 列表
来源：http://jc.hahajie.cn

Py:   for item in arr: print(item)
来源：http://ds.jianghongdianzi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://df.521024.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://th.shtwfgs.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ay.jianghongdianzi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://bu.shxzskj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fn.shtwfgs.cn

Ruby: arr.each { |item| puts item }
来源：http://ni.nszjky.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bi.haigaiapp.cn

[B06] 遍历字典 / 对象
来源：http://gk.gzmigu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sa.lnxyls.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fs.yuntaijiaju.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ou.chemitech.net.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tp.panjiajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://up.wgjwhj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nq.nszjky.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ky.nszjky.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jg.hahajie.cn

[B07] while 循环
来源：http://mf.jianghongdianzi.cn

Py:   while i < 10: i += 1
来源：http://nm.huixiangedu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://tq.hnjuh.cn

JS:   while (i < 10) { i++; }
来源：http://fo.huanxung.cn

TS:   while (i < 10) { i++; }
来源：http://uc.nicolike.cn

Java: while (i < 10) { i++; }
来源：http://pq.muxihuayi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yf.yuexingan06.cn

Ruby: while i < 10; i += 1; end
来源：http://bu.hnjuh.cn

C#:   while (i < 10) { i++; }
来源：http://ue.lnxyls.cn

[B08] do-while（至少执行一次）
来源：http://rl.hahajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://oz.huanxung.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jc.bjjhwx.cn

JS:   do { i++; } while (i < 10);
来源：http://cb.gzmigu.cn

TS:   do { i++; } while (i < 10);
来源：http://qo.jianghongdianzi.cn

Java: do { i++; } while (i < 10);
来源：http://di.wgjwhj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://cr.hnjuh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://yh.newstarts.cn

C#:   do { i++; } while (i < 10);
来源：http://yq.jctech888.com.cn

[B09] break 与 continue
来源：http://fy.lnxyls.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://na.colortex.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sn.shxzukj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hw.haigaiapp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cm.521024.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fe.chemitech.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xk.gzmigu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vq.asd995.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dj.hahajie.cn

[B10] 遍历同时拿索引
来源：http://je.newstarts.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lq.9csxet.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ax.huanxung.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dc.haigaiapp.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vh.szsharing.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vv.szxytkj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://el.yuntaijiaju.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zs.hahajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pw.nszjky.cn

[B11] 生成数字序列 / 区间
来源：http://ln.yuexingan06.cn

Py:   list(range(0, 10, 2))
来源：http://fg.bjjhwx.cn

PHP:  range(0, 10, 2);
来源：http://mr.newstarts.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vb.yuntaijiaju.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ng.bookmarksfly.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fw.chemitech.net.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zh.yuntaijiaju.cn

Ruby: (0...10).step(2).to_a
来源：http://lg.huanxung.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ly.gzmigu.cn

[B12] 跳出多层循环
来源：http://sk.chemitech.net.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://oh.huixinmuqiang.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://rd.yuntaijiaju.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lq.panjiajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gw.nicolike.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mf.521024.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ok.muxihuayi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hc.newstarts.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uw.shxzskj.cn

[B13] 判断是否为数字
来源：http://rd.nicolike.cn

Py:   isinstance(x, (int, float))
来源：http://ml.yuexingan06.cn

PHP:  is_numeric($x)
来源：http://rk.yuexingan06.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nc.szsharing.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ff.huixiangedu.cn

Java: x instanceof Number
来源：http://zl.colortex.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hi.nszjky.cn

Ruby: x.is_a?(Numeric)
来源：http://al.yuexingan06.cn

C#:   x is int or double or decimal
来源：http://vz.nszjky.cn

[B14] 判断值是否在集合内
来源：http://jb.bookmarksfly.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gc.bjjhwx.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ou.newstarts.cn

JS:   [1, 2, 3].includes(x)
来源：http://qf.newstarts.cn

TS:   [1, 2, 3].includes(x)
来源：http://uy.huixiangedu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xa.lnxyls.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kk.chemitech.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fs.muxihuayi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ki.bookmarksfly.cn

[B15] 布尔运算与取反
来源：http://xl.hahajie.cn

Py:   a and b or not c
来源：http://ks.yuntaijiaju.cn

PHP:  $a && $b || !$c
来源：http://xh.9csxet.cn

JS:   a && b || !c
来源：http://qg.gzmigu.cn

TS:   a && b || !c
来源：http://qi.lnxyls.cn

Java: a && b || !c
来源：http://bu.huixiangedu.cn

Go:   a && b || !c
来源：http://vc.gzmigu.cn

Ruby: a && b || !c
来源：http://xp.newstarts.cn

C#:   a && b || !c
来源：http://bv.yuexingan06.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qh.szxytkj.cn

Py:   if not data: return
来源：http://dr.chemitech.net.cn

PHP:  if (!$data) { return; }
来源：http://vo.wgjwhj.cn

JS:   if (!data) return;
来源：http://op.muxihuayi.cn

TS:   if (!data) return;
来源：http://yx.shtwfgs.cn

Java: if (data == null) return;
来源：http://db.colortex.cn

Go:   if data == nil { return }
来源：http://jk.huanxung.cn

Ruby: return if data.nil?
来源：http://my.jctech888.com.cn

C#:   if (data == null) return;
来源：http://kk.newstarts.cn

================================================================================
来源：http://yf.shtwfgs.cn

C. 函数与作用域
来源：http://eq.lnxyls.cn

================================================================================
来源：http://fz.muxihuayi.cn

[C01] 定义函数
来源：http://cw.shtwfgs.cn

Py:   def add(a, b): return a + b
来源：http://wg.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gh.newstarts.cn

JS:   function add(a, b) { return a + b; }
来源：http://ma.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hu.huanxung.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://nz.yuntaijiaju.cn

Go:   func add(a, b int) int { return a + b }
来源：http://fg.szsharing.cn

Ruby: def add(a, b); a + b; end
来源：http://uk.jctech888.com.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ir.9csxet.cn

[C02] 默认参数
来源：http://qe.shxzukj.cn

Py:   def greet(name="World"): return name
来源：http://ss.hnjuh.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dw.muxihuayi.cn

JS:   function greet(name = "World") { return name; }
来源：http://ry.bjjhwx.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yj.521024.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ru.huanxung.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pa.jianghongdianzi.cn

Ruby: def greet(name = "World") = name
来源：http://xh.hahajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://dr.9csxet.cn

[C03] 可变参数
来源：http://qy.newstarts.cn

Py:   def total(*args): return sum(args)
来源：http://gf.szxytkj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cb.szxytkj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bv.chemitech.net.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qk.jianghongdianzi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wk.asd995.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jd.nszjky.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rn.szxytkj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pl.bjjhwx.cn

[C04] 命名参数 / 关键字参数
来源：http://rd.haigaiapp.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pb.lnxyls.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://oc.huanxung.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://je.szsharing.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qt.bookmarksfly.cn

Java: // 无：用 Builder 模式或 record
来源：http://vr.gzmigu.cn

Go:   // 无：用配置结构体参数
来源：http://an.shtwfgs.cn

Ruby: f(a: 1, b: 2)
来源：http://yr.haigaiapp.cn

C#:   f(a: 1, b: 2)
来源：http://xg.521024.cn

[C05] 返回多个值
来源：http://gh.hahajie.cn

Py:   return a, b
来源：http://hd.huanxung.cn

PHP:  return [$a, $b];
来源：http://zu.hahajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ow.wgjwhj.cn

TS:   return { a, b };
来源：http://jk.shtwfgs.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://di.lnxyls.cn

Go:   return a, b
来源：http://li.shtwfgs.cn

Ruby: return a, b
来源：http://ts.bookmarksfly.cn

C#:   return (a, b);              // ValueTuple
来源：http://vc.nicolike.cn

[C06] 匿名函数 / lambda
来源：http://ys.haigaiapp.cn

Py:   square = lambda x: x * x
来源：http://dq.jianghongdianzi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qa.9csxet.cn

JS:   const square = x => x * x;
来源：http://ic.panjiajie.cn

TS:   const square = (x: number): number => x * x;
来源：http://qq.huixinmuqiang.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ry.szsharing.cn

Go:   sq := func(x int) int { return x * x }
来源：http://uz.nicolike.cn

Ruby: square = ->(x) { x * x }
来源：http://fa.huixinmuqiang.cn

C#:   Func<int, int> square = x => x * x;
来源：http://tq.szsharing.cn

[C07] 把函数作为参数传入
来源：http://li.huanxung.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jg.newstarts.cn

PHP:  array_map("strtoupper", $arr);
来源：http://fc.lnxyls.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://us.huanxung.cn

TS:   arr.map(String)
来源：http://jv.jianghongdianzi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ct.wgjwhj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sn.shxzukj.cn

Ruby: arr.map(&:upcase)
来源：http://yc.shxzskj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ui.yuexingan06.cn

[C08] 闭包
来源：http://hh.bookmarksfly.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ya.asd995.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mm.bookmarksfly.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fn.huixinmuqiang.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wh.bjjhwx.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ik.shtwfgs.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gy.jianghongdianzi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bf.newstarts.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://sv.colortex.cn

[C09] 递归
来源：http://tz.nszjky.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jt.szxytkj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://eh.521024.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gz.nszjky.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yv.szxytkj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://so.newstarts.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qi.wgjwhj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xx.nszjky.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rl.9csxet.cn

[C10] 变量作用域
来源：http://xa.jianghongdianzi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yh.jianghongdianzi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ns.chemitech.net.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kq.chemitech.net.cn

TS:   同 JS
来源：http://pp.huixiangedu.cn

Java: 方法内为块级作用域
来源：http://gq.hnjuh.cn

Go:   花括号块级作用域
来源：http://ds.haigaiapp.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nj.huixiangedu.cn

C#:   块级作用域
来源：http://zx.nicolike.cn

[C11] 模块导入与导出
来源：http://kt.asd995.cn

Py:   from module import func
来源：http://ne.panjiajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://sh.bookmarksfly.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://oj.colortex.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jz.shxzukj.cn

Java: import java.util.List;
来源：http://qr.muxihuayi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jp.hnjuh.cn

Ruby: require "json"; require_relative "./util"
来源：http://ke.hnjuh.cn

C#:   using System.Text;
来源：http://fx.huanxung.cn

[C12] 立即执行函数 IIFE
来源：http://nd.lnxyls.cn

Py:   (lambda: print("run"))()
来源：http://yu.nszjky.cn

PHP:  (function () { echo "run"; })();
来源：http://jb.huixiangedu.cn

JS:   (() => { console.log("run"); })();
来源：http://wr.huanxung.cn

TS:   (() => { console.log("run"); })();
来源：http://nd.panjiajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://es.bookmarksfly.cn

Go:   func() { fmt.Println("run") }()
来源：http://bh.hahajie.cn

Ruby: -> { puts "run" }.call
来源：http://sq.wgjwhj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wr.jctech888.com.cn

[C13] 类型声明 / 类型注解
来源：http://ul.newstarts.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ht.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dm.shxzskj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yy.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fi.shtwfgs.cn

Java: int add(int a, int b) { return a + b; }
来源：http://nc.nicolike.cn

Go:   func add(a, b int) int
来源：http://fw.newstarts.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nr.asd995.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fs.chemitech.net.cn

[C14] 泛型函数
来源：http://vo.shxzskj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://og.hahajie.cn

PHP:  // 无泛型
来源：http://xe.lnxyls.cn

JS:   // 无泛型
来源：http://ra.chemitech.net.cn


<!-- 参考信息 -->