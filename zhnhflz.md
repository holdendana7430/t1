代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://ck.panjiajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zh.gzmigu.cn

JS:   (3.14159).toFixed(2)
来源：http://ac.yuntaijiaju.cn

TS:   (3.14159).toFixed(2)
来源：http://la.newstarts.cn

Java: String.format("%.2f", 3.14159)
来源：http://fd.jctech888.com.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pb.chemitech.net.cn

Ruby: format("%.2f", 3.14159)
来源：http://xy.muxihuayi.cn

C#:   3.14159.ToString("F2")
来源：http://nl.wgjwhj.cn

[A22] 获取字符串长度
来源：http://um.521024.cn

Py:   len(s)
来源：http://eq.shxzskj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zs.jianghongdianzi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://du.bjjhwx.cn

TS:   s.length
来源：http://pf.jianghongdianzi.cn

Java: s.length()
来源：http://hd.bookmarksfly.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vd.jianghongdianzi.cn

Ruby: s.length
来源：http://wu.yuntaijiaju.cn

C#:   s.Length
来源：http://at.huixiangedu.cn

[A23] 大小写转换
来源：http://ud.lnxyls.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://my.yuexingan06.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://su.shtwfgs.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wv.muxihuayi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zz.nicolike.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xb.521024.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://el.yuntaijiaju.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ji.szsharing.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://lr.jianghongdianzi.cn

[A24] 去除首尾空白
来源：http://fa.shxzukj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://og.shtwfgs.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wj.haigaiapp.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ph.szxytkj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uu.asd995.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ij.shxzukj.cn

Go:   strings.TrimSpace(s)
来源：http://kf.nszjky.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fp.panjiajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://bd.huixiangedu.cn

[A25] 字符串比较
来源：http://kz.9csxet.cn

Py:   s1 == s2; s1 != s2
来源：http://qr.shxzskj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jq.hnjuh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hp.jctech888.com.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gl.colortex.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vg.szsharing.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ka.hahajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ox.hahajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://za.jctech888.com.cn

[A26] 类型转换总览
来源：http://ft.wgjwhj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vt.haigaiapp.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://aa.9csxet.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://de.nszjky.cn

TS:   Number() String() Boolean() x as number
来源：http://mv.szxytkj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kh.szxytkj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xt.gzmigu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://qw.panjiajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yl.newstarts.cn

================================================================================
来源：http://lr.jctech888.com.cn

B. 流程控制
来源：http://gz.bookmarksfly.cn

================================================================================
来源：http://dv.yuntaijiaju.cn

[B01] 条件判断 if / else
来源：http://gu.muxihuayi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ea.bookmarksfly.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ow.gzmigu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sx.bjjhwx.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bs.shxzukj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://se.szsharing.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ji.muxihuayi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://md.wgjwhj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qj.9csxet.cn

[B02] 多分支 else if / elif
来源：http://br.huixiangedu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://la.muxihuayi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hm.521024.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ah.jianghongdianzi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://em.hnjuh.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zq.szsharing.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ag.wgjwhj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mr.chemitech.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ek.yuexingan06.cn

[B03] switch / match / case
来源：http://pe.asd995.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bm.shxzskj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ia.521024.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pl.szxytkj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nj.lnxyls.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qi.bjjhwx.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qc.gzmigu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dz.yuexingan06.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bi.bookmarksfly.cn

[B04] for 计数循环
来源：http://hj.521024.cn

Py:   for i in range(10): print(i)
来源：http://ey.newstarts.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ir.huanxung.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ol.huixiangedu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zi.hahajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yz.yuntaijiaju.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qg.521024.cn

Ruby: 10.times { |i| puts i }
来源：http://tk.shxzskj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hf.gzmigu.cn

[B05] 遍历数组 / 列表
来源：http://ly.colortex.cn

Py:   for item in arr: print(item)
来源：http://eg.bookmarksfly.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kv.yuntaijiaju.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://vs.yuexingan06.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://sh.huanxung.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://so.jctech888.com.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vg.nicolike.cn

Ruby: arr.each { |item| puts item }
来源：http://fj.gzmigu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hl.newstarts.cn

[B06] 遍历字典 / 对象
来源：http://fh.szsharing.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://et.9csxet.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zd.asd995.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rk.szxytkj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jm.9csxet.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ri.huixinmuqiang.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://td.huixiangedu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qh.szsharing.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dp.huanxung.cn

[B07] while 循环
来源：http://tj.521024.cn

Py:   while i < 10: i += 1
来源：http://ha.huixinmuqiang.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fl.bookmarksfly.cn

JS:   while (i < 10) { i++; }
来源：http://gs.nszjky.cn

TS:   while (i < 10) { i++; }
来源：http://kz.shxzukj.cn

