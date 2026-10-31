代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://nv.chemitech.net.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mf.hnjuh.cn

Ruby: format("%.2f", 3.14159)
来源：http://gf.asd995.cn

C#:   3.14159.ToString("F2")
来源：http://ns.bookmarksfly.cn

[A22] 获取字符串长度
来源：http://xj.jctech888.com.cn

Py:   len(s)
来源：http://dl.panjiajie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jo.shxzskj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pw.shxzskj.cn

TS:   s.length
来源：http://lo.shtwfgs.cn

Java: s.length()
来源：http://jz.hahajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xf.gzmigu.cn

Ruby: s.length
来源：http://ds.hnjuh.cn

C#:   s.Length
来源：http://qs.shtwfgs.cn

[A23] 大小写转换
来源：http://hh.hahajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ti.lnxyls.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ns.panjiajie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ex.jctech888.com.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://br.shxzukj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vy.jianghongdianzi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ba.gzmigu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gi.521024.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://jo.yuexingan06.cn

[A24] 去除首尾空白
来源：http://zo.szxytkj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ud.panjiajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wl.jctech888.com.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mx.chemitech.net.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://do.huixinmuqiang.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qs.nszjky.cn

Go:   strings.TrimSpace(s)
来源：http://iw.chemitech.net.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tg.asd995.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gn.yuntaijiaju.cn

[A25] 字符串比较
来源：http://ft.newstarts.cn

Py:   s1 == s2; s1 != s2
来源：http://pt.haigaiapp.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ih.chemitech.net.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dp.panjiajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://eq.chemitech.net.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ca.nszjky.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ox.jctech888.com.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://mr.newstarts.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pw.chemitech.net.cn

[A26] 类型转换总览
来源：http://zi.gzmigu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://oz.panjiajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yg.chemitech.net.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://el.chemitech.net.cn

TS:   Number() String() Boolean() x as number
来源：http://hp.szxytkj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wx.yuexingan06.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pt.haigaiapp.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://nv.muxihuayi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hr.521024.cn

================================================================================
来源：http://cn.lnxyls.cn

B. 流程控制
来源：http://jz.szxytkj.cn

================================================================================
来源：http://xi.szsharing.cn

[B01] 条件判断 if / else
来源：http://zt.jctech888.com.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://tu.9csxet.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lq.hahajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fb.jianghongdianzi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hq.shxzukj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://wc.hnjuh.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://il.yuntaijiaju.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ja.szsharing.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mv.bookmarksfly.cn

[B02] 多分支 else if / elif
来源：http://na.jctech888.com.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ai.yuexingan06.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qj.bjjhwx.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://or.shxzukj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fo.lnxyls.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://em.panjiajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://of.bookmarksfly.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://di.panjiajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pi.521024.cn

[B03] switch / match / case
来源：http://st.panjiajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jz.lnxyls.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sd.hnjuh.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cf.huixiangedu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://va.newstarts.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wm.asd995.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vv.9csxet.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wy.521024.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xo.chemitech.net.cn

[B04] for 计数循环
来源：http://lh.szsharing.cn

Py:   for i in range(10): print(i)
来源：http://wx.huixinmuqiang.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cz.huanxung.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tp.hahajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yk.shtwfgs.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mn.muxihuayi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gl.jianghongdianzi.cn

Ruby: 10.times { |i| puts i }
来源：http://uk.nicolike.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hu.bjjhwx.cn

[B05] 遍历数组 / 列表
来源：http://pj.panjiajie.cn

Py:   for item in arr: print(item)
来源：http://mt.yuntaijiaju.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hq.lnxyls.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dh.shxzskj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mz.hahajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vx.muxihuayi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://se.hahajie.cn

Ruby: arr.each { |item| puts item }
来源：http://tp.nszjky.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jc.gzmigu.cn

[B06] 遍历字典 / 对象
来源：http://ah.szsharing.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xj.yuexingan06.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tt.nicolike.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nv.chemitech.net.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pg.jctech888.com.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rj.huixiangedu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qv.muxihuayi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ti.huanxung.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://te.shxzukj.cn

[B07] while 循环
来源：http://fp.9csxet.cn

Py:   while i < 10: i += 1
来源：http://ia.haigaiapp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qb.huixiangedu.cn

JS:   while (i < 10) { i++; }
来源：http://km.521024.cn

TS:   while (i < 10) { i++; }
来源：http://vd.bjjhwx.cn

Java: while (i < 10) { i++; }
来源：http://ox.nszjky.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zj.yuexingan06.cn

Ruby: while i < 10; i += 1; end
来源：http://kx.szsharing.cn

C#:   while (i < 10) { i++; }
来源：http://zk.yuexingan06.cn

