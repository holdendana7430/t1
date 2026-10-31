代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://da.colortex.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qt.chemitech.net.cn

JS:   (3.14159).toFixed(2)
来源：http://od.hahajie.cn

TS:   (3.14159).toFixed(2)
来源：http://ra.haigaiapp.cn

Java: String.format("%.2f", 3.14159)
来源：http://xq.yuexingan06.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://av.huixinmuqiang.cn

Ruby: format("%.2f", 3.14159)
来源：http://bs.bjjhwx.cn

C#:   3.14159.ToString("F2")
来源：http://xn.9csxet.cn

[A22] 获取字符串长度
来源：http://bu.hahajie.cn

Py:   len(s)
来源：http://ck.jianghongdianzi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pp.yuexingan06.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wt.nszjky.cn

TS:   s.length
来源：http://sj.bjjhwx.cn

Java: s.length()
来源：http://ie.9csxet.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xw.shtwfgs.cn

Ruby: s.length
来源：http://gu.newstarts.cn

C#:   s.Length
来源：http://xe.hnjuh.cn

[A23] 大小写转换
来源：http://nz.shxzskj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://cz.muxihuayi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://eb.gzmigu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fl.bjjhwx.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wr.asd995.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pr.huanxung.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dp.jianghongdianzi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jj.jctech888.com.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://iq.lnxyls.cn

[A24] 去除首尾空白
来源：http://jm.nicolike.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jl.hnjuh.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bl.jianghongdianzi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ce.yuexingan06.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uo.yuexingan06.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://im.huixinmuqiang.cn

Go:   strings.TrimSpace(s)
来源：http://vy.newstarts.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://av.shtwfgs.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://es.wgjwhj.cn

[A25] 字符串比较
来源：http://hi.lnxyls.cn

Py:   s1 == s2; s1 != s2
来源：http://la.haigaiapp.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kf.bjjhwx.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yt.9csxet.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xi.muxihuayi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rt.chemitech.net.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://al.hahajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://pg.asd995.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dc.jianghongdianzi.cn

[A26] 类型转换总览
来源：http://ie.jctech888.com.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wt.521024.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rk.muxihuayi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nv.huixiangedu.cn

TS:   Number() String() Boolean() x as number
来源：http://ls.nszjky.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nu.nszjky.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ng.gzmigu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://aq.newstarts.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gf.newstarts.cn

================================================================================
来源：http://fv.nszjky.cn

B. 流程控制
来源：http://sr.gzmigu.cn

================================================================================
来源：http://ae.wgjwhj.cn

[B01] 条件判断 if / else
来源：http://bu.chemitech.net.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vh.szsharing.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xj.hahajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://uk.lnxyls.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lh.yuexingan06.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ls.gzmigu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nu.shtwfgs.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://le.panjiajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gw.asd995.cn

[B02] 多分支 else if / elif
来源：http://ty.wgjwhj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zm.huanxung.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yx.lnxyls.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gq.bjjhwx.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mf.huixinmuqiang.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cx.panjiajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vy.gzmigu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kz.huixinmuqiang.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://px.521024.cn

[B03] switch / match / case
来源：http://mr.jianghongdianzi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sy.yuexingan06.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://id.haigaiapp.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qz.jctech888.com.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ee.muxihuayi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qf.jctech888.com.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ko.bookmarksfly.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zq.szxytkj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vz.yuntaijiaju.cn

[B04] for 计数循环
来源：http://py.gzmigu.cn

Py:   for i in range(10): print(i)
来源：http://wo.bjjhwx.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fk.yuexingan06.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gp.gzmigu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tt.521024.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://iy.nszjky.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ar.asd995.cn

Ruby: 10.times { |i| puts i }
来源：http://io.asd995.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hy.huanxung.cn

[B05] 遍历数组 / 列表
来源：http://cz.muxihuayi.cn

Py:   for item in arr: print(item)
来源：http://ri.panjiajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ti.wgjwhj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hp.hnjuh.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yg.szxytkj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lr.bjjhwx.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://li.hnjuh.cn

Ruby: arr.each { |item| puts item }
来源：http://bj.yuntaijiaju.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wj.nszjky.cn

[B06] 遍历字典 / 对象
来源：http://ex.jianghongdianzi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://wu.shtwfgs.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qd.yuntaijiaju.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cm.521024.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ez.huixiangedu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ni.colortex.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bf.yuexingan06.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://uc.bjjhwx.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rc.shxzskj.cn

[B07] while 循环
来源：http://nj.huixinmuqiang.cn

Py:   while i < 10: i += 1
来源：http://ee.bjjhwx.cn

PHP:  while ($i < 10) { $i++; }
来源：http://nu.shxzskj.cn

