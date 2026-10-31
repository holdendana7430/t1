代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cp.asd995.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://nk.wgjwhj.cn

[A24] 去除首尾空白
来源：http://fm.521024.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sy.huixinmuqiang.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xg.shxzskj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qk.colortex.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nl.jctech888.com.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tf.yuexingan06.cn

Go:   strings.TrimSpace(s)
来源：http://bd.nszjky.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ut.hnjuh.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lt.panjiajie.cn

[A25] 字符串比较
来源：http://hz.newstarts.cn

Py:   s1 == s2; s1 != s2
来源：http://sd.yuexingan06.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://so.521024.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ok.lnxyls.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xg.huanxung.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fi.szsharing.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rq.haigaiapp.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://lp.huanxung.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ny.jianghongdianzi.cn

[A26] 类型转换总览
来源：http://qg.szxytkj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ec.hahajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cm.huanxung.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fc.newstarts.cn

TS:   Number() String() Boolean() x as number
来源：http://ta.szxytkj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nh.9csxet.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://eg.shxzskj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://jx.panjiajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lz.9csxet.cn

================================================================================
来源：http://os.gzmigu.cn

B. 流程控制
来源：http://tn.huixinmuqiang.cn

================================================================================
来源：http://ut.szsharing.cn

[B01] 条件判断 if / else
来源：http://jt.9csxet.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://am.shxzukj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mz.shtwfgs.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qe.521024.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pn.chemitech.net.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bp.bjjhwx.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fs.szxytkj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://al.chemitech.net.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dx.yuexingan06.cn

[B02] 多分支 else if / elif
来源：http://af.asd995.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://in.wgjwhj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://av.szxytkj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ob.nszjky.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kh.shtwfgs.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gs.bjjhwx.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bf.nszjky.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qz.hahajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yz.nszjky.cn

[B03] switch / match / case
来源：http://nj.huixinmuqiang.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dh.huixinmuqiang.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gn.panjiajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ui.newstarts.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uf.shxzskj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://od.muxihuayi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ak.bjjhwx.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hp.jctech888.com.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ek.shtwfgs.cn

[B04] for 计数循环
来源：http://zv.nszjky.cn

Py:   for i in range(10): print(i)
来源：http://kp.szsharing.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tx.521024.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tc.huixinmuqiang.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bw.jctech888.com.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xh.szxytkj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yl.nicolike.cn

Ruby: 10.times { |i| puts i }
来源：http://to.nicolike.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jx.jianghongdianzi.cn

[B05] 遍历数组 / 列表
来源：http://oq.szxytkj.cn

Py:   for item in arr: print(item)
来源：http://cq.shxzukj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ey.nszjky.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ws.hahajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://by.9csxet.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://uk.panjiajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://op.hnjuh.cn

Ruby: arr.each { |item| puts item }
来源：http://wk.huanxung.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ic.lnxyls.cn

[B06] 遍历字典 / 对象
来源：http://za.bookmarksfly.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://kn.panjiajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rc.jianghongdianzi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wh.shxzskj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jb.521024.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://eu.bjjhwx.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://uj.muxihuayi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bt.yuexingan06.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nv.shxzskj.cn

[B07] while 循环
来源：http://vp.shtwfgs.cn

Py:   while i < 10: i += 1
来源：http://cw.nszjky.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ks.gzmigu.cn

JS:   while (i < 10) { i++; }
来源：http://dg.9csxet.cn

TS:   while (i < 10) { i++; }
来源：http://kp.huixinmuqiang.cn

Java: while (i < 10) { i++; }
来源：http://mu.szsharing.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zc.huixiangedu.cn

Ruby: while i < 10; i += 1; end
来源：http://ot.nszjky.cn

C#:   while (i < 10) { i++; }
来源：http://ud.wgjwhj.cn

[B08] do-while（至少执行一次）
来源：http://mh.jctech888.com.cn

Py:   # 无 do-while：用 while True + break
来源：http://yq.shtwfgs.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://be.huixinmuqiang.cn

JS:   do { i++; } while (i < 10);
来源：http://hz.9csxet.cn

TS:   do { i++; } while (i < 10);
来源：http://uc.nicolike.cn

Java: do { i++; } while (i < 10);
来源：http://go.bookmarksfly.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ew.bjjhwx.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wu.yuntaijiaju.cn

C#:   do { i++; } while (i < 10);
来源：http://zo.panjiajie.cn

[B09] break 与 continue
来源：http://ta.shxzskj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fy.wgjwhj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xo.yuntaijiaju.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://td.bookmarksfly.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cz.9csxet.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://co.wgjwhj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ek.lnxyls.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nm.yuntaijiaju.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vs.asd995.cn

