代发 wailian999

[A22] 获取字符串长度
来源：http://nj.nicolike.cn

Py:   len(s)
来源：http://br.panjiajie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://me.gzmigu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tv.bookmarksfly.cn

TS:   s.length
来源：http://jp.9csxet.cn

Java: s.length()
来源：http://ff.lnxyls.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://rn.haigaiapp.cn

Ruby: s.length
来源：http://cv.shxzskj.cn

C#:   s.Length
来源：http://fz.huixiangedu.cn

[A23] 大小写转换
来源：http://kr.shxzskj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ap.hnjuh.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ny.bjjhwx.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://me.nicolike.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://au.asd995.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wz.9csxet.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jd.wgjwhj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ba.gzmigu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://br.colortex.cn

[A24] 去除首尾空白
来源：http://mi.szsharing.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tw.shxzukj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ec.yuntaijiaju.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ue.nicolike.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mi.szxytkj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ws.gzmigu.cn

Go:   strings.TrimSpace(s)
来源：http://pc.shxzskj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tz.muxihuayi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://bn.bookmarksfly.cn

[A25] 字符串比较
来源：http://zl.muxihuayi.cn

Py:   s1 == s2; s1 != s2
来源：http://in.szsharing.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ue.nicolike.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://se.shtwfgs.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zv.shtwfgs.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cj.huixiangedu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://al.szxytkj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ps.panjiajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wq.huixiangedu.cn

[A26] 类型转换总览
来源：http://we.shxzskj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xt.huanxung.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gh.colortex.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gj.muxihuayi.cn

TS:   Number() String() Boolean() x as number
来源：http://ps.panjiajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lh.jianghongdianzi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://km.yuntaijiaju.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mv.chemitech.net.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ig.nicolike.cn

================================================================================
来源：http://zl.shxzukj.cn

B. 流程控制
来源：http://uy.bookmarksfly.cn

================================================================================
来源：http://kp.huanxung.cn

[B01] 条件判断 if / else
来源：http://zr.yuntaijiaju.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://uo.wgjwhj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mg.shxzskj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jh.nicolike.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vf.lnxyls.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://np.9csxet.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vg.9csxet.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gp.9csxet.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ij.newstarts.cn

[B02] 多分支 else if / elif
来源：http://vy.9csxet.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cz.nszjky.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lz.yuntaijiaju.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sg.szxytkj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oi.haigaiapp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vi.lnxyls.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rd.bookmarksfly.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kr.newstarts.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sc.521024.cn

[B03] switch / match / case
来源：http://jq.shxzukj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ne.asd995.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kh.lnxyls.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hx.jctech888.com.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xz.hnjuh.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xr.szsharing.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mo.jctech888.com.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fq.gzmigu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cs.asd995.cn

[B04] for 计数循环
来源：http://sw.haigaiapp.cn

Py:   for i in range(10): print(i)
来源：http://ib.yuexingan06.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ms.muxihuayi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://aa.huixiangedu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://le.chemitech.net.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yu.hnjuh.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hy.muxihuayi.cn

Ruby: 10.times { |i| puts i }
来源：http://is.jianghongdianzi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rl.gzmigu.cn

[B05] 遍历数组 / 列表
来源：http://aw.shxzskj.cn

Py:   for item in arr: print(item)
来源：http://we.wgjwhj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.newstarts.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zq.shtwfgs.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ns.521024.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://tt.shtwfgs.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rc.panjiajie.cn

Ruby: arr.each { |item| puts item }
来源：http://hz.muxihuayi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fj.nszjky.cn

[B06] 遍历字典 / 对象
来源：http://kr.haigaiapp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://bb.yuntaijiaju.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ob.szsharing.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zv.panjiajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hu.nicolike.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qu.chemitech.net.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hg.yuexingan06.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hm.lnxyls.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ku.nicolike.cn

[B07] while 循环
来源：http://se.shxzskj.cn

Py:   while i < 10: i += 1
来源：http://et.chemitech.net.cn

PHP:  while ($i < 10) { $i++; }
来源：http://yc.newstarts.cn

JS:   while (i < 10) { i++; }
来源：http://io.gzmigu.cn

TS:   while (i < 10) { i++; }
来源：http://is.huixinmuqiang.cn

Java: while (i < 10) { i++; }
来源：http://pl.nszjky.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lp.colortex.cn

Ruby: while i < 10; i += 1; end
来源：http://yy.huixiangedu.cn

C#:   while (i < 10) { i++; }
来源：http://jv.shtwfgs.cn

[B08] do-while（至少执行一次）
来源：http://je.lnxyls.cn

Py:   # 无 do-while：用 while True + break
来源：http://re.shxzskj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ri.muxihuayi.cn

