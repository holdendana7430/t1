代发 wailian999

[A22] 获取字符串长度
来源：http://rv.panjiajie.cn

Py:   len(s)
来源：http://ya.521024.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ur.yuexingan06.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://td.chemitech.net.cn

TS:   s.length
来源：http://zb.shtwfgs.cn

Java: s.length()
来源：http://so.shtwfgs.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://yz.chemitech.net.cn

Ruby: s.length
来源：http://ph.szsharing.cn

C#:   s.Length
来源：http://eh.shtwfgs.cn

[A23] 大小写转换
来源：http://vu.jctech888.com.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://rj.shxzukj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vx.nszjky.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ie.panjiajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ba.yuntaijiaju.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gf.huanxung.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bd.szsharing.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yj.jctech888.com.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://xn.9csxet.cn

[A24] 去除首尾空白
来源：http://qd.bookmarksfly.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sw.yuntaijiaju.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hd.muxihuayi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yp.chemitech.net.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vr.9csxet.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zq.jctech888.com.cn

Go:   strings.TrimSpace(s)
来源：http://oc.szxytkj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ru.521024.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yg.gzmigu.cn

[A25] 字符串比较
来源：http://kq.newstarts.cn

Py:   s1 == s2; s1 != s2
来源：http://wq.haigaiapp.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ou.yuntaijiaju.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jn.colortex.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qz.newstarts.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://sl.szsharing.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hv.chemitech.net.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://sy.asd995.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wm.asd995.cn

[A26] 类型转换总览
来源：http://cb.yuntaijiaju.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cg.yuntaijiaju.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pg.lnxyls.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jn.asd995.cn

TS:   Number() String() Boolean() x as number
来源：http://cr.nszjky.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ck.bjjhwx.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ax.muxihuayi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://sh.shxzskj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bb.newstarts.cn

================================================================================
来源：http://lj.wgjwhj.cn

B. 流程控制
来源：http://rm.shxzskj.cn

================================================================================
来源：http://dd.lnxyls.cn

[B01] 条件判断 if / else
来源：http://hv.lnxyls.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://kp.shtwfgs.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://au.colortex.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vg.jctech888.com.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tj.newstarts.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://wo.hahajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jb.shxzukj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vi.hahajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gc.newstarts.cn

[B02] 多分支 else if / elif
来源：http://ls.hnjuh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zy.shtwfgs.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nn.lnxyls.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qt.9csxet.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jl.nicolike.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gl.yuexingan06.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ed.haigaiapp.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vk.yuntaijiaju.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cn.yuntaijiaju.cn

[B03] switch / match / case
来源：http://lg.nszjky.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sj.szsharing.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://eh.jianghongdianzi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fc.shtwfgs.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sn.521024.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tg.521024.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ac.huixiangedu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xn.nicolike.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pw.521024.cn

[B04] for 计数循环
来源：http://nd.hahajie.cn

Py:   for i in range(10): print(i)
来源：http://cd.yuexingan06.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fy.jianghongdianzi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ct.521024.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nr.panjiajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ss.szxytkj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gf.jianghongdianzi.cn

Ruby: 10.times { |i| puts i }
来源：http://bo.bjjhwx.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lr.521024.cn

[B05] 遍历数组 / 列表
来源：http://xd.colortex.cn

Py:   for item in arr: print(item)
来源：http://qi.colortex.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rm.szxytkj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://kn.gzmigu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://lp.panjiajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pr.shxzukj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pg.shtwfgs.cn

Ruby: arr.each { |item| puts item }
来源：http://an.lnxyls.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yv.huixinmuqiang.cn

[B06] 遍历字典 / 对象
来源：http://sr.colortex.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vd.huixinmuqiang.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nu.panjiajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nl.huixinmuqiang.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://se.colortex.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ze.shxzukj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zd.bjjhwx.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xe.521024.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ax.nicolike.cn

[B07] while 循环
来源：http://ha.lnxyls.cn

Py:   while i < 10: i += 1
来源：http://cc.nicolike.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ei.yuexingan06.cn

JS:   while (i < 10) { i++; }
来源：http://uf.jctech888.com.cn

TS:   while (i < 10) { i++; }
来源：http://ah.nszjky.cn

Java: while (i < 10) { i++; }
来源：http://pp.huixinmuqiang.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bm.jianghongdianzi.cn

Ruby: while i < 10; i += 1; end
来源：http://ba.jctech888.com.cn

C#:   while (i < 10) { i++; }
来源：http://xu.nszjky.cn

[B08] do-while（至少执行一次）
来源：http://pr.szxytkj.cn

Py:   # 无 do-while：用 while True + break
来源：http://pg.bjjhwx.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ys.shxzukj.cn

JS:   do { i++; } while (i < 10);
来源：http://tn.newstarts.cn

