代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://ay.panjiajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ye.newstarts.cn

JS:   (3.14159).toFixed(2)
来源：http://qr.wgjwhj.cn

TS:   (3.14159).toFixed(2)
来源：http://ui.huixinmuqiang.cn

Java: String.format("%.2f", 3.14159)
来源：http://lu.nszjky.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://rl.bookmarksfly.cn

Ruby: format("%.2f", 3.14159)
来源：http://al.jianghongdianzi.cn

C#:   3.14159.ToString("F2")
来源：http://ir.nszjky.cn

[A22] 获取字符串长度
来源：http://zl.chemitech.net.cn

Py:   len(s)
来源：http://ff.colortex.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tq.muxihuayi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ep.gzmigu.cn

TS:   s.length
来源：http://ah.521024.cn

Java: s.length()
来源：http://cj.jianghongdianzi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xu.9csxet.cn

Ruby: s.length
来源：http://cj.bookmarksfly.cn

C#:   s.Length
来源：http://tz.521024.cn

[A23] 大小写转换
来源：http://bl.shxzukj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://yj.521024.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cz.nszjky.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kh.huanxung.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ct.huanxung.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ew.bjjhwx.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pp.nicolike.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dd.hnjuh.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ht.hahajie.cn

[A24] 去除首尾空白
来源：http://mt.wgjwhj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ua.bjjhwx.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kc.szsharing.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fa.hahajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wu.shxzskj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://np.newstarts.cn

Go:   strings.TrimSpace(s)
来源：http://im.lnxyls.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tz.szsharing.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ks.521024.cn

[A25] 字符串比较
来源：http://td.colortex.cn

Py:   s1 == s2; s1 != s2
来源：http://dn.huanxung.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fw.hnjuh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dp.szsharing.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tl.haigaiapp.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bh.jctech888.com.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ti.jianghongdianzi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://wh.gzmigu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bw.muxihuayi.cn

[A26] 类型转换总览
来源：http://vj.nicolike.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sd.nszjky.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qf.lnxyls.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://su.colortex.cn

TS:   Number() String() Boolean() x as number
来源：http://nk.szsharing.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://oi.bjjhwx.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pt.szxytkj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://fm.shtwfgs.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://er.jctech888.com.cn

================================================================================
来源：http://yg.jctech888.com.cn

B. 流程控制
来源：http://ux.jctech888.com.cn

================================================================================
来源：http://dy.jianghongdianzi.cn

[B01] 条件判断 if / else
来源：http://md.huanxung.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xt.nicolike.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jd.nicolike.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kx.gzmigu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://za.bjjhwx.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://yj.newstarts.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mh.nicolike.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dl.9csxet.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gd.hnjuh.cn

[B02] 多分支 else if / elif
来源：http://ij.chemitech.net.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://uq.panjiajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.huixinmuqiang.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ag.lnxyls.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gj.newstarts.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sm.wgjwhj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cm.wgjwhj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tf.bjjhwx.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lt.chemitech.net.cn

[B03] switch / match / case
来源：http://wo.jctech888.com.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qu.colortex.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hy.hnjuh.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ry.shtwfgs.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kn.chemitech.net.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gd.bookmarksfly.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hy.jctech888.com.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lx.haigaiapp.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rw.9csxet.cn

[B04] for 计数循环
来源：http://cg.bjjhwx.cn

Py:   for i in range(10): print(i)
来源：http://jx.szxytkj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zt.yuexingan06.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pm.521024.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zs.asd995.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bi.yuexingan06.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xz.asd995.cn

Ruby: 10.times { |i| puts i }
来源：http://ej.asd995.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vq.bjjhwx.cn

[B05] 遍历数组 / 列表
来源：http://xd.nicolike.cn

Py:   for item in arr: print(item)
来源：http://ao.yuexingan06.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://di.chemitech.net.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wf.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://da.wgjwhj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://as.jctech888.com.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qd.yuntaijiaju.cn

Ruby: arr.each { |item| puts item }
来源：http://wj.lnxyls.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xd.9csxet.cn

[B06] 遍历字典 / 对象
来源：http://gk.shxzskj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pq.jctech888.com.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xy.gzmigu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xu.gzmigu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ui.jctech888.com.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qz.bjjhwx.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mm.newstarts.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ym.yuexingan06.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bd.bjjhwx.cn

[B07] while 循环
来源：http://fu.haigaiapp.cn

Py:   while i < 10: i += 1
来源：http://ew.lnxyls.cn

PHP:  while ($i < 10) { $i++; }
来源：http://oi.hahajie.cn

JS:   while (i < 10) { i++; }
来源：http://ai.newstarts.cn

TS:   while (i < 10) { i++; }
来源：http://rq.panjiajie.cn

