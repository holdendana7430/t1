代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://km.nszjky.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ii.nszjky.cn

Ruby: format("%.2f", 3.14159)
来源：http://tp.jctech888.com.cn

C#:   3.14159.ToString("F2")
来源：http://ih.huixiangedu.cn

[A22] 获取字符串长度
来源：http://jx.lnxyls.cn

Py:   len(s)
来源：http://oe.haigaiapp.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nk.nszjky.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rc.huixinmuqiang.cn

TS:   s.length
来源：http://cd.jctech888.com.cn

Java: s.length()
来源：http://oc.shxzskj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://eu.muxihuayi.cn

Ruby: s.length
来源：http://cd.szxytkj.cn

C#:   s.Length
来源：http://or.huixinmuqiang.cn

[A23] 大小写转换
来源：http://vy.chemitech.net.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://du.huanxung.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xe.gzmigu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://eq.huixiangedu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://se.nszjky.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ek.panjiajie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ns.asd995.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ze.huixiangedu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ir.szxytkj.cn

[A24] 去除首尾空白
来源：http://rd.9csxet.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rq.nicolike.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gi.bookmarksfly.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ja.haigaiapp.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ir.nicolike.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bf.shtwfgs.cn

Go:   strings.TrimSpace(s)
来源：http://yg.shxzskj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wb.chemitech.net.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fd.bjjhwx.cn

[A25] 字符串比较
来源：http://fp.nszjky.cn

Py:   s1 == s2; s1 != s2
来源：http://yz.chemitech.net.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qx.huixiangedu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pe.wgjwhj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wu.szxytkj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yu.9csxet.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://my.szsharing.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://wx.newstarts.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ey.szsharing.cn

[A26] 类型转换总览
来源：http://qv.hahajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pz.wgjwhj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qf.chemitech.net.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wb.9csxet.cn

TS:   Number() String() Boolean() x as number
来源：http://yq.asd995.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mt.bookmarksfly.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ef.colortex.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vq.9csxet.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xb.521024.cn

================================================================================
来源：http://hx.shtwfgs.cn

B. 流程控制
来源：http://du.szxytkj.cn

================================================================================
来源：http://fs.shtwfgs.cn

[B01] 条件判断 if / else
来源：http://sh.9csxet.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://av.nicolike.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lp.haigaiapp.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mh.colortex.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jf.haigaiapp.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://cp.asd995.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ho.asd995.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wu.hnjuh.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zc.yuntaijiaju.cn

[B02] 多分支 else if / elif
来源：http://pn.muxihuayi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ev.hnjuh.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kq.huixinmuqiang.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vs.colortex.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nd.huixinmuqiang.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uo.chemitech.net.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zh.huanxung.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://oo.yuexingan06.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://be.bjjhwx.cn

[B03] switch / match / case
来源：http://kw.szxytkj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jb.wgjwhj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mi.shtwfgs.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ic.jianghongdianzi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bq.yuexingan06.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rt.nszjky.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mj.huixinmuqiang.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://aq.yuexingan06.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vx.newstarts.cn

[B04] for 计数循环
来源：http://qn.jctech888.com.cn

Py:   for i in range(10): print(i)
来源：http://gt.jianghongdianzi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zb.yuntaijiaju.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nr.szxytkj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yl.shtwfgs.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vm.yuexingan06.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wj.hnjuh.cn

Ruby: 10.times { |i| puts i }
来源：http://ab.jianghongdianzi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dv.huixiangedu.cn

[B05] 遍历数组 / 列表
来源：http://rj.wgjwhj.cn

Py:   for item in arr: print(item)
来源：http://ke.haigaiapp.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://iu.shxzukj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://eu.haigaiapp.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ba.jctech888.com.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fd.huixinmuqiang.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gs.huixiangedu.cn

Ruby: arr.each { |item| puts item }
来源：http://el.szxytkj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ek.szxytkj.cn

[B06] 遍历字典 / 对象
来源：http://yx.wgjwhj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://kv.bookmarksfly.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ke.hahajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ho.asd995.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iq.haigaiapp.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tv.jianghongdianzi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wr.jianghongdianzi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ur.bjjhwx.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wb.jianghongdianzi.cn

[B07] while 循环
来源：http://ss.jianghongdianzi.cn

Py:   while i < 10: i += 1
来源：http://tn.haigaiapp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vf.lnxyls.cn

JS:   while (i < 10) { i++; }
来源：http://dr.asd995.cn

TS:   while (i < 10) { i++; }
来源：http://ho.nicolike.cn

Java: while (i < 10) { i++; }
来源：http://fh.chemitech.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bz.panjiajie.cn

Ruby: while i < 10; i += 1; end
来源：http://da.yuntaijiaju.cn