JS:   do { i++; } while (i < 10);
来源：http://wt.bookmarksfly.cn

TS:   do { i++; } while (i < 10);
来源：http://ep.asd995.cn

Java: do { i++; } while (i < 10);
来源：http://lb.jctech888.com.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ve.shxzskj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fk.bookmarksfly.cn

C#:   do { i++; } while (i < 10);
来源：http://fd.yuntaijiaju.cn

[B09] break 与 continue
来源：http://ry.yuexingan06.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://md.lnxyls.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vs.lnxyls.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kx.szxytkj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xm.shtwfgs.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://al.bookmarksfly.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nz.haigaiapp.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tg.521024.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ya.yuexingan06.cn

[B10] 遍历同时拿索引
来源：http://dg.bookmarksfly.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ix.bookmarksfly.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://oz.shtwfgs.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ju.yuntaijiaju.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gy.hnjuh.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://of.newstarts.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tf.shxzukj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://at.huixiangedu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://oo.hahajie.cn

[B11] 生成数字序列 / 区间
来源：http://rr.panjiajie.cn

Py:   list(range(0, 10, 2))
来源：http://qz.gzmigu.cn

PHP:  range(0, 10, 2);
来源：http://ho.9csxet.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iq.9csxet.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gw.colortex.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://na.huixinmuqiang.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ho.huixinmuqiang.cn

Ruby: (0...10).step(2).to_a
来源：http://sf.panjiajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fn.muxihuayi.cn

[B12] 跳出多层循环
来源：http://rj.muxihuayi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ca.yuntaijiaju.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ro.asd995.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ag.colortex.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://oz.lnxyls.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://br.gzmigu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lf.haigaiapp.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ap.haigaiapp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vz.shxzukj.cn

[B13] 判断是否为数字
来源：http://ee.newstarts.cn

Py:   isinstance(x, (int, float))
来源：http://pa.nicolike.cn

PHP:  is_numeric($x)
来源：http://rk.shxzskj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://al.yuexingan06.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bn.jianghongdianzi.cn

Java: x instanceof Number
来源：http://ba.wgjwhj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xa.szxytkj.cn

Ruby: x.is_a?(Numeric)
来源：http://kb.panjiajie.cn

C#:   x is int or double or decimal
来源：http://ax.nicolike.cn

[B14] 判断值是否在集合内
来源：http://xy.hahajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nc.nszjky.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cg.shtwfgs.cn

JS:   [1, 2, 3].includes(x)
来源：http://jv.yuntaijiaju.cn

TS:   [1, 2, 3].includes(x)
来源：http://le.bookmarksfly.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ah.hnjuh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sn.szxytkj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://uk.nszjky.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vd.huixiangedu.cn

[B15] 布尔运算与取反
来源：http://px.hnjuh.cn

Py:   a and b or not c
来源：http://oi.bjjhwx.cn

PHP:  $a && $b || !$c
来源：http://qd.panjiajie.cn

JS:   a && b || !c
来源：http://tz.hahajie.cn

TS:   a && b || !c
来源：http://gf.shxzukj.cn

Java: a && b || !c
来源：http://rz.panjiajie.cn

Go:   a && b || !c
来源：http://ru.wgjwhj.cn

Ruby: a && b || !c
来源：http://ga.huanxung.cn

C#:   a && b || !c
来源：http://ue.9csxet.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gv.shtwfgs.cn

Py:   if not data: return
来源：http://zg.hahajie.cn

PHP:  if (!$data) { return; }
来源：http://lw.nicolike.cn

JS:   if (!data) return;
来源：http://fa.shtwfgs.cn

TS:   if (!data) return;
来源：http://yp.shxzskj.cn

Java: if (data == null) return;
来源：http://md.szxytkj.cn

Go:   if data == nil { return }
来源：http://ph.shxzukj.cn

Ruby: return if data.nil?
来源：http://ga.nszjky.cn

C#:   if (data == null) return;
来源：http://sr.gzmigu.cn

================================================================================
来源：http://pu.shxzukj.cn

C. 函数与作用域
来源：http://gg.szsharing.cn

================================================================================
来源：http://kv.newstarts.cn

[C01] 定义函数
来源：http://gr.huanxung.cn

Py:   def add(a, b): return a + b
来源：http://mg.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ny.muxihuayi.cn

JS:   function add(a, b) { return a + b; }
来源：http://hb.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tu.newstarts.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://iv.jctech888.com.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hw.yuexingan06.cn

Ruby: def add(a, b); a + b; end
来源：http://vu.nicolike.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pb.szsharing.cn

[C02] 默认参数
来源：http://lh.shxzukj.cn

