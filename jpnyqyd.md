代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://ni.nicolike.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ch.jianghongdianzi.cn

Ruby: format("%.2f", 3.14159)
来源：http://wj.szxytkj.cn

C#:   3.14159.ToString("F2")
来源：http://tj.9csxet.cn

[A22] 获取字符串长度
来源：http://xs.haigaiapp.cn

Py:   len(s)
来源：http://ye.chemitech.net.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vm.huixinmuqiang.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rd.hahajie.cn

TS:   s.length
来源：http://hx.asd995.cn

Java: s.length()
来源：http://vm.shxzukj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ac.nicolike.cn

Ruby: s.length
来源：http://xn.huanxung.cn

C#:   s.Length
来源：http://nw.jctech888.com.cn

[A23] 大小写转换
来源：http://bi.bjjhwx.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://df.szxytkj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hl.521024.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://uf.colortex.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tv.lnxyls.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pv.panjiajie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yt.9csxet.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fd.huixiangedu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://yw.bjjhwx.cn

[A24] 去除首尾空白
来源：http://fb.szxytkj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fw.colortex.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lh.jianghongdianzi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://he.huanxung.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xh.huixinmuqiang.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zl.chemitech.net.cn

Go:   strings.TrimSpace(s)
来源：http://oe.huanxung.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://df.shtwfgs.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://bb.szxytkj.cn

[A25] 字符串比较
来源：http://xv.chemitech.net.cn

Py:   s1 == s2; s1 != s2
来源：http://np.jctech888.com.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ls.hahajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vu.lnxyls.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wx.panjiajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://at.lnxyls.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kb.szxytkj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://wr.colortex.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://li.chemitech.net.cn

[A26] 类型转换总览
来源：http://ww.521024.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sv.asd995.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ab.hnjuh.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jn.jctech888.com.cn

TS:   Number() String() Boolean() x as number
来源：http://mq.huanxung.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lp.shtwfgs.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tn.shtwfgs.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://md.bookmarksfly.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rv.huixiangedu.cn

================================================================================
来源：http://uh.jianghongdianzi.cn

B. 流程控制
来源：http://cz.wgjwhj.cn

================================================================================
来源：http://jx.haigaiapp.cn

[B01] 条件判断 if / else
来源：http://mu.huixiangedu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://sw.jctech888.com.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jz.newstarts.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ka.jctech888.com.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ht.yuntaijiaju.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://to.nszjky.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nw.asd995.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hi.chemitech.net.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ea.wgjwhj.cn

[B02] 多分支 else if / elif
来源：http://do.asd995.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lw.szsharing.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qy.haigaiapp.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ga.asd995.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ns.yuexingan06.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cw.nicolike.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tv.shtwfgs.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tp.huanxung.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gh.huixiangedu.cn

[B03] switch / match / case
来源：http://sv.jianghongdianzi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hu.wgjwhj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ad.bjjhwx.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qx.hnjuh.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ud.gzmigu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dd.gzmigu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ov.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nv.521024.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lk.shtwfgs.cn

[B04] for 计数循环
来源：http://qg.huixinmuqiang.cn

Py:   for i in range(10): print(i)
来源：http://ny.szsharing.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qw.jctech888.com.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sb.shxzskj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dw.nszjky.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://da.haigaiapp.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qx.yuntaijiaju.cn

Ruby: 10.times { |i| puts i }
来源：http://gl.muxihuayi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://af.bookmarksfly.cn

[B05] 遍历数组 / 列表
来源：http://jt.nszjky.cn

Py:   for item in arr: print(item)
来源：http://yz.wgjwhj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hg.huixiangedu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://xj.asd995.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://sx.panjiajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://of.huixinmuqiang.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fy.panjiajie.cn

Ruby: arr.each { |item| puts item }
来源：http://mz.huixinmuqiang.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kp.huanxung.cn

[B06] 遍历字典 / 对象
来源：http://ia.huanxung.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xe.newstarts.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vm.haigaiapp.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mu.nszjky.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ev.wgjwhj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ao.jianghongdianzi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dy.shtwfgs.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hl.shxzukj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ol.bjjhwx.cn

[B07] while 循环
来源：http://py.colortex.cn

Py:   while i < 10: i += 1
来源：http://yy.yuntaijiaju.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zz.hnjuh.cn

JS:   while (i < 10) { i++; }
来源：http://xr.hnjuh.cn

TS:   while (i < 10) { i++; }
来源：http://mp.hahajie.cn

Java: while (i < 10) { i++; }
来源：http://nm.shtwfgs.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wh.muxihuayi.cn

Ruby: while i < 10; i += 1; end
来源：http://gz.shtwfgs.cn