TS:   do { i++; } while (i < 10);
来源：http://an.chemitech.net.cn

Java: do { i++; } while (i < 10);
来源：http://rs.huixiangedu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://yy.nszjky.cn

Ruby: begin; i += 1; end while i < 10
来源：http://eh.wgjwhj.cn

C#:   do { i++; } while (i < 10);
来源：http://av.yuexingan06.cn

[B09] break 与 continue
来源：http://vy.huixiangedu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ei.shtwfgs.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zh.lnxyls.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cf.shtwfgs.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tx.huixinmuqiang.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fm.asd995.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mz.chemitech.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ii.yuntaijiaju.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ac.muxihuayi.cn

[B10] 遍历同时拿索引
来源：http://bm.hahajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ub.shtwfgs.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wc.9csxet.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yr.jianghongdianzi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ep.bjjhwx.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ql.panjiajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ve.jianghongdianzi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vr.huanxung.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dc.521024.cn

[B11] 生成数字序列 / 区间
来源：http://xi.9csxet.cn

Py:   list(range(0, 10, 2))
来源：http://ks.szxytkj.cn

PHP:  range(0, 10, 2);
来源：http://sm.hahajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jj.yuexingan06.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bg.newstarts.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gu.hahajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ga.bjjhwx.cn

Ruby: (0...10).step(2).to_a
来源：http://mk.panjiajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vy.asd995.cn

[B12] 跳出多层循环
来源：http://hi.szsharing.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xz.huanxung.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mb.muxihuayi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dq.lnxyls.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kl.yuexingan06.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fz.yuexingan06.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://oy.hnjuh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://un.yuntaijiaju.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rp.asd995.cn

[B13] 判断是否为数字
来源：http://os.jctech888.com.cn

Py:   isinstance(x, (int, float))
来源：http://sc.chemitech.net.cn

PHP:  is_numeric($x)
来源：http://ju.bookmarksfly.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cv.jianghongdianzi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rd.chemitech.net.cn

Java: x instanceof Number
来源：http://iy.huixiangedu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ko.haigaiapp.cn

Ruby: x.is_a?(Numeric)
来源：http://wj.huanxung.cn

C#:   x is int or double or decimal
来源：http://zi.shxzukj.cn

[B14] 判断值是否在集合内
来源：http://qj.huixinmuqiang.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fq.yuntaijiaju.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://om.szsharing.cn

JS:   [1, 2, 3].includes(x)
来源：http://gd.521024.cn

TS:   [1, 2, 3].includes(x)
来源：http://nb.521024.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hc.nszjky.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vx.szxytkj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xm.lnxyls.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mu.lnxyls.cn

[B15] 布尔运算与取反
来源：http://xc.shxzskj.cn

Py:   a and b or not c
来源：http://wl.521024.cn

PHP:  $a && $b || !$c
来源：http://vy.huixiangedu.cn

JS:   a && b || !c
来源：http://zv.bookmarksfly.cn

TS:   a && b || !c
来源：http://pb.gzmigu.cn

Java: a && b || !c
来源：http://vm.shxzskj.cn

Go:   a && b || !c
来源：http://yo.shxzukj.cn

Ruby: a && b || !c
来源：http://bg.shtwfgs.cn

C#:   a && b || !c
来源：http://tz.hahajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://rr.wgjwhj.cn

Py:   if not data: return
来源：http://hf.chemitech.net.cn

PHP:  if (!$data) { return; }
来源：http://oa.bjjhwx.cn

JS:   if (!data) return;
来源：http://im.nszjky.cn

TS:   if (!data) return;
来源：http://vs.chemitech.net.cn

Java: if (data == null) return;
来源：http://id.shxzskj.cn

Go:   if data == nil { return }
来源：http://bi.jianghongdianzi.cn

Ruby: return if data.nil?
来源：http://du.shtwfgs.cn

C#:   if (data == null) return;
来源：http://ub.nszjky.cn

================================================================================
来源：http://yq.jctech888.com.cn

C. 函数与作用域
来源：http://kd.huanxung.cn

================================================================================
来源：http://jc.lnxyls.cn

[C01] 定义函数
来源：http://ff.hnjuh.cn

Py:   def add(a, b): return a + b
来源：http://zv.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cn.jianghongdianzi.cn

JS:   function add(a, b) { return a + b; }
来源：http://zq.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jw.hahajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://oy.colortex.cn

Go:   func add(a, b int) int { return a + b }
来源：http://js.lnxyls.cn

Ruby: def add(a, b); a + b; end
来源：http://iq.szxytkj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ie.9csxet.cn

[C02] 默认参数
来源：http://wl.colortex.cn

Py:   def greet(name="World"): return name
来源：http://hg.521024.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yy.wgjwhj.cn

