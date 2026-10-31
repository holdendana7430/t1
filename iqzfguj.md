代发 wailian999

[A22] 获取字符串长度
来源：http://tb.chemitech.net.cn

Py:   len(s)
来源：http://sy.bjjhwx.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vv.huixinmuqiang.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zz.bjjhwx.cn

TS:   s.length
来源：http://kn.panjiajie.cn

Java: s.length()
来源：http://yr.521024.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jv.bookmarksfly.cn

Ruby: s.length
来源：http://rr.shtwfgs.cn

C#:   s.Length
来源：http://is.chemitech.net.cn

[A23] 大小写转换
来源：http://dt.haigaiapp.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://xu.huixiangedu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dh.nszjky.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yj.yuntaijiaju.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qf.shxzskj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mh.colortex.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zb.jianghongdianzi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ge.jianghongdianzi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://fc.gzmigu.cn

[A24] 去除首尾空白
来源：http://bc.521024.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bf.huanxung.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ih.yuntaijiaju.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yo.panjiajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://an.shxzskj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://yw.hahajie.cn

Go:   strings.TrimSpace(s)
来源：http://tt.huixinmuqiang.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://uz.hahajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vk.wgjwhj.cn

[A25] 字符串比较
来源：http://xw.haigaiapp.cn

Py:   s1 == s2; s1 != s2
来源：http://wm.panjiajie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sd.shxzukj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ot.521024.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hp.huixiangedu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bm.panjiajie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xa.hahajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://fx.szsharing.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wg.huixinmuqiang.cn

[A26] 类型转换总览
来源：http://we.jctech888.com.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xu.bookmarksfly.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jb.wgjwhj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ym.panjiajie.cn

TS:   Number() String() Boolean() x as number
来源：http://hj.panjiajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ep.shxzukj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cs.shtwfgs.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ob.shxzukj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wy.huixinmuqiang.cn

================================================================================
来源：http://hm.wgjwhj.cn

B. 流程控制
来源：http://or.lnxyls.cn

================================================================================
来源：http://io.521024.cn

[B01] 条件判断 if / else
来源：http://se.lnxyls.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://yi.lnxyls.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://za.9csxet.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bt.hnjuh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nn.9csxet.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qy.szsharing.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pn.wgjwhj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vj.shtwfgs.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yh.shxzskj.cn

[B02] 多分支 else if / elif
来源：http://im.szsharing.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ak.szxytkj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zo.shtwfgs.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://du.bookmarksfly.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kw.hahajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kg.newstarts.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bm.haigaiapp.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rd.haigaiapp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uz.hnjuh.cn

[B03] switch / match / case
来源：http://aa.gzmigu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xx.newstarts.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mw.bookmarksfly.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pu.szsharing.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yv.hahajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://oh.nszjky.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://su.shxzukj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://em.9csxet.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ex.jianghongdianzi.cn

[B04] for 计数循环
来源：http://tv.szxytkj.cn

Py:   for i in range(10): print(i)
来源：http://sp.huanxung.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jr.hahajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ht.colortex.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mq.shxzukj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zy.szsharing.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://th.hahajie.cn

Ruby: 10.times { |i| puts i }
来源：http://tx.521024.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qa.shxzukj.cn

[B05] 遍历数组 / 列表
来源：http://ul.jctech888.com.cn

Py:   for item in arr: print(item)
来源：http://bc.colortex.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://az.wgjwhj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wq.huixiangedu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://sc.asd995.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vf.9csxet.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wj.lnxyls.cn

Ruby: arr.each { |item| puts item }
来源：http://xx.gzmigu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://md.yuexingan06.cn

[B06] 遍历字典 / 对象
来源：http://os.wgjwhj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://eb.shtwfgs.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hx.hnjuh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zw.szsharing.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gi.521024.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://we.muxihuayi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jv.muxihuayi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bu.huixiangedu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xd.yuexingan06.cn

[B07] while 循环
来源：http://qr.huixinmuqiang.cn

Py:   while i < 10: i += 1
来源：http://ec.jctech888.com.cn

PHP:  while ($i < 10) { $i++; }
来源：http://jr.hnjuh.cn

JS:   while (i < 10) { i++; }
来源：http://ym.asd995.cn

TS:   while (i < 10) { i++; }
来源：http://fg.yuexingan06.cn

Java: while (i < 10) { i++; }
来源：http://yj.muxihuayi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zr.huixinmuqiang.cn

Ruby: while i < 10; i += 1; end
来源：http://vp.nicolike.cn

C#:   while (i < 10) { i++; }
来源：http://ig.nszjky.cn

[B08] do-while（至少执行一次）
来源：http://pt.huixinmuqiang.cn

Py:   # 无 do-while：用 while True + break
来源：http://bf.haigaiapp.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://di.newstarts.cn

