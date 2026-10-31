代发 wailian999

[A22] 获取字符串长度
来源：http://tq.nicolike.cn

Py:   len(s)
来源：http://mw.huixinmuqiang.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hv.panjiajie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tz.shxzukj.cn

TS:   s.length
来源：http://bp.yuexingan06.cn

Java: s.length()
来源：http://si.bookmarksfly.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lg.shtwfgs.cn

Ruby: s.length
来源：http://on.bookmarksfly.cn

C#:   s.Length
来源：http://fo.huanxung.cn

[A23] 大小写转换
来源：http://nv.shtwfgs.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://tl.asd995.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ko.hahajie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://na.huanxung.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fx.nszjky.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zg.jctech888.com.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bs.bjjhwx.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fo.9csxet.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://fz.panjiajie.cn

[A24] 去除首尾空白
来源：http://kr.asd995.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://um.yuntaijiaju.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sv.nszjky.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ig.yuexingan06.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vj.szxytkj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://sb.szsharing.cn

Go:   strings.TrimSpace(s)
来源：http://oi.9csxet.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kq.nszjky.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://aj.lnxyls.cn

[A25] 字符串比较
来源：http://th.gzmigu.cn

Py:   s1 == s2; s1 != s2
来源：http://wq.huixiangedu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pk.shxzskj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bu.nszjky.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://uk.huanxung.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ty.haigaiapp.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://uz.nszjky.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://er.yuexingan06.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cx.huanxung.cn

[A26] 类型转换总览
来源：http://of.shxzukj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://nf.nicolike.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pu.bjjhwx.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ex.szxytkj.cn

TS:   Number() String() Boolean() x as number
来源：http://ab.yuntaijiaju.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pf.yuntaijiaju.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fs.asd995.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://xi.yuntaijiaju.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yn.colortex.cn

================================================================================
来源：http://du.asd995.cn

B. 流程控制
来源：http://ff.bjjhwx.cn

================================================================================
来源：http://dq.521024.cn

[B01] 条件判断 if / else
来源：http://yf.hahajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://yq.asd995.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cy.hahajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tx.521024.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dr.newstarts.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://iy.hnjuh.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ci.9csxet.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bx.bookmarksfly.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xa.haigaiapp.cn

[B02] 多分支 else if / elif
来源：http://oe.szxytkj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://du.bookmarksfly.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xq.yuexingan06.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vh.huanxung.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dh.muxihuayi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ok.nicolike.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xb.wgjwhj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kz.colortex.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://me.shxzukj.cn

[B03] switch / match / case
来源：http://gr.szsharing.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qc.521024.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kf.yuntaijiaju.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ej.wgjwhj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dt.szsharing.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://we.muxihuayi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qr.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sj.chemitech.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gk.hnjuh.cn

[B04] for 计数循环
来源：http://bm.hnjuh.cn

Py:   for i in range(10): print(i)
来源：http://ex.szxytkj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://iu.huanxung.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qy.shxzukj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sj.szsharing.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://aw.shxzukj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://do.huanxung.cn

Ruby: 10.times { |i| puts i }
来源：http://xo.chemitech.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://oj.szxytkj.cn

[B05] 遍历数组 / 列表
来源：http://zg.521024.cn

Py:   for item in arr: print(item)
来源：http://dg.newstarts.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tt.szxytkj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://nm.bookmarksfly.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fn.huixiangedu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qw.panjiajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gn.shxzskj.cn

Ruby: arr.each { |item| puts item }
来源：http://ti.shtwfgs.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zu.shxzskj.cn

[B06] 遍历字典 / 对象
来源：http://kr.asd995.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://df.asd995.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ah.bjjhwx.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sw.chemitech.net.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cv.bjjhwx.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://px.haigaiapp.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nn.hnjuh.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tp.huixiangedu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zb.nicolike.cn

[B07] while 循环
来源：http://lu.9csxet.cn

Py:   while i < 10: i += 1
来源：http://kb.szxytkj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://pn.newstarts.cn

JS:   while (i < 10) { i++; }
来源：http://ne.jianghongdianzi.cn

TS:   while (i < 10) { i++; }
来源：http://gx.bjjhwx.cn

Java: while (i < 10) { i++; }
来源：http://xh.chemitech.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nt.szsharing.cn

Ruby: while i < 10; i += 1; end
来源：http://fo.bjjhwx.cn

C#:   while (i < 10) { i++; }
来源：http://fr.huixiangedu.cn

[B08] do-while（至少执行一次）
来源：http://yl.asd995.cn

Py:   # 无 do-while：用 while True + break
来源：http://zh.bookmarksfly.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://bh.shxzskj.cn

