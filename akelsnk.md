代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wl.lnxyls.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://pp.bookmarksfly.cn

[A24] 去除首尾空白
来源：http://la.hahajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cc.bookmarksfly.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jr.chemitech.net.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gm.asd995.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zw.panjiajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://al.hnjuh.cn

Go:   strings.TrimSpace(s)
来源：http://ef.haigaiapp.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bv.haigaiapp.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://su.hnjuh.cn

[A25] 字符串比较
来源：http://ny.gzmigu.cn

Py:   s1 == s2; s1 != s2
来源：http://je.gzmigu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tf.nszjky.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bs.gzmigu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://sh.jctech888.com.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rz.muxihuayi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tf.nszjky.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://fr.hahajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fo.panjiajie.cn

[A26] 类型转换总览
来源：http://fn.panjiajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jk.muxihuayi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qm.huanxung.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jo.lnxyls.cn

TS:   Number() String() Boolean() x as number
来源：http://pq.521024.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hq.shxzukj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jv.huixinmuqiang.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://uk.asd995.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jz.shxzukj.cn

================================================================================
来源：http://as.yuexingan06.cn

B. 流程控制
来源：http://da.huanxung.cn

================================================================================
来源：http://uj.szxytkj.cn

[B01] 条件判断 if / else
来源：http://dr.asd995.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ka.gzmigu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hg.panjiajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yz.jctech888.com.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://de.521024.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ll.gzmigu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lt.nicolike.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ly.hnjuh.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://su.wgjwhj.cn

[B02] 多分支 else if / elif
来源：http://vd.huixiangedu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cb.wgjwhj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sz.newstarts.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://un.wgjwhj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yi.hnjuh.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oc.panjiajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vr.lnxyls.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ez.hnjuh.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://my.shxzskj.cn

[B03] switch / match / case
来源：http://fj.lnxyls.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nl.9csxet.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nu.jctech888.com.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bg.wgjwhj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yz.shxzukj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cj.9csxet.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ek.jctech888.com.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://os.bjjhwx.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bx.chemitech.net.cn

[B04] for 计数循环
来源：http://wj.lnxyls.cn

Py:   for i in range(10): print(i)
来源：http://ya.nszjky.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pz.huixinmuqiang.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qw.yuexingan06.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rp.9csxet.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lv.bookmarksfly.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gl.9csxet.cn

Ruby: 10.times { |i| puts i }
来源：http://xz.colortex.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tf.haigaiapp.cn

[B05] 遍历数组 / 列表
来源：http://oe.panjiajie.cn

Py:   for item in arr: print(item)
来源：http://hl.521024.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dc.hnjuh.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://my.asd995.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://vl.haigaiapp.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://uq.lnxyls.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kc.bjjhwx.cn

Ruby: arr.each { |item| puts item }
来源：http://wd.szsharing.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jj.yuntaijiaju.cn

[B06] 遍历字典 / 对象
来源：http://ir.nicolike.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://kv.chemitech.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fy.yuexingan06.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pd.asd995.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mw.szsharing.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mz.wgjwhj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ep.yuexingan06.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cd.bjjhwx.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gc.szsharing.cn

[B07] while 循环
来源：http://pg.shxzskj.cn

Py:   while i < 10: i += 1
来源：http://re.nicolike.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hg.yuntaijiaju.cn

JS:   while (i < 10) { i++; }
来源：http://on.szsharing.cn

TS:   while (i < 10) { i++; }
来源：http://wa.nicolike.cn

Java: while (i < 10) { i++; }
来源：http://dd.szxytkj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rl.huixinmuqiang.cn

Ruby: while i < 10; i += 1; end
来源：http://xz.szsharing.cn

C#:   while (i < 10) { i++; }
来源：http://wl.huixiangedu.cn

[B08] do-while（至少执行一次）
来源：http://ri.newstarts.cn

Py:   # 无 do-while：用 while True + break
来源：http://kc.huixiangedu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ze.huixiangedu.cn

JS:   do { i++; } while (i < 10);
来源：http://qg.haigaiapp.cn

TS:   do { i++; } while (i < 10);
来源：http://lm.shxzukj.cn

Java: do { i++; } while (i < 10);
来源：http://cp.huanxung.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bu.hahajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ms.haigaiapp.cn

C#:   do { i++; } while (i < 10);
来源：http://bt.szxytkj.cn

[B09] break 与 continue
来源：http://lx.szxytkj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tv.nszjky.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wu.shtwfgs.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kv.newstarts.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ha.szxytkj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vi.huixiangedu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zd.shtwfgs.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gk.panjiajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ww.nszjky.cn