[B08] do-while（至少执行一次）
来源：http://vy.shxzskj.cn

Py:   # 无 do-while：用 while True + break
来源：http://vl.muxihuayi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://du.asd995.cn

JS:   do { i++; } while (i < 10);
来源：http://fr.lnxyls.cn

TS:   do { i++; } while (i < 10);
来源：http://pz.lnxyls.cn

Java: do { i++; } while (i < 10);
来源：http://td.yuntaijiaju.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://tf.bjjhwx.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pz.bookmarksfly.cn

C#:   do { i++; } while (i < 10);
来源：http://ut.wgjwhj.cn

[B09] break 与 continue
来源：http://qm.szsharing.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sv.521024.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fo.shtwfgs.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qw.szxytkj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eu.chemitech.net.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lu.asd995.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zi.jianghongdianzi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://uw.bookmarksfly.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gw.newstarts.cn

[B10] 遍历同时拿索引
来源：http://rh.jianghongdianzi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tr.yuexingan06.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rt.muxihuayi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pu.hahajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gy.muxihuayi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xj.hnjuh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lb.huixinmuqiang.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ie.521024.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rx.muxihuayi.cn

[B11] 生成数字序列 / 区间
来源：http://us.szxytkj.cn

Py:   list(range(0, 10, 2))
来源：http://kp.shxzukj.cn

PHP:  range(0, 10, 2);
来源：http://ok.lnxyls.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jx.shtwfgs.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nl.shtwfgs.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pv.yuexingan06.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://or.hahajie.cn

Ruby: (0...10).step(2).to_a
来源：http://yh.9csxet.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://eq.shtwfgs.cn

[B12] 跳出多层循环
来源：http://km.asd995.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://cg.shtwfgs.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://pc.huixiangedu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yr.jctech888.com.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dm.521024.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yd.panjiajie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xg.huanxung.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lg.bookmarksfly.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kq.yuntaijiaju.cn

[B13] 判断是否为数字
来源：http://cf.9csxet.cn

Py:   isinstance(x, (int, float))
来源：http://lp.nicolike.cn

PHP:  is_numeric($x)
来源：http://oq.shtwfgs.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ln.huanxung.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oa.szsharing.cn

Java: x instanceof Number
来源：http://sg.szsharing.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yt.colortex.cn

Ruby: x.is_a?(Numeric)
来源：http://qc.haigaiapp.cn

C#:   x is int or double or decimal
来源：http://lk.huanxung.cn

[B14] 判断值是否在集合内
来源：http://kv.shtwfgs.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ko.panjiajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dp.yuntaijiaju.cn

JS:   [1, 2, 3].includes(x)
来源：http://gf.yuexingan06.cn

TS:   [1, 2, 3].includes(x)
来源：http://hb.nicolike.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rp.9csxet.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qp.wgjwhj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://tc.hnjuh.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hj.bookmarksfly.cn

[B15] 布尔运算与取反
来源：http://fa.szsharing.cn

Py:   a and b or not c
来源：http://el.nszjky.cn

PHP:  $a && $b || !$c
来源：http://jy.gzmigu.cn

JS:   a && b || !c
来源：http://cg.jctech888.com.cn

TS:   a && b || !c
来源：http://xr.huixinmuqiang.cn

Java: a && b || !c
来源：http://dc.9csxet.cn

Go:   a && b || !c
来源：http://tm.haigaiapp.cn

Ruby: a && b || !c
来源：http://iy.nicolike.cn

C#:   a && b || !c
来源：http://fb.chemitech.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fi.jctech888.com.cn

Py:   if not data: return
来源：http://zw.haigaiapp.cn

PHP:  if (!$data) { return; }
来源：http://et.szxytkj.cn

JS:   if (!data) return;
来源：http://ka.bjjhwx.cn

TS:   if (!data) return;
来源：http://lu.wgjwhj.cn

Java: if (data == null) return;
来源：http://kb.wgjwhj.cn

Go:   if data == nil { return }
来源：http://ln.521024.cn

Ruby: return if data.nil?
来源：http://bl.muxihuayi.cn

C#:   if (data == null) return;
来源：http://jv.chemitech.net.cn

================================================================================
来源：http://hw.szsharing.cn

C. 函数与作用域
来源：http://bu.9csxet.cn

================================================================================
来源：http://oy.bjjhwx.cn

[C01] 定义函数
来源：http://hp.shxzskj.cn

Py:   def add(a, b): return a + b
来源：http://ww.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yt.nicolike.cn

JS:   function add(a, b) { return a + b; }
来源：http://dl.panjiajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://al.szxytkj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://yy.gzmigu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://yr.huanxung.cn

