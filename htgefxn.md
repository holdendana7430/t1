代发 wailian999

[A22] 获取字符串长度
来源：http://kq.nszjky.cn

Py:   len(s)
来源：http://fn.bookmarksfly.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jv.wgjwhj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ue.9csxet.cn

TS:   s.length
来源：http://di.colortex.cn

Java: s.length()
来源：http://qo.hahajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xu.521024.cn

Ruby: s.length
来源：http://um.nszjky.cn

C#:   s.Length
来源：http://fj.wgjwhj.cn

[A23] 大小写转换
来源：http://ef.nszjky.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://nc.lnxyls.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ns.szxytkj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gu.haigaiapp.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tm.huixinmuqiang.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qa.bookmarksfly.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sz.szsharing.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://oo.jctech888.com.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://bn.panjiajie.cn

[A24] 去除首尾空白
来源：http://yg.lnxyls.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://kn.newstarts.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tt.muxihuayi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qj.lnxyls.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nk.nszjky.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qn.colortex.cn

Go:   strings.TrimSpace(s)
来源：http://rm.shxzukj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mh.newstarts.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://va.newstarts.cn

[A25] 字符串比较
来源：http://zk.yuntaijiaju.cn

Py:   s1 == s2; s1 != s2
来源：http://ca.haigaiapp.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://th.hnjuh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wb.nszjky.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dg.shtwfgs.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://an.panjiajie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ax.huanxung.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://zb.shtwfgs.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xi.huanxung.cn

[A26] 类型转换总览
来源：http://hw.jctech888.com.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vd.shxzskj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lt.lnxyls.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ly.9csxet.cn

TS:   Number() String() Boolean() x as number
来源：http://me.newstarts.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ld.hnjuh.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://aw.shxzskj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://qp.huanxung.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://of.huanxung.cn

================================================================================
来源：http://cm.bookmarksfly.cn

B. 流程控制
来源：http://dd.shtwfgs.cn

================================================================================
来源：http://vy.huanxung.cn

[B01] 条件判断 if / else
来源：http://lr.newstarts.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://kb.asd995.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ny.9csxet.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qz.colortex.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qs.shxzukj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://zu.panjiajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kk.jctech888.com.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://za.bookmarksfly.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mc.shxzukj.cn

[B02] 多分支 else if / elif
来源：http://dm.szxytkj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hl.panjiajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mn.nicolike.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lf.yuntaijiaju.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lw.chemitech.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://er.jianghongdianzi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bh.huixinmuqiang.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nc.shxzukj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://az.newstarts.cn

[B03] switch / match / case
来源：http://un.nszjky.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qd.huixinmuqiang.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://br.lnxyls.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://be.bjjhwx.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bx.szxytkj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ov.nicolike.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ud.colortex.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yd.colortex.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://li.shxzskj.cn

[B04] for 计数循环
来源：http://tk.bookmarksfly.cn

Py:   for i in range(10): print(i)
来源：http://ax.nicolike.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yc.huixinmuqiang.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://em.huixinmuqiang.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eq.hahajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gu.muxihuayi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bx.nicolike.cn

Ruby: 10.times { |i| puts i }
来源：http://vk.9csxet.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ac.haigaiapp.cn

[B05] 遍历数组 / 列表
来源：http://jn.shxzskj.cn

Py:   for item in arr: print(item)
来源：http://yc.bookmarksfly.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wi.nicolike.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ae.haigaiapp.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://eq.nszjky.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sp.yuexingan06.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ip.bjjhwx.cn

Ruby: arr.each { |item| puts item }
来源：http://ol.hahajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vq.hnjuh.cn

[B06] 遍历字典 / 对象
来源：http://zc.jctech888.com.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://kf.szxytkj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gh.szxytkj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://by.521024.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xr.szxytkj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vj.hahajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://uy.hahajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sq.shtwfgs.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://aj.jctech888.com.cn

[B07] while 循环
来源：http://ir.huixinmuqiang.cn

Py:   while i < 10: i += 1
来源：http://xk.newstarts.cn

PHP:  while ($i < 10) { $i++; }
来源：http://jm.hahajie.cn

JS:   while (i < 10) { i++; }
来源：http://ct.colortex.cn

TS:   while (i < 10) { i++; }
来源：http://ms.lnxyls.cn

Java: while (i < 10) { i++; }
来源：http://za.huixiangedu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qr.panjiajie.cn

Ruby: while i < 10; i += 1; end
来源：http://vh.szsharing.cn

C#:   while (i < 10) { i++; }
来源：http://gt.9csxet.cn

[B08] do-while（至少执行一次）
来源：http://xk.bookmarksfly.cn

Py:   # 无 do-while：用 while True + break
来源：http://bi.gzmigu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mv.newstarts.cn

