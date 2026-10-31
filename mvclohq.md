代发 wailian999

TS:   s.length
来源：http://zi.jctech888.com.cn

Java: s.length()
来源：http://wk.lnxyls.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wd.muxihuayi.cn

Ruby: s.length
来源：http://xj.wgjwhj.cn

C#:   s.Length
来源：http://xz.haigaiapp.cn

[A23] 大小写转换
来源：http://ji.bookmarksfly.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wl.hahajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://td.asd995.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qw.asd995.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bc.jctech888.com.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://md.jianghongdianzi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lm.colortex.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xr.nicolike.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://hh.gzmigu.cn

[A24] 去除首尾空白
来源：http://ri.colortex.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vc.shtwfgs.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rw.wgjwhj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cc.huixinmuqiang.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.shtwfgs.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ld.colortex.cn

Go:   strings.TrimSpace(s)
来源：http://lm.yuntaijiaju.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ww.nicolike.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mm.newstarts.cn

[A25] 字符串比较
来源：http://gl.muxihuayi.cn

Py:   s1 == s2; s1 != s2
来源：http://vo.gzmigu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ue.lnxyls.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://no.bjjhwx.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cc.muxihuayi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fj.colortex.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mw.colortex.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://jb.bjjhwx.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://za.jianghongdianzi.cn

[A26] 类型转换总览
来源：http://ef.huixiangedu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dt.colortex.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zi.panjiajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nc.shtwfgs.cn

TS:   Number() String() Boolean() x as number
来源：http://hl.wgjwhj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ow.muxihuayi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kf.wgjwhj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://yg.hnjuh.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rz.shxzukj.cn

================================================================================
来源：http://ua.nicolike.cn

B. 流程控制
来源：http://eg.yuntaijiaju.cn

================================================================================
来源：http://yq.shxzskj.cn

[B01] 条件判断 if / else
来源：http://gs.nszjky.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://rx.nicolike.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wg.panjiajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bz.szxytkj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vm.asd995.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://iy.panjiajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ab.shxzskj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ql.wgjwhj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hs.jctech888.com.cn

[B02] 多分支 else if / elif
来源：http://gj.hahajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pt.hnjuh.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xo.huixinmuqiang.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dt.wgjwhj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cz.jctech888.com.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pq.hahajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hb.colortex.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wo.bookmarksfly.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mi.jianghongdianzi.cn

[B03] switch / match / case
来源：http://ux.szsharing.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://et.nicolike.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://go.bookmarksfly.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rn.nszjky.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vj.asd995.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jv.wgjwhj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xn.shxzskj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://aq.shxzukj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mt.hnjuh.cn

[B04] for 计数循环
来源：http://bi.colortex.cn

Py:   for i in range(10): print(i)
来源：http://wr.9csxet.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zh.yuexingan06.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dk.bookmarksfly.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rh.bjjhwx.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://sz.yuntaijiaju.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ju.newstarts.cn

Ruby: 10.times { |i| puts i }
来源：http://hu.gzmigu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dw.lnxyls.cn

[B05] 遍历数组 / 列表
来源：http://hw.bjjhwx.cn

Py:   for item in arr: print(item)
来源：http://mq.huixinmuqiang.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ui.gzmigu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://cy.szsharing.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ia.yuntaijiaju.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wo.huixiangedu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://py.lnxyls.cn

Ruby: arr.each { |item| puts item }
来源：http://zs.wgjwhj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bs.wgjwhj.cn

[B06] 遍历字典 / 对象
来源：http://yp.jctech888.com.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mk.haigaiapp.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tb.9csxet.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ob.huixiangedu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wb.shxzskj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://st.colortex.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hv.huixiangedu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yg.colortex.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hg.gzmigu.cn

[B07] while 循环
来源：http://oo.nszjky.cn

Py:   while i < 10: i += 1
来源：http://hk.nszjky.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bv.shtwfgs.cn

JS:   while (i < 10) { i++; }
来源：http://gn.haigaiapp.cn

TS:   while (i < 10) { i++; }
来源：http://cl.521024.cn

Java: while (i < 10) { i++; }
来源：http://ie.lnxyls.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wm.asd995.cn

Ruby: while i < 10; i += 1; end
来源：http://jp.shxzskj.cn

C#:   while (i < 10) { i++; }
来源：http://fb.newstarts.cn

[B08] do-while（至少执行一次）
来源：http://mj.bjjhwx.cn

Py:   # 无 do-while：用 while True + break
来源：http://yl.asd995.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vm.newstarts.cn

JS:   do { i++; } while (i < 10);
来源：http://qn.nicolike.cn

TS:   do { i++; } while (i < 10);
来源：http://iz.colortex.cn

Java: do { i++; } while (i < 10);
来源：http://ga.muxihuayi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sg.lnxyls.cn