[B10] 遍历同时拿索引
来源：http://ab.shtwfgs.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pc.bookmarksfly.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cc.bjjhwx.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cx.chemitech.net.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uk.shxzukj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yg.szsharing.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bg.chemitech.net.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jf.yuntaijiaju.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qg.szxytkj.cn

[B11] 生成数字序列 / 区间
来源：http://nm.bookmarksfly.cn

Py:   list(range(0, 10, 2))
来源：http://ex.huixiangedu.cn

PHP:  range(0, 10, 2);
来源：http://et.nszjky.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://au.shxzskj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ge.haigaiapp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tf.hahajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ym.shxzskj.cn

Ruby: (0...10).step(2).to_a
来源：http://mu.bookmarksfly.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gk.nszjky.cn

[B12] 跳出多层循环
来源：http://ah.lnxyls.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://nu.yuexingan06.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://pj.huixinmuqiang.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sh.bjjhwx.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bi.shxzukj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gx.huixinmuqiang.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tm.huanxung.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cm.asd995.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ol.huanxung.cn

[B13] 判断是否为数字
来源：http://xe.gzmigu.cn

Py:   isinstance(x, (int, float))
来源：http://cs.szsharing.cn

PHP:  is_numeric($x)
来源：http://jn.shtwfgs.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qh.nszjky.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ee.huixiangedu.cn

Java: x instanceof Number
来源：http://zs.hahajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cf.wgjwhj.cn

Ruby: x.is_a?(Numeric)
来源：http://gp.panjiajie.cn

C#:   x is int or double or decimal
来源：http://ey.nicolike.cn

[B14] 判断值是否在集合内
来源：http://qn.szsharing.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://on.jctech888.com.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nw.hahajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://fs.hnjuh.cn

TS:   [1, 2, 3].includes(x)
来源：http://ag.jianghongdianzi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vt.jctech888.com.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dm.yuntaijiaju.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vy.yuntaijiaju.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mv.huixinmuqiang.cn

[B15] 布尔运算与取反
来源：http://mz.9csxet.cn

Py:   a and b or not c
来源：http://bx.nicolike.cn

PHP:  $a && $b || !$c
来源：http://km.huixiangedu.cn

JS:   a && b || !c
来源：http://wv.jctech888.com.cn

TS:   a && b || !c
来源：http://fm.chemitech.net.cn

Java: a && b || !c
来源：http://ol.newstarts.cn

Go:   a && b || !c
来源：http://fx.szsharing.cn

Ruby: a && b || !c
来源：http://mm.jianghongdianzi.cn

C#:   a && b || !c
来源：http://ub.szxytkj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jn.jianghongdianzi.cn

Py:   if not data: return
来源：http://uk.shtwfgs.cn

PHP:  if (!$data) { return; }
来源：http://fd.hnjuh.cn

JS:   if (!data) return;
来源：http://bp.nszjky.cn

TS:   if (!data) return;
来源：http://ih.wgjwhj.cn

Java: if (data == null) return;
来源：http://gs.lnxyls.cn

Go:   if data == nil { return }
来源：http://sw.shxzskj.cn

Ruby: return if data.nil?
来源：http://su.huanxung.cn

C#:   if (data == null) return;
来源：http://hx.haigaiapp.cn

================================================================================
来源：http://vj.panjiajie.cn

C. 函数与作用域
来源：http://fv.shtwfgs.cn

================================================================================
来源：http://lx.shtwfgs.cn

[C01] 定义函数
来源：http://fa.hnjuh.cn

Py:   def add(a, b): return a + b
来源：http://am.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mw.shtwfgs.cn

JS:   function add(a, b) { return a + b; }
来源：http://my.panjiajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mk.9csxet.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ij.newstarts.cn

Go:   func add(a, b int) int { return a + b }
来源：http://nx.colortex.cn

Ruby: def add(a, b); a + b; end
来源：http://ss.shtwfgs.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ok.jctech888.com.cn

[C02] 默认参数
来源：http://nk.bjjhwx.cn

Py:   def greet(name="World"): return name
来源：http://wq.huixinmuqiang.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://eh.9csxet.cn

JS:   function greet(name = "World") { return name; }
来源：http://ig.jianghongdianzi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ld.hahajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wj.colortex.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nn.panjiajie.cn

Ruby: def greet(name = "World") = name
来源：http://zd.szsharing.cn

C#:   string Greet(string name = "World") => name;
来源：http://lv.lnxyls.cn

[C03] 可变参数
来源：http://rh.szxytkj.cn

Py:   def total(*args): return sum(args)
来源：http://ne.hnjuh.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fy.muxihuayi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xd.shxzskj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ji.yuntaijiaju.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yi.bookmarksfly.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fm.muxihuayi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://jv.bookmarksfly.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ag.9csxet.cn

