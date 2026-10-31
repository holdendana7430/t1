代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://sg.shxzukj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://dq.newstarts.cn

Ruby: format("%.2f", 3.14159)
来源：http://tt.szxytkj.cn

C#:   3.14159.ToString("F2")
来源：http://vr.colortex.cn

[A22] 获取字符串长度
来源：http://if.huixiangedu.cn

Py:   len(s)
来源：http://ig.muxihuayi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xt.huixiangedu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gb.wgjwhj.cn

TS:   s.length
来源：http://hj.shxzskj.cn

Java: s.length()
来源：http://rz.jianghongdianzi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tc.asd995.cn

Ruby: s.length
来源：http://lx.huanxung.cn

C#:   s.Length
来源：http://vb.shxzskj.cn

[A23] 大小写转换
来源：http://iv.huixinmuqiang.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vq.521024.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rf.yuntaijiaju.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://sf.bookmarksfly.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dk.bjjhwx.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://am.colortex.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://oc.hnjuh.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ie.huanxung.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://dc.gzmigu.cn

[A24] 去除首尾空白
来源：http://jm.bookmarksfly.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jr.bjjhwx.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sv.huanxung.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xu.nicolike.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zg.huixiangedu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nx.panjiajie.cn

Go:   strings.TrimSpace(s)
来源：http://ri.jctech888.com.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zq.wgjwhj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jc.hahajie.cn

[A25] 字符串比较
来源：http://ms.chemitech.net.cn

Py:   s1 == s2; s1 != s2
来源：http://ah.521024.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mq.panjiajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yn.colortex.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://js.521024.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://by.hahajie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xp.huixiangedu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://pk.nicolike.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tk.yuntaijiaju.cn

[A26] 类型转换总览
来源：http://re.shtwfgs.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lp.gzmigu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ac.newstarts.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ir.colortex.cn

TS:   Number() String() Boolean() x as number
来源：http://wd.bjjhwx.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://aq.shxzskj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://io.szsharing.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zs.chemitech.net.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yx.bjjhwx.cn

================================================================================
来源：http://go.bookmarksfly.cn

B. 流程控制
来源：http://mx.jctech888.com.cn

================================================================================
来源：http://ce.nszjky.cn

[B01] 条件判断 if / else
来源：http://zv.huixiangedu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://pm.szxytkj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hu.colortex.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bk.lnxyls.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rr.huanxung.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://kp.szxytkj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://at.muxihuayi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ju.bjjhwx.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mm.shxzukj.cn

[B02] 多分支 else if / elif
来源：http://db.shxzskj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ud.lnxyls.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fx.bookmarksfly.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fi.colortex.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vh.chemitech.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sn.szxytkj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bk.yuntaijiaju.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pt.yuntaijiaju.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fc.szxytkj.cn

[B03] switch / match / case
来源：http://vf.lnxyls.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bg.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ve.521024.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mr.shxzskj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bi.lnxyls.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://oh.yuexingan06.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://va.bjjhwx.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qu.nszjky.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bq.colortex.cn

[B04] for 计数循环
来源：http://fa.huixinmuqiang.cn

Py:   for i in range(10): print(i)
来源：http://mc.wgjwhj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cf.gzmigu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bs.gzmigu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sy.asd995.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bn.hahajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gf.hahajie.cn

Ruby: 10.times { |i| puts i }
来源：http://dz.chemitech.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zm.gzmigu.cn

[B05] 遍历数组 / 列表
来源：http://kv.jctech888.com.cn

Py:   for item in arr: print(item)
来源：http://sm.bjjhwx.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tr.szsharing.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://aw.nicolike.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gs.huixiangedu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://bu.huixinmuqiang.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mk.yuntaijiaju.cn

Ruby: arr.each { |item| puts item }
来源：http://py.muxihuayi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gx.shxzskj.cn

[B06] 遍历字典 / 对象
来源：http://py.haigaiapp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://us.colortex.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yz.hnjuh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uf.huixinmuqiang.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://co.panjiajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://if.huixiangedu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ba.colortex.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rn.szsharing.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bu.hnjuh.cn

[B07] while 循环
来源：http://yn.9csxet.cn

Py:   while i < 10: i += 1
来源：http://aj.yuntaijiaju.cn

PHP:  while ($i < 10) { $i++; }
来源：http://dg.shtwfgs.cn

JS:   while (i < 10) { i++; }
来源：http://oz.szsharing.cn

TS:   while (i < 10) { i++; }
来源：http://ou.shtwfgs.cn

Java: while (i < 10) { i++; }
来源：http://an.chemitech.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fq.nicolike.cn

Ruby: while i < 10; i += 1; end
来源：http://ud.huixiangedu.cn

