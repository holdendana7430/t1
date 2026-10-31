代发 wailian999

C#:   s.Length
来源：http://eh.bjjhwx.cn

[A23] 大小写转换
来源：http://ni.9csxet.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://mb.gzmigu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dv.colortex.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://lw.9csxet.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fr.huixiangedu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://af.521024.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qy.asd995.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dd.huixinmuqiang.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://wv.colortex.cn

[A24] 去除首尾空白
来源：http://rl.muxihuayi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jq.yuexingan06.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xz.chemitech.net.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qo.hnjuh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qn.colortex.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://iy.szxytkj.cn

Go:   strings.TrimSpace(s)
来源：http://zx.yuntaijiaju.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qu.chemitech.net.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://aa.asd995.cn

[A25] 字符串比较
来源：http://xp.yuntaijiaju.cn

Py:   s1 == s2; s1 != s2
来源：http://ll.huanxung.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zl.haigaiapp.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xf.szsharing.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yf.521024.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://sn.chemitech.net.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pc.haigaiapp.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://jz.huixiangedu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jg.huixinmuqiang.cn

[A26] 类型转换总览
来源：http://dc.yuntaijiaju.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qj.huanxung.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qi.shxzukj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bj.huixiangedu.cn

TS:   Number() String() Boolean() x as number
来源：http://kn.shtwfgs.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://sh.newstarts.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ga.gzmigu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ez.asd995.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pc.hahajie.cn

================================================================================
来源：http://zt.521024.cn

B. 流程控制
来源：http://yo.colortex.cn

================================================================================
来源：http://cm.chemitech.net.cn

[B01] 条件判断 if / else
来源：http://cj.huanxung.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xd.521024.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sr.chemitech.net.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://el.yuntaijiaju.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://es.shtwfgs.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ae.jctech888.com.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://td.bjjhwx.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gw.newstarts.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fu.muxihuayi.cn

[B02] 多分支 else if / elif
来源：http://tq.szxytkj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ms.9csxet.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tn.jctech888.com.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ut.szsharing.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ow.szsharing.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ev.chemitech.net.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ts.yuntaijiaju.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nw.panjiajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ub.bookmarksfly.cn

[B03] switch / match / case
来源：http://wh.nicolike.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vl.bjjhwx.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ie.panjiajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ji.shxzukj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://an.shxzukj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qu.chemitech.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mo.huixinmuqiang.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zf.newstarts.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lp.bjjhwx.cn

[B04] for 计数循环
来源：http://ex.muxihuayi.cn

Py:   for i in range(10): print(i)
来源：http://cn.asd995.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://in.gzmigu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wt.huixiangedu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vj.hnjuh.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hg.huixiangedu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nl.colortex.cn

Ruby: 10.times { |i| puts i }
来源：http://co.chemitech.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pr.shxzukj.cn

[B05] 遍历数组 / 列表
来源：http://pj.huanxung.cn

Py:   for item in arr: print(item)
来源：http://wn.jianghongdianzi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cw.hnjuh.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qa.gzmigu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://oi.nszjky.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qo.chemitech.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zl.nicolike.cn

Ruby: arr.each { |item| puts item }
来源：http://aj.huixinmuqiang.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ho.bjjhwx.cn

[B06] 遍历字典 / 对象
来源：http://hq.jianghongdianzi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ne.muxihuayi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gn.hnjuh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jc.yuntaijiaju.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zl.shxzskj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yl.9csxet.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rj.szxytkj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pm.yuexingan06.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pg.szsharing.cn

[B07] while 循环
来源：http://si.chemitech.net.cn

Py:   while i < 10: i += 1
来源：http://xl.bookmarksfly.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ty.nicolike.cn

JS:   while (i < 10) { i++; }
来源：http://yu.muxihuayi.cn

TS:   while (i < 10) { i++; }
来源：http://mt.521024.cn

Java: while (i < 10) { i++; }
来源：http://so.asd995.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://im.nszjky.cn

Ruby: while i < 10; i += 1; end
来源：http://cm.hahajie.cn

C#:   while (i < 10) { i++; }
来源：http://dq.panjiajie.cn

[B08] do-while（至少执行一次）
来源：http://dn.asd995.cn

Py:   # 无 do-while：用 while True + break
来源：http://vz.szxytkj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://yy.chemitech.net.cn

JS:   do { i++; } while (i < 10);
来源：http://pz.lnxyls.cn

TS:   do { i++; } while (i < 10);
来源：http://mm.wgjwhj.cn

Java: do { i++; } while (i < 10);
来源：http://zg.yuexingan06.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ou.szsharing.cn

Ruby: begin; i += 1; end while i < 10
来源：http://my.521024.cn

C#:   do { i++; } while (i < 10);
来源：http://me.521024.cn

