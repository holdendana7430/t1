代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://ne.yuexingan06.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hd.muxihuayi.cn

JS:   (3.14159).toFixed(2)
来源：http://wz.muxihuayi.cn

TS:   (3.14159).toFixed(2)
来源：http://lp.huanxung.cn

Java: String.format("%.2f", 3.14159)
来源：http://ap.yuntaijiaju.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qe.shxzskj.cn

Ruby: format("%.2f", 3.14159)
来源：http://uq.shtwfgs.cn

C#:   3.14159.ToString("F2")
来源：http://dh.szsharing.cn

[A22] 获取字符串长度
来源：http://zi.bookmarksfly.cn

Py:   len(s)
来源：http://sa.521024.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fx.yuntaijiaju.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://sh.muxihuayi.cn

TS:   s.length
来源：http://nj.muxihuayi.cn

Java: s.length()
来源：http://ft.jianghongdianzi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bi.huanxung.cn

Ruby: s.length
来源：http://du.jianghongdianzi.cn

C#:   s.Length
来源：http://ls.hahajie.cn

[A23] 大小写转换
来源：http://mz.huixiangedu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://gx.muxihuayi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wu.muxihuayi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kh.521024.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mm.shxzukj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ja.wgjwhj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lx.haigaiapp.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bw.shxzskj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://kd.haigaiapp.cn

[A24] 去除首尾空白
来源：http://nh.chemitech.net.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://yj.panjiajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mx.jianghongdianzi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://in.asd995.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qz.shtwfgs.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zk.gzmigu.cn

Go:   strings.TrimSpace(s)
来源：http://iu.chemitech.net.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dn.gzmigu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ho.9csxet.cn

[A25] 字符串比较
来源：http://bz.bjjhwx.cn

Py:   s1 == s2; s1 != s2
来源：http://za.chemitech.net.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ac.hnjuh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bh.muxihuayi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://na.9csxet.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zz.szsharing.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yz.szxytkj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://av.bjjhwx.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cy.chemitech.net.cn

[A26] 类型转换总览
来源：http://kn.lnxyls.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bq.huixinmuqiang.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xz.huixinmuqiang.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hx.huixinmuqiang.cn

TS:   Number() String() Boolean() x as number
来源：http://mv.huixinmuqiang.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hr.huixinmuqiang.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yx.szsharing.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vu.muxihuayi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nf.colortex.cn

================================================================================
来源：http://nv.huanxung.cn

B. 流程控制
来源：http://ub.colortex.cn

================================================================================
来源：http://wg.nszjky.cn

[B01] 条件判断 if / else
来源：http://vc.521024.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vf.gzmigu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yx.shxzskj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gs.nszjky.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ec.lnxyls.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vz.jctech888.com.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mi.szsharing.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yr.bookmarksfly.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ra.lnxyls.cn

[B02] 多分支 else if / elif
来源：http://td.shtwfgs.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kd.shxzukj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xh.muxihuayi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://je.bjjhwx.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fv.shxzskj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lg.yuntaijiaju.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://iu.bookmarksfly.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ie.9csxet.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ni.asd995.cn

[B03] switch / match / case
来源：http://mp.wgjwhj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gc.muxihuayi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fn.yuexingan06.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://iq.nszjky.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uq.huixiangedu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vb.newstarts.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jo.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ng.9csxet.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xe.jianghongdianzi.cn

[B04] for 计数循环
来源：http://ar.asd995.cn

Py:   for i in range(10): print(i)
来源：http://ac.yuexingan06.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rw.colortex.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qv.shtwfgs.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oe.yuexingan06.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nu.asd995.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zr.nicolike.cn

Ruby: 10.times { |i| puts i }
来源：http://nk.szxytkj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dh.panjiajie.cn

[B05] 遍历数组 / 列表
来源：http://zx.gzmigu.cn

Py:   for item in arr: print(item)
来源：http://fw.9csxet.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wu.panjiajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ez.haigaiapp.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://jj.shtwfgs.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qy.colortex.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ka.asd995.cn

Ruby: arr.each { |item| puts item }
来源：http://dc.shxzukj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cf.bookmarksfly.cn

[B06] 遍历字典 / 对象
来源：http://xc.huanxung.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://cx.hnjuh.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cq.wgjwhj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lf.shxzskj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mu.lnxyls.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cn.yuntaijiaju.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wr.szxytkj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mw.huanxung.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ny.nszjky.cn

[B07] while 循环
来源：http://lz.szsharing.cn

Py:   while i < 10: i += 1
来源：http://xc.jctech888.com.cn

PHP:  while ($i < 10) { $i++; }
来源：http://tl.wgjwhj.cn