Py:   def greet(name="World"): return name
来源：http://dp.colortex.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vg.shtwfgs.cn

JS:   function greet(name = "World") { return name; }
来源：http://yv.shxzukj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xf.szsharing.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ri.hahajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rq.colortex.cn

Ruby: def greet(name = "World") = name
来源：http://xc.hahajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://ac.shtwfgs.cn

[C03] 可变参数
来源：http://pi.521024.cn

Py:   def total(*args): return sum(args)
来源：http://su.hahajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ul.shtwfgs.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jg.colortex.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://db.huixinmuqiang.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pf.asd995.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cb.newstarts.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rg.chemitech.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pb.yuntaijiaju.cn

[C04] 命名参数 / 关键字参数
来源：http://yp.bookmarksfly.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xm.szsharing.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zc.jianghongdianzi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gm.shxzukj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zd.colortex.cn

Java: // 无：用 Builder 模式或 record
来源：http://hl.muxihuayi.cn

Go:   // 无：用配置结构体参数
来源：http://oy.panjiajie.cn

Ruby: f(a: 1, b: 2)
来源：http://tk.gzmigu.cn

C#:   f(a: 1, b: 2)
来源：http://iu.bookmarksfly.cn

[C05] 返回多个值
来源：http://ny.shxzukj.cn

Py:   return a, b
来源：http://lz.wgjwhj.cn

PHP:  return [$a, $b];
来源：http://zy.haigaiapp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pw.yuntaijiaju.cn

TS:   return { a, b };
来源：http://ct.newstarts.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://it.huixiangedu.cn

Go:   return a, b
来源：http://oe.yuexingan06.cn

Ruby: return a, b
来源：http://oe.colortex.cn

C#:   return (a, b);              // ValueTuple
来源：http://qy.panjiajie.cn

[C06] 匿名函数 / lambda
来源：http://ru.jianghongdianzi.cn

Py:   square = lambda x: x * x
来源：http://fz.lnxyls.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qw.shxzukj.cn

JS:   const square = x => x * x;
来源：http://yy.huanxung.cn

TS:   const square = (x: number): number => x * x;
来源：http://wt.yuntaijiaju.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wc.chemitech.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://nu.newstarts.cn

Ruby: square = ->(x) { x * x }
来源：http://xv.yuexingan06.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dh.huanxung.cn

[C07] 把函数作为参数传入
来源：http://hw.521024.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bv.9csxet.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hv.lnxyls.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vd.shxzukj.cn

TS:   arr.map(String)
来源：http://dh.nicolike.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ts.yuntaijiaju.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fi.chemitech.net.cn

Ruby: arr.map(&:upcase)
来源：http://xs.panjiajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jt.bookmarksfly.cn

[C08] 闭包
来源：http://rd.yuexingan06.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hk.jctech888.com.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cc.szsharing.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://iv.yuexingan06.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://id.colortex.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xw.muxihuayi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kv.szxytkj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yb.gzmigu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jz.szxytkj.cn

[C09] 递归
来源：http://hq.yuexingan06.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mg.shxzskj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jq.asd995.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tu.nicolike.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yy.shxzukj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yw.huixinmuqiang.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ix.haigaiapp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yd.szsharing.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jn.colortex.cn

[C10] 变量作用域
来源：http://pk.yuntaijiaju.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xz.haigaiapp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ag.gzmigu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ul.haigaiapp.cn

TS:   同 JS
来源：http://do.jctech888.com.cn

Java: 方法内为块级作用域
来源：http://bv.9csxet.cn

Go:   花括号块级作用域
来源：http://zo.gzmigu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bs.hnjuh.cn

C#:   块级作用域
来源：http://gx.asd995.cn

[C11] 模块导入与导出
来源：http://mx.szxytkj.cn

Py:   from module import func
来源：http://dc.hnjuh.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qu.huixiangedu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vf.shxzskj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zi.huanxung.cn

Java: import java.util.List;
来源：http://pp.yuexingan06.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jv.muxihuayi.cn

Ruby: require "json"; require_relative "./util"
来源：http://ci.yuntaijiaju.cn

C#:   using System.Text;
来源：http://yr.9csxet.cn

[C12] 立即执行函数 IIFE
来源：http://rc.wgjwhj.cn

Py:   (lambda: print("run"))()
来源：http://xd.szsharing.cn

PHP:  (function () { echo "run"; })();
来源：http://jb.yuntaijiaju.cn

JS:   (() => { console.log("run"); })();
来源：http://cy.yuexingan06.cn

TS:   (() => { console.log("run"); })();
来源：http://sp.jianghongdianzi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mt.9csxet.cn


<!-- 参考信息 -->