Ruby: begin; i += 1; end while i < 10
来源：http://dt.huixinmuqiang.cn

C#:   do { i++; } while (i < 10);
来源：http://uy.jctech888.com.cn

[B09] break 与 continue
来源：http://oa.shtwfgs.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yz.shtwfgs.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://oq.huanxung.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hs.shtwfgs.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://es.lnxyls.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qs.muxihuayi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sx.nicolike.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zq.szsharing.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nm.huixinmuqiang.cn

[B10] 遍历同时拿索引
来源：http://vp.gzmigu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hr.9csxet.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ir.jianghongdianzi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sr.muxihuayi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yu.huixiangedu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mi.shxzskj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ok.szxytkj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ng.nicolike.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kw.9csxet.cn

[B11] 生成数字序列 / 区间
来源：http://zv.jianghongdianzi.cn

Py:   list(range(0, 10, 2))
来源：http://tm.shtwfgs.cn

PHP:  range(0, 10, 2);
来源：http://xp.shxzukj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://my.lnxyls.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://au.szsharing.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kc.chemitech.net.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ae.bjjhwx.cn

Ruby: (0...10).step(2).to_a
来源：http://gm.bookmarksfly.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kw.jianghongdianzi.cn

[B12] 跳出多层循环
来源：http://gd.yuexingan06.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pd.lnxyls.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://bh.hnjuh.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gx.9csxet.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fq.huixiangedu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tf.shxzukj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mk.panjiajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sl.lnxyls.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ir.szsharing.cn

[B13] 判断是否为数字
来源：http://iv.nszjky.cn

Py:   isinstance(x, (int, float))
来源：http://fw.huanxung.cn

PHP:  is_numeric($x)
来源：http://wp.wgjwhj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xq.yuntaijiaju.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mz.yuntaijiaju.cn

Java: x instanceof Number
来源：http://zk.9csxet.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qq.huixiangedu.cn

Ruby: x.is_a?(Numeric)
来源：http://ex.asd995.cn

C#:   x is int or double or decimal
来源：http://mr.shxzskj.cn

[B14] 判断值是否在集合内
来源：http://yq.bjjhwx.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bw.shxzskj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nv.asd995.cn

JS:   [1, 2, 3].includes(x)
来源：http://gm.bookmarksfly.cn

TS:   [1, 2, 3].includes(x)
来源：http://iy.nicolike.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ws.huixinmuqiang.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pu.hahajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fw.shxzukj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yf.asd995.cn

[B15] 布尔运算与取反
来源：http://jx.shtwfgs.cn

Py:   a and b or not c
来源：http://fv.szsharing.cn

PHP:  $a && $b || !$c
来源：http://sj.szsharing.cn

JS:   a && b || !c
来源：http://np.shxzskj.cn

TS:   a && b || !c
来源：http://ph.jianghongdianzi.cn

Java: a && b || !c
来源：http://on.jctech888.com.cn

Go:   a && b || !c
来源：http://uj.hnjuh.cn

Ruby: a && b || !c
来源：http://hu.nicolike.cn

C#:   a && b || !c
来源：http://to.asd995.cn

[B16] 卫语句：不满足条件提前返回
来源：http://su.bookmarksfly.cn

Py:   if not data: return
来源：http://gr.9csxet.cn

PHP:  if (!$data) { return; }
来源：http://to.jctech888.com.cn

JS:   if (!data) return;
来源：http://os.muxihuayi.cn

TS:   if (!data) return;
来源：http://op.shtwfgs.cn

Java: if (data == null) return;
来源：http://jl.nszjky.cn

Go:   if data == nil { return }
来源：http://be.521024.cn

Ruby: return if data.nil?
来源：http://ze.nszjky.cn

C#:   if (data == null) return;
来源：http://iz.szsharing.cn

================================================================================
来源：http://qo.nicolike.cn

C. 函数与作用域
来源：http://by.bjjhwx.cn

================================================================================
来源：http://ia.wgjwhj.cn

[C01] 定义函数
来源：http://vl.shxzskj.cn

Py:   def add(a, b): return a + b
来源：http://hb.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ii.wgjwhj.cn

JS:   function add(a, b) { return a + b; }
来源：http://dz.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://st.521024.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://eh.asd995.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mh.nszjky.cn

Ruby: def add(a, b); a + b; end
来源：http://tv.huixinmuqiang.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hd.nicolike.cn

[C02] 默认参数
来源：http://vz.newstarts.cn

Py:   def greet(name="World"): return name
来源：http://dj.bjjhwx.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://go.shxzskj.cn

JS:   function greet(name = "World") { return name; }
来源：http://sh.panjiajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://au.muxihuayi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dv.szsharing.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xa.yuntaijiaju.cn

Ruby: def greet(name = "World") = name
来源：http://fe.huixinmuqiang.cn

