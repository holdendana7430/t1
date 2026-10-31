代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://io.hnjuh.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://xw.bjjhwx.cn

[A24] 去除首尾空白
来源：http://wf.shxzskj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://za.bjjhwx.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hw.huanxung.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jf.colortex.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ct.panjiajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://st.yuntaijiaju.cn

Go:   strings.TrimSpace(s)
来源：http://mi.szsharing.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://co.bjjhwx.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tb.wgjwhj.cn

[A25] 字符串比较
来源：http://gj.yuntaijiaju.cn

Py:   s1 == s2; s1 != s2
来源：http://af.nicolike.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ia.9csxet.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://iq.asd995.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ax.huanxung.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qt.asd995.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mj.bjjhwx.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://qg.gzmigu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yy.shxzukj.cn

[A26] 类型转换总览
来源：http://vm.huanxung.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jx.newstarts.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pl.jctech888.com.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://me.haigaiapp.cn

TS:   Number() String() Boolean() x as number
来源：http://df.bookmarksfly.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bm.521024.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dy.521024.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ur.huixiangedu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cv.yuexingan06.cn

================================================================================
来源：http://fc.hnjuh.cn

B. 流程控制
来源：http://js.yuexingan06.cn

================================================================================
来源：http://lp.huixiangedu.cn

[B01] 条件判断 if / else
来源：http://cw.asd995.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://op.9csxet.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sl.yuntaijiaju.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ez.nszjky.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ax.bookmarksfly.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://eh.nszjky.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kt.521024.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rx.newstarts.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cj.shxzukj.cn

[B02] 多分支 else if / elif
来源：http://go.huixinmuqiang.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bs.yuntaijiaju.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jh.shtwfgs.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fk.colortex.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tx.9csxet.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wt.bjjhwx.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ku.panjiajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yk.gzmigu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zu.shxzskj.cn

[B03] switch / match / case
来源：http://to.jctech888.com.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yl.shxzukj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ou.bookmarksfly.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zt.yuexingan06.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kj.gzmigu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jx.muxihuayi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xn.9csxet.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hc.bjjhwx.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cg.jianghongdianzi.cn

[B04] for 计数循环
来源：http://lg.jianghongdianzi.cn

Py:   for i in range(10): print(i)
来源：http://cz.newstarts.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gr.huanxung.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://az.hnjuh.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dq.colortex.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://no.muxihuayi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fq.yuexingan06.cn

Ruby: 10.times { |i| puts i }
来源：http://bf.colortex.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zc.szxytkj.cn

[B05] 遍历数组 / 列表
来源：http://kg.hahajie.cn

Py:   for item in arr: print(item)
来源：http://fw.yuntaijiaju.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://is.lnxyls.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://px.wgjwhj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ry.nszjky.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://tj.hnjuh.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jv.yuntaijiaju.cn

Ruby: arr.each { |item| puts item }
来源：http://qy.szsharing.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://og.szsharing.cn

[B06] 遍历字典 / 对象
来源：http://xv.colortex.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://lp.nszjky.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vx.gzmigu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://la.hahajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cd.jctech888.com.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vd.huanxung.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qd.hahajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nu.hnjuh.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nx.hnjuh.cn

[B07] while 循环
来源：http://gi.hnjuh.cn

Py:   while i < 10: i += 1
来源：http://ja.521024.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fx.gzmigu.cn

JS:   while (i < 10) { i++; }
来源：http://rd.szsharing.cn

TS:   while (i < 10) { i++; }
来源：http://ux.jianghongdianzi.cn

Java: while (i < 10) { i++; }
来源：http://ls.9csxet.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gl.hahajie.cn

Ruby: while i < 10; i += 1; end
来源：http://pl.yuntaijiaju.cn

C#:   while (i < 10) { i++; }
来源：http://yj.szxytkj.cn

[B08] do-while（至少执行一次）
来源：http://uc.wgjwhj.cn

Py:   # 无 do-while：用 while True + break
来源：http://jk.lnxyls.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://rx.521024.cn

JS:   do { i++; } while (i < 10);
来源：http://ro.huixinmuqiang.cn

TS:   do { i++; } while (i < 10);
来源：http://ak.huixiangedu.cn

Java: do { i++; } while (i < 10);
来源：http://fv.huixiangedu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://dm.szxytkj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cq.szxytkj.cn

C#:   do { i++; } while (i < 10);
来源：http://iw.nicolike.cn

[B09] break 与 continue
来源：http://ll.panjiajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dc.szsharing.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://da.szsharing.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uj.nszjky.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lv.521024.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://np.nicolike.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nz.lnxyls.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mv.jianghongdianzi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yp.huixinmuqiang.cn

