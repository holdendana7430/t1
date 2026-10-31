代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yj.huixinmuqiang.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xs.szxytkj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mv.nszjky.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kw.szxytkj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dr.huixiangedu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://cj.huanxung.cn

[A24] 去除首尾空白
来源：http://iq.panjiajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ie.huixinmuqiang.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://to.hnjuh.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sc.muxihuayi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mq.huixiangedu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://yk.nicolike.cn

Go:   strings.TrimSpace(s)
来源：http://jc.hnjuh.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://sx.muxihuayi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://as.jctech888.com.cn

[A25] 字符串比较
来源：http://fa.muxihuayi.cn

Py:   s1 == s2; s1 != s2
来源：http://ad.colortex.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zg.bjjhwx.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ss.haigaiapp.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://br.colortex.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://um.jctech888.com.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hr.nicolike.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ia.shxzskj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fl.huanxung.cn

[A26] 类型转换总览
来源：http://gl.hnjuh.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ft.9csxet.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uw.shxzukj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gr.shxzukj.cn

TS:   Number() String() Boolean() x as number
来源：http://gz.yuntaijiaju.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ns.shxzskj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pp.gzmigu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://qe.szxytkj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kp.haigaiapp.cn

================================================================================
来源：http://vi.yuexingan06.cn

B. 流程控制
来源：http://kc.colortex.cn

================================================================================
来源：http://qm.szxytkj.cn

[B01] 条件判断 if / else
来源：http://ol.huixiangedu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vs.wgjwhj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://aq.yuexingan06.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jp.521024.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hu.nszjky.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://fr.shxzukj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ur.521024.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bs.gzmigu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://so.yuntaijiaju.cn

[B02] 多分支 else if / elif
来源：http://iw.chemitech.net.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sh.gzmigu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qq.wgjwhj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://it.huixiangedu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kt.gzmigu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ex.szxytkj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hp.9csxet.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xs.asd995.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wg.bjjhwx.cn

[B03] switch / match / case
来源：http://qs.jianghongdianzi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rn.shxzskj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://am.521024.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://us.shtwfgs.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tt.asd995.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ge.shxzukj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tc.jianghongdianzi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://km.9csxet.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hs.shtwfgs.cn

[B04] for 计数循环
来源：http://dq.jctech888.com.cn

Py:   for i in range(10): print(i)
来源：http://os.haigaiapp.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qi.yuexingan06.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wh.yuexingan06.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cw.jianghongdianzi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://if.nicolike.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pf.haigaiapp.cn

Ruby: 10.times { |i| puts i }
来源：http://ot.yuntaijiaju.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ic.9csxet.cn

[B05] 遍历数组 / 列表
来源：http://fb.colortex.cn

Py:   for item in arr: print(item)
来源：http://aq.9csxet.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rf.bjjhwx.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://pe.bookmarksfly.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fl.jianghongdianzi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vj.hahajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cn.shtwfgs.cn

Ruby: arr.each { |item| puts item }
来源：http://tv.yuexingan06.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vg.shxzskj.cn

[B06] 遍历字典 / 对象
来源：http://qz.hahajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hd.hnjuh.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vt.huixinmuqiang.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dv.huixiangedu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://be.panjiajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ob.huixinmuqiang.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://aa.shxzskj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pf.shxzukj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://px.shtwfgs.cn

[B07] while 循环
来源：http://hi.wgjwhj.cn

Py:   while i < 10: i += 1
来源：http://ib.szxytkj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zo.lnxyls.cn

JS:   while (i < 10) { i++; }
来源：http://ni.chemitech.net.cn

TS:   while (i < 10) { i++; }
来源：http://yn.hnjuh.cn

Java: while (i < 10) { i++; }
来源：http://rr.yuexingan06.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ti.asd995.cn

Ruby: while i < 10; i += 1; end
来源：http://oo.muxihuayi.cn

C#:   while (i < 10) { i++; }
来源：http://mi.panjiajie.cn

[B08] do-while（至少执行一次）
来源：http://lu.chemitech.net.cn

Py:   # 无 do-while：用 while True + break
来源：http://sy.panjiajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xe.jctech888.com.cn

JS:   do { i++; } while (i < 10);
来源：http://vw.szxytkj.cn

TS:   do { i++; } while (i < 10);
来源：http://fu.panjiajie.cn

Java: do { i++; } while (i < 10);
来源：http://ux.yuexingan06.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xc.nicolike.cn

Ruby: begin; i += 1; end while i < 10
来源：http://sl.chemitech.net.cn

C#:   do { i++; } while (i < 10);
来源：http://jd.bjjhwx.cn

[B09] break 与 continue
来源：http://bg.newstarts.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://re.hnjuh.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ui.newstarts.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lq.szxytkj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zu.lnxyls.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ez.shxzskj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kf.521024.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://po.muxihuayi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bf.shtwfgs.cn