Ruby: def add(a, b); a + b; end
来源：http://mz.yuntaijiaju.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://so.wgjwhj.cn

[C02] 默认参数
来源：http://kd.jctech888.com.cn

Py:   def greet(name="World"): return name
来源：http://gy.nszjky.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://st.huanxung.cn

JS:   function greet(name = "World") { return name; }
来源：http://yo.chemitech.net.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xg.gzmigu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qf.jianghongdianzi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://oa.yuntaijiaju.cn

Ruby: def greet(name = "World") = name
来源：http://ap.wgjwhj.cn

C#:   string Greet(string name = "World") => name;
来源：http://nu.shxzukj.cn

[C03] 可变参数
来源：http://yt.nicolike.cn

Py:   def total(*args): return sum(args)
来源：http://ze.haigaiapp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fn.jctech888.com.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fv.bjjhwx.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yf.huixinmuqiang.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://td.jianghongdianzi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ny.haigaiapp.cn

Ruby: def total(*nums); nums.sum; end
来源：http://dc.521024.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mm.521024.cn

[C04] 命名参数 / 关键字参数
来源：http://vw.huixinmuqiang.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zm.yuntaijiaju.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bt.chemitech.net.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://km.asd995.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gm.jctech888.com.cn

Java: // 无：用 Builder 模式或 record
来源：http://pq.muxihuayi.cn

Go:   // 无：用配置结构体参数
来源：http://go.huixinmuqiang.cn

Ruby: f(a: 1, b: 2)
来源：http://dy.hnjuh.cn

C#:   f(a: 1, b: 2)
来源：http://sx.nszjky.cn

[C05] 返回多个值
来源：http://ug.asd995.cn

Py:   return a, b
来源：http://cx.colortex.cn

PHP:  return [$a, $b];
来源：http://hr.huixiangedu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fu.nicolike.cn

TS:   return { a, b };
来源：http://hs.lnxyls.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wv.szxytkj.cn

Go:   return a, b
来源：http://em.szsharing.cn

Ruby: return a, b
来源：http://zg.yuntaijiaju.cn

C#:   return (a, b);              // ValueTuple
来源：http://le.haigaiapp.cn

[C06] 匿名函数 / lambda
来源：http://gw.szxytkj.cn

Py:   square = lambda x: x * x
来源：http://ll.muxihuayi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://hp.huixiangedu.cn

JS:   const square = x => x * x;
来源：http://fw.nicolike.cn

TS:   const square = (x: number): number => x * x;
来源：http://ge.newstarts.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rv.szsharing.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ds.jctech888.com.cn

Ruby: square = ->(x) { x * x }
来源：http://vz.szsharing.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bu.jctech888.com.cn

[C07] 把函数作为参数传入
来源：http://px.newstarts.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ql.hnjuh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://du.hahajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://la.szsharing.cn

TS:   arr.map(String)
来源：http://zs.yuntaijiaju.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xh.haigaiapp.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fk.bjjhwx.cn

Ruby: arr.map(&:upcase)
来源：http://dc.shtwfgs.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wy.huanxung.cn

[C08] 闭包
来源：http://rl.panjiajie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jr.newstarts.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://in.haigaiapp.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wi.huixinmuqiang.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dh.yuntaijiaju.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hh.521024.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lv.jctech888.com.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xc.huixiangedu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vz.jianghongdianzi.cn

[C09] 递归
来源：http://db.shxzukj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zu.panjiajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gx.lnxyls.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ol.hnjuh.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bu.panjiajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pl.huixinmuqiang.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://am.hahajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jm.hnjuh.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bk.yuntaijiaju.cn

[C10] 变量作用域
来源：http://zd.shxzukj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vc.bookmarksfly.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ol.shtwfgs.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tt.chemitech.net.cn

TS:   同 JS
来源：http://bi.huixinmuqiang.cn

Java: 方法内为块级作用域
来源：http://pv.szsharing.cn

Go:   花括号块级作用域
来源：http://ud.wgjwhj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ah.asd995.cn

C#:   块级作用域
来源：http://qb.nicolike.cn

[C11] 模块导入与导出
来源：http://no.chemitech.net.cn

Py:   from module import func
来源：http://fe.shxzskj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://jn.jctech888.com.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ge.hahajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dh.521024.cn

Java: import java.util.List;
来源：http://ug.chemitech.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zo.hahajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://pp.haigaiapp.cn

C#:   using System.Text;
来源：http://mh.huixiangedu.cn

[C12] 立即执行函数 IIFE
来源：http://qk.shtwfgs.cn

Py:   (lambda: print("run"))()
来源：http://xp.nicolike.cn


<!-- 参考信息 -->