JS:   do { i++; } while (i < 10);
来源：http://kj.yuexingan06.cn

TS:   do { i++; } while (i < 10);
来源：http://ip.lnxyls.cn

Java: do { i++; } while (i < 10);
来源：http://bd.bookmarksfly.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ew.shxzskj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rw.szxytkj.cn

C#:   do { i++; } while (i < 10);
来源：http://at.muxihuayi.cn

[B09] break 与 continue
来源：http://yw.muxihuayi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://an.hnjuh.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yp.wgjwhj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qe.521024.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zh.bjjhwx.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ke.szxytkj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bm.newstarts.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nm.szxytkj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tx.gzmigu.cn

[B10] 遍历同时拿索引
来源：http://lc.asd995.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://js.asd995.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lw.huixiangedu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uq.lnxyls.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uv.jianghongdianzi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wz.szsharing.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sa.shxzskj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ip.muxihuayi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://do.gzmigu.cn

[B11] 生成数字序列 / 区间
来源：http://cs.521024.cn

Py:   list(range(0, 10, 2))
来源：http://yw.chemitech.net.cn

PHP:  range(0, 10, 2);
来源：http://fo.panjiajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ii.jctech888.com.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gf.gzmigu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vi.wgjwhj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pt.colortex.cn

Ruby: (0...10).step(2).to_a
来源：http://ih.huixinmuqiang.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kh.nicolike.cn

[B12] 跳出多层循环
来源：http://es.nszjky.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hm.jianghongdianzi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://dv.521024.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dy.szxytkj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yw.szxytkj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fe.yuntaijiaju.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ul.wgjwhj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ti.shtwfgs.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fq.bjjhwx.cn

[B13] 判断是否为数字
来源：http://zp.yuexingan06.cn

Py:   isinstance(x, (int, float))
来源：http://kx.nszjky.cn

PHP:  is_numeric($x)
来源：http://vu.szxytkj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xz.haigaiapp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://um.lnxyls.cn

Java: x instanceof Number
来源：http://uy.haigaiapp.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cc.nszjky.cn

Ruby: x.is_a?(Numeric)
来源：http://es.huixinmuqiang.cn

C#:   x is int or double or decimal
来源：http://xd.shxzskj.cn

[B14] 判断值是否在集合内
来源：http://re.huixiangedu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wd.huanxung.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://eq.nszjky.cn

JS:   [1, 2, 3].includes(x)
来源：http://xm.szsharing.cn

TS:   [1, 2, 3].includes(x)
来源：http://zp.bjjhwx.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://lt.9csxet.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ys.bjjhwx.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zh.muxihuayi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ny.szxytkj.cn

[B15] 布尔运算与取反
来源：http://eg.huixinmuqiang.cn

Py:   a and b or not c
来源：http://kp.newstarts.cn

PHP:  $a && $b || !$c
来源：http://ke.colortex.cn

JS:   a && b || !c
来源：http://sr.yuexingan06.cn

TS:   a && b || !c
来源：http://fo.hahajie.cn

Java: a && b || !c
来源：http://ep.shxzukj.cn

Go:   a && b || !c
来源：http://xs.szxytkj.cn

Ruby: a && b || !c
来源：http://yy.9csxet.cn

C#:   a && b || !c
来源：http://hx.yuntaijiaju.cn

[B16] 卫语句：不满足条件提前返回
来源：http://va.yuntaijiaju.cn

Py:   if not data: return
来源：http://vg.hnjuh.cn

PHP:  if (!$data) { return; }
来源：http://xd.hahajie.cn

JS:   if (!data) return;
来源：http://hi.gzmigu.cn

TS:   if (!data) return;
来源：http://cz.haigaiapp.cn

Java: if (data == null) return;
来源：http://zp.newstarts.cn

Go:   if data == nil { return }
来源：http://fq.jctech888.com.cn

Ruby: return if data.nil?
来源：http://bt.521024.cn

C#:   if (data == null) return;
来源：http://ai.muxihuayi.cn

================================================================================
来源：http://yd.521024.cn

C. 函数与作用域
来源：http://ik.521024.cn

================================================================================
来源：http://bp.bookmarksfly.cn

[C01] 定义函数
来源：http://zu.colortex.cn

Py:   def add(a, b): return a + b
来源：http://gp.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vz.9csxet.cn

JS:   function add(a, b) { return a + b; }
来源：http://pu.panjiajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rf.huanxung.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lf.jianghongdianzi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xz.yuexingan06.cn

Ruby: def add(a, b); a + b; end
来源：http://vh.shtwfgs.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pi.wgjwhj.cn

[C02] 默认参数
来源：http://ea.yuexingan06.cn

Py:   def greet(name="World"): return name
来源：http://gs.nicolike.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yx.hnjuh.cn