C#:   while (i < 10) { i++; }
来源：http://mo.muxihuayi.cn

[B08] do-while（至少执行一次）
来源：http://cc.shxzukj.cn

Py:   # 无 do-while：用 while True + break
来源：http://rs.shxzskj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ba.9csxet.cn

JS:   do { i++; } while (i < 10);
来源：http://em.newstarts.cn

TS:   do { i++; } while (i < 10);
来源：http://kz.haigaiapp.cn

Java: do { i++; } while (i < 10);
来源：http://gy.newstarts.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ix.lnxyls.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ku.huixiangedu.cn

C#:   do { i++; } while (i < 10);
来源：http://gc.9csxet.cn

[B09] break 与 continue
来源：http://ah.521024.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sf.newstarts.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rr.lnxyls.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lu.shxzskj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pk.szsharing.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ae.huixiangedu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bw.9csxet.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ij.yuexingan06.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mv.bookmarksfly.cn

[B10] 遍历同时拿索引
来源：http://xm.asd995.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pn.bookmarksfly.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hd.jianghongdianzi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sz.colortex.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nj.nicolike.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fu.521024.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qp.szxytkj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://in.bjjhwx.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bd.haigaiapp.cn

[B11] 生成数字序列 / 区间
来源：http://xt.newstarts.cn

Py:   list(range(0, 10, 2))
来源：http://uz.hnjuh.cn

PHP:  range(0, 10, 2);
来源：http://qa.huixinmuqiang.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wh.huixinmuqiang.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mw.szsharing.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://oe.szsharing.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://of.newstarts.cn

Ruby: (0...10).step(2).to_a
来源：http://ra.asd995.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ow.nicolike.cn

[B12] 跳出多层循环
来源：http://ea.shtwfgs.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://rd.nszjky.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fz.wgjwhj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://er.bookmarksfly.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ra.9csxet.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mz.szxytkj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vk.newstarts.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gg.shxzukj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://iq.colortex.cn

[B13] 判断是否为数字
来源：http://bd.521024.cn

Py:   isinstance(x, (int, float))
来源：http://hd.wgjwhj.cn

PHP:  is_numeric($x)
来源：http://kz.colortex.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ce.gzmigu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tc.shxzskj.cn

Java: x instanceof Number
来源：http://dl.yuntaijiaju.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yq.521024.cn

Ruby: x.is_a?(Numeric)
来源：http://js.huanxung.cn

C#:   x is int or double or decimal
来源：http://iz.asd995.cn

[B14] 判断值是否在集合内
来源：http://ob.chemitech.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ul.9csxet.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://eb.haigaiapp.cn

JS:   [1, 2, 3].includes(x)
来源：http://fb.shxzskj.cn

TS:   [1, 2, 3].includes(x)
来源：http://qf.jctech888.com.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://yy.hahajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zf.nicolike.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mc.szxytkj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zf.nicolike.cn

[B15] 布尔运算与取反
来源：http://ba.yuexingan06.cn

Py:   a and b or not c
来源：http://vr.jctech888.com.cn

PHP:  $a && $b || !$c
来源：http://ml.shtwfgs.cn

JS:   a && b || !c
来源：http://en.jianghongdianzi.cn

TS:   a && b || !c
来源：http://ms.chemitech.net.cn

Java: a && b || !c
来源：http://bq.lnxyls.cn

Go:   a && b || !c
来源：http://pj.shxzukj.cn

Ruby: a && b || !c
来源：http://zp.wgjwhj.cn

C#:   a && b || !c
来源：http://mk.nicolike.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ur.hnjuh.cn

Py:   if not data: return
来源：http://rz.szxytkj.cn

PHP:  if (!$data) { return; }
来源：http://cr.nszjky.cn

JS:   if (!data) return;
来源：http://uj.nszjky.cn

TS:   if (!data) return;
来源：http://nh.521024.cn

Java: if (data == null) return;
来源：http://ch.huixinmuqiang.cn

Go:   if data == nil { return }
来源：http://kj.shxzskj.cn

Ruby: return if data.nil?
来源：http://qt.nicolike.cn

C#:   if (data == null) return;
来源：http://mw.521024.cn

================================================================================
来源：http://qp.nszjky.cn

C. 函数与作用域
来源：http://yd.szsharing.cn

================================================================================
来源：http://zq.wgjwhj.cn

[C01] 定义函数
来源：http://qn.nicolike.cn

Py:   def add(a, b): return a + b
来源：http://qk.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jt.bjjhwx.cn

JS:   function add(a, b) { return a + b; }
来源：http://jv.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xq.panjiajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hp.jctech888.com.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ue.wgjwhj.cn