[B09] break 与 continue
来源：http://rn.yuexingan06.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://st.9csxet.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jd.chemitech.net.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jn.shxzskj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://df.muxihuayi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://id.jctech888.com.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://on.hnjuh.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://en.szsharing.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vv.lnxyls.cn

[B10] 遍历同时拿索引
来源：http://dv.hnjuh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jj.9csxet.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zc.shtwfgs.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jh.szxytkj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ey.szsharing.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vl.haigaiapp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cx.521024.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ty.newstarts.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://il.colortex.cn

[B11] 生成数字序列 / 区间
来源：http://be.521024.cn

Py:   list(range(0, 10, 2))
来源：http://zb.yuexingan06.cn

PHP:  range(0, 10, 2);
来源：http://vt.9csxet.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rt.nszjky.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uf.hahajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rk.yuexingan06.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://el.panjiajie.cn

Ruby: (0...10).step(2).to_a
来源：http://du.jctech888.com.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fq.muxihuayi.cn

[B12] 跳出多层循环
来源：http://tz.shxzukj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://vz.hahajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mr.shtwfgs.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ow.colortex.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pv.lnxyls.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dj.szxytkj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ze.yuexingan06.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hr.huanxung.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tr.yuntaijiaju.cn

[B13] 判断是否为数字
来源：http://oo.yuexingan06.cn

Py:   isinstance(x, (int, float))
来源：http://qf.huixinmuqiang.cn

PHP:  is_numeric($x)
来源：http://vd.jctech888.com.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ck.huixinmuqiang.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iz.huixiangedu.cn

Java: x instanceof Number
来源：http://vg.521024.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wj.chemitech.net.cn

Ruby: x.is_a?(Numeric)
来源：http://xm.hahajie.cn

C#:   x is int or double or decimal
来源：http://tn.haigaiapp.cn

[B14] 判断值是否在集合内
来源：http://jj.jctech888.com.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://io.asd995.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ag.bjjhwx.cn

JS:   [1, 2, 3].includes(x)
来源：http://hu.shtwfgs.cn

TS:   [1, 2, 3].includes(x)
来源：http://po.bjjhwx.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://iv.nszjky.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://di.nicolike.cn

Ruby: [1, 2, 3].include?(x)
来源：http://yf.wgjwhj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pd.haigaiapp.cn

[B15] 布尔运算与取反
来源：http://ah.asd995.cn

Py:   a and b or not c
来源：http://ix.gzmigu.cn

PHP:  $a && $b || !$c
来源：http://zt.yuexingan06.cn

JS:   a && b || !c
来源：http://aw.haigaiapp.cn

TS:   a && b || !c
来源：http://ef.panjiajie.cn

Java: a && b || !c
来源：http://zu.newstarts.cn

Go:   a && b || !c
来源：http://pf.hahajie.cn

Ruby: a && b || !c
来源：http://mm.szsharing.cn

C#:   a && b || !c
来源：http://om.lnxyls.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xd.521024.cn

Py:   if not data: return
来源：http://ik.bjjhwx.cn

PHP:  if (!$data) { return; }
来源：http://lw.colortex.cn

JS:   if (!data) return;
来源：http://tj.bookmarksfly.cn

TS:   if (!data) return;
来源：http://yf.9csxet.cn

Java: if (data == null) return;
来源：http://wp.huixiangedu.cn

Go:   if data == nil { return }
来源：http://ia.nszjky.cn

Ruby: return if data.nil?
来源：http://le.yuntaijiaju.cn

C#:   if (data == null) return;
来源：http://ec.newstarts.cn

================================================================================
来源：http://rt.szxytkj.cn

C. 函数与作用域
来源：http://ht.521024.cn

================================================================================
来源：http://ry.haigaiapp.cn

[C01] 定义函数
来源：http://ll.newstarts.cn

Py:   def add(a, b): return a + b
来源：http://vx.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dr.asd995.cn

JS:   function add(a, b) { return a + b; }
来源：http://qt.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vn.gzmigu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hs.hahajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://cc.shxzskj.cn

Ruby: def add(a, b); a + b; end
来源：http://ph.gzmigu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kc.9csxet.cn

[C02] 默认参数
来源：http://pz.jctech888.com.cn

Py:   def greet(name="World"): return name
来源：http://xs.jianghongdianzi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lo.lnxyls.cn

JS:   function greet(name = "World") { return name; }
来源：http://rw.szxytkj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://uo.muxihuayi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ff.yuntaijiaju.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ti.haigaiapp.cn

Ruby: def greet(name = "World") = name
来源：http://ee.newstarts.cn

C#:   string Greet(string name = "World") => name;
来源：http://lk.szsharing.cn

[C03] 可变参数
来源：http://sf.jianghongdianzi.cn