JS:   function greet(name = "World") { return name; }
来源：http://fw.muxihuayi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qd.jianghongdianzi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qc.muxihuayi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cl.nicolike.cn

Ruby: def greet(name = "World") = name
来源：http://df.bookmarksfly.cn

C#:   string Greet(string name = "World") => name;
来源：http://kf.bjjhwx.cn

[C03] 可变参数
来源：http://cv.gzmigu.cn

Py:   def total(*args): return sum(args)
来源：http://qi.haigaiapp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pa.bjjhwx.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://go.hahajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mk.haigaiapp.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gh.shxzukj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ld.colortex.cn

Ruby: def total(*nums); nums.sum; end
来源：http://br.bjjhwx.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wd.nszjky.cn

[C04] 命名参数 / 关键字参数
来源：http://tz.bjjhwx.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uh.huixinmuqiang.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vt.lnxyls.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fz.haigaiapp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uw.shxzukj.cn

Java: // 无：用 Builder 模式或 record
来源：http://lh.lnxyls.cn

Go:   // 无：用配置结构体参数
来源：http://ce.shxzukj.cn

Ruby: f(a: 1, b: 2)
来源：http://xm.huixiangedu.cn

C#:   f(a: 1, b: 2)
来源：http://gm.yuexingan06.cn

[C05] 返回多个值
来源：http://tm.hahajie.cn

Py:   return a, b
来源：http://dg.szsharing.cn

PHP:  return [$a, $b];
来源：http://tl.huixiangedu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zm.gzmigu.cn

TS:   return { a, b };
来源：http://tc.wgjwhj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xi.gzmigu.cn

Go:   return a, b
来源：http://sm.nszjky.cn

Ruby: return a, b
来源：http://sn.huanxung.cn

C#:   return (a, b);              // ValueTuple
来源：http://ix.yuntaijiaju.cn

[C06] 匿名函数 / lambda
来源：http://oi.bjjhwx.cn

Py:   square = lambda x: x * x
来源：http://dy.shtwfgs.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://oi.huixinmuqiang.cn

JS:   const square = x => x * x;
来源：http://sb.wgjwhj.cn

TS:   const square = (x: number): number => x * x;
来源：http://di.hahajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bn.haigaiapp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hn.shtwfgs.cn

Ruby: square = ->(x) { x * x }
来源：http://fz.haigaiapp.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hz.hahajie.cn

[C07] 把函数作为参数传入
来源：http://dx.jianghongdianzi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nk.bjjhwx.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ir.521024.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ae.9csxet.cn

TS:   arr.map(String)
来源：http://eh.jctech888.com.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yc.yuntaijiaju.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hm.jianghongdianzi.cn

Ruby: arr.map(&:upcase)
来源：http://co.haigaiapp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ze.lnxyls.cn

[C08] 闭包
来源：http://ea.yuexingan06.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jc.jianghongdianzi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://oj.hahajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rj.jianghongdianzi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kc.nicolike.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://eu.wgjwhj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xv.szsharing.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ex.hahajie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zn.shtwfgs.cn

[C09] 递归
来源：http://qr.szxytkj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qo.bjjhwx.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qy.hnjuh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rz.chemitech.net.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ll.nszjky.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ld.huanxung.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ji.panjiajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ht.shtwfgs.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cn.nicolike.cn

[C10] 变量作用域
来源：http://rg.yuntaijiaju.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qc.hahajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gm.shxzskj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://em.huixinmuqiang.cn

TS:   同 JS
来源：http://up.chemitech.net.cn

Java: 方法内为块级作用域
来源：http://hl.shxzukj.cn

Go:   花括号块级作用域
来源：http://dk.lnxyls.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tf.9csxet.cn

C#:   块级作用域
来源：http://bk.panjiajie.cn

[C11] 模块导入与导出
来源：http://vg.haigaiapp.cn

Py:   from module import func
来源：http://gy.lnxyls.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://cp.521024.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qv.hahajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sg.9csxet.cn

Java: import java.util.List;
来源：http://gx.wgjwhj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lq.asd995.cn

Ruby: require "json"; require_relative "./util"
来源：http://fp.asd995.cn

C#:   using System.Text;
来源：http://dm.shtwfgs.cn

[C12] 立即执行函数 IIFE
来源：http://zl.nszjky.cn

Py:   (lambda: print("run"))()
来源：http://dw.shtwfgs.cn

PHP:  (function () { echo "run"; })();
来源：http://tz.newstarts.cn

JS:   (() => { console.log("run"); })();
来源：http://ss.yuntaijiaju.cn

TS:   (() => { console.log("run"); })();
来源：http://fw.huanxung.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ss.nicolike.cn


<!-- 参考信息 -->