C#:   while (i < 10) { i++; }
来源：http://vu.jianghongdianzi.cn

[B08] do-while（至少执行一次）
来源：http://ff.wgjwhj.cn

Py:   # 无 do-while：用 while True + break
来源：http://en.huixiangedu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://kr.hnjuh.cn

JS:   do { i++; } while (i < 10);
来源：http://ot.bookmarksfly.cn

TS:   do { i++; } while (i < 10);
来源：http://xv.nicolike.cn

Java: do { i++; } while (i < 10);
来源：http://cc.yuexingan06.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://zv.yuntaijiaju.cn

Ruby: begin; i += 1; end while i < 10
来源：http://sl.nicolike.cn

C#:   do { i++; } while (i < 10);
来源：http://nf.huixinmuqiang.cn

[B09] break 与 continue
来源：http://tc.lnxyls.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yk.lnxyls.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kt.gzmigu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tc.yuntaijiaju.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pw.gzmigu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://la.gzmigu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sn.haigaiapp.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fr.hahajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ms.szsharing.cn

[B10] 遍历同时拿索引
来源：http://sy.asd995.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kv.yuntaijiaju.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qw.huixinmuqiang.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://iz.hnjuh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://za.hnjuh.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bz.haigaiapp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lv.bookmarksfly.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jp.yuntaijiaju.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ql.lnxyls.cn

[B11] 生成数字序列 / 区间
来源：http://oc.muxihuayi.cn

Py:   list(range(0, 10, 2))
来源：http://zw.521024.cn

PHP:  range(0, 10, 2);
来源：http://tc.shxzskj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tk.nszjky.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qf.chemitech.net.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ek.newstarts.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ay.shxzskj.cn

Ruby: (0...10).step(2).to_a
来源：http://ap.hnjuh.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cn.bjjhwx.cn

[B12] 跳出多层循环
来源：http://iv.nszjky.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://lr.shxzukj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ep.9csxet.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vf.gzmigu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pl.colortex.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gq.wgjwhj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kd.bookmarksfly.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qp.panjiajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pa.bjjhwx.cn

[B13] 判断是否为数字
来源：http://iy.szxytkj.cn

Py:   isinstance(x, (int, float))
来源：http://wc.jctech888.com.cn

PHP:  is_numeric($x)
来源：http://qd.hnjuh.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wy.yuntaijiaju.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lo.huixiangedu.cn

Java: x instanceof Number
来源：http://sl.colortex.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hs.shxzskj.cn

Ruby: x.is_a?(Numeric)
来源：http://tx.newstarts.cn

C#:   x is int or double or decimal
来源：http://km.jianghongdianzi.cn

[B14] 判断值是否在集合内
来源：http://pu.nicolike.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mu.nszjky.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cj.szsharing.cn

JS:   [1, 2, 3].includes(x)
来源：http://gp.muxihuayi.cn

TS:   [1, 2, 3].includes(x)
来源：http://om.yuexingan06.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://fa.huanxung.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rc.shtwfgs.cn

Ruby: [1, 2, 3].include?(x)
来源：http://eg.jctech888.com.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dg.newstarts.cn

[B15] 布尔运算与取反
来源：http://co.wgjwhj.cn

Py:   a and b or not c
来源：http://lt.shxzukj.cn

PHP:  $a && $b || !$c
来源：http://dq.bookmarksfly.cn

JS:   a && b || !c
来源：http://dj.nszjky.cn

TS:   a && b || !c
来源：http://br.521024.cn

Java: a && b || !c
来源：http://hv.gzmigu.cn

Go:   a && b || !c
来源：http://mh.bjjhwx.cn

Ruby: a && b || !c
来源：http://xz.bookmarksfly.cn

C#:   a && b || !c
来源：http://ic.szsharing.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ri.muxihuayi.cn

Py:   if not data: return
来源：http://xh.lnxyls.cn

PHP:  if (!$data) { return; }
来源：http://ks.521024.cn

JS:   if (!data) return;
来源：http://pi.bookmarksfly.cn

TS:   if (!data) return;
来源：http://oq.yuntaijiaju.cn

Java: if (data == null) return;
来源：http://ia.shxzskj.cn

Go:   if data == nil { return }
来源：http://us.hnjuh.cn

Ruby: return if data.nil?
来源：http://te.shtwfgs.cn

C#:   if (data == null) return;
来源：http://pm.gzmigu.cn

================================================================================
来源：http://ss.szsharing.cn

C. 函数与作用域
来源：http://nl.asd995.cn

================================================================================
来源：http://mp.9csxet.cn

[C01] 定义函数
来源：http://cm.huanxung.cn

Py:   def add(a, b): return a + b
来源：http://hr.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lr.9csxet.cn