Java: while (i < 10) { i++; }
来源：http://yk.nicolike.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fo.bookmarksfly.cn

Ruby: while i < 10; i += 1; end
来源：http://kh.asd995.cn

C#:   while (i < 10) { i++; }
来源：http://kp.yuntaijiaju.cn

[B08] do-while（至少执行一次）
来源：http://dm.huixiangedu.cn

Py:   # 无 do-while：用 while True + break
来源：http://rj.asd995.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ki.shxzukj.cn

JS:   do { i++; } while (i < 10);
来源：http://ww.hahajie.cn

TS:   do { i++; } while (i < 10);
来源：http://az.jianghongdianzi.cn

Java: do { i++; } while (i < 10);
来源：http://wa.muxihuayi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://hh.nicolike.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wc.yuntaijiaju.cn

C#:   do { i++; } while (i < 10);
来源：http://xr.gzmigu.cn

[B09] break 与 continue
来源：http://dl.panjiajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cw.szxytkj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tu.lnxyls.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bq.nszjky.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wu.lnxyls.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://om.nicolike.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yd.szsharing.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hq.huixiangedu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pm.yuntaijiaju.cn

[B10] 遍历同时拿索引
来源：http://se.jianghongdianzi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://am.szsharing.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mj.szxytkj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rj.wgjwhj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://en.huixiangedu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zw.hnjuh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ct.szxytkj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uu.panjiajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gb.gzmigu.cn

[B11] 生成数字序列 / 区间
来源：http://im.hahajie.cn

Py:   list(range(0, 10, 2))
来源：http://tw.chemitech.net.cn

PHP:  range(0, 10, 2);
来源：http://te.bookmarksfly.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://km.bookmarksfly.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vv.9csxet.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wv.gzmigu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nv.yuntaijiaju.cn

Ruby: (0...10).step(2).to_a
来源：http://cv.bookmarksfly.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sf.nicolike.cn

[B12] 跳出多层循环
来源：http://kk.nicolike.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://nl.hnjuh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://cg.shtwfgs.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fj.yuexingan06.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xq.bookmarksfly.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ph.huanxung.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sq.521024.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wv.panjiajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vt.521024.cn

[B13] 判断是否为数字
来源：http://bi.haigaiapp.cn

Py:   isinstance(x, (int, float))
来源：http://dv.lnxyls.cn

PHP:  is_numeric($x)
来源：http://qq.yuexingan06.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mr.nicolike.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fa.hahajie.cn

Java: x instanceof Number
来源：http://lt.nszjky.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gx.shtwfgs.cn

Ruby: x.is_a?(Numeric)
来源：http://qt.521024.cn

C#:   x is int or double or decimal
来源：http://qw.huixinmuqiang.cn

[B14] 判断值是否在集合内
来源：http://tm.jianghongdianzi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wa.shxzskj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lf.shxzukj.cn

JS:   [1, 2, 3].includes(x)
来源：http://ab.huanxung.cn

TS:   [1, 2, 3].includes(x)
来源：http://nw.huixiangedu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://lz.lnxyls.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sa.jctech888.com.cn

Ruby: [1, 2, 3].include?(x)
来源：http://lx.gzmigu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ve.9csxet.cn

[B15] 布尔运算与取反
来源：http://lt.yuntaijiaju.cn

Py:   a and b or not c
来源：http://qb.nicolike.cn

PHP:  $a && $b || !$c
来源：http://dt.yuntaijiaju.cn

JS:   a && b || !c
来源：http://ey.shxzskj.cn

TS:   a && b || !c
来源：http://az.hahajie.cn

Java: a && b || !c
来源：http://qa.yuntaijiaju.cn

Go:   a && b || !c
来源：http://xo.colortex.cn

Ruby: a && b || !c
来源：http://oo.nszjky.cn

C#:   a && b || !c
来源：http://aw.huanxung.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jp.hnjuh.cn

Py:   if not data: return
来源：http://mw.nszjky.cn

PHP:  if (!$data) { return; }
来源：http://nq.haigaiapp.cn

JS:   if (!data) return;
来源：http://lc.hahajie.cn

TS:   if (!data) return;
来源：http://np.9csxet.cn

Java: if (data == null) return;
来源：http://lx.shxzskj.cn

Go:   if data == nil { return }
来源：http://ax.yuexingan06.cn

Ruby: return if data.nil?
来源：http://vo.bjjhwx.cn

C#:   if (data == null) return;
来源：http://qn.gzmigu.cn

================================================================================
来源：http://kx.shtwfgs.cn

C. 函数与作用域
来源：http://rx.shxzskj.cn

================================================================================
来源：http://jc.yuexingan06.cn