Java: while (i < 10) { i++; }
来源：http://on.bjjhwx.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vo.bookmarksfly.cn

Ruby: while i < 10; i += 1; end
来源：http://ci.9csxet.cn

C#:   while (i < 10) { i++; }
来源：http://pk.asd995.cn

[B08] do-while（至少执行一次）
来源：http://dp.szsharing.cn

Py:   # 无 do-while：用 while True + break
来源：http://dw.haigaiapp.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://rr.szsharing.cn

JS:   do { i++; } while (i < 10);
来源：http://xp.chemitech.net.cn

TS:   do { i++; } while (i < 10);
来源：http://hv.muxihuayi.cn

Java: do { i++; } while (i < 10);
来源：http://xs.huanxung.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://qi.chemitech.net.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vm.jianghongdianzi.cn

C#:   do { i++; } while (i < 10);
来源：http://hx.hnjuh.cn

[B09] break 与 continue
来源：http://kz.lnxyls.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ea.colortex.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wr.szxytkj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ip.jianghongdianzi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pb.muxihuayi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ew.nicolike.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wp.yuntaijiaju.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bh.jctech888.com.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fe.bjjhwx.cn

[B10] 遍历同时拿索引
来源：http://kl.lnxyls.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vr.newstarts.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xw.colortex.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rq.huanxung.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fb.bookmarksfly.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zo.shtwfgs.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ld.huanxung.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fx.huixinmuqiang.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dn.panjiajie.cn

[B11] 生成数字序列 / 区间
来源：http://oa.yuntaijiaju.cn

Py:   list(range(0, 10, 2))
来源：http://fg.jianghongdianzi.cn

PHP:  range(0, 10, 2);
来源：http://ds.yuntaijiaju.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vx.huixinmuqiang.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yi.huixiangedu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qa.hnjuh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://md.gzmigu.cn

Ruby: (0...10).step(2).to_a
来源：http://gn.bookmarksfly.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ky.wgjwhj.cn

[B12] 跳出多层循环
来源：http://ny.yuntaijiaju.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://oe.hnjuh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://xa.szsharing.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://oo.haigaiapp.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ub.hahajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rd.jianghongdianzi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nh.huixinmuqiang.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wt.chemitech.net.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://is.jianghongdianzi.cn

[B13] 判断是否为数字
来源：http://jy.jctech888.com.cn

Py:   isinstance(x, (int, float))
来源：http://dd.bjjhwx.cn

PHP:  is_numeric($x)
来源：http://il.wgjwhj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lc.521024.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vw.yuntaijiaju.cn

Java: x instanceof Number
来源：http://cz.muxihuayi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://be.szxytkj.cn

Ruby: x.is_a?(Numeric)
来源：http://ck.newstarts.cn

C#:   x is int or double or decimal
来源：http://cw.nszjky.cn

[B14] 判断值是否在集合内
来源：http://am.bjjhwx.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ru.shtwfgs.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://uk.lnxyls.cn

JS:   [1, 2, 3].includes(x)
来源：http://bo.bookmarksfly.cn

TS:   [1, 2, 3].includes(x)
来源：http://gd.asd995.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ia.szsharing.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gl.shxzukj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xa.chemitech.net.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bj.szsharing.cn

[B15] 布尔运算与取反
来源：http://au.szsharing.cn

Py:   a and b or not c
来源：http://ud.huixiangedu.cn

PHP:  $a && $b || !$c
来源：http://xv.jctech888.com.cn

JS:   a && b || !c
来源：http://uy.szxytkj.cn

TS:   a && b || !c
来源：http://te.yuntaijiaju.cn

Java: a && b || !c
来源：http://xx.bjjhwx.cn

Go:   a && b || !c
来源：http://ve.hahajie.cn

Ruby: a && b || !c
来源：http://ig.szxytkj.cn

C#:   a && b || !c
来源：http://re.yuexingan06.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vs.shtwfgs.cn

Py:   if not data: return
来源：http://cm.jctech888.com.cn

PHP:  if (!$data) { return; }
来源：http://fk.colortex.cn

JS:   if (!data) return;
来源：http://fx.gzmigu.cn

TS:   if (!data) return;
来源：http://tr.521024.cn

Java: if (data == null) return;
来源：http://fu.bookmarksfly.cn

Go:   if data == nil { return }
来源：http://zz.szsharing.cn

Ruby: return if data.nil?
来源：http://pb.shtwfgs.cn

C#:   if (data == null) return;
来源：http://sf.521024.cn

================================================================================
来源：http://bv.huanxung.cn

C. 函数与作用域
来源：http://mk.shxzskj.cn

================================================================================
来源：http://gm.huixinmuqiang.cn

[C01] 定义函数
来源：http://qb.colortex.cn