JS:   function add(a, b) { return a + b; }
来源：http://yx.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ze.panjiajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fb.chemitech.net.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ie.yuntaijiaju.cn

Ruby: def add(a, b); a + b; end
来源：http://ob.bjjhwx.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lm.newstarts.cn

[C02] 默认参数
来源：http://wh.newstarts.cn

Py:   def greet(name="World"): return name
来源：http://jl.jctech888.com.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cl.bookmarksfly.cn

JS:   function greet(name = "World") { return name; }
来源：http://it.shxzukj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://nk.9csxet.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://tl.huixinmuqiang.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bc.szxytkj.cn

Ruby: def greet(name = "World") = name
来源：http://ak.haigaiapp.cn

C#:   string Greet(string name = "World") => name;
来源：http://ps.newstarts.cn

[C03] 可变参数
来源：http://wq.gzmigu.cn

Py:   def total(*args): return sum(args)
来源：http://pz.panjiajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lj.huanxung.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sn.newstarts.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kd.shxzukj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ql.newstarts.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wa.shxzukj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tz.521024.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qa.huanxung.cn

[C04] 命名参数 / 关键字参数
来源：http://kf.bjjhwx.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cw.chemitech.net.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ht.haigaiapp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yb.huixinmuqiang.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mt.huixiangedu.cn

Java: // 无：用 Builder 模式或 record
来源：http://kv.colortex.cn

Go:   // 无：用配置结构体参数
来源：http://ro.huanxung.cn

Ruby: f(a: 1, b: 2)
来源：http://aa.9csxet.cn

C#:   f(a: 1, b: 2)
来源：http://rg.9csxet.cn

[C05] 返回多个值
来源：http://ep.jianghongdianzi.cn

Py:   return a, b
来源：http://vr.hahajie.cn

PHP:  return [$a, $b];
来源：http://th.shxzskj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yg.szsharing.cn

TS:   return { a, b };
来源：http://sw.huixinmuqiang.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qi.wgjwhj.cn

Go:   return a, b
来源：http://jc.jianghongdianzi.cn

Ruby: return a, b
来源：http://fz.hahajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://we.shxzskj.cn

[C06] 匿名函数 / lambda
来源：http://oe.bjjhwx.cn

Py:   square = lambda x: x * x
来源：http://yj.lnxyls.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://uz.lnxyls.cn

JS:   const square = x => x * x;
来源：http://zh.jctech888.com.cn

TS:   const square = (x: number): number => x * x;
来源：http://qn.hnjuh.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bd.hahajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ic.gzmigu.cn

Ruby: square = ->(x) { x * x }
来源：http://qv.jctech888.com.cn

C#:   Func<int, int> square = x => x * x;
来源：http://jy.panjiajie.cn

[C07] 把函数作为参数传入
来源：http://uc.colortex.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ej.shxzukj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jn.asd995.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ly.szxytkj.cn

TS:   arr.map(String)
来源：http://nz.gzmigu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jl.huanxung.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zr.shxzskj.cn

Ruby: arr.map(&:upcase)
来源：http://kr.shxzukj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://sm.colortex.cn

[C08] 闭包
来源：http://fn.asd995.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kt.huixinmuqiang.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ks.shxzukj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ny.9csxet.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gk.huixiangedu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gi.bookmarksfly.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://eh.asd995.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ut.bookmarksfly.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yy.nicolike.cn

[C09] 递归
来源：http://iv.panjiajie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rt.szsharing.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xj.yuntaijiaju.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vs.nszjky.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qx.bjjhwx.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tn.gzmigu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jc.szxytkj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://no.9csxet.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ks.yuexingan06.cn

[C10] 变量作用域
来源：http://lv.colortex.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ie.gzmigu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rw.nszjky.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://na.hnjuh.cn

TS:   同 JS
来源：http://hh.chemitech.net.cn

Java: 方法内为块级作用域
来源：http://gs.szsharing.cn

Go:   花括号块级作用域
来源：http://gl.521024.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kg.shxzskj.cn

C#:   块级作用域
来源：http://ac.shxzskj.cn

[C11] 模块导入与导出
来源：http://cy.muxihuayi.cn

Py:   from module import func
来源：http://rh.gzmigu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wg.huixiangedu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jz.yuexingan06.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gp.chemitech.net.cn

Java: import java.util.List;
来源：http://un.521024.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sf.asd995.cn

Ruby: require "json"; require_relative "./util"
来源：http://cn.hahajie.cn

C#:   using System.Text;
来源：http://ch.shtwfgs.cn

[C12] 立即执行函数 IIFE
来源：http://ej.gzmigu.cn

Py:   (lambda: print("run"))()
来源：http://ym.wgjwhj.cn


<!-- 参考信息 -->