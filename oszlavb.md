代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://jq.chemitech.net.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://tt.hahajie.cn

JS:   (3.14159).toFixed(2)
来源：http://vn.muxihuayi.cn

TS:   (3.14159).toFixed(2)
来源：http://fj.panjiajie.cn

Java: String.format("%.2f", 3.14159)
来源：http://nd.gzmigu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zc.szsharing.cn

Ruby: format("%.2f", 3.14159)
来源：http://vy.lnxyls.cn

C#:   3.14159.ToString("F2")
来源：http://sn.shxzskj.cn

[A22] 获取字符串长度
来源：http://ta.shxzskj.cn

Py:   len(s)
来源：http://in.wgjwhj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://or.9csxet.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://sc.hnjuh.cn

TS:   s.length
来源：http://rf.szxytkj.cn

Java: s.length()
来源：http://bi.colortex.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://or.bjjhwx.cn

Ruby: s.length
来源：http://gu.szxytkj.cn

C#:   s.Length
来源：http://xu.9csxet.cn

[A23] 大小写转换
来源：http://bk.shtwfgs.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://eb.9csxet.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fl.huixinmuqiang.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://aj.yuntaijiaju.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kw.yuexingan06.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ot.muxihuayi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lo.shxzukj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lj.panjiajie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://io.yuexingan06.cn

[A24] 去除首尾空白
来源：http://pm.asd995.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xq.huixinmuqiang.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hx.nicolike.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://en.gzmigu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bz.gzmigu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gz.nicolike.cn

Go:   strings.TrimSpace(s)
来源：http://tb.shxzskj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hj.yuexingan06.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vm.jctech888.com.cn

[A25] 字符串比较
来源：http://ez.bjjhwx.cn

Py:   s1 == s2; s1 != s2
来源：http://ex.szxytkj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://un.521024.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rp.shtwfgs.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vm.jianghongdianzi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://og.nicolike.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wq.shxzukj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://es.jctech888.com.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kj.yuexingan06.cn

[A26] 类型转换总览
来源：http://jk.bookmarksfly.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://id.jctech888.com.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dj.huixiangedu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jp.shxzskj.cn

TS:   Number() String() Boolean() x as number
来源：http://se.lnxyls.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kb.bookmarksfly.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://le.gzmigu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lp.huanxung.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zv.yuntaijiaju.cn

================================================================================
来源：http://fj.shtwfgs.cn

B. 流程控制
来源：http://av.wgjwhj.cn

================================================================================
来源：http://lr.jianghongdianzi.cn

[B01] 条件判断 if / else
来源：http://qr.shxzukj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ib.nicolike.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jb.haigaiapp.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rw.hnjuh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lw.haigaiapp.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://sn.huanxung.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ug.szxytkj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gp.panjiajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cr.521024.cn

[B02] 多分支 else if / elif
来源：http://fg.newstarts.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zs.szsharing.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://oo.yuntaijiaju.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qf.nicolike.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sq.huixinmuqiang.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kq.szsharing.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://iw.haigaiapp.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dj.hnjuh.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bo.huanxung.cn

[B03] switch / match / case
来源：http://hi.colortex.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rq.muxihuayi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ma.muxihuayi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://aa.9csxet.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qj.shxzukj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://na.jianghongdianzi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ce.521024.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://et.wgjwhj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pi.haigaiapp.cn

[B04] for 计数循环
来源：http://oa.chemitech.net.cn

Py:   for i in range(10): print(i)
来源：http://hs.wgjwhj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dd.hahajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sj.hnjuh.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vy.newstarts.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://km.yuexingan06.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ua.shtwfgs.cn

Ruby: 10.times { |i| puts i }
来源：http://gj.shtwfgs.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://se.shxzskj.cn

[B05] 遍历数组 / 列表
来源：http://ci.panjiajie.cn

Py:   for item in arr: print(item)
来源：http://iq.huanxung.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pi.jianghongdianzi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dv.panjiajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://vi.bookmarksfly.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://oz.hahajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://eg.jianghongdianzi.cn

Ruby: arr.each { |item| puts item }
来源：http://nn.chemitech.net.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ov.nszjky.cn

[B06] 遍历字典 / 对象
来源：http://cu.huixinmuqiang.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mp.huixinmuqiang.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rf.hahajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kw.nszjky.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ay.panjiajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fe.newstarts.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kz.yuexingan06.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rh.hnjuh.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cb.shtwfgs.cn

[B07] while 循环
来源：http://rb.jctech888.com.cn

Py:   while i < 10: i += 1
来源：http://ht.colortex.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bo.shtwfgs.cn

JS:   while (i < 10) { i++; }
来源：http://gf.bjjhwx.cn