[B10] 遍历同时拿索引
来源：http://od.nszjky.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vz.shxzskj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yc.bjjhwx.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://la.chemitech.net.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hx.bookmarksfly.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kn.hnjuh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hx.hnjuh.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wj.asd995.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ke.muxihuayi.cn

[B11] 生成数字序列 / 区间
来源：http://dd.shxzskj.cn

Py:   list(range(0, 10, 2))
来源：http://zs.nicolike.cn

PHP:  range(0, 10, 2);
来源：http://pg.9csxet.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ok.asd995.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ia.huixiangedu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nk.huixiangedu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dc.bookmarksfly.cn

Ruby: (0...10).step(2).to_a
来源：http://bg.bookmarksfly.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sy.hnjuh.cn

[B12] 跳出多层循环
来源：http://vm.huixinmuqiang.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bp.muxihuayi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://xt.shxzukj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gt.muxihuayi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fr.huixiangedu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://su.shtwfgs.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bl.asd995.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vg.9csxet.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://re.hahajie.cn

[B13] 判断是否为数字
来源：http://qv.muxihuayi.cn

Py:   isinstance(x, (int, float))
来源：http://jl.9csxet.cn

PHP:  is_numeric($x)
来源：http://zk.hnjuh.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sr.panjiajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ls.nszjky.cn

Java: x instanceof Number
来源：http://jc.nszjky.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gt.gzmigu.cn

Ruby: x.is_a?(Numeric)
来源：http://cw.lnxyls.cn

C#:   x is int or double or decimal
来源：http://ek.hnjuh.cn

[B14] 判断值是否在集合内
来源：http://pg.gzmigu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qc.gzmigu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cn.shtwfgs.cn

JS:   [1, 2, 3].includes(x)
来源：http://cg.asd995.cn

TS:   [1, 2, 3].includes(x)
来源：http://en.haigaiapp.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://mn.panjiajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ht.huixiangedu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://dt.asd995.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://af.shtwfgs.cn

[B15] 布尔运算与取反
来源：http://em.shxzukj.cn

Py:   a and b or not c
来源：http://xp.bookmarksfly.cn

PHP:  $a && $b || !$c
来源：http://wk.bjjhwx.cn

JS:   a && b || !c
来源：http://yh.shxzskj.cn

TS:   a && b || !c
来源：http://sx.wgjwhj.cn

Java: a && b || !c
来源：http://sq.gzmigu.cn

Go:   a && b || !c
来源：http://mo.chemitech.net.cn

Ruby: a && b || !c
来源：http://oc.yuntaijiaju.cn

C#:   a && b || !c
来源：http://dm.wgjwhj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://yn.szsharing.cn

Py:   if not data: return
来源：http://sh.shtwfgs.cn

PHP:  if (!$data) { return; }
来源：http://hq.gzmigu.cn

JS:   if (!data) return;
来源：http://tj.szxytkj.cn

TS:   if (!data) return;
来源：http://ok.chemitech.net.cn

Java: if (data == null) return;
来源：http://ku.wgjwhj.cn

Go:   if data == nil { return }
来源：http://vq.wgjwhj.cn

Ruby: return if data.nil?
来源：http://us.shxzskj.cn

C#:   if (data == null) return;
来源：http://sc.bjjhwx.cn

================================================================================
来源：http://pl.huanxung.cn

C. 函数与作用域
来源：http://cu.nszjky.cn

================================================================================
来源：http://xv.shtwfgs.cn

[C01] 定义函数
来源：http://ap.bjjhwx.cn

Py:   def add(a, b): return a + b
来源：http://nj.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://an.jctech888.com.cn

JS:   function add(a, b) { return a + b; }
来源：http://oq.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xs.nszjky.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://jh.hnjuh.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dt.chemitech.net.cn

Ruby: def add(a, b); a + b; end
来源：http://ky.muxihuayi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://du.colortex.cn

[C02] 默认参数
来源：http://db.hahajie.cn

Py:   def greet(name="World"): return name
来源：http://ub.lnxyls.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://pe.shxzukj.cn

JS:   function greet(name = "World") { return name; }
来源：http://jc.szxytkj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qo.huixinmuqiang.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://aa.huixiangedu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kn.bookmarksfly.cn

Ruby: def greet(name = "World") = name
来源：http://bz.szxytkj.cn

C#:   string Greet(string name = "World") => name;
来源：http://kg.wgjwhj.cn

[C03] 可变参数
来源：http://dz.hnjuh.cn

Py:   def total(*args): return sum(args)
来源：http://ie.panjiajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fl.szsharing.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kp.szsharing.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uz.yuntaijiaju.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ze.lnxyls.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://us.nicolike.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ae.shtwfgs.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://km.panjiajie.cn