JS:   do { i++; } while (i < 10);
来源：http://bm.nszjky.cn

TS:   do { i++; } while (i < 10);
来源：http://ip.szxytkj.cn

Java: do { i++; } while (i < 10);
来源：http://bt.bookmarksfly.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://cq.lnxyls.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vv.panjiajie.cn

C#:   do { i++; } while (i < 10);
来源：http://mr.bookmarksfly.cn

[B09] break 与 continue
来源：http://uq.521024.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wr.huixinmuqiang.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bs.wgjwhj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://my.bookmarksfly.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xx.panjiajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lj.gzmigu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qm.huixiangedu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hj.yuexingan06.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ma.jianghongdianzi.cn

[B10] 遍历同时拿索引
来源：http://ry.newstarts.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jc.szsharing.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lr.bookmarksfly.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nt.bjjhwx.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jt.muxihuayi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ae.haigaiapp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cb.bookmarksfly.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kt.panjiajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ua.panjiajie.cn

[B11] 生成数字序列 / 区间
来源：http://gd.521024.cn

Py:   list(range(0, 10, 2))
来源：http://eh.jianghongdianzi.cn

PHP:  range(0, 10, 2);
来源：http://nv.wgjwhj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fm.nicolike.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://no.szsharing.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jl.haigaiapp.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kh.huanxung.cn

Ruby: (0...10).step(2).to_a
来源：http://en.shtwfgs.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xt.shxzukj.cn

[B12] 跳出多层循环
来源：http://wj.colortex.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ja.asd995.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://yw.gzmigu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lk.huixinmuqiang.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gd.bookmarksfly.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sf.yuntaijiaju.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pz.shtwfgs.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qx.haigaiapp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ns.hnjuh.cn

[B13] 判断是否为数字
来源：http://ht.wgjwhj.cn

Py:   isinstance(x, (int, float))
来源：http://cp.newstarts.cn

PHP:  is_numeric($x)
来源：http://kl.lnxyls.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://np.chemitech.net.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nj.jctech888.com.cn

Java: x instanceof Number
来源：http://qk.wgjwhj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nh.nicolike.cn

Ruby: x.is_a?(Numeric)
来源：http://eq.jctech888.com.cn

C#:   x is int or double or decimal
来源：http://jw.shxzskj.cn

[B14] 判断值是否在集合内
来源：http://et.nicolike.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ay.lnxyls.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://we.chemitech.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://or.newstarts.cn

TS:   [1, 2, 3].includes(x)
来源：http://jl.gzmigu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ci.jianghongdianzi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sw.asd995.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qx.shxzskj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://id.hahajie.cn

[B15] 布尔运算与取反
来源：http://nx.newstarts.cn

Py:   a and b or not c
来源：http://qq.jianghongdianzi.cn

PHP:  $a && $b || !$c
来源：http://xj.shxzskj.cn

JS:   a && b || !c
来源：http://sb.huixinmuqiang.cn

TS:   a && b || !c
来源：http://vi.haigaiapp.cn

Java: a && b || !c
来源：http://kb.gzmigu.cn

Go:   a && b || !c
来源：http://fx.521024.cn

Ruby: a && b || !c
来源：http://hm.bookmarksfly.cn

C#:   a && b || !c
来源：http://fz.hahajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ho.yuntaijiaju.cn

Py:   if not data: return
来源：http://tp.hahajie.cn

PHP:  if (!$data) { return; }
来源：http://to.panjiajie.cn

JS:   if (!data) return;
来源：http://uz.gzmigu.cn

TS:   if (!data) return;
来源：http://un.jctech888.com.cn

Java: if (data == null) return;
来源：http://cw.huixiangedu.cn

Go:   if data == nil { return }
来源：http://hh.shxzskj.cn

Ruby: return if data.nil?
来源：http://rq.szxytkj.cn

C#:   if (data == null) return;
来源：http://lg.asd995.cn

================================================================================
来源：http://ev.jctech888.com.cn

C. 函数与作用域
来源：http://mt.9csxet.cn

================================================================================
来源：http://bv.szxytkj.cn

[C01] 定义函数
来源：http://dx.shxzskj.cn

Py:   def add(a, b): return a + b
来源：http://ds.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ik.yuexingan06.cn

JS:   function add(a, b) { return a + b; }
来源：http://be.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kl.yuntaijiaju.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ec.huixinmuqiang.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jl.hnjuh.cn

Ruby: def add(a, b); a + b; end
来源：http://qa.shxzskj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pb.yuexingan06.cn

[C02] 默认参数
来源：http://fj.yuexingan06.cn

Py:   def greet(name="World"): return name
来源：http://jf.newstarts.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ar.huanxung.cn