[B10] 遍历同时拿索引
来源：http://bh.gzmigu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ev.szxytkj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qy.shtwfgs.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wv.panjiajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nz.521024.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qx.szxytkj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pz.bjjhwx.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xc.9csxet.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cp.yuexingan06.cn

[B11] 生成数字序列 / 区间
来源：http://ry.nszjky.cn

Py:   list(range(0, 10, 2))
来源：http://uc.shtwfgs.cn

PHP:  range(0, 10, 2);
来源：http://oh.huanxung.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sp.9csxet.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://px.chemitech.net.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://is.haigaiapp.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yh.yuexingan06.cn

Ruby: (0...10).step(2).to_a
来源：http://tk.huanxung.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fs.nszjky.cn

[B12] 跳出多层循环
来源：http://vl.521024.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://az.hnjuh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://kz.shtwfgs.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mc.hahajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://av.bookmarksfly.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lu.jianghongdianzi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rs.colortex.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://km.huixinmuqiang.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lu.9csxet.cn

[B13] 判断是否为数字
来源：http://ou.shxzukj.cn

Py:   isinstance(x, (int, float))
来源：http://nj.colortex.cn

PHP:  is_numeric($x)
来源：http://ov.shxzskj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vn.panjiajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sa.yuexingan06.cn

Java: x instanceof Number
来源：http://zk.lnxyls.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xl.hahajie.cn

Ruby: x.is_a?(Numeric)
来源：http://ur.yuntaijiaju.cn

C#:   x is int or double or decimal
来源：http://nz.jctech888.com.cn

[B14] 判断值是否在集合内
来源：http://ko.haigaiapp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nf.newstarts.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yi.nszjky.cn

JS:   [1, 2, 3].includes(x)
来源：http://mt.shxzskj.cn

TS:   [1, 2, 3].includes(x)
来源：http://ta.haigaiapp.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://re.haigaiapp.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://os.9csxet.cn

Ruby: [1, 2, 3].include?(x)
来源：http://so.yuexingan06.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bp.jianghongdianzi.cn

[B15] 布尔运算与取反
来源：http://oe.521024.cn

Py:   a and b or not c
来源：http://dr.hahajie.cn

PHP:  $a && $b || !$c
来源：http://nh.muxihuayi.cn

JS:   a && b || !c
来源：http://jg.newstarts.cn

TS:   a && b || !c
来源：http://rb.9csxet.cn

Java: a && b || !c
来源：http://rp.chemitech.net.cn

Go:   a && b || !c
来源：http://nu.huanxung.cn

Ruby: a && b || !c
来源：http://ua.huanxung.cn

C#:   a && b || !c
来源：http://iy.huixiangedu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://mg.gzmigu.cn

Py:   if not data: return
来源：http://sc.hahajie.cn

PHP:  if (!$data) { return; }
来源：http://po.panjiajie.cn

JS:   if (!data) return;
来源：http://jc.newstarts.cn

TS:   if (!data) return;
来源：http://na.asd995.cn

Java: if (data == null) return;
来源：http://mn.jctech888.com.cn

Go:   if data == nil { return }
来源：http://jd.nszjky.cn

Ruby: return if data.nil?
来源：http://rz.chemitech.net.cn

C#:   if (data == null) return;
来源：http://nv.hnjuh.cn

================================================================================
来源：http://va.yuexingan06.cn

C. 函数与作用域
来源：http://pq.asd995.cn

================================================================================
来源：http://na.521024.cn

[C01] 定义函数
来源：http://rf.huanxung.cn

Py:   def add(a, b): return a + b
来源：http://hr.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pi.yuexingan06.cn

JS:   function add(a, b) { return a + b; }
来源：http://nn.panjiajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://py.colortex.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://et.yuexingan06.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rh.hahajie.cn

Ruby: def add(a, b); a + b; end
来源：http://nw.shtwfgs.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xf.wgjwhj.cn

[C02] 默认参数
来源：http://fs.9csxet.cn

Py:   def greet(name="World"): return name
来源：http://qs.shtwfgs.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tb.lnxyls.cn

JS:   function greet(name = "World") { return name; }
来源：http://cd.wgjwhj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qf.asd995.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://sh.521024.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fx.jctech888.com.cn

Ruby: def greet(name = "World") = name
来源：http://nx.newstarts.cn

C#:   string Greet(string name = "World") => name;
来源：http://cy.huanxung.cn

[C03] 可变参数
来源：http://pl.521024.cn

Py:   def total(*args): return sum(args)
来源：http://ac.hahajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yi.yuntaijiaju.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fc.huanxung.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://aw.jctech888.com.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cu.hahajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xu.newstarts.cn

Ruby: def total(*nums); nums.sum; end
来源：http://cn.muxihuayi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rq.9csxet.cn