Py:   def total(*args): return sum(args)
来源：http://zv.jianghongdianzi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://md.521024.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ui.szsharing.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mf.hnjuh.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ch.jctech888.com.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vl.huixiangedu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ja.shxzskj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dz.shtwfgs.cn

[C04] 命名参数 / 关键字参数
来源：http://hz.asd995.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ki.shxzukj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ka.wgjwhj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mk.panjiajie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jt.huixinmuqiang.cn

Java: // 无：用 Builder 模式或 record
来源：http://sc.muxihuayi.cn

Go:   // 无：用配置结构体参数
来源：http://mq.gzmigu.cn

Ruby: f(a: 1, b: 2)
来源：http://hw.jianghongdianzi.cn

C#:   f(a: 1, b: 2)
来源：http://ge.9csxet.cn

[C05] 返回多个值
来源：http://jd.lnxyls.cn

Py:   return a, b
来源：http://is.huixinmuqiang.cn

PHP:  return [$a, $b];
来源：http://cd.szsharing.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://za.haigaiapp.cn

TS:   return { a, b };
来源：http://sg.bjjhwx.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://se.shxzukj.cn

Go:   return a, b
来源：http://li.panjiajie.cn

Ruby: return a, b
来源：http://ok.huanxung.cn

C#:   return (a, b);              // ValueTuple
来源：http://kh.hnjuh.cn

[C06] 匿名函数 / lambda
来源：http://cr.bjjhwx.cn

Py:   square = lambda x: x * x
来源：http://uz.haigaiapp.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wk.huixinmuqiang.cn

JS:   const square = x => x * x;
来源：http://zh.jctech888.com.cn

TS:   const square = (x: number): number => x * x;
来源：http://yk.newstarts.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://te.huanxung.cn

Go:   sq := func(x int) int { return x * x }
来源：http://lx.hahajie.cn

Ruby: square = ->(x) { x * x }
来源：http://yn.521024.cn

C#:   Func<int, int> square = x => x * x;
来源：http://sj.yuexingan06.cn

[C07] 把函数作为参数传入
来源：http://ay.jianghongdianzi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://uo.newstarts.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ei.gzmigu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yb.szsharing.cn

TS:   arr.map(String)
来源：http://el.colortex.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ft.hnjuh.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uo.haigaiapp.cn

Ruby: arr.map(&:upcase)
来源：http://hh.chemitech.net.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hk.huanxung.cn

[C08] 闭包
来源：http://sv.bjjhwx.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ss.jctech888.com.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mr.shtwfgs.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gr.hnjuh.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tn.hnjuh.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bt.huixiangedu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qa.newstarts.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yq.shxzukj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ht.szxytkj.cn

[C09] 递归
来源：http://xq.lnxyls.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cc.muxihuayi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mj.gzmigu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ue.jctech888.com.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://js.shxzskj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tg.wgjwhj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kr.panjiajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tc.yuexingan06.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bk.haigaiapp.cn

[C10] 变量作用域
来源：http://uc.jianghongdianzi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ib.hahajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ox.shxzukj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tl.colortex.cn

TS:   同 JS
来源：http://lb.jctech888.com.cn

Java: 方法内为块级作用域
来源：http://cy.chemitech.net.cn

Go:   花括号块级作用域
来源：http://ud.gzmigu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dq.shtwfgs.cn

C#:   块级作用域
来源：http://ry.huixinmuqiang.cn

[C11] 模块导入与导出
来源：http://yf.colortex.cn

Py:   from module import func
来源：http://rp.shtwfgs.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://em.jianghongdianzi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fw.gzmigu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cm.wgjwhj.cn

Java: import java.util.List;
来源：http://wy.yuexingan06.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fq.jctech888.com.cn

Ruby: require "json"; require_relative "./util"
来源：http://rt.9csxet.cn

C#:   using System.Text;
来源：http://vo.hnjuh.cn

[C12] 立即执行函数 IIFE
来源：http://ud.huixinmuqiang.cn

Py:   (lambda: print("run"))()
来源：http://qh.521024.cn

PHP:  (function () { echo "run"; })();
来源：http://ka.yuntaijiaju.cn

JS:   (() => { console.log("run"); })();
来源：http://bq.muxihuayi.cn

TS:   (() => { console.log("run"); })();
来源：http://uu.jianghongdianzi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lj.bjjhwx.cn

Go:   func() { fmt.Println("run") }()
来源：http://gd.hnjuh.cn

Ruby: -> { puts "run" }.call
来源：http://jw.bjjhwx.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fg.huixiangedu.cn

[C13] 类型声明 / 类型注解
来源：http://kw.chemitech.net.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cj.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nz.bjjhwx.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sv.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vd.9csxet.cn


<!-- 参考信息 -->