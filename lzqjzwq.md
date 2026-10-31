代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://ll.gzmigu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qa.szxytkj.cn

JS:   (3.14159).toFixed(2)
来源：http://ob.nszjky.cn

TS:   (3.14159).toFixed(2)
来源：http://ko.hahajie.cn

Java: String.format("%.2f", 3.14159)
来源：http://tt.huixiangedu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nr.hahajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://me.muxihuayi.cn

C#:   3.14159.ToString("F2")
来源：http://qs.nicolike.cn

[A22] 获取字符串长度
来源：http://he.nszjky.cn

Py:   len(s)
来源：http://hz.shxzskj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://kh.newstarts.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nm.shxzskj.cn

TS:   s.length
来源：http://uy.szxytkj.cn

Java: s.length()
来源：http://io.yuexingan06.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zd.colortex.cn

Ruby: s.length
来源：http://px.yuexingan06.cn

C#:   s.Length
来源：http://qi.yuexingan06.cn

[A23] 大小写转换
来源：http://te.yuntaijiaju.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ct.jianghongdianzi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jz.hahajie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gq.9csxet.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ug.colortex.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://aw.bjjhwx.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://or.gzmigu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://oz.huixinmuqiang.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://rl.shxzukj.cn

[A24] 去除首尾空白
来源：http://qu.huixiangedu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vj.newstarts.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ut.huixinmuqiang.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oh.shxzukj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yx.wgjwhj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://go.jctech888.com.cn

Go:   strings.TrimSpace(s)
来源：http://zv.bookmarksfly.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gc.huanxung.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://le.huanxung.cn

[A25] 字符串比较
来源：http://il.gzmigu.cn

Py:   s1 == s2; s1 != s2
来源：http://up.nicolike.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pw.hnjuh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qz.yuexingan06.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zz.9csxet.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kx.521024.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zy.shtwfgs.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ag.yuexingan06.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zf.shtwfgs.cn

[A26] 类型转换总览
来源：http://mz.yuexingan06.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lh.huixinmuqiang.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vp.jctech888.com.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://aq.lnxyls.cn

TS:   Number() String() Boolean() x as number
来源：http://dx.hnjuh.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://sq.muxihuayi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vu.shxzukj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://oo.newstarts.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://sn.huixiangedu.cn

================================================================================
来源：http://iy.bookmarksfly.cn

B. 流程控制
来源：http://nu.bjjhwx.cn

================================================================================
来源：http://uy.521024.cn

[B01] 条件判断 if / else
来源：http://kx.jctech888.com.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://qp.9csxet.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vc.jctech888.com.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yz.9csxet.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ao.yuexingan06.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qm.lnxyls.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fh.hnjuh.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lv.nicolike.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vf.chemitech.net.cn

[B02] 多分支 else if / elif
来源：http://ho.panjiajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gs.jctech888.com.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tw.yuexingan06.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wf.jianghongdianzi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pc.chemitech.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xc.asd995.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vf.lnxyls.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pr.newstarts.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://md.yuntaijiaju.cn

[B03] switch / match / case
来源：http://dq.huixinmuqiang.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sh.jctech888.com.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qe.shtwfgs.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sy.szsharing.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fx.yuexingan06.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pv.huixiangedu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cg.yuntaijiaju.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sv.huixiangedu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yl.bjjhwx.cn

[B04] for 计数循环
来源：http://xz.9csxet.cn

Py:   for i in range(10): print(i)
来源：http://pe.panjiajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sa.szxytkj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xc.asd995.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ft.panjiajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zt.hahajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bd.jianghongdianzi.cn

Ruby: 10.times { |i| puts i }
来源：http://qg.haigaiapp.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vm.huanxung.cn

[B05] 遍历数组 / 列表
来源：http://hs.bjjhwx.cn

Py:   for item in arr: print(item)
来源：http://yc.asd995.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nh.shxzskj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ma.shxzskj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ky.panjiajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://df.huixiangedu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://io.colortex.cn

Ruby: arr.each { |item| puts item }
来源：http://fz.colortex.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gl.yuntaijiaju.cn

[B06] 遍历字典 / 对象
来源：http://er.gzmigu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://lp.huixinmuqiang.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dh.yuntaijiaju.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mb.huanxung.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zu.szsharing.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cf.szxytkj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gv.huanxung.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://oa.jctech888.com.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://di.nszjky.cn

[B07] while 循环
来源：http://nk.wgjwhj.cn

Py:   while i < 10: i += 1
来源：http://nq.colortex.cn

PHP:  while ($i < 10) { $i++; }
来源：http://em.shxzskj.cn

JS:   while (i < 10) { i++; }
来源：http://fm.szxytkj.cn