C#:   while (i < 10) { i++; }
来源：http://da.shxzukj.cn

[B08] do-while（至少执行一次）
来源：http://rt.nszjky.cn

Py:   # 无 do-while：用 while True + break
来源：http://zq.nszjky.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://yw.bjjhwx.cn

JS:   do { i++; } while (i < 10);
来源：http://ur.yuntaijiaju.cn

TS:   do { i++; } while (i < 10);
来源：http://zi.521024.cn

Java: do { i++; } while (i < 10);
来源：http://gf.wgjwhj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xw.hahajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pt.szxytkj.cn

C#:   do { i++; } while (i < 10);
来源：http://vo.yuntaijiaju.cn

[B09] break 与 continue
来源：http://rz.szsharing.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dm.9csxet.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bp.wgjwhj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://su.bjjhwx.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ag.newstarts.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cb.szxytkj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xi.jianghongdianzi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ym.yuexingan06.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://id.szsharing.cn

[B10] 遍历同时拿索引
来源：http://za.asd995.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lt.panjiajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mw.gzmigu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ej.nszjky.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ek.yuntaijiaju.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rj.hahajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://im.asd995.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://su.yuntaijiaju.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zy.haigaiapp.cn

[B11] 生成数字序列 / 区间
来源：http://bj.colortex.cn

Py:   list(range(0, 10, 2))
来源：http://ld.jctech888.com.cn

PHP:  range(0, 10, 2);
来源：http://te.huanxung.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lf.muxihuayi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uz.muxihuayi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://si.shtwfgs.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rn.bookmarksfly.cn

Ruby: (0...10).step(2).to_a
来源：http://xm.shxzskj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gi.wgjwhj.cn

[B12] 跳出多层循环
来源：http://ga.9csxet.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://sz.newstarts.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fn.yuexingan06.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xy.9csxet.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fx.nicolike.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xy.szxytkj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ma.yuntaijiaju.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yf.521024.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kk.shxzukj.cn

[B13] 判断是否为数字
来源：http://ea.haigaiapp.cn

Py:   isinstance(x, (int, float))
来源：http://at.wgjwhj.cn

PHP:  is_numeric($x)
来源：http://nh.szsharing.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uy.haigaiapp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cv.asd995.cn

Java: x instanceof Number
来源：http://ha.lnxyls.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uv.hnjuh.cn

Ruby: x.is_a?(Numeric)
来源：http://ac.haigaiapp.cn

C#:   x is int or double or decimal
来源：http://vp.chemitech.net.cn

[B14] 判断值是否在集合内
来源：http://tj.newstarts.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cm.szsharing.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ix.huanxung.cn

JS:   [1, 2, 3].includes(x)
来源：http://px.jianghongdianzi.cn

TS:   [1, 2, 3].includes(x)
来源：http://hf.gzmigu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ia.gzmigu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vm.haigaiapp.cn

Ruby: [1, 2, 3].include?(x)
来源：http://pd.muxihuayi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yx.wgjwhj.cn

[B15] 布尔运算与取反
来源：http://bd.bjjhwx.cn

Py:   a and b or not c
来源：http://sx.yuntaijiaju.cn

PHP:  $a && $b || !$c
来源：http://de.521024.cn

JS:   a && b || !c
来源：http://sw.9csxet.cn

TS:   a && b || !c
来源：http://ja.panjiajie.cn

Java: a && b || !c
来源：http://wa.panjiajie.cn

Go:   a && b || !c
来源：http://rn.gzmigu.cn

Ruby: a && b || !c
来源：http://qq.asd995.cn

C#:   a && b || !c
来源：http://tk.colortex.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lu.hahajie.cn

Py:   if not data: return
来源：http://uy.9csxet.cn

PHP:  if (!$data) { return; }
来源：http://rs.shxzskj.cn

JS:   if (!data) return;
来源：http://hv.521024.cn

TS:   if (!data) return;
来源：http://wo.huixiangedu.cn

Java: if (data == null) return;
来源：http://ry.shxzskj.cn

Go:   if data == nil { return }
来源：http://hk.asd995.cn

Ruby: return if data.nil?
来源：http://xg.panjiajie.cn

C#:   if (data == null) return;
来源：http://mq.yuntaijiaju.cn

================================================================================
来源：http://qa.huixiangedu.cn

C. 函数与作用域
来源：http://it.nicolike.cn

================================================================================
来源：http://zx.muxihuayi.cn

[C01] 定义函数
来源：http://iu.nszjky.cn

Py:   def add(a, b): return a + b
来源：http://lc.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pf.panjiajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://mp.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kz.bjjhwx.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://kz.nicolike.cn