TS:   while (i < 10) { i++; }
来源：http://mf.asd995.cn

Java: while (i < 10) { i++; }
来源：http://yo.9csxet.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sa.huixinmuqiang.cn

Ruby: while i < 10; i += 1; end
来源：http://pq.huanxung.cn

C#:   while (i < 10) { i++; }
来源：http://az.panjiajie.cn

[B08] do-while（至少执行一次）
来源：http://nx.lnxyls.cn

Py:   # 无 do-while：用 while True + break
来源：http://zn.huanxung.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://io.asd995.cn

JS:   do { i++; } while (i < 10);
来源：http://vl.huixinmuqiang.cn

TS:   do { i++; } while (i < 10);
来源：http://wx.chemitech.net.cn

Java: do { i++; } while (i < 10);
来源：http://eo.haigaiapp.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://qd.haigaiapp.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ca.nszjky.cn

C#:   do { i++; } while (i < 10);
来源：http://ej.bookmarksfly.cn

[B09] break 与 continue
来源：http://ez.jctech888.com.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ql.asd995.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://me.szxytkj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eb.huixinmuqiang.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://af.muxihuayi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://es.gzmigu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qc.szsharing.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fq.colortex.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bd.lnxyls.cn

[B10] 遍历同时拿索引
来源：http://qu.jianghongdianzi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gk.newstarts.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ty.bookmarksfly.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ah.asd995.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ki.shxzukj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hk.jctech888.com.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zr.huixinmuqiang.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nk.gzmigu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lh.huanxung.cn

[B11] 生成数字序列 / 区间
来源：http://hu.haigaiapp.cn

Py:   list(range(0, 10, 2))
来源：http://ja.huixinmuqiang.cn

PHP:  range(0, 10, 2);
来源：http://sl.bookmarksfly.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mz.wgjwhj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yj.gzmigu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ho.chemitech.net.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zz.hahajie.cn

Ruby: (0...10).step(2).to_a
来源：http://zq.muxihuayi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xu.bjjhwx.cn

[B12] 跳出多层循环
来源：http://wj.asd995.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ru.lnxyls.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gb.huixinmuqiang.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cf.nszjky.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fw.huixinmuqiang.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kk.9csxet.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ir.huanxung.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xb.9csxet.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://aq.wgjwhj.cn

[B13] 判断是否为数字
来源：http://im.yuntaijiaju.cn

Py:   isinstance(x, (int, float))
来源：http://kh.nicolike.cn

PHP:  is_numeric($x)
来源：http://yv.yuexingan06.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nt.wgjwhj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pw.muxihuayi.cn

Java: x instanceof Number
来源：http://mw.bjjhwx.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://on.bookmarksfly.cn

Ruby: x.is_a?(Numeric)
来源：http://jr.huixinmuqiang.cn

C#:   x is int or double or decimal
来源：http://aw.huanxung.cn

[B14] 判断值是否在集合内
来源：http://fq.9csxet.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vt.gzmigu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qu.hahajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://ne.szxytkj.cn

TS:   [1, 2, 3].includes(x)
来源：http://ma.newstarts.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://zs.nszjky.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rp.newstarts.cn

Ruby: [1, 2, 3].include?(x)
来源：http://bb.bookmarksfly.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ru.newstarts.cn

[B15] 布尔运算与取反
来源：http://fx.521024.cn

Py:   a and b or not c
来源：http://rz.newstarts.cn

PHP:  $a && $b || !$c
来源：http://wu.huanxung.cn

JS:   a && b || !c
来源：http://vg.asd995.cn

TS:   a && b || !c
来源：http://wn.szsharing.cn

Java: a && b || !c
来源：http://nh.colortex.cn

Go:   a && b || !c
来源：http://do.panjiajie.cn

Ruby: a && b || !c
来源：http://hn.huixinmuqiang.cn

C#:   a && b || !c
来源：http://im.yuexingan06.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zw.panjiajie.cn

Py:   if not data: return
来源：http://eg.newstarts.cn

PHP:  if (!$data) { return; }
来源：http://ms.szxytkj.cn

JS:   if (!data) return;
来源：http://bo.bjjhwx.cn

TS:   if (!data) return;
来源：http://ge.szsharing.cn

Java: if (data == null) return;
来源：http://kd.shtwfgs.cn

Go:   if data == nil { return }
来源：http://un.nszjky.cn

Ruby: return if data.nil?
来源：http://ac.panjiajie.cn

C#:   if (data == null) return;
来源：http://ll.shxzskj.cn

================================================================================
来源：http://jc.szxytkj.cn

C. 函数与作用域
来源：http://wv.lnxyls.cn

================================================================================
来源：http://mx.huixinmuqiang.cn

[C01] 定义函数
来源：http://pm.haigaiapp.cn

