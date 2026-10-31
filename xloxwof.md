代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rk.haigaiapp.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://bt.nicolike.cn

[A24] 去除首尾空白
来源：http://ku.521024.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://uy.hnjuh.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ks.huixiangedu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uj.9csxet.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bj.wgjwhj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cn.chemitech.net.cn

Go:   strings.TrimSpace(s)
来源：http://df.colortex.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zi.shxzukj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://be.yuexingan06.cn

[A25] 字符串比较
来源：http://ua.muxihuayi.cn

Py:   s1 == s2; s1 != s2
来源：http://hs.haigaiapp.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nn.shxzskj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://sm.hahajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bv.shtwfgs.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tp.bjjhwx.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://va.yuexingan06.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rw.panjiajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wq.szsharing.cn

[A26] 类型转换总览
来源：http://xl.shxzukj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ry.colortex.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ya.yuexingan06.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ax.shtwfgs.cn

TS:   Number() String() Boolean() x as number
来源：http://dz.shxzskj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xd.shxzukj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lu.wgjwhj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://re.shtwfgs.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zk.huanxung.cn

================================================================================
来源：http://du.newstarts.cn

B. 流程控制
来源：http://yf.shtwfgs.cn

================================================================================
来源：http://dm.szsharing.cn

[B01] 条件判断 if / else
来源：http://fe.colortex.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ut.shxzukj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wf.shxzukj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rd.asd995.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://cg.panjiajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qp.gzmigu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://sd.szsharing.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dv.hnjuh.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kp.szxytkj.cn

[B02] 多分支 else if / elif
来源：http://iv.yuntaijiaju.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://an.nicolike.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vw.colortex.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://os.panjiajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sp.yuexingan06.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://by.shtwfgs.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ug.newstarts.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ca.jctech888.com.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ws.nicolike.cn

[B03] switch / match / case
来源：http://fk.bjjhwx.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wu.yuntaijiaju.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ey.chemitech.net.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tg.chemitech.net.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wx.jianghongdianzi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zj.yuntaijiaju.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fs.nicolike.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://br.szxytkj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ca.9csxet.cn

[B04] for 计数循环
来源：http://hc.panjiajie.cn

Py:   for i in range(10): print(i)
来源：http://bm.muxihuayi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vl.bjjhwx.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bl.colortex.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ik.lnxyls.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rw.gzmigu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ss.huixiangedu.cn

Ruby: 10.times { |i| puts i }
来源：http://uz.huixinmuqiang.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hu.hnjuh.cn

[B05] 遍历数组 / 列表
来源：http://ch.chemitech.net.cn

Py:   for item in arr: print(item)
来源：http://gb.9csxet.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cb.shtwfgs.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://jd.nicolike.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://od.shxzukj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://op.shxzskj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tw.521024.cn

Ruby: arr.each { |item| puts item }
来源：http://td.huanxung.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gu.yuntaijiaju.cn

[B06] 遍历字典 / 对象
来源：http://uv.hahajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://kv.szxytkj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://te.521024.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zb.nszjky.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://px.wgjwhj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dd.521024.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qu.asd995.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mo.szxytkj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ot.9csxet.cn

[B07] while 循环
来源：http://sc.jctech888.com.cn

Py:   while i < 10: i += 1
来源：http://nk.haigaiapp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ts.huanxung.cn

JS:   while (i < 10) { i++; }
来源：http://ro.asd995.cn

TS:   while (i < 10) { i++; }
来源：http://rc.hnjuh.cn

Java: while (i < 10) { i++; }
来源：http://qo.huixinmuqiang.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ji.521024.cn

Ruby: while i < 10; i += 1; end
来源：http://mj.yuntaijiaju.cn

C#:   while (i < 10) { i++; }
来源：http://wv.newstarts.cn

[B08] do-while（至少执行一次）
来源：http://yn.lnxyls.cn

Py:   # 无 do-while：用 while True + break
来源：http://cu.hnjuh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jv.huanxung.cn

JS:   do { i++; } while (i < 10);
来源：http://zh.huanxung.cn

TS:   do { i++; } while (i < 10);
来源：http://fu.gzmigu.cn

Java: do { i++; } while (i < 10);
来源：http://nt.szsharing.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://cv.shxzskj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ia.yuexingan06.cn

C#:   do { i++; } while (i < 10);
来源：http://zq.huixiangedu.cn

[B09] break 与 continue
来源：http://jf.shtwfgs.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ad.huanxung.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sc.hahajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xs.521024.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gq.shxzukj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gs.newstarts.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ra.wgjwhj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jl.newstarts.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ji.hnjuh.cn