[C04] 命名参数 / 关键字参数
来源：http://qh.newstarts.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ek.chemitech.net.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wu.colortex.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uz.hnjuh.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ka.muxihuayi.cn

Java: // 无：用 Builder 模式或 record
来源：http://cl.asd995.cn

Go:   // 无：用配置结构体参数
来源：http://du.szxytkj.cn

Ruby: f(a: 1, b: 2)
来源：http://zz.yuntaijiaju.cn

C#:   f(a: 1, b: 2)
来源：http://jx.huixiangedu.cn

[C05] 返回多个值
来源：http://pa.nszjky.cn

Py:   return a, b
来源：http://ax.jianghongdianzi.cn

PHP:  return [$a, $b];
来源：http://ql.nszjky.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ed.nicolike.cn

TS:   return { a, b };
来源：http://xq.hahajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ht.hahajie.cn

Go:   return a, b
来源：http://vx.jctech888.com.cn

Ruby: return a, b
来源：http://kr.9csxet.cn

C#:   return (a, b);              // ValueTuple
来源：http://cj.yuntaijiaju.cn

[C06] 匿名函数 / lambda
来源：http://uo.newstarts.cn

Py:   square = lambda x: x * x
来源：http://ba.jctech888.com.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ez.chemitech.net.cn

JS:   const square = x => x * x;
来源：http://oc.muxihuayi.cn

TS:   const square = (x: number): number => x * x;
来源：http://et.yuexingan06.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yu.hnjuh.cn

Go:   sq := func(x int) int { return x * x }
来源：http://un.yuntaijiaju.cn

Ruby: square = ->(x) { x * x }
来源：http://xv.yuntaijiaju.cn

C#:   Func<int, int> square = x => x * x;
来源：http://uc.huixiangedu.cn

[C07] 把函数作为参数传入
来源：http://hu.9csxet.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ra.lnxyls.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hh.asd995.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wu.yuexingan06.cn

TS:   arr.map(String)
来源：http://qh.haigaiapp.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cf.shtwfgs.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wp.shxzskj.cn

Ruby: arr.map(&:upcase)
来源：http://qw.hnjuh.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://vg.colortex.cn

[C08] 闭包
来源：http://vm.bookmarksfly.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fe.huixiangedu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://st.9csxet.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nj.chemitech.net.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ja.newstarts.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xr.huixinmuqiang.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jc.huixinmuqiang.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hn.bjjhwx.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yt.shtwfgs.cn

[C09] 递归
来源：http://sb.yuntaijiaju.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qh.yuexingan06.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gh.shtwfgs.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://us.wgjwhj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yt.huixinmuqiang.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fn.chemitech.net.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zl.nicolike.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://on.yuntaijiaju.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kv.nszjky.cn

[C10] 变量作用域
来源：http://dz.haigaiapp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vy.panjiajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ds.shxzukj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ve.panjiajie.cn

TS:   同 JS
来源：http://xh.shtwfgs.cn

Java: 方法内为块级作用域
来源：http://zx.newstarts.cn

Go:   花括号块级作用域
来源：http://cz.muxihuayi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lg.haigaiapp.cn

C#:   块级作用域
来源：http://he.huixinmuqiang.cn

[C11] 模块导入与导出
来源：http://pg.panjiajie.cn

Py:   from module import func
来源：http://gw.9csxet.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://eq.nicolike.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://no.huanxung.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wd.chemitech.net.cn

Java: import java.util.List;
来源：http://sv.huixinmuqiang.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ke.huanxung.cn

Ruby: require "json"; require_relative "./util"
来源：http://ba.nszjky.cn

C#:   using System.Text;
来源：http://ze.muxihuayi.cn

[C12] 立即执行函数 IIFE
来源：http://lb.hahajie.cn

Py:   (lambda: print("run"))()
来源：http://my.yuntaijiaju.cn

PHP:  (function () { echo "run"; })();
来源：http://nu.lnxyls.cn

JS:   (() => { console.log("run"); })();
来源：http://nb.wgjwhj.cn

TS:   (() => { console.log("run"); })();
来源：http://ph.yuntaijiaju.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sn.yuntaijiaju.cn

Go:   func() { fmt.Println("run") }()
来源：http://su.jctech888.com.cn

Ruby: -> { puts "run" }.call
来源：http://st.newstarts.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://hi.hahajie.cn

[C13] 类型声明 / 类型注解
来源：http://wa.jianghongdianzi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ct.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ax.521024.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ud.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rf.yuexingan06.cn

Java: int add(int a, int b) { return a + b; }
来源：http://uq.yuexingan06.cn

Go:   func add(a, b int) int
来源：http://ac.bookmarksfly.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kg.chemitech.net.cn

C#:   int Add(int a, int b) => a + b;
来源：http://re.muxihuayi.cn


<!-- 参考信息 -->