JS:   while (i < 10) { i++; }
来源：http://qo.9csxet.cn

TS:   while (i < 10) { i++; }
来源：http://vi.haigaiapp.cn

Java: while (i < 10) { i++; }
来源：http://bs.jianghongdianzi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vr.panjiajie.cn

Ruby: while i < 10; i += 1; end
来源：http://ax.shtwfgs.cn

C#:   while (i < 10) { i++; }
来源：http://wv.nszjky.cn

[B08] do-while（至少执行一次）
来源：http://ir.shxzukj.cn

Py:   # 无 do-while：用 while True + break
来源：http://ku.panjiajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://yl.nicolike.cn

JS:   do { i++; } while (i < 10);
来源：http://rd.yuexingan06.cn

TS:   do { i++; } while (i < 10);
来源：http://pk.newstarts.cn

Java: do { i++; } while (i < 10);
来源：http://jw.shxzukj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bw.hahajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://nk.nszjky.cn

C#:   do { i++; } while (i < 10);
来源：http://jo.jianghongdianzi.cn

[B09] break 与 continue
来源：http://ho.jianghongdianzi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://oy.huixiangedu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tb.shxzskj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mb.huanxung.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wx.hahajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bl.bookmarksfly.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fn.muxihuayi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://oi.chemitech.net.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dr.huixinmuqiang.cn

[B10] 遍历同时拿索引
来源：http://oq.chemitech.net.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gz.szsharing.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vd.colortex.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fm.lnxyls.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cs.nszjky.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ai.shtwfgs.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://go.chemitech.net.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tj.jianghongdianzi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://eo.colortex.cn

[B11] 生成数字序列 / 区间
来源：http://mo.yuexingan06.cn

Py:   list(range(0, 10, 2))
来源：http://om.colortex.cn

PHP:  range(0, 10, 2);
来源：http://xo.szxytkj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bo.panjiajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://io.huixiangedu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qy.bjjhwx.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kg.szxytkj.cn

Ruby: (0...10).step(2).to_a
来源：http://iy.yuexingan06.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://am.shxzskj.cn

[B12] 跳出多层循环
来源：http://xu.shtwfgs.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://al.nszjky.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ov.shxzskj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cd.shxzskj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kw.newstarts.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ig.bookmarksfly.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ys.huanxung.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yu.muxihuayi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yz.gzmigu.cn

[B13] 判断是否为数字
来源：http://mb.colortex.cn

Py:   isinstance(x, (int, float))
来源：http://ln.chemitech.net.cn

PHP:  is_numeric($x)
来源：http://ay.jctech888.com.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hp.bjjhwx.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qr.chemitech.net.cn

Java: x instanceof Number
来源：http://hp.chemitech.net.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jn.jctech888.com.cn

Ruby: x.is_a?(Numeric)
来源：http://yj.nicolike.cn

C#:   x is int or double or decimal
来源：http://ft.nszjky.cn

[B14] 判断值是否在集合内
来源：http://hw.szsharing.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gp.haigaiapp.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fd.haigaiapp.cn

JS:   [1, 2, 3].includes(x)
来源：http://yf.huanxung.cn

TS:   [1, 2, 3].includes(x)
来源：http://yx.colortex.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rr.shxzskj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ep.chemitech.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xj.bjjhwx.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vw.huixiangedu.cn

[B15] 布尔运算与取反
来源：http://rs.newstarts.cn

Py:   a and b or not c
来源：http://pc.gzmigu.cn

PHP:  $a && $b || !$c
来源：http://is.shxzukj.cn

JS:   a && b || !c
来源：http://wx.9csxet.cn

TS:   a && b || !c
来源：http://ge.colortex.cn

Java: a && b || !c
来源：http://mw.lnxyls.cn

Go:   a && b || !c
来源：http://cc.nicolike.cn

Ruby: a && b || !c
来源：http://af.haigaiapp.cn

C#:   a && b || !c
来源：http://kn.jianghongdianzi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://dg.hnjuh.cn

Py:   if not data: return
来源：http://fb.lnxyls.cn

PHP:  if (!$data) { return; }
来源：http://gt.wgjwhj.cn

JS:   if (!data) return;
来源：http://ow.shtwfgs.cn

TS:   if (!data) return;
来源：http://zd.colortex.cn

Java: if (data == null) return;
来源：http://ry.shxzukj.cn

Go:   if data == nil { return }
来源：http://tb.chemitech.net.cn

Ruby: return if data.nil?
来源：http://ng.chemitech.net.cn

C#:   if (data == null) return;
来源：http://zz.yuntaijiaju.cn

================================================================================
来源：http://qz.521024.cn

C. 函数与作用域
来源：http://pe.newstarts.cn

================================================================================
来源：http://ac.bjjhwx.cn