[B10] 遍历同时拿索引
来源：http://ar.gzmigu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://iu.shxzukj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://le.chemitech.net.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mo.szsharing.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://be.gzmigu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ge.nszjky.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qr.wgjwhj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://di.yuntaijiaju.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rv.hnjuh.cn

[B11] 生成数字序列 / 区间
来源：http://mg.9csxet.cn

Py:   list(range(0, 10, 2))
来源：http://wc.shxzukj.cn

PHP:  range(0, 10, 2);
来源：http://fm.bjjhwx.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pu.hnjuh.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fm.newstarts.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://eo.yuexingan06.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mn.shtwfgs.cn

Ruby: (0...10).step(2).to_a
来源：http://jy.bjjhwx.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nu.szsharing.cn

[B12] 跳出多层循环
来源：http://mg.521024.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://vs.521024.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zo.9csxet.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xb.521024.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://oc.shxzskj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qe.nicolike.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gj.muxihuayi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://om.huixiangedu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ii.shtwfgs.cn

[B13] 判断是否为数字
来源：http://iz.shxzukj.cn

Py:   isinstance(x, (int, float))
来源：http://af.asd995.cn

PHP:  is_numeric($x)
来源：http://bj.huixinmuqiang.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ya.nszjky.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pm.yuexingan06.cn

Java: x instanceof Number
来源：http://lq.szsharing.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bz.yuexingan06.cn

Ruby: x.is_a?(Numeric)
来源：http://cl.nicolike.cn

C#:   x is int or double or decimal
来源：http://sf.wgjwhj.cn

[B14] 判断值是否在集合内
来源：http://hn.haigaiapp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bf.nszjky.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fx.hahajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://hz.shxzukj.cn

TS:   [1, 2, 3].includes(x)
来源：http://ac.521024.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xp.szsharing.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jm.yuexingan06.cn

Ruby: [1, 2, 3].include?(x)
来源：http://yj.szsharing.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fl.huixiangedu.cn

[B15] 布尔运算与取反
来源：http://es.huanxung.cn

Py:   a and b or not c
来源：http://ao.newstarts.cn

PHP:  $a && $b || !$c
来源：http://do.szxytkj.cn

JS:   a && b || !c
来源：http://qr.szsharing.cn

TS:   a && b || !c
来源：http://jo.9csxet.cn

Java: a && b || !c
来源：http://wp.szxytkj.cn

Go:   a && b || !c
来源：http://qd.shtwfgs.cn

Ruby: a && b || !c
来源：http://qm.chemitech.net.cn

C#:   a && b || !c
来源：http://nz.shxzskj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://wm.hahajie.cn

Py:   if not data: return
来源：http://wg.wgjwhj.cn

PHP:  if (!$data) { return; }
来源：http://du.521024.cn

JS:   if (!data) return;
来源：http://pj.nicolike.cn

TS:   if (!data) return;
来源：http://nb.huixinmuqiang.cn

Java: if (data == null) return;
来源：http://xw.shxzskj.cn

Go:   if data == nil { return }
来源：http://sr.haigaiapp.cn

Ruby: return if data.nil?
来源：http://sd.jianghongdianzi.cn

C#:   if (data == null) return;
来源：http://ml.bjjhwx.cn

================================================================================
来源：http://tw.newstarts.cn

C. 函数与作用域
来源：http://dv.szsharing.cn

================================================================================
来源：http://zy.jianghongdianzi.cn

[C01] 定义函数
来源：http://qx.chemitech.net.cn

Py:   def add(a, b): return a + b
来源：http://zy.shxzskj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cs.hnjuh.cn

JS:   function add(a, b) { return a + b; }
来源：http://on.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qh.asd995.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://es.jianghongdianzi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://np.huixiangedu.cn

Ruby: def add(a, b); a + b; end
来源：http://cj.szxytkj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jy.wgjwhj.cn

[C02] 默认参数
来源：http://iy.bookmarksfly.cn

Py:   def greet(name="World"): return name
来源：http://ve.haigaiapp.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bo.shxzskj.cn

JS:   function greet(name = "World") { return name; }
来源：http://dd.huixiangedu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://go.shxzukj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://up.newstarts.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hq.hnjuh.cn

Ruby: def greet(name = "World") = name
来源：http://el.nicolike.cn

C#:   string Greet(string name = "World") => name;
来源：http://mq.bookmarksfly.cn

[C03] 可变参数
来源：http://rj.gzmigu.cn

Py:   def total(*args): return sum(args)
来源：http://ba.9csxet.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ec.jctech888.com.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zd.jianghongdianzi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://es.gzmigu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lz.jctech888.com.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bf.newstarts.cn

Ruby: def total(*nums); nums.sum; end
来源：http://lt.colortex.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tf.bookmarksfly.cn