[C01] 定义函数
来源：http://rv.huanxung.cn

Py:   def add(a, b): return a + b
来源：http://mf.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rd.yuexingan06.cn

JS:   function add(a, b) { return a + b; }
来源：http://tg.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bs.9csxet.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://di.muxihuayi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://kl.nicolike.cn

Ruby: def add(a, b); a + b; end
来源：http://yf.wgjwhj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://is.jctech888.com.cn

[C02] 默认参数
来源：http://jt.asd995.cn

Py:   def greet(name="World"): return name
来源：http://kb.jianghongdianzi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://df.nicolike.cn

JS:   function greet(name = "World") { return name; }
来源：http://jk.shtwfgs.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yb.hnjuh.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://la.jctech888.com.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://oj.jianghongdianzi.cn

Ruby: def greet(name = "World") = name
来源：http://pi.panjiajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://cc.lnxyls.cn

[C03] 可变参数
来源：http://az.9csxet.cn

Py:   def total(*args): return sum(args)
来源：http://br.bjjhwx.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uc.yuntaijiaju.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rq.gzmigu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ss.shxzskj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wg.9csxet.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nv.yuntaijiaju.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pg.chemitech.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ie.szxytkj.cn

[C04] 命名参数 / 关键字参数
来源：http://og.gzmigu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uf.wgjwhj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rc.huixinmuqiang.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vk.bjjhwx.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wt.yuexingan06.cn

Java: // 无：用 Builder 模式或 record
来源：http://jr.szsharing.cn

Go:   // 无：用配置结构体参数
来源：http://ij.shxzskj.cn

Ruby: f(a: 1, b: 2)
来源：http://oh.bjjhwx.cn

C#:   f(a: 1, b: 2)
来源：http://su.huixinmuqiang.cn

[C05] 返回多个值
来源：http://ge.wgjwhj.cn

Py:   return a, b
来源：http://cy.shxzskj.cn

PHP:  return [$a, $b];
来源：http://lw.shtwfgs.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://tc.wgjwhj.cn

TS:   return { a, b };
来源：http://fj.yuexingan06.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bj.hahajie.cn

Go:   return a, b
来源：http://yl.haigaiapp.cn

Ruby: return a, b
来源：http://hq.huanxung.cn

C#:   return (a, b);              // ValueTuple
来源：http://ck.huanxung.cn

[C06] 匿名函数 / lambda
来源：http://fs.bookmarksfly.cn

Py:   square = lambda x: x * x
来源：http://qj.jianghongdianzi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xc.szsharing.cn

JS:   const square = x => x * x;
来源：http://ma.9csxet.cn

TS:   const square = (x: number): number => x * x;
来源：http://ur.yuntaijiaju.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://br.chemitech.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ns.szxytkj.cn

Ruby: square = ->(x) { x * x }
来源：http://ql.yuntaijiaju.cn

C#:   Func<int, int> square = x => x * x;
来源：http://lz.jianghongdianzi.cn

[C07] 把函数作为参数传入
来源：http://tx.bjjhwx.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ux.shtwfgs.cn

PHP:  array_map("strtoupper", $arr);
来源：http://lc.newstarts.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zd.hnjuh.cn

TS:   arr.map(String)
来源：http://kz.jianghongdianzi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ia.hnjuh.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wv.asd995.cn

Ruby: arr.map(&:upcase)
来源：http://mo.9csxet.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ja.bjjhwx.cn

[C08] 闭包
来源：http://iy.yuntaijiaju.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bf.colortex.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://de.jctech888.com.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bs.colortex.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://en.newstarts.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rk.nicolike.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wf.szxytkj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hu.huanxung.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://im.szxytkj.cn

[C09] 递归
来源：http://wa.colortex.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://oy.yuexingan06.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uo.nszjky.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ex.haigaiapp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pj.shxzukj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qb.yuntaijiaju.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pm.hahajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ym.yuexingan06.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ea.szxytkj.cn

[C10] 变量作用域
来源：http://zo.nicolike.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xb.haigaiapp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wu.521024.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rd.gzmigu.cn

TS:   同 JS
来源：http://wg.shtwfgs.cn

Java: 方法内为块级作用域
来源：http://jm.nszjky.cn

Go:   花括号块级作用域
来源：http://tt.muxihuayi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uk.szxytkj.cn

C#:   块级作用域
来源：http://wd.muxihuayi.cn

[C11] 模块导入与导出
来源：http://ay.huixiangedu.cn

Py:   from module import func
来源：http://hf.shxzukj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://iz.newstarts.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://er.panjiajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ts.jctech888.com.cn

Java: import java.util.List;
来源：http://fj.newstarts.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ek.nszjky.cn


<!-- 参考信息 -->