C#:   string Greet(string name = "World") => name;
来源：http://bk.asd995.cn

[C03] 可变参数
来源：http://cc.chemitech.net.cn

Py:   def total(*args): return sum(args)
来源：http://wt.haigaiapp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ie.panjiajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hf.gzmigu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wh.szsharing.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ym.szxytkj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vv.yuntaijiaju.cn

Ruby: def total(*nums); nums.sum; end
来源：http://es.wgjwhj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sc.newstarts.cn

[C04] 命名参数 / 关键字参数
来源：http://xv.huanxung.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ft.gzmigu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://la.9csxet.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cf.huanxung.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vm.yuexingan06.cn

Java: // 无：用 Builder 模式或 record
来源：http://oh.newstarts.cn

Go:   // 无：用配置结构体参数
来源：http://jo.chemitech.net.cn

Ruby: f(a: 1, b: 2)
来源：http://sa.muxihuayi.cn

C#:   f(a: 1, b: 2)
来源：http://um.bookmarksfly.cn

[C05] 返回多个值
来源：http://ao.haigaiapp.cn

Py:   return a, b
来源：http://lz.bookmarksfly.cn

PHP:  return [$a, $b];
来源：http://zy.chemitech.net.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vh.bjjhwx.cn

TS:   return { a, b };
来源：http://ty.panjiajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bj.huixinmuqiang.cn

Go:   return a, b
来源：http://cm.huixinmuqiang.cn

Ruby: return a, b
来源：http://uk.huanxung.cn

C#:   return (a, b);              // ValueTuple
来源：http://kz.huanxung.cn

[C06] 匿名函数 / lambda
来源：http://dz.haigaiapp.cn

Py:   square = lambda x: x * x
来源：http://bw.panjiajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://dz.huixinmuqiang.cn

JS:   const square = x => x * x;
来源：http://yj.colortex.cn

TS:   const square = (x: number): number => x * x;
来源：http://xf.asd995.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fm.lnxyls.cn

Go:   sq := func(x int) int { return x * x }
来源：http://aa.chemitech.net.cn

Ruby: square = ->(x) { x * x }
来源：http://kn.huixiangedu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wn.gzmigu.cn

[C07] 把函数作为参数传入
来源：http://ru.szxytkj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ea.chemitech.net.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ge.shtwfgs.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cx.yuexingan06.cn

TS:   arr.map(String)
来源：http://fx.nszjky.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://iq.bookmarksfly.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fy.yuexingan06.cn

Ruby: arr.map(&:upcase)
来源：http://un.jianghongdianzi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mr.chemitech.net.cn

[C08] 闭包
来源：http://aa.521024.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cd.nszjky.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kf.hahajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vd.jianghongdianzi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vo.nicolike.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uc.hnjuh.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hh.bookmarksfly.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://th.nicolike.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zm.huixiangedu.cn

[C09] 递归
来源：http://mu.newstarts.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://er.hahajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bt.jianghongdianzi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wy.hahajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gb.shxzskj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fq.huanxung.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xi.wgjwhj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://re.shtwfgs.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sl.lnxyls.cn

[C10] 变量作用域
来源：http://ic.nicolike.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tt.muxihuayi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mc.colortex.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ec.bjjhwx.cn

TS:   同 JS
来源：http://ru.szxytkj.cn

Java: 方法内为块级作用域
来源：http://wp.szxytkj.cn

Go:   花括号块级作用域
来源：http://zo.shxzukj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pv.yuntaijiaju.cn

C#:   块级作用域
来源：http://cc.hnjuh.cn

[C11] 模块导入与导出
来源：http://el.asd995.cn

Py:   from module import func
来源：http://hz.shtwfgs.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ap.shxzukj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://er.wgjwhj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://od.haigaiapp.cn

Java: import java.util.List;
来源：http://lf.colortex.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ob.nicolike.cn

Ruby: require "json"; require_relative "./util"
来源：http://nn.nszjky.cn

C#:   using System.Text;
来源：http://rz.haigaiapp.cn

[C12] 立即执行函数 IIFE
来源：http://qq.huixinmuqiang.cn

Py:   (lambda: print("run"))()
来源：http://sq.chemitech.net.cn

PHP:  (function () { echo "run"; })();
来源：http://kl.huanxung.cn

JS:   (() => { console.log("run"); })();
来源：http://ke.wgjwhj.cn

TS:   (() => { console.log("run"); })();
来源：http://bu.bookmarksfly.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://iy.9csxet.cn

Go:   func() { fmt.Println("run") }()
来源：http://gt.panjiajie.cn

Ruby: -> { puts "run" }.call
来源：http://qn.haigaiapp.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://uw.asd995.cn

[C13] 类型声明 / 类型注解
来源：http://sr.chemitech.net.cn


<!-- 参考信息 -->