JS:   function greet(name = "World") { return name; }
来源：http://bl.shtwfgs.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lr.szxytkj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ea.huixiangedu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xg.asd995.cn

Ruby: def greet(name = "World") = name
来源：http://zg.huanxung.cn

C#:   string Greet(string name = "World") => name;
来源：http://bm.shxzskj.cn

[C03] 可变参数
来源：http://jy.nicolike.cn

Py:   def total(*args): return sum(args)
来源：http://xr.szxytkj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yy.huixiangedu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ic.hnjuh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kc.nicolike.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zf.shtwfgs.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://od.lnxyls.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fm.wgjwhj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wc.szxytkj.cn

[C04] 命名参数 / 关键字参数
来源：http://ws.bjjhwx.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jy.jianghongdianzi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ol.shtwfgs.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ui.bjjhwx.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yo.521024.cn

Java: // 无：用 Builder 模式或 record
来源：http://dr.muxihuayi.cn

Go:   // 无：用配置结构体参数
来源：http://ps.nszjky.cn

Ruby: f(a: 1, b: 2)
来源：http://mc.szxytkj.cn

C#:   f(a: 1, b: 2)
来源：http://rq.gzmigu.cn

[C05] 返回多个值
来源：http://sh.nicolike.cn

Py:   return a, b
来源：http://xv.panjiajie.cn

PHP:  return [$a, $b];
来源：http://iq.gzmigu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ig.huixiangedu.cn

TS:   return { a, b };
来源：http://hq.huanxung.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ap.asd995.cn

Go:   return a, b
来源：http://wd.haigaiapp.cn

Ruby: return a, b
来源：http://ko.szsharing.cn

C#:   return (a, b);              // ValueTuple
来源：http://dz.lnxyls.cn

[C06] 匿名函数 / lambda
来源：http://sg.9csxet.cn

Py:   square = lambda x: x * x
来源：http://co.asd995.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://nd.bookmarksfly.cn

JS:   const square = x => x * x;
来源：http://bn.asd995.cn

TS:   const square = (x: number): number => x * x;
来源：http://xk.chemitech.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jg.nicolike.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qs.9csxet.cn

Ruby: square = ->(x) { x * x }
来源：http://hz.hahajie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://te.haigaiapp.cn

[C07] 把函数作为参数传入
来源：http://qk.9csxet.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yc.nszjky.cn

PHP:  array_map("strtoupper", $arr);
来源：http://rt.yuntaijiaju.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tj.bookmarksfly.cn

TS:   arr.map(String)
来源：http://ci.nszjky.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qc.9csxet.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://es.panjiajie.cn

Ruby: arr.map(&:upcase)
来源：http://dt.shtwfgs.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://up.jianghongdianzi.cn

[C08] 闭包
来源：http://yc.nszjky.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wu.panjiajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xm.szsharing.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zq.newstarts.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://st.shxzskj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gc.nicolike.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sv.nszjky.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vh.gzmigu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ui.jctech888.com.cn

[C09] 递归
来源：http://if.hnjuh.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yt.shtwfgs.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://em.9csxet.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://df.hahajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ge.521024.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uq.yuexingan06.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ax.wgjwhj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mu.muxihuayi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jj.huixiangedu.cn

[C10] 变量作用域
来源：http://fm.shxzskj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://br.huanxung.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gz.yuexingan06.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dj.huixinmuqiang.cn

TS:   同 JS
来源：http://or.szsharing.cn

Java: 方法内为块级作用域
来源：http://ty.huanxung.cn

Go:   花括号块级作用域
来源：http://uz.huixiangedu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qn.huixinmuqiang.cn

C#:   块级作用域
来源：http://bw.szsharing.cn

[C11] 模块导入与导出
来源：http://ih.asd995.cn

Py:   from module import func
来源：http://iy.lnxyls.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://uc.521024.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://sc.lnxyls.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ma.lnxyls.cn

Java: import java.util.List;
来源：http://po.521024.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xa.shxzskj.cn

Ruby: require "json"; require_relative "./util"
来源：http://pi.huanxung.cn

C#:   using System.Text;
来源：http://wt.gzmigu.cn

[C12] 立即执行函数 IIFE
来源：http://ab.jianghongdianzi.cn

Py:   (lambda: print("run"))()
来源：http://ya.szxytkj.cn

PHP:  (function () { echo "run"; })();
来源：http://hp.muxihuayi.cn

JS:   (() => { console.log("run"); })();
来源：http://vv.bjjhwx.cn

TS:   (() => { console.log("run"); })();
来源：http://fm.9csxet.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nf.muxihuayi.cn


<!-- 参考信息 -->