Go:   func add(a, b int) int { return a + b }
来源：http://wz.shxzskj.cn

Ruby: def add(a, b); a + b; end
来源：http://dh.colortex.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xq.huanxung.cn

[C02] 默认参数
来源：http://sk.asd995.cn

Py:   def greet(name="World"): return name
来源：http://ec.chemitech.net.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bu.yuntaijiaju.cn

JS:   function greet(name = "World") { return name; }
来源：http://fj.panjiajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xv.huixinmuqiang.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://up.huixiangedu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://so.newstarts.cn

Ruby: def greet(name = "World") = name
来源：http://gu.shxzskj.cn

C#:   string Greet(string name = "World") => name;
来源：http://jo.haigaiapp.cn

[C03] 可变参数
来源：http://xa.huixiangedu.cn

Py:   def total(*args): return sum(args)
来源：http://sz.huixiangedu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://be.shtwfgs.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tm.newstarts.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cl.newstarts.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rb.hahajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cc.jctech888.com.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ia.wgjwhj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wf.521024.cn

[C04] 命名参数 / 关键字参数
来源：http://ci.asd995.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jx.wgjwhj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wz.huixiangedu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lu.jctech888.com.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vy.newstarts.cn

Java: // 无：用 Builder 模式或 record
来源：http://my.huixiangedu.cn

Go:   // 无：用配置结构体参数
来源：http://ke.newstarts.cn

Ruby: f(a: 1, b: 2)
来源：http://sm.huixinmuqiang.cn

C#:   f(a: 1, b: 2)
来源：http://mq.hahajie.cn

[C05] 返回多个值
来源：http://vo.colortex.cn

Py:   return a, b
来源：http://fc.nszjky.cn

PHP:  return [$a, $b];
来源：http://eq.szsharing.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://un.huixiangedu.cn

TS:   return { a, b };
来源：http://hk.jctech888.com.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ky.newstarts.cn

Go:   return a, b
来源：http://sf.huixinmuqiang.cn

Ruby: return a, b
来源：http://ds.nszjky.cn

C#:   return (a, b);              // ValueTuple
来源：http://dh.huixiangedu.cn

[C06] 匿名函数 / lambda
来源：http://jp.szxytkj.cn

Py:   square = lambda x: x * x
来源：http://tr.huixinmuqiang.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://sf.yuntaijiaju.cn

JS:   const square = x => x * x;
来源：http://mt.jctech888.com.cn

TS:   const square = (x: number): number => x * x;
来源：http://ta.shxzukj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gg.asd995.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fw.bjjhwx.cn

Ruby: square = ->(x) { x * x }
来源：http://dt.shxzukj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://he.lnxyls.cn

[C07] 把函数作为参数传入
来源：http://zm.yuntaijiaju.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gz.bookmarksfly.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ni.huanxung.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bc.colortex.cn

TS:   arr.map(String)
来源：http://py.asd995.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qa.szsharing.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qr.szsharing.cn

Ruby: arr.map(&:upcase)
来源：http://mi.nicolike.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ja.shxzskj.cn

[C08] 闭包
来源：http://xa.yuntaijiaju.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cq.asd995.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://av.haigaiapp.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fc.hahajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yf.huanxung.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ov.huixiangedu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://oq.panjiajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://oj.wgjwhj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rm.szxytkj.cn

[C09] 递归
来源：http://dh.bookmarksfly.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bw.haigaiapp.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ox.shxzskj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://um.huixinmuqiang.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hy.9csxet.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kt.jianghongdianzi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jc.asd995.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://iy.shxzskj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yp.szsharing.cn

[C10] 变量作用域
来源：http://xh.szsharing.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dj.colortex.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zg.yuntaijiaju.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cz.yuexingan06.cn

TS:   同 JS
来源：http://ak.hnjuh.cn

Java: 方法内为块级作用域
来源：http://tg.szxytkj.cn

Go:   花括号块级作用域
来源：http://me.wgjwhj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lu.jianghongdianzi.cn

C#:   块级作用域
来源：http://dt.521024.cn

[C11] 模块导入与导出
来源：http://mr.colortex.cn

Py:   from module import func
来源：http://lq.huixinmuqiang.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://nt.shxzukj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fm.huixiangedu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vc.szsharing.cn

Java: import java.util.List;
来源：http://lt.szxytkj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lr.hahajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://jf.hahajie.cn

C#:   using System.Text;
来源：http://mj.asd995.cn

[C12] 立即执行函数 IIFE
来源：http://zb.hnjuh.cn

Py:   (lambda: print("run"))()
来源：http://qe.haigaiapp.cn


<!-- 参考信息 -->