[C01] 定义函数
来源：http://yv.chemitech.net.cn

Py:   def add(a, b): return a + b
来源：http://sb.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iw.shxzukj.cn

JS:   function add(a, b) { return a + b; }
来源：http://ur.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rs.colortex.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gi.huanxung.cn

Go:   func add(a, b int) int { return a + b }
来源：http://bz.szsharing.cn

Ruby: def add(a, b); a + b; end
来源：http://fp.shxzskj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cl.huanxung.cn

[C02] 默认参数
来源：http://ih.nszjky.cn

Py:   def greet(name="World"): return name
来源：http://ge.newstarts.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wl.panjiajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://wh.chemitech.net.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://mm.yuexingan06.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qk.asd995.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zg.jctech888.com.cn

Ruby: def greet(name = "World") = name
来源：http://zp.shtwfgs.cn

C#:   string Greet(string name = "World") => name;
来源：http://cn.gzmigu.cn

[C03] 可变参数
来源：http://qy.yuntaijiaju.cn

Py:   def total(*args): return sum(args)
来源：http://sn.muxihuayi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qe.newstarts.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ji.hnjuh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fo.shtwfgs.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ih.jctech888.com.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tq.nszjky.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hv.muxihuayi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://eq.shxzukj.cn

[C04] 命名参数 / 关键字参数
来源：http://yn.yuntaijiaju.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dj.bookmarksfly.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qu.shxzskj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hl.huixinmuqiang.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ai.shtwfgs.cn

Java: // 无：用 Builder 模式或 record
来源：http://kv.wgjwhj.cn

Go:   // 无：用配置结构体参数
来源：http://lw.bjjhwx.cn

Ruby: f(a: 1, b: 2)
来源：http://vz.muxihuayi.cn

C#:   f(a: 1, b: 2)
来源：http://on.szsharing.cn

[C05] 返回多个值
来源：http://lu.newstarts.cn

Py:   return a, b
来源：http://it.wgjwhj.cn

PHP:  return [$a, $b];
来源：http://bc.bjjhwx.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ue.panjiajie.cn

TS:   return { a, b };
来源：http://qu.wgjwhj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://si.521024.cn

Go:   return a, b
来源：http://hx.shxzukj.cn

Ruby: return a, b
来源：http://iz.huixinmuqiang.cn

C#:   return (a, b);              // ValueTuple
来源：http://cy.9csxet.cn

[C06] 匿名函数 / lambda
来源：http://og.bjjhwx.cn

Py:   square = lambda x: x * x
来源：http://xm.haigaiapp.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://gi.bjjhwx.cn

JS:   const square = x => x * x;
来源：http://xc.nszjky.cn

TS:   const square = (x: number): number => x * x;
来源：http://jb.yuexingan06.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dq.chemitech.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://bj.nszjky.cn

Ruby: square = ->(x) { x * x }
来源：http://ar.521024.cn

C#:   Func<int, int> square = x => x * x;
来源：http://oc.colortex.cn

[C07] 把函数作为参数传入
来源：http://go.haigaiapp.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qm.asd995.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hn.szsharing.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://df.shtwfgs.cn

TS:   arr.map(String)
来源：http://bt.nicolike.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ey.9csxet.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bu.chemitech.net.cn

Ruby: arr.map(&:upcase)
来源：http://ej.wgjwhj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wy.nszjky.cn

[C08] 闭包
来源：http://nt.bjjhwx.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wr.huixinmuqiang.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yt.yuexingan06.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cx.yuntaijiaju.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wc.huixinmuqiang.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rw.colortex.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fz.huixinmuqiang.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://do.lnxyls.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://el.newstarts.cn

[C09] 递归
来源：http://ja.shxzukj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wh.yuntaijiaju.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dt.asd995.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qp.huixinmuqiang.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dw.chemitech.net.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://eu.muxihuayi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xi.shxzskj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ho.jctech888.com.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ab.panjiajie.cn

[C10] 变量作用域
来源：http://mf.gzmigu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yv.yuexingan06.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hq.shxzskj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dg.hnjuh.cn

TS:   同 JS
来源：http://fg.huixinmuqiang.cn

Java: 方法内为块级作用域
来源：http://bu.nicolike.cn

Go:   花括号块级作用域
来源：http://og.newstarts.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vh.huixiangedu.cn

C#:   块级作用域
来源：http://gv.chemitech.net.cn

[C11] 模块导入与导出
来源：http://ky.jianghongdianzi.cn

Py:   from module import func
来源：http://ih.muxihuayi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qc.nicolike.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ye.wgjwhj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kn.szsharing.cn

Java: import java.util.List;
来源：http://nz.9csxet.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fn.wgjwhj.cn


<!-- 参考信息 -->