[B10] 遍历同时拿索引
来源：http://bx.newstarts.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://du.haigaiapp.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ph.bookmarksfly.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://un.szxytkj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kj.muxihuayi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fa.muxihuayi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://oq.asd995.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://za.gzmigu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mx.hahajie.cn

[B11] 生成数字序列 / 区间
来源：http://bf.asd995.cn

Py:   list(range(0, 10, 2))
来源：http://la.newstarts.cn

PHP:  range(0, 10, 2);
来源：http://yr.bookmarksfly.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ln.asd995.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ih.yuntaijiaju.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rm.nszjky.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hq.521024.cn

Ruby: (0...10).step(2).to_a
来源：http://ae.yuntaijiaju.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pd.nszjky.cn

[B12] 跳出多层循环
来源：http://qd.jctech888.com.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://md.yuexingan06.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://iw.asd995.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wc.hnjuh.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.huixiangedu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://te.colortex.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hw.shxzskj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jm.shxzukj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sy.nicolike.cn

[B13] 判断是否为数字
来源：http://yi.chemitech.net.cn

Py:   isinstance(x, (int, float))
来源：http://px.nicolike.cn

PHP:  is_numeric($x)
来源：http://rf.lnxyls.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bh.lnxyls.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ip.shtwfgs.cn

Java: x instanceof Number
来源：http://nj.521024.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mj.huanxung.cn

Ruby: x.is_a?(Numeric)
来源：http://tg.huixiangedu.cn

C#:   x is int or double or decimal
来源：http://mn.huanxung.cn

[B14] 判断值是否在集合内
来源：http://ac.wgjwhj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ci.bookmarksfly.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xg.bookmarksfly.cn

JS:   [1, 2, 3].includes(x)
来源：http://fq.hnjuh.cn

TS:   [1, 2, 3].includes(x)
来源：http://rz.chemitech.net.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://to.nicolike.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://va.gzmigu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fb.wgjwhj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ll.hahajie.cn

[B15] 布尔运算与取反
来源：http://lq.521024.cn

Py:   a and b or not c
来源：http://he.bjjhwx.cn

PHP:  $a && $b || !$c
来源：http://uq.jianghongdianzi.cn

JS:   a && b || !c
来源：http://cc.jctech888.com.cn

TS:   a && b || !c
来源：http://ko.hahajie.cn

Java: a && b || !c
来源：http://wn.huanxung.cn

Go:   a && b || !c
来源：http://ld.chemitech.net.cn

Ruby: a && b || !c
来源：http://as.asd995.cn

C#:   a && b || !c
来源：http://uw.chemitech.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ah.shxzskj.cn

Py:   if not data: return
来源：http://zs.colortex.cn

PHP:  if (!$data) { return; }
来源：http://mu.asd995.cn

JS:   if (!data) return;
来源：http://wg.newstarts.cn

TS:   if (!data) return;
来源：http://nq.haigaiapp.cn

Java: if (data == null) return;
来源：http://tk.muxihuayi.cn

Go:   if data == nil { return }
来源：http://xa.jianghongdianzi.cn

Ruby: return if data.nil?
来源：http://pt.shtwfgs.cn

C#:   if (data == null) return;
来源：http://rb.yuexingan06.cn

================================================================================
来源：http://ss.bjjhwx.cn

C. 函数与作用域
来源：http://ld.szxytkj.cn

================================================================================
来源：http://le.jctech888.com.cn

[C01] 定义函数
来源：http://kx.huanxung.cn

Py:   def add(a, b): return a + b
来源：http://np.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gm.521024.cn

JS:   function add(a, b) { return a + b; }
来源：http://wq.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://os.huanxung.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wl.521024.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ep.yuntaijiaju.cn

Ruby: def add(a, b); a + b; end
来源：http://tj.asd995.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://co.colortex.cn

[C02] 默认参数
来源：http://mb.huanxung.cn

Py:   def greet(name="World"): return name
来源：http://qb.9csxet.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fv.yuntaijiaju.cn

JS:   function greet(name = "World") { return name; }
来源：http://bf.yuntaijiaju.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://dl.hnjuh.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://je.jianghongdianzi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ab.shxzskj.cn

Ruby: def greet(name = "World") = name
来源：http://gf.szsharing.cn

C#:   string Greet(string name = "World") => name;
来源：http://ik.jianghongdianzi.cn

[C03] 可变参数
来源：http://sh.muxihuayi.cn

Py:   def total(*args): return sum(args)
来源：http://zz.yuexingan06.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zz.huixiangedu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pp.yuntaijiaju.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fm.hnjuh.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ry.colortex.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vx.colortex.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qq.huixiangedu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bw.bookmarksfly.cn

[C04] 命名参数 / 关键字参数
来源：http://rt.muxihuayi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ef.panjiajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://by.newstarts.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sd.haigaiapp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uf.jctech888.com.cn