JS:   while (i < 10) { i++; }
来源：http://hc.lnxyls.cn

TS:   while (i < 10) { i++; }
来源：http://lq.asd995.cn

Java: while (i < 10) { i++; }
来源：http://na.jctech888.com.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://eo.szxytkj.cn

Ruby: while i < 10; i += 1; end
来源：http://ww.chemitech.net.cn

C#:   while (i < 10) { i++; }
来源：http://vx.haigaiapp.cn

[B08] do-while（至少执行一次）
来源：http://hj.nicolike.cn

Py:   # 无 do-while：用 while True + break
来源：http://rf.asd995.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://tu.muxihuayi.cn

JS:   do { i++; } while (i < 10);
来源：http://sz.asd995.cn

TS:   do { i++; } while (i < 10);
来源：http://nc.shtwfgs.cn

Java: do { i++; } while (i < 10);
来源：http://yk.bookmarksfly.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://lp.shxzskj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://kc.lnxyls.cn

C#:   do { i++; } while (i < 10);
来源：http://iu.szsharing.cn

[B09] break 与 continue
来源：http://sq.panjiajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nn.hnjuh.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cx.nicolike.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gz.jianghongdianzi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uv.huanxung.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ss.gzmigu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tg.bookmarksfly.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://in.lnxyls.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ja.wgjwhj.cn

[B10] 遍历同时拿索引
来源：http://ss.panjiajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rs.huixiangedu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://oq.newstarts.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mb.lnxyls.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gt.newstarts.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qm.newstarts.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ic.gzmigu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://es.jianghongdianzi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qa.colortex.cn

[B11] 生成数字序列 / 区间
来源：http://mf.yuexingan06.cn

Py:   list(range(0, 10, 2))
来源：http://jf.szsharing.cn

PHP:  range(0, 10, 2);
来源：http://fr.hahajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fm.asd995.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://et.muxihuayi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pj.bookmarksfly.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jx.9csxet.cn

Ruby: (0...10).step(2).to_a
来源：http://ru.nszjky.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rq.haigaiapp.cn

[B12] 跳出多层循环
来源：http://uy.9csxet.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://py.szsharing.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gd.521024.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tc.shxzukj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bx.bjjhwx.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://op.panjiajie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mr.hahajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mx.jianghongdianzi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uk.huixinmuqiang.cn

[B13] 判断是否为数字
来源：http://ui.yuexingan06.cn

Py:   isinstance(x, (int, float))
来源：http://np.newstarts.cn

PHP:  is_numeric($x)
来源：http://vw.hahajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://id.asd995.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sf.muxihuayi.cn

Java: x instanceof Number
来源：http://bw.huixiangedu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jc.chemitech.net.cn

Ruby: x.is_a?(Numeric)
来源：http://pz.yuexingan06.cn

C#:   x is int or double or decimal
来源：http://vw.chemitech.net.cn

[B14] 判断值是否在集合内
来源：http://gl.9csxet.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lf.huanxung.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hh.huixiangedu.cn

JS:   [1, 2, 3].includes(x)
来源：http://wv.panjiajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://lz.muxihuayi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://oq.bjjhwx.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wz.huixinmuqiang.cn

Ruby: [1, 2, 3].include?(x)
来源：http://pw.huanxung.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yv.yuexingan06.cn

[B15] 布尔运算与取反
来源：http://tm.jctech888.com.cn

Py:   a and b or not c
来源：http://zm.lnxyls.cn

PHP:  $a && $b || !$c
来源：http://hv.shxzskj.cn

JS:   a && b || !c
来源：http://fp.lnxyls.cn

TS:   a && b || !c
来源：http://nm.bookmarksfly.cn

Java: a && b || !c
来源：http://vb.yuntaijiaju.cn

Go:   a && b || !c
来源：http://pa.gzmigu.cn

Ruby: a && b || !c
来源：http://jx.colortex.cn

C#:   a && b || !c
来源：http://sn.panjiajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://sr.muxihuayi.cn

Py:   if not data: return
来源：http://np.huixiangedu.cn

PHP:  if (!$data) { return; }
来源：http://ru.szxytkj.cn

JS:   if (!data) return;
来源：http://ei.521024.cn

TS:   if (!data) return;
来源：http://rh.chemitech.net.cn

Java: if (data == null) return;
来源：http://gp.yuexingan06.cn

Go:   if data == nil { return }
来源：http://mp.newstarts.cn

Ruby: return if data.nil?
来源：http://me.gzmigu.cn

C#:   if (data == null) return;
来源：http://vs.shxzskj.cn

================================================================================
来源：http://vj.muxihuayi.cn

C. 函数与作用域
来源：http://cn.huanxung.cn