Py:   def add(a, b): return a + b
来源：http://jl.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yb.yuntaijiaju.cn

JS:   function add(a, b) { return a + b; }
来源：http://mu.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pe.szxytkj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://pk.lnxyls.cn

Go:   func add(a, b int) int { return a + b }
来源：http://yx.hahajie.cn

Ruby: def add(a, b); a + b; end
来源：http://jb.shtwfgs.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://iw.shxzukj.cn

[C02] 默认参数
来源：http://ln.huixiangedu.cn

Py:   def greet(name="World"): return name
来源：http://rf.yuntaijiaju.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://pd.panjiajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://uv.bjjhwx.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bh.huixiangedu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qr.szsharing.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xp.yuntaijiaju.cn

Ruby: def greet(name = "World") = name
来源：http://ns.yuntaijiaju.cn

C#:   string Greet(string name = "World") => name;
来源：http://fx.szxytkj.cn

[C03] 可变参数
来源：http://qn.shtwfgs.cn

Py:   def total(*args): return sum(args)
来源：http://lz.yuexingan06.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://na.wgjwhj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dx.panjiajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jm.bjjhwx.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ms.hahajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cp.hnjuh.cn

Ruby: def total(*nums); nums.sum; end
来源：http://do.nicolike.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yt.521024.cn

[C04] 命名参数 / 关键字参数
来源：http://ok.nicolike.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://km.chemitech.net.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fl.yuntaijiaju.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jm.jctech888.com.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://re.bjjhwx.cn

Java: // 无：用 Builder 模式或 record
来源：http://xj.nicolike.cn

Go:   // 无：用配置结构体参数
来源：http://st.9csxet.cn

Ruby: f(a: 1, b: 2)
来源：http://gg.lnxyls.cn

C#:   f(a: 1, b: 2)
来源：http://qn.shtwfgs.cn

[C05] 返回多个值
来源：http://vq.asd995.cn

Py:   return a, b
来源：http://hg.hnjuh.cn

PHP:  return [$a, $b];
来源：http://da.colortex.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://as.bjjhwx.cn

TS:   return { a, b };
来源：http://hh.shxzukj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://il.hnjuh.cn

Go:   return a, b
来源：http://xa.nicolike.cn

Ruby: return a, b
来源：http://ae.jctech888.com.cn

C#:   return (a, b);              // ValueTuple
来源：http://pu.haigaiapp.cn

[C06] 匿名函数 / lambda
来源：http://ch.gzmigu.cn

Py:   square = lambda x: x * x
来源：http://dr.9csxet.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ou.shtwfgs.cn

JS:   const square = x => x * x;
来源：http://ce.gzmigu.cn

TS:   const square = (x: number): number => x * x;
来源：http://ps.hnjuh.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tv.hahajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://nr.521024.cn

Ruby: square = ->(x) { x * x }
来源：http://yl.huanxung.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hq.bookmarksfly.cn

[C07] 把函数作为参数传入
来源：http://aa.gzmigu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lt.bjjhwx.cn

PHP:  array_map("strtoupper", $arr);
来源：http://eb.shtwfgs.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ii.nszjky.cn

TS:   arr.map(String)
来源：http://ih.jctech888.com.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vn.yuexingan06.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dh.jianghongdianzi.cn

Ruby: arr.map(&:upcase)
来源：http://ez.huanxung.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://bh.shxzukj.cn

[C08] 闭包
来源：http://zn.jianghongdianzi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://aq.hnjuh.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ep.jianghongdianzi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://il.muxihuayi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bc.szsharing.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fs.yuexingan06.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mq.gzmigu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ia.huixiangedu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gl.yuexingan06.cn

[C09] 递归
来源：http://xu.panjiajie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mn.hnjuh.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://za.wgjwhj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ff.gzmigu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://us.shxzukj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xk.szsharing.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ef.wgjwhj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ef.9csxet.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://is.panjiajie.cn

[C10] 变量作用域
来源：http://jv.bjjhwx.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://aq.haigaiapp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jc.hnjuh.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dh.huixinmuqiang.cn

TS:   同 JS
来源：http://ki.colortex.cn

Java: 方法内为块级作用域
来源：http://bn.521024.cn

Go:   花括号块级作用域
来源：http://qu.bjjhwx.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yy.huixinmuqiang.cn

C#:   块级作用域
来源：http://qo.bjjhwx.cn

[C11] 模块导入与导出
来源：http://ic.bookmarksfly.cn

Py:   from module import func
来源：http://ht.shtwfgs.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ef.hahajie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rg.hahajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rm.huanxung.cn

Java: import java.util.List;
来源：http://ux.newstarts.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dv.chemitech.net.cn


<!-- 参考信息 -->