TS:   while (i < 10) { i++; }
来源：http://bo.panjiajie.cn

Java: while (i < 10) { i++; }
来源：http://vv.hnjuh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://oh.521024.cn

Ruby: while i < 10; i += 1; end
来源：http://tf.nicolike.cn

C#:   while (i < 10) { i++; }
来源：http://fk.jctech888.com.cn

[B08] do-while（至少执行一次）
来源：http://ib.nicolike.cn

Py:   # 无 do-while：用 while True + break
来源：http://ef.huanxung.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://te.jianghongdianzi.cn

JS:   do { i++; } while (i < 10);
来源：http://to.asd995.cn

TS:   do { i++; } while (i < 10);
来源：http://re.yuexingan06.cn

Java: do { i++; } while (i < 10);
来源：http://uy.521024.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sa.szsharing.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ls.newstarts.cn

C#:   do { i++; } while (i < 10);
来源：http://ln.bjjhwx.cn

[B09] break 与 continue
来源：http://xq.lnxyls.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ry.asd995.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://iq.shxzskj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dp.panjiajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tt.huanxung.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ju.colortex.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xv.lnxyls.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jx.yuntaijiaju.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://me.szxytkj.cn

[B10] 遍历同时拿索引
来源：http://tf.huixinmuqiang.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qk.shtwfgs.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yv.bookmarksfly.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cd.szxytkj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ai.szsharing.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mh.jctech888.com.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yc.panjiajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xo.shxzskj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jq.hahajie.cn

[B11] 生成数字序列 / 区间
来源：http://nn.bookmarksfly.cn

Py:   list(range(0, 10, 2))
来源：http://dn.9csxet.cn

PHP:  range(0, 10, 2);
来源：http://aq.hnjuh.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cy.shxzukj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bq.nszjky.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fl.newstarts.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kn.hahajie.cn

Ruby: (0...10).step(2).to_a
来源：http://ku.newstarts.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dm.shxzskj.cn

[B12] 跳出多层循环
来源：http://de.muxihuayi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fi.haigaiapp.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://nk.bjjhwx.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wf.jctech888.com.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://az.bookmarksfly.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cv.huixiangedu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wc.jianghongdianzi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://oz.colortex.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rr.521024.cn

[B13] 判断是否为数字
来源：http://vu.asd995.cn

Py:   isinstance(x, (int, float))
来源：http://qe.haigaiapp.cn

PHP:  is_numeric($x)
来源：http://mf.huixinmuqiang.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ld.yuntaijiaju.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lt.bjjhwx.cn

Java: x instanceof Number
来源：http://hw.lnxyls.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cj.szsharing.cn

Ruby: x.is_a?(Numeric)
来源：http://mu.9csxet.cn

C#:   x is int or double or decimal
来源：http://yk.colortex.cn

[B14] 判断值是否在集合内
来源：http://kj.521024.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qr.nicolike.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hj.huixinmuqiang.cn

JS:   [1, 2, 3].includes(x)
来源：http://tk.szsharing.cn

TS:   [1, 2, 3].includes(x)
来源：http://fq.bookmarksfly.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://wh.asd995.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ix.lnxyls.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ap.szxytkj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ro.9csxet.cn

[B15] 布尔运算与取反
来源：http://eg.bookmarksfly.cn

Py:   a and b or not c
来源：http://cm.wgjwhj.cn

PHP:  $a && $b || !$c
来源：http://bf.yuexingan06.cn

JS:   a && b || !c
来源：http://vc.9csxet.cn

TS:   a && b || !c
来源：http://ct.hnjuh.cn

Java: a && b || !c
来源：http://ay.nicolike.cn

Go:   a && b || !c
来源：http://wk.huanxung.cn

Ruby: a && b || !c
来源：http://qr.gzmigu.cn

C#:   a && b || !c
来源：http://ce.521024.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bm.huanxung.cn

Py:   if not data: return
来源：http://az.jianghongdianzi.cn

PHP:  if (!$data) { return; }
来源：http://ke.huixiangedu.cn

JS:   if (!data) return;
来源：http://xr.jctech888.com.cn

TS:   if (!data) return;
来源：http://bi.bjjhwx.cn

Java: if (data == null) return;
来源：http://bh.hahajie.cn

Go:   if data == nil { return }
来源：http://rw.jctech888.com.cn

Ruby: return if data.nil?
来源：http://pg.asd995.cn

C#:   if (data == null) return;
来源：http://ll.bjjhwx.cn

================================================================================
来源：http://hw.colortex.cn

C. 函数与作用域
来源：http://tk.nicolike.cn