JS:   function greet(name = "World") { return name; }
来源：http://zn.jianghongdianzi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hr.nszjky.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zs.huanxung.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zc.nicolike.cn

Ruby: def greet(name = "World") = name
来源：http://hs.asd995.cn

C#:   string Greet(string name = "World") => name;
来源：http://mb.wgjwhj.cn

[C03] 可变参数
来源：http://ln.colortex.cn

Py:   def total(*args): return sum(args)
来源：http://fj.bjjhwx.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nf.muxihuayi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://uu.yuexingan06.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bk.shxzskj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yt.asd995.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://la.colortex.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xs.szsharing.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hh.szsharing.cn

[C04] 命名参数 / 关键字参数
来源：http://ry.9csxet.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sk.jctech888.com.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zo.jianghongdianzi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dd.huixinmuqiang.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rr.haigaiapp.cn

Java: // 无：用 Builder 模式或 record
来源：http://gj.nszjky.cn

Go:   // 无：用配置结构体参数
来源：http://cm.panjiajie.cn

Ruby: f(a: 1, b: 2)
来源：http://iq.chemitech.net.cn

C#:   f(a: 1, b: 2)
来源：http://nn.yuexingan06.cn

[C05] 返回多个值
来源：http://zm.lnxyls.cn

Py:   return a, b
来源：http://qz.bookmarksfly.cn

PHP:  return [$a, $b];
来源：http://wd.nszjky.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xb.newstarts.cn

TS:   return { a, b };
来源：http://pb.bookmarksfly.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bs.wgjwhj.cn

Go:   return a, b
来源：http://ef.shxzskj.cn

Ruby: return a, b
来源：http://kr.szxytkj.cn

C#:   return (a, b);              // ValueTuple
来源：http://de.lnxyls.cn

[C06] 匿名函数 / lambda
来源：http://be.jctech888.com.cn

Py:   square = lambda x: x * x
来源：http://wa.hahajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://sq.shtwfgs.cn

JS:   const square = x => x * x;
来源：http://ky.shtwfgs.cn

TS:   const square = (x: number): number => x * x;
来源：http://xg.521024.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://oi.newstarts.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gm.hnjuh.cn

Ruby: square = ->(x) { x * x }
来源：http://jr.521024.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qr.bookmarksfly.cn

[C07] 把函数作为参数传入
来源：http://sr.huanxung.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jt.9csxet.cn

PHP:  array_map("strtoupper", $arr);
来源：http://lq.huixiangedu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kg.asd995.cn

TS:   arr.map(String)
来源：http://hv.huixiangedu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ox.bjjhwx.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zw.hnjuh.cn

Ruby: arr.map(&:upcase)
来源：http://tb.hnjuh.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://oc.bjjhwx.cn

[C08] 闭包
来源：http://lr.yuexingan06.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ut.jianghongdianzi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qv.haigaiapp.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hj.shxzukj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nq.asd995.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hj.yuexingan06.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zv.huixinmuqiang.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jy.hnjuh.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ay.panjiajie.cn

[C09] 递归
来源：http://sw.jctech888.com.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://am.szsharing.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zs.wgjwhj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://od.yuexingan06.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uo.lnxyls.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gy.huanxung.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://te.lnxyls.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hn.bookmarksfly.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kc.jianghongdianzi.cn

[C10] 变量作用域
来源：http://fk.shtwfgs.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zr.huanxung.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lk.colortex.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://un.newstarts.cn

TS:   同 JS
来源：http://yy.asd995.cn

Java: 方法内为块级作用域
来源：http://po.jianghongdianzi.cn

Go:   花括号块级作用域
来源：http://zs.huanxung.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lv.jianghongdianzi.cn

C#:   块级作用域
来源：http://uk.gzmigu.cn

[C11] 模块导入与导出
来源：http://oq.muxihuayi.cn

Py:   from module import func
来源：http://gs.huixiangedu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kj.shtwfgs.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zw.shxzukj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gw.szxytkj.cn

Java: import java.util.List;
来源：http://fr.huixinmuqiang.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://eg.nicolike.cn

Ruby: require "json"; require_relative "./util"
来源：http://rh.shxzskj.cn

C#:   using System.Text;
来源：http://ek.colortex.cn

[C12] 立即执行函数 IIFE
来源：http://bz.shxzskj.cn

Py:   (lambda: print("run"))()
来源：http://ad.chemitech.net.cn

PHP:  (function () { echo "run"; })();
来源：http://pl.bookmarksfly.cn

JS:   (() => { console.log("run"); })();
来源：http://hq.9csxet.cn

TS:   (() => { console.log("run"); })();
来源：http://tr.shtwfgs.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ca.shxzukj.cn


<!-- 参考信息 -->