================================================================================
来源：http://wc.9csxet.cn

[C01] 定义函数
来源：http://qy.huixiangedu.cn

Py:   def add(a, b): return a + b
来源：http://lj.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ts.lnxyls.cn

JS:   function add(a, b) { return a + b; }
来源：http://ie.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://aq.asd995.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lz.huixiangedu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ri.shxzskj.cn

Ruby: def add(a, b); a + b; end
来源：http://qd.szsharing.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://df.nicolike.cn

[C02] 默认参数
来源：http://uy.huixinmuqiang.cn

Py:   def greet(name="World"): return name
来源：http://az.jianghongdianzi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://sy.hahajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://ft.521024.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rb.panjiajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hd.wgjwhj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gv.yuntaijiaju.cn

Ruby: def greet(name = "World") = name
来源：http://vw.shxzskj.cn

C#:   string Greet(string name = "World") => name;
来源：http://px.asd995.cn

[C03] 可变参数
来源：http://ol.9csxet.cn

Py:   def total(*args): return sum(args)
来源：http://rf.colortex.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hx.jctech888.com.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gu.huixiangedu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vn.huixiangedu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gq.nszjky.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tt.newstarts.cn

Ruby: def total(*nums); nums.sum; end
来源：http://cv.colortex.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zs.yuntaijiaju.cn

[C04] 命名参数 / 关键字参数
来源：http://hv.hahajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fb.jianghongdianzi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tt.szsharing.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xp.bookmarksfly.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ah.muxihuayi.cn

Java: // 无：用 Builder 模式或 record
来源：http://fa.huixiangedu.cn

Go:   // 无：用配置结构体参数
来源：http://ev.yuntaijiaju.cn

Ruby: f(a: 1, b: 2)
来源：http://tw.muxihuayi.cn

C#:   f(a: 1, b: 2)
来源：http://rx.lnxyls.cn

[C05] 返回多个值
来源：http://vr.yuntaijiaju.cn

Py:   return a, b
来源：http://gk.jianghongdianzi.cn

PHP:  return [$a, $b];
来源：http://hw.huixinmuqiang.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ka.panjiajie.cn

TS:   return { a, b };
来源：http://ul.hahajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lr.haigaiapp.cn

Go:   return a, b
来源：http://ao.9csxet.cn

Ruby: return a, b
来源：http://go.hahajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://la.lnxyls.cn

[C06] 匿名函数 / lambda
来源：http://gv.shxzukj.cn

Py:   square = lambda x: x * x
来源：http://lx.huixiangedu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://yi.nszjky.cn

JS:   const square = x => x * x;
来源：http://uc.bjjhwx.cn

TS:   const square = (x: number): number => x * x;
来源：http://hx.bookmarksfly.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dg.nicolike.cn

Go:   sq := func(x int) int { return x * x }
来源：http://bg.shxzskj.cn

Ruby: square = ->(x) { x * x }
来源：http://us.muxihuayi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ow.huixinmuqiang.cn

[C07] 把函数作为参数传入
来源：http://mz.521024.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fg.asd995.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jk.huixiangedu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qo.yuntaijiaju.cn

TS:   arr.map(String)
来源：http://bm.yuntaijiaju.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xt.hahajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wg.szsharing.cn

Ruby: arr.map(&:upcase)
来源：http://dm.hnjuh.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://oo.shtwfgs.cn

[C08] 闭包
来源：http://ld.shxzukj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ah.bookmarksfly.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vv.jianghongdianzi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ey.bjjhwx.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zv.colortex.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://al.haigaiapp.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pe.hahajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hh.huixinmuqiang.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ou.lnxyls.cn

[C09] 递归
来源：http://pn.shtwfgs.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uw.bjjhwx.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pw.szxytkj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pq.521024.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yo.asd995.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tv.asd995.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lt.bookmarksfly.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yl.lnxyls.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qo.haigaiapp.cn

[C10] 变量作用域
来源：http://wa.huixinmuqiang.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cc.szxytkj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lk.lnxyls.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bc.shxzukj.cn

TS:   同 JS
来源：http://vq.nicolike.cn

Java: 方法内为块级作用域
来源：http://iz.shxzskj.cn

Go:   花括号块级作用域
来源：http://dn.hahajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pg.newstarts.cn

C#:   块级作用域
来源：http://sr.hahajie.cn

[C11] 模块导入与导出
来源：http://yy.lnxyls.cn

Py:   from module import func
来源：http://xv.shxzskj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pa.jianghongdianzi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ln.nszjky.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hr.shxzukj.cn

Java: import java.util.List;
来源：http://ly.9csxet.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bk.colortex.cn


<!-- 参考信息 -->