Java: // 无：用 Builder 模式或 record
来源：http://vv.hahajie.cn

Go:   // 无：用配置结构体参数
来源：http://qs.bjjhwx.cn

Ruby: f(a: 1, b: 2)
来源：http://gh.bookmarksfly.cn

C#:   f(a: 1, b: 2)
来源：http://js.jianghongdianzi.cn

[C05] 返回多个值
来源：http://pl.shxzskj.cn

Py:   return a, b
来源：http://og.shxzukj.cn

PHP:  return [$a, $b];
来源：http://th.szsharing.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wv.bookmarksfly.cn

TS:   return { a, b };
来源：http://uv.jctech888.com.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xb.nicolike.cn

Go:   return a, b
来源：http://jz.shxzskj.cn

Ruby: return a, b
来源：http://fk.jctech888.com.cn

C#:   return (a, b);              // ValueTuple
来源：http://vq.szsharing.cn

[C06] 匿名函数 / lambda
来源：http://ef.huanxung.cn

Py:   square = lambda x: x * x
来源：http://nc.shxzukj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ft.yuexingan06.cn

JS:   const square = x => x * x;
来源：http://ky.huanxung.cn

TS:   const square = (x: number): number => x * x;
来源：http://zz.shtwfgs.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sa.jctech888.com.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gx.bookmarksfly.cn

Ruby: square = ->(x) { x * x }
来源：http://bi.asd995.cn

C#:   Func<int, int> square = x => x * x;
来源：http://yn.panjiajie.cn

[C07] 把函数作为参数传入
来源：http://xy.huixinmuqiang.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pa.521024.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zg.huixiangedu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pa.bjjhwx.cn

TS:   arr.map(String)
来源：http://jg.chemitech.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://le.shxzukj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mf.gzmigu.cn

Ruby: arr.map(&:upcase)
来源：http://rk.bjjhwx.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cs.asd995.cn

[C08] 闭包
来源：http://iv.huixiangedu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ds.huixinmuqiang.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lg.bookmarksfly.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ti.shxzskj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vl.panjiajie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ef.lnxyls.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://it.bjjhwx.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ig.yuexingan06.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ii.wgjwhj.cn

[C09] 递归
来源：http://mx.newstarts.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://um.shxzskj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zw.521024.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wh.huanxung.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bs.huixinmuqiang.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bo.shxzskj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mu.hahajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yr.haigaiapp.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ft.hnjuh.cn

[C10] 变量作用域
来源：http://hx.huixiangedu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pq.521024.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ca.nicolike.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ks.shtwfgs.cn

TS:   同 JS
来源：http://vc.newstarts.cn

Java: 方法内为块级作用域
来源：http://bt.bjjhwx.cn

Go:   花括号块级作用域
来源：http://nu.bjjhwx.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hn.asd995.cn

C#:   块级作用域
来源：http://gs.jctech888.com.cn

[C11] 模块导入与导出
来源：http://ve.colortex.cn

Py:   from module import func
来源：http://ws.9csxet.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pe.jctech888.com.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://cv.hnjuh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bl.yuexingan06.cn

Java: import java.util.List;
来源：http://ju.yuntaijiaju.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tf.shtwfgs.cn

Ruby: require "json"; require_relative "./util"
来源：http://gk.hnjuh.cn

C#:   using System.Text;
来源：http://nk.nszjky.cn

[C12] 立即执行函数 IIFE
来源：http://wj.asd995.cn

Py:   (lambda: print("run"))()
来源：http://zw.szxytkj.cn

PHP:  (function () { echo "run"; })();
来源：http://ba.nszjky.cn

JS:   (() => { console.log("run"); })();
来源：http://sg.huixiangedu.cn

TS:   (() => { console.log("run"); })();
来源：http://qh.bookmarksfly.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cg.9csxet.cn

Go:   func() { fmt.Println("run") }()
来源：http://yx.wgjwhj.cn

Ruby: -> { puts "run" }.call
来源：http://vk.nicolike.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fa.lnxyls.cn

[C13] 类型声明 / 类型注解
来源：http://hu.yuexingan06.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jq.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bv.bookmarksfly.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kh.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tb.bjjhwx.cn

Java: int add(int a, int b) { return a + b; }
来源：http://op.shtwfgs.cn

Go:   func add(a, b int) int
来源：http://mm.521024.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fs.shxzskj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ps.hahajie.cn

[C14] 泛型函数
来源：http://nf.jctech888.com.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ng.shxzskj.cn

PHP:  // 无泛型
来源：http://lk.nicolike.cn

JS:   // 无泛型
来源：http://qa.newstarts.cn


<!-- 参考信息 -->