Py:   def add(a, b): return a + b
来源：http://vo.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zr.haigaiapp.cn

JS:   function add(a, b) { return a + b; }
来源：http://ql.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zh.huanxung.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ai.hahajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://je.newstarts.cn

Ruby: def add(a, b); a + b; end
来源：http://hg.colortex.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://km.nicolike.cn

[C02] 默认参数
来源：http://wc.nszjky.cn

Py:   def greet(name="World"): return name
来源：http://fb.szsharing.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://am.colortex.cn

JS:   function greet(name = "World") { return name; }
来源：http://tk.jctech888.com.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://tu.yuexingan06.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://if.shtwfgs.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zz.colortex.cn

Ruby: def greet(name = "World") = name
来源：http://qu.colortex.cn

C#:   string Greet(string name = "World") => name;
来源：http://li.bookmarksfly.cn

[C03] 可变参数
来源：http://eq.521024.cn

Py:   def total(*args): return sum(args)
来源：http://wu.nszjky.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hn.szsharing.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hm.9csxet.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lt.yuexingan06.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zx.nszjky.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fs.huixiangedu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fo.yuntaijiaju.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://uu.lnxyls.cn

[C04] 命名参数 / 关键字参数
来源：http://ts.bjjhwx.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ke.shxzukj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vw.asd995.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yj.nszjky.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dp.huixiangedu.cn

Java: // 无：用 Builder 模式或 record
来源：http://xf.shtwfgs.cn

Go:   // 无：用配置结构体参数
来源：http://dk.szxytkj.cn

Ruby: f(a: 1, b: 2)
来源：http://co.jctech888.com.cn

C#:   f(a: 1, b: 2)
来源：http://yj.bjjhwx.cn

[C05] 返回多个值
来源：http://yp.gzmigu.cn

Py:   return a, b
来源：http://fn.szsharing.cn

PHP:  return [$a, $b];
来源：http://nf.nszjky.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dq.gzmigu.cn

TS:   return { a, b };
来源：http://wo.bjjhwx.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lz.521024.cn

Go:   return a, b
来源：http://rq.haigaiapp.cn

Ruby: return a, b
来源：http://fm.yuexingan06.cn

C#:   return (a, b);              // ValueTuple
来源：http://ey.asd995.cn

[C06] 匿名函数 / lambda
来源：http://oc.bookmarksfly.cn

Py:   square = lambda x: x * x
来源：http://wx.newstarts.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://lt.lnxyls.cn

JS:   const square = x => x * x;
来源：http://bo.wgjwhj.cn

TS:   const square = (x: number): number => x * x;
来源：http://hl.shxzukj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qo.521024.cn

Go:   sq := func(x int) int { return x * x }
来源：http://no.huixiangedu.cn

Ruby: square = ->(x) { x * x }
来源：http://hg.szsharing.cn

C#:   Func<int, int> square = x => x * x;
来源：http://rz.shtwfgs.cn

[C07] 把函数作为参数传入
来源：http://al.muxihuayi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ld.jctech888.com.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ew.chemitech.net.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://it.nicolike.cn

TS:   arr.map(String)
来源：http://wj.gzmigu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bu.colortex.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kd.huanxung.cn

Ruby: arr.map(&:upcase)
来源：http://pf.colortex.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mh.muxihuayi.cn

[C08] 闭包
来源：http://mo.chemitech.net.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bi.wgjwhj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://br.haigaiapp.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nn.chemitech.net.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zf.huixinmuqiang.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xx.bjjhwx.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vx.muxihuayi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hx.yuntaijiaju.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kd.huixinmuqiang.cn

[C09] 递归
来源：http://ab.bookmarksfly.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ek.yuntaijiaju.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fx.muxihuayi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hc.bookmarksfly.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qe.haigaiapp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rh.lnxyls.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ky.panjiajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kq.lnxyls.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ik.yuexingan06.cn

[C10] 变量作用域
来源：http://eo.lnxyls.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wx.jctech888.com.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kt.yuntaijiaju.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vn.jctech888.com.cn

TS:   同 JS
来源：http://ad.521024.cn

Java: 方法内为块级作用域
来源：http://ns.shtwfgs.cn

Go:   花括号块级作用域
来源：http://aa.bjjhwx.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zc.hahajie.cn

C#:   块级作用域
来源：http://ok.huixiangedu.cn

[C11] 模块导入与导出
来源：http://qw.gzmigu.cn

Py:   from module import func
来源：http://pt.szxytkj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://rz.bjjhwx.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://un.jianghongdianzi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hc.jianghongdianzi.cn

Java: import java.util.List;
来源：http://lq.colortex.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ue.hnjuh.cn


<!-- 参考信息 -->