JS:   do { i++; } while (i < 10);
来源：http://zl.panjiajie.cn

TS:   do { i++; } while (i < 10);
来源：http://uv.newstarts.cn

Java: do { i++; } while (i < 10);
来源：http://uq.shtwfgs.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://cx.huanxung.cn

Ruby: begin; i += 1; end while i < 10
来源：http://go.jianghongdianzi.cn

C#:   do { i++; } while (i < 10);
来源：http://pk.jctech888.com.cn

[B09] break 与 continue
来源：http://ho.asd995.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yc.nicolike.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ch.hahajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ek.hnjuh.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vy.chemitech.net.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hm.szxytkj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hc.shxzskj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mq.yuexingan06.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://or.bjjhwx.cn

[B10] 遍历同时拿索引
来源：http://hh.szsharing.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vm.521024.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qs.shxzukj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ps.newstarts.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kq.huanxung.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jb.lnxyls.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lf.colortex.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://um.hahajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://is.haigaiapp.cn

[B11] 生成数字序列 / 区间
来源：http://iv.szsharing.cn

Py:   list(range(0, 10, 2))
来源：http://vk.bjjhwx.cn

PHP:  range(0, 10, 2);
来源：http://sm.bjjhwx.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kl.huanxung.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bu.asd995.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ts.hnjuh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qc.asd995.cn

Ruby: (0...10).step(2).to_a
来源：http://ht.huixinmuqiang.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ka.shtwfgs.cn

[B12] 跳出多层循环
来源：http://cr.bookmarksfly.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yo.yuexingan06.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://jd.haigaiapp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://np.shxzukj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ii.jianghongdianzi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ac.huixiangedu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://te.hahajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dd.hahajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ov.yuexingan06.cn

[B13] 判断是否为数字
来源：http://rc.chemitech.net.cn

Py:   isinstance(x, (int, float))
来源：http://ep.yuntaijiaju.cn

PHP:  is_numeric($x)
来源：http://sj.bjjhwx.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ps.lnxyls.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://we.nszjky.cn

Java: x instanceof Number
来源：http://kw.bjjhwx.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lu.hahajie.cn

Ruby: x.is_a?(Numeric)
来源：http://sk.gzmigu.cn

C#:   x is int or double or decimal
来源：http://su.nicolike.cn

[B14] 判断值是否在集合内
来源：http://mo.panjiajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xz.shtwfgs.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vv.huanxung.cn

JS:   [1, 2, 3].includes(x)
来源：http://dl.szsharing.cn

TS:   [1, 2, 3].includes(x)
来源：http://mq.jianghongdianzi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ox.nicolike.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rr.9csxet.cn

Ruby: [1, 2, 3].include?(x)
来源：http://op.szsharing.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://an.bjjhwx.cn

[B15] 布尔运算与取反
来源：http://hb.chemitech.net.cn

Py:   a and b or not c
来源：http://yq.hnjuh.cn

PHP:  $a && $b || !$c
来源：http://ee.jianghongdianzi.cn

JS:   a && b || !c
来源：http://ka.9csxet.cn

TS:   a && b || !c
来源：http://id.bookmarksfly.cn

Java: a && b || !c
来源：http://if.huixiangedu.cn

Go:   a && b || !c
来源：http://gu.yuntaijiaju.cn

Ruby: a && b || !c
来源：http://oy.newstarts.cn

C#:   a && b || !c
来源：http://mz.wgjwhj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://uj.hnjuh.cn

Py:   if not data: return
来源：http://ma.asd995.cn

PHP:  if (!$data) { return; }
来源：http://vo.wgjwhj.cn

JS:   if (!data) return;
来源：http://hu.huanxung.cn

TS:   if (!data) return;
来源：http://fa.nszjky.cn

Java: if (data == null) return;
来源：http://dk.muxihuayi.cn

Go:   if data == nil { return }
来源：http://ng.jianghongdianzi.cn

Ruby: return if data.nil?
来源：http://qz.9csxet.cn

C#:   if (data == null) return;
来源：http://wx.jctech888.com.cn

================================================================================
来源：http://fk.shxzskj.cn

C. 函数与作用域
来源：http://zi.szsharing.cn

================================================================================
来源：http://sv.muxihuayi.cn

[C01] 定义函数
来源：http://xl.jianghongdianzi.cn

Py:   def add(a, b): return a + b
来源：http://pk.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kt.yuexingan06.cn

JS:   function add(a, b) { return a + b; }
来源：http://ad.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://up.huanxung.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zn.huixiangedu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ry.hahajie.cn

Ruby: def add(a, b); a + b; end
来源：http://fk.nicolike.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bv.asd995.cn

[C02] 默认参数
来源：http://bq.hnjuh.cn

Py:   def greet(name="World"): return name
来源：http://ws.jctech888.com.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://la.521024.cn