[C04] 命名参数 / 关键字参数
来源：http://by.9csxet.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://el.yuexingan06.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://um.nszjky.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qj.huixinmuqiang.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://oc.shxzskj.cn

Java: // 无：用 Builder 模式或 record
来源：http://zk.chemitech.net.cn

Go:   // 无：用配置结构体参数
来源：http://nt.nszjky.cn

Ruby: f(a: 1, b: 2)
来源：http://zs.jianghongdianzi.cn

C#:   f(a: 1, b: 2)
来源：http://sf.haigaiapp.cn

[C05] 返回多个值
来源：http://br.lnxyls.cn

Py:   return a, b
来源：http://re.colortex.cn

PHP:  return [$a, $b];
来源：http://ma.huixiangedu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://bi.asd995.cn

TS:   return { a, b };
来源：http://to.bookmarksfly.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://my.yuexingan06.cn

Go:   return a, b
来源：http://kb.hahajie.cn

Ruby: return a, b
来源：http://bc.hnjuh.cn

C#:   return (a, b);              // ValueTuple
来源：http://pd.shxzskj.cn

[C06] 匿名函数 / lambda
来源：http://hs.szsharing.cn

Py:   square = lambda x: x * x
来源：http://qm.hahajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://nf.521024.cn

JS:   const square = x => x * x;
来源：http://vt.jianghongdianzi.cn

TS:   const square = (x: number): number => x * x;
来源：http://xh.nszjky.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gk.yuntaijiaju.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rn.wgjwhj.cn

Ruby: square = ->(x) { x * x }
来源：http://vf.chemitech.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bz.szxytkj.cn

[C07] 把函数作为参数传入
来源：http://kk.huixiangedu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sa.muxihuayi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://yv.szxytkj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ch.lnxyls.cn

TS:   arr.map(String)
来源：http://yv.haigaiapp.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zx.bookmarksfly.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yy.hnjuh.cn

Ruby: arr.map(&:upcase)
来源：http://cf.asd995.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://to.panjiajie.cn

[C08] 闭包
来源：http://vl.szxytkj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fz.shxzskj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nm.haigaiapp.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nu.szsharing.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qx.521024.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ev.huixiangedu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fz.gzmigu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rc.chemitech.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gf.gzmigu.cn

[C09] 递归
来源：http://br.colortex.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yt.yuexingan06.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ks.hnjuh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kk.huixinmuqiang.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://on.newstarts.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tr.chemitech.net.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nd.bjjhwx.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://re.colortex.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ot.hahajie.cn

[C10] 变量作用域
来源：http://jj.lnxyls.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fy.hnjuh.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://go.asd995.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cl.jctech888.com.cn

TS:   同 JS
来源：http://eu.jctech888.com.cn

Java: 方法内为块级作用域
来源：http://qz.shxzukj.cn

Go:   花括号块级作用域
来源：http://ha.huixinmuqiang.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ur.shtwfgs.cn

C#:   块级作用域
来源：http://my.lnxyls.cn

[C11] 模块导入与导出
来源：http://zf.shtwfgs.cn

Py:   from module import func
来源：http://ti.gzmigu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://cl.haigaiapp.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://en.shxzukj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://oc.jianghongdianzi.cn

Java: import java.util.List;
来源：http://ax.bjjhwx.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ja.huixiangedu.cn

Ruby: require "json"; require_relative "./util"
来源：http://yp.muxihuayi.cn

C#:   using System.Text;
来源：http://nm.bjjhwx.cn

[C12] 立即执行函数 IIFE
来源：http://bq.shxzukj.cn

Py:   (lambda: print("run"))()
来源：http://iu.9csxet.cn

PHP:  (function () { echo "run"; })();
来源：http://ij.nicolike.cn

JS:   (() => { console.log("run"); })();
来源：http://cw.bjjhwx.cn

TS:   (() => { console.log("run"); })();
来源：http://dw.bjjhwx.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jx.9csxet.cn

Go:   func() { fmt.Println("run") }()
来源：http://ox.wgjwhj.cn

Ruby: -> { puts "run" }.call
来源：http://em.jianghongdianzi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://kz.asd995.cn

[C13] 类型声明 / 类型注解
来源：http://lp.shxzukj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hc.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rj.muxihuayi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gn.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xz.gzmigu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wf.jctech888.com.cn

Go:   func add(a, b int) int
来源：http://mm.huanxung.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ar.shxzukj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cc.lnxyls.cn

[C14] 泛型函数
来源：http://bu.521024.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://an.muxihuayi.cn

PHP:  // 无泛型
来源：http://oh.chemitech.net.cn

JS:   // 无泛型
来源：http://ed.huixiangedu.cn


<!-- 参考信息 -->