[C04] 命名参数 / 关键字参数
来源：http://oz.huanxung.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://iu.newstarts.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vy.colortex.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mf.hahajie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qc.jianghongdianzi.cn

Java: // 无：用 Builder 模式或 record
来源：http://gi.huixiangedu.cn

Go:   // 无：用配置结构体参数
来源：http://vx.jianghongdianzi.cn

Ruby: f(a: 1, b: 2)
来源：http://fm.bookmarksfly.cn

C#:   f(a: 1, b: 2)
来源：http://bk.yuntaijiaju.cn

[C05] 返回多个值
来源：http://zh.asd995.cn

Py:   return a, b
来源：http://wz.bookmarksfly.cn

PHP:  return [$a, $b];
来源：http://re.shxzskj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fw.nszjky.cn

TS:   return { a, b };
来源：http://wl.huixiangedu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dp.chemitech.net.cn

Go:   return a, b
来源：http://tc.shxzskj.cn

Ruby: return a, b
来源：http://fh.lnxyls.cn

C#:   return (a, b);              // ValueTuple
来源：http://bj.gzmigu.cn

[C06] 匿名函数 / lambda
来源：http://jj.nicolike.cn

Py:   square = lambda x: x * x
来源：http://wc.muxihuayi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://nk.haigaiapp.cn

JS:   const square = x => x * x;
来源：http://xj.jctech888.com.cn

TS:   const square = (x: number): number => x * x;
来源：http://bk.yuexingan06.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kl.521024.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zm.shtwfgs.cn

Ruby: square = ->(x) { x * x }
来源：http://vd.shxzskj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qg.muxihuayi.cn

[C07] 把函数作为参数传入
来源：http://pa.muxihuayi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hm.colortex.cn

PHP:  array_map("strtoupper", $arr);
来源：http://yj.chemitech.net.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pv.bookmarksfly.cn

TS:   arr.map(String)
来源：http://xx.shtwfgs.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://oh.muxihuayi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bt.shtwfgs.cn

Ruby: arr.map(&:upcase)
来源：http://rx.wgjwhj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://yh.bjjhwx.cn

[C08] 闭包
来源：http://jd.panjiajie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rv.shxzukj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cf.shxzukj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cz.yuntaijiaju.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://oc.jianghongdianzi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hs.szsharing.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yy.newstarts.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://oy.hnjuh.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kt.huanxung.cn

[C09] 递归
来源：http://xr.hahajie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yz.asd995.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://be.colortex.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mi.szsharing.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ll.huixinmuqiang.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://um.muxihuayi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tv.shxzukj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ic.chemitech.net.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://co.panjiajie.cn

[C10] 变量作用域
来源：http://ej.bookmarksfly.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jq.hahajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ig.hnjuh.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://di.hahajie.cn

TS:   同 JS
来源：http://sc.asd995.cn

Java: 方法内为块级作用域
来源：http://uu.haigaiapp.cn

Go:   花括号块级作用域
来源：http://dt.yuntaijiaju.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://da.shxzskj.cn

C#:   块级作用域
来源：http://uw.huixinmuqiang.cn

[C11] 模块导入与导出
来源：http://ac.colortex.cn

Py:   from module import func
来源：http://nt.haigaiapp.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pa.jianghongdianzi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://se.yuexingan06.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vw.jianghongdianzi.cn

Java: import java.util.List;
来源：http://xg.panjiajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qc.panjiajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://mv.huixinmuqiang.cn

C#:   using System.Text;
来源：http://ed.yuntaijiaju.cn

[C12] 立即执行函数 IIFE
来源：http://mm.haigaiapp.cn

Py:   (lambda: print("run"))()
来源：http://wo.huanxung.cn

PHP:  (function () { echo "run"; })();
来源：http://hg.yuexingan06.cn

JS:   (() => { console.log("run"); })();
来源：http://zy.hahajie.cn

TS:   (() => { console.log("run"); })();
来源：http://ky.nicolike.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zi.bjjhwx.cn

Go:   func() { fmt.Println("run") }()
来源：http://bd.szsharing.cn

Ruby: -> { puts "run" }.call
来源：http://jg.chemitech.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://nf.wgjwhj.cn

[C13] 类型声明 / 类型注解
来源：http://zb.chemitech.net.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ul.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fn.muxihuayi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sv.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hc.gzmigu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tt.muxihuayi.cn

Go:   func add(a, b int) int
来源：http://yf.bjjhwx.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://aa.haigaiapp.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nl.bookmarksfly.cn

[C14] 泛型函数
来源：http://pe.panjiajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ip.nicolike.cn

PHP:  // 无泛型
来源：http://zv.colortex.cn

JS:   // 无泛型
来源：http://ho.szsharing.cn


<!-- 参考信息 -->