JS:   function greet(name = "World") { return name; }
来源：http://ne.wgjwhj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://dv.shtwfgs.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://im.colortex.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cr.szxytkj.cn

Ruby: def greet(name = "World") = name
来源：http://qk.hnjuh.cn

C#:   string Greet(string name = "World") => name;
来源：http://ho.nicolike.cn

[C03] 可变参数
来源：http://ll.muxihuayi.cn

Py:   def total(*args): return sum(args)
来源：http://ka.shxzukj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ha.chemitech.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kb.huixiangedu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ql.haigaiapp.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ka.521024.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nv.jctech888.com.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ec.hahajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lk.hahajie.cn

[C04] 命名参数 / 关键字参数
来源：http://jc.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gw.gzmigu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ff.huixinmuqiang.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fy.bjjhwx.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cl.asd995.cn

Java: // 无：用 Builder 模式或 record
来源：http://jj.nszjky.cn

Go:   // 无：用配置结构体参数
来源：http://qq.colortex.cn

Ruby: f(a: 1, b: 2)
来源：http://bp.bjjhwx.cn

C#:   f(a: 1, b: 2)
来源：http://rs.yuntaijiaju.cn

[C05] 返回多个值
来源：http://kn.gzmigu.cn

Py:   return a, b
来源：http://zg.hnjuh.cn

PHP:  return [$a, $b];
来源：http://ma.lnxyls.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ah.nicolike.cn

TS:   return { a, b };
来源：http://kd.9csxet.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qa.yuexingan06.cn

Go:   return a, b
来源：http://mh.521024.cn

Ruby: return a, b
来源：http://ps.bjjhwx.cn

C#:   return (a, b);              // ValueTuple
来源：http://xc.shxzskj.cn

[C06] 匿名函数 / lambda
来源：http://jl.jctech888.com.cn

Py:   square = lambda x: x * x
来源：http://vb.jianghongdianzi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://cv.bjjhwx.cn

JS:   const square = x => x * x;
来源：http://mp.jianghongdianzi.cn

TS:   const square = (x: number): number => x * x;
来源：http://xo.lnxyls.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xw.9csxet.cn

Go:   sq := func(x int) int { return x * x }
来源：http://og.nszjky.cn

Ruby: square = ->(x) { x * x }
来源：http://xz.newstarts.cn

C#:   Func<int, int> square = x => x * x;
来源：http://pe.nicolike.cn

[C07] 把函数作为参数传入
来源：http://hc.nszjky.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dh.521024.cn

PHP:  array_map("strtoupper", $arr);
来源：http://tk.panjiajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xi.gzmigu.cn

TS:   arr.map(String)
来源：http://so.gzmigu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ut.panjiajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kn.szsharing.cn

Ruby: arr.map(&:upcase)
来源：http://ml.nicolike.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ht.szxytkj.cn

[C08] 闭包
来源：http://ps.chemitech.net.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wo.hahajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://eh.521024.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://iq.shxzukj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://um.lnxyls.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ty.jianghongdianzi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lh.haigaiapp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ur.9csxet.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gp.haigaiapp.cn

[C09] 递归
来源：http://zl.haigaiapp.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lw.hnjuh.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ex.asd995.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://du.521024.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pw.newstarts.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ex.yuntaijiaju.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vn.haigaiapp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://eg.nicolike.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fm.jianghongdianzi.cn

[C10] 变量作用域
来源：http://zz.9csxet.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jm.asd995.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ht.szxytkj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sb.nszjky.cn

TS:   同 JS
来源：http://jw.haigaiapp.cn

Java: 方法内为块级作用域
来源：http://pf.bjjhwx.cn

Go:   花括号块级作用域
来源：http://ud.asd995.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pl.haigaiapp.cn

C#:   块级作用域
来源：http://hs.gzmigu.cn

[C11] 模块导入与导出
来源：http://lr.shtwfgs.cn

Py:   from module import func
来源：http://lm.nszjky.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://uc.colortex.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ts.huixinmuqiang.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zm.wgjwhj.cn

Java: import java.util.List;
来源：http://xb.gzmigu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mk.asd995.cn

Ruby: require "json"; require_relative "./util"
来源：http://oj.colortex.cn

C#:   using System.Text;
来源：http://dc.asd995.cn

[C12] 立即执行函数 IIFE
来源：http://ak.521024.cn

Py:   (lambda: print("run"))()
来源：http://tw.shxzukj.cn

PHP:  (function () { echo "run"; })();
来源：http://za.hahajie.cn

JS:   (() => { console.log("run"); })();
来源：http://tu.9csxet.cn

TS:   (() => { console.log("run"); })();
来源：http://mz.hahajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jv.shtwfgs.cn


<!-- 参考信息 -->