================================================================================
来源：http://zk.huixiangedu.cn

[C01] 定义函数
来源：http://ss.shtwfgs.cn

Py:   def add(a, b): return a + b
来源：http://hm.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vf.panjiajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://ro.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wp.muxihuayi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vq.bookmarksfly.cn

Go:   func add(a, b int) int { return a + b }
来源：http://iy.yuexingan06.cn

Ruby: def add(a, b); a + b; end
来源：http://zh.chemitech.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ij.bookmarksfly.cn

[C02] 默认参数
来源：http://id.yuntaijiaju.cn

Py:   def greet(name="World"): return name
来源：http://td.huanxung.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ul.wgjwhj.cn

JS:   function greet(name = "World") { return name; }
来源：http://id.jianghongdianzi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://em.521024.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://un.panjiajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hs.bookmarksfly.cn

Ruby: def greet(name = "World") = name
来源：http://qj.lnxyls.cn

C#:   string Greet(string name = "World") => name;
来源：http://th.muxihuayi.cn

[C03] 可变参数
来源：http://mo.szxytkj.cn

Py:   def total(*args): return sum(args)
来源：http://kl.newstarts.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pp.huanxung.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rf.panjiajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mv.gzmigu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vf.bjjhwx.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hd.szxytkj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ao.szsharing.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ci.gzmigu.cn

[C04] 命名参数 / 关键字参数
来源：http://pq.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zk.huanxung.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gt.bookmarksfly.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ib.yuntaijiaju.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mj.asd995.cn

Java: // 无：用 Builder 模式或 record
来源：http://sv.jianghongdianzi.cn

Go:   // 无：用配置结构体参数
来源：http://lf.jctech888.com.cn

Ruby: f(a: 1, b: 2)
来源：http://dn.colortex.cn

C#:   f(a: 1, b: 2)
来源：http://hr.hnjuh.cn

[C05] 返回多个值
来源：http://is.huixinmuqiang.cn

Py:   return a, b
来源：http://do.jianghongdianzi.cn

PHP:  return [$a, $b];
来源：http://kr.nicolike.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://nu.nszjky.cn

TS:   return { a, b };
来源：http://lg.szxytkj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vq.haigaiapp.cn

Go:   return a, b
来源：http://xk.panjiajie.cn

Ruby: return a, b
来源：http://bm.panjiajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://is.szsharing.cn

[C06] 匿名函数 / lambda
来源：http://xy.jianghongdianzi.cn

Py:   square = lambda x: x * x
来源：http://yb.jctech888.com.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://os.lnxyls.cn

JS:   const square = x => x * x;
来源：http://cg.yuexingan06.cn

TS:   const square = (x: number): number => x * x;
来源：http://xj.huixiangedu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kw.lnxyls.cn

Go:   sq := func(x int) int { return x * x }
来源：http://oy.muxihuayi.cn

Ruby: square = ->(x) { x * x }
来源：http://tj.shxzskj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zn.newstarts.cn

[C07] 把函数作为参数传入
来源：http://rh.gzmigu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://be.shtwfgs.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ni.521024.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uz.lnxyls.cn

TS:   arr.map(String)
来源：http://wm.gzmigu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hj.wgjwhj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://am.521024.cn

Ruby: arr.map(&:upcase)
来源：http://op.bookmarksfly.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mj.colortex.cn

[C08] 闭包
来源：http://ey.bjjhwx.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ug.shxzukj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vz.9csxet.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wr.shtwfgs.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tu.bjjhwx.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yf.gzmigu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zg.hahajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://if.huixiangedu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gy.wgjwhj.cn

[C09] 递归
来源：http://vw.haigaiapp.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ob.521024.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hv.hahajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zz.jctech888.com.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ab.newstarts.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yq.muxihuayi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dq.lnxyls.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rr.gzmigu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mx.yuexingan06.cn

[C10] 变量作用域
来源：http://va.9csxet.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yu.jctech888.com.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jl.yuntaijiaju.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sl.huixinmuqiang.cn

TS:   同 JS
来源：http://mg.yuntaijiaju.cn

Java: 方法内为块级作用域
来源：http://pc.lnxyls.cn

Go:   花括号块级作用域
来源：http://we.yuntaijiaju.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://za.wgjwhj.cn

C#:   块级作用域
来源：http://nl.bjjhwx.cn

[C11] 模块导入与导出
来源：http://qg.huanxung.cn

Py:   from module import func
来源：http://yz.huanxung.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://yp.huixinmuqiang.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://wy.huixinmuqiang.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xv.shxzskj.cn

Java: import java.util.List;
来源：http://eb.9csxet.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://be.huanxung.cn


<!-- 参考信息 -->