[C04] 命名参数 / 关键字参数
来源：http://so.shtwfgs.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ps.wgjwhj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hf.shtwfgs.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gr.huixinmuqiang.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wj.szsharing.cn

Java: // 无：用 Builder 模式或 record
来源：http://mz.shtwfgs.cn

Go:   // 无：用配置结构体参数
来源：http://lp.szxytkj.cn

Ruby: f(a: 1, b: 2)
来源：http://xs.chemitech.net.cn

C#:   f(a: 1, b: 2)
来源：http://op.huixiangedu.cn

[C05] 返回多个值
来源：http://ui.newstarts.cn

Py:   return a, b
来源：http://pn.szsharing.cn

PHP:  return [$a, $b];
来源：http://dr.huanxung.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://bs.huanxung.cn

TS:   return { a, b };
来源：http://gj.hahajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kr.huixiangedu.cn

Go:   return a, b
来源：http://kn.panjiajie.cn

Ruby: return a, b
来源：http://xl.panjiajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://nq.wgjwhj.cn

[C06] 匿名函数 / lambda
来源：http://wm.hnjuh.cn

Py:   square = lambda x: x * x
来源：http://li.huixinmuqiang.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://er.colortex.cn

JS:   const square = x => x * x;
来源：http://wz.jctech888.com.cn

TS:   const square = (x: number): number => x * x;
来源：http://ju.chemitech.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fu.521024.cn

Go:   sq := func(x int) int { return x * x }
来源：http://uh.shxzukj.cn

Ruby: square = ->(x) { x * x }
来源：http://of.yuexingan06.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wb.szxytkj.cn

[C07] 把函数作为参数传入
来源：http://kw.gzmigu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yd.newstarts.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jr.haigaiapp.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fw.lnxyls.cn

TS:   arr.map(String)
来源：http://fd.szxytkj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wg.huixinmuqiang.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jz.hahajie.cn

Ruby: arr.map(&:upcase)
来源：http://fa.521024.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://uw.asd995.cn

[C08] 闭包
来源：http://yv.bjjhwx.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://at.hnjuh.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://au.521024.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jr.panjiajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tj.yuntaijiaju.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vy.hahajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bf.521024.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ka.huixinmuqiang.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://am.colortex.cn

[C09] 递归
来源：http://wf.shtwfgs.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ay.hahajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://um.muxihuayi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fz.chemitech.net.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://os.shxzukj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sz.lnxyls.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fq.nszjky.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://er.szsharing.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yz.szsharing.cn

[C10] 变量作用域
来源：http://mk.yuexingan06.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qu.chemitech.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bp.jctech888.com.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://st.shxzukj.cn

TS:   同 JS
来源：http://ab.hnjuh.cn

Java: 方法内为块级作用域
来源：http://fi.panjiajie.cn

Go:   花括号块级作用域
来源：http://en.jianghongdianzi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mz.nszjky.cn

C#:   块级作用域
来源：http://uh.colortex.cn

[C11] 模块导入与导出
来源：http://ep.huanxung.cn

Py:   from module import func
来源：http://xj.shtwfgs.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vu.bjjhwx.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ed.huanxung.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dr.jctech888.com.cn

Java: import java.util.List;
来源：http://oh.huixinmuqiang.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ck.muxihuayi.cn

Ruby: require "json"; require_relative "./util"
来源：http://vy.haigaiapp.cn

C#:   using System.Text;
来源：http://gm.lnxyls.cn

[C12] 立即执行函数 IIFE
来源：http://gq.haigaiapp.cn

Py:   (lambda: print("run"))()
来源：http://ne.bjjhwx.cn

PHP:  (function () { echo "run"; })();
来源：http://jc.huixiangedu.cn

JS:   (() => { console.log("run"); })();
来源：http://hz.lnxyls.cn

TS:   (() => { console.log("run"); })();
来源：http://hm.wgjwhj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fl.huanxung.cn

Go:   func() { fmt.Println("run") }()
来源：http://mz.hahajie.cn

Ruby: -> { puts "run" }.call
来源：http://mm.wgjwhj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://vj.newstarts.cn

[C13] 类型声明 / 类型注解
来源：http://tf.shtwfgs.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xc.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jb.521024.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xm.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hv.lnxyls.cn

Java: int add(int a, int b) { return a + b; }
来源：http://yc.muxihuayi.cn

Go:   func add(a, b int) int
来源：http://nz.shxzskj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dv.9csxet.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tk.jianghongdianzi.cn

[C14] 泛型函数
来源：http://yj.jianghongdianzi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wx.yuexingan06.cn

PHP:  // 无泛型
来源：http://no.yuexingan06.cn

JS:   // 无泛型
来源：http://ms.nicolike.cn


<!-- 参考信息 -->