Ruby: def add(a, b); a + b; end
来源：http://qf.bookmarksfly.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vd.9csxet.cn

[C02] 默认参数
来源：http://vz.huanxung.cn

Py:   def greet(name="World"): return name
来源：http://qk.shxzskj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://re.huanxung.cn

JS:   function greet(name = "World") { return name; }
来源：http://ty.lnxyls.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://sz.yuntaijiaju.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://xe.colortex.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lm.newstarts.cn

Ruby: def greet(name = "World") = name
来源：http://ny.521024.cn

C#:   string Greet(string name = "World") => name;
来源：http://oh.shxzukj.cn

[C03] 可变参数
来源：http://bd.yuntaijiaju.cn

Py:   def total(*args): return sum(args)
来源：http://fi.bjjhwx.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rt.shxzukj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jy.9csxet.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://iv.chemitech.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fd.bjjhwx.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zy.huixinmuqiang.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rt.huixiangedu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ms.wgjwhj.cn

[C04] 命名参数 / 关键字参数
来源：http://yj.bookmarksfly.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fh.nszjky.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sf.shtwfgs.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sw.szsharing.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zq.chemitech.net.cn

Java: // 无：用 Builder 模式或 record
来源：http://ei.9csxet.cn

Go:   // 无：用配置结构体参数
来源：http://ja.muxihuayi.cn

Ruby: f(a: 1, b: 2)
来源：http://mx.nszjky.cn

C#:   f(a: 1, b: 2)
来源：http://eu.yuntaijiaju.cn

[C05] 返回多个值
来源：http://np.bjjhwx.cn

Py:   return a, b
来源：http://tb.9csxet.cn

PHP:  return [$a, $b];
来源：http://gd.muxihuayi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ti.chemitech.net.cn

TS:   return { a, b };
来源：http://lg.jctech888.com.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jw.newstarts.cn

Go:   return a, b
来源：http://gm.huixiangedu.cn

Ruby: return a, b
来源：http://yr.colortex.cn

C#:   return (a, b);              // ValueTuple
来源：http://cm.yuexingan06.cn

[C06] 匿名函数 / lambda
来源：http://lj.huanxung.cn

Py:   square = lambda x: x * x
来源：http://lm.huixinmuqiang.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zl.muxihuayi.cn

JS:   const square = x => x * x;
来源：http://wi.asd995.cn

TS:   const square = (x: number): number => x * x;
来源：http://gz.szsharing.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yy.gzmigu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hi.bookmarksfly.cn

Ruby: square = ->(x) { x * x }
来源：http://xd.asd995.cn

C#:   Func<int, int> square = x => x * x;
来源：http://te.nicolike.cn

[C07] 把函数作为参数传入
来源：http://ha.muxihuayi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pd.huanxung.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vp.chemitech.net.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qq.nszjky.cn

TS:   arr.map(String)
来源：http://ei.nicolike.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vq.lnxyls.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ef.huixinmuqiang.cn

Ruby: arr.map(&:upcase)
来源：http://ry.wgjwhj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://rd.szsharing.cn

[C08] 闭包
来源：http://ph.colortex.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://up.9csxet.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dh.panjiajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rk.haigaiapp.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gj.yuexingan06.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zs.asd995.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rg.huixinmuqiang.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hc.shtwfgs.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gv.asd995.cn

[C09] 递归
来源：http://cd.shtwfgs.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pm.panjiajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fr.shxzskj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bj.panjiajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ed.hahajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wn.szsharing.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gi.szsharing.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://oz.yuexingan06.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fp.521024.cn

[C10] 变量作用域
来源：http://sa.jianghongdianzi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sd.shxzukj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ta.hahajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jx.shtwfgs.cn

TS:   同 JS
来源：http://db.newstarts.cn

Java: 方法内为块级作用域
来源：http://of.jctech888.com.cn

Go:   花括号块级作用域
来源：http://uh.9csxet.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vj.huanxung.cn

C#:   块级作用域
来源：http://ah.huixinmuqiang.cn

[C11] 模块导入与导出
来源：http://ro.shxzskj.cn

Py:   from module import func
来源：http://yk.nszjky.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://lg.panjiajie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://cu.szsharing.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://oh.chemitech.net.cn

Java: import java.util.List;
来源：http://fu.chemitech.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gx.shtwfgs.cn

Ruby: require "json"; require_relative "./util"
来源：http://jh.panjiajie.cn

C#:   using System.Text;
来源：http://jc.huixiangedu.cn

[C12] 立即执行函数 IIFE
来源：http://ca.newstarts.cn

Py:   (lambda: print("run"))()
来源：http://qg.nszjky.cn


<!-- 参考信息 -->