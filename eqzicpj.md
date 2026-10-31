代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://ut.huixinmuqiang.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pp.huixinmuqiang.cn

Ruby: format("%.2f", 3.14159)
来源：http://xv.gzmigu.cn

C#:   3.14159.ToString("F2")
来源：http://gf.colortex.cn

[A22] 获取字符串长度
来源：http://hc.9csxet.cn

Py:   len(s)
来源：http://ik.nszjky.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://iq.bjjhwx.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hh.yuexingan06.cn

TS:   s.length
来源：http://uw.panjiajie.cn

Java: s.length()
来源：http://hf.lnxyls.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ph.yuexingan06.cn

Ruby: s.length
来源：http://tm.wgjwhj.cn

C#:   s.Length
来源：http://ff.hnjuh.cn

[A23] 大小写转换
来源：http://nr.yuexingan06.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://sm.muxihuayi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ed.muxihuayi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nn.jctech888.com.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wj.yuntaijiaju.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vs.panjiajie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pm.haigaiapp.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hn.haigaiapp.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ei.shxzskj.cn

[A24] 去除首尾空白
来源：http://mj.gzmigu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pa.521024.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pa.yuntaijiaju.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ei.shtwfgs.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ht.wgjwhj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ob.bookmarksfly.cn

Go:   strings.TrimSpace(s)
来源：http://nz.yuntaijiaju.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://uj.hahajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yj.huixinmuqiang.cn

[A25] 字符串比较
来源：http://ih.nszjky.cn

Py:   s1 == s2; s1 != s2
来源：http://ou.bjjhwx.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://iz.yuntaijiaju.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tf.9csxet.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jt.chemitech.net.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ma.yuntaijiaju.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xc.jctech888.com.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://qc.szsharing.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qk.huanxung.cn

[A26] 类型转换总览
来源：http://ji.lnxyls.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xz.huixiangedu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ax.hahajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zi.lnxyls.cn

TS:   Number() String() Boolean() x as number
来源：http://zp.huixiangedu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wd.lnxyls.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://oc.bjjhwx.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rh.szxytkj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gx.bjjhwx.cn

================================================================================
来源：http://jp.huixiangedu.cn

B. 流程控制
来源：http://qz.521024.cn

================================================================================
来源：http://zn.huanxung.cn

[B01] 条件判断 if / else
来源：http://tx.bjjhwx.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ms.hnjuh.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mn.gzmigu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://eu.jianghongdianzi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xy.jctech888.com.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://yg.chemitech.net.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jd.shxzskj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wc.szxytkj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://iu.shxzukj.cn

[B02] 多分支 else if / elif
来源：http://hy.hahajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rv.chemitech.net.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qh.wgjwhj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gk.yuntaijiaju.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xv.hahajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rl.yuntaijiaju.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ah.9csxet.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nw.chemitech.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ux.jctech888.com.cn

[B03] switch / match / case
来源：http://jd.yuexingan06.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xw.huixinmuqiang.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dy.szsharing.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ra.bjjhwx.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rb.shxzskj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rp.szsharing.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kb.szxytkj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://me.521024.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wo.521024.cn

[B04] for 计数循环
来源：http://mc.yuexingan06.cn

Py:   for i in range(10): print(i)
来源：http://mw.jctech888.com.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bf.chemitech.net.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ec.shxzukj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zx.shtwfgs.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://aj.jctech888.com.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mb.gzmigu.cn

Ruby: 10.times { |i| puts i }
来源：http://iu.bookmarksfly.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ag.szsharing.cn

[B05] 遍历数组 / 列表
来源：http://re.shxzskj.cn

Py:   for item in arr: print(item)
来源：http://hp.bjjhwx.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zx.asd995.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://jm.muxihuayi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fb.newstarts.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://mw.newstarts.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zx.jianghongdianzi.cn

Ruby: arr.each { |item| puts item }
来源：http://js.yuexingan06.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yx.gzmigu.cn

[B06] 遍历字典 / 对象
来源：http://ow.shtwfgs.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://nq.muxihuayi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ok.gzmigu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pm.hnjuh.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ok.hnjuh.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://co.gzmigu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ch.yuexingan06.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fa.muxihuayi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jp.bookmarksfly.cn

[B07] while 循环
来源：http://bi.bookmarksfly.cn

Py:   while i < 10: i += 1
来源：http://wd.yuexingan06.cn

PHP:  while ($i < 10) { $i++; }
来源：http://po.huixiangedu.cn

JS:   while (i < 10) { i++; }
来源：http://ki.bjjhwx.cn

TS:   while (i < 10) { i++; }
来源：http://ub.jctech888.com.cn

Java: while (i < 10) { i++; }
来源：http://zj.wgjwhj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ob.muxihuayi.cn

Ruby: while i < 10; i += 1; end
来源：http://ji.bjjhwx.cn

C#:   while (i < 10) { i++; }
来源：http://jy.gzmigu.cn

[B08] do-while（至少执行一次）
来源：http://vm.wgjwhj.cn

Py:   # 无 do-while：用 while True + break
来源：http://kz.szsharing.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vb.newstarts.cn

JS:   do { i++; } while (i < 10);
来源：http://ge.bookmarksfly.cn

TS:   do { i++; } while (i < 10);
来源：http://hu.szxytkj.cn

Java: do { i++; } while (i < 10);
来源：http://mc.521024.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ai.wgjwhj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rr.nszjky.cn

C#:   do { i++; } while (i < 10);
来源：http://dg.bjjhwx.cn

[B09] break 与 continue
来源：http://so.colortex.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gp.jctech888.com.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uy.wgjwhj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xr.lnxyls.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ii.shxzukj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ws.bookmarksfly.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ra.asd995.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://co.521024.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wl.yuntaijiaju.cn

[B10] 遍历同时拿索引
来源：http://zt.huixiangedu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fo.hnjuh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://op.jianghongdianzi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vl.huixinmuqiang.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://os.panjiajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mx.jianghongdianzi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hh.huixiangedu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://oi.haigaiapp.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://aj.gzmigu.cn

[B11] 生成数字序列 / 区间
来源：http://cn.shxzukj.cn

Py:   list(range(0, 10, 2))
来源：http://ix.szxytkj.cn

PHP:  range(0, 10, 2);
来源：http://xk.panjiajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qs.jctech888.com.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ov.shxzskj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ao.huixinmuqiang.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fy.yuntaijiaju.cn

Ruby: (0...10).step(2).to_a
来源：http://qs.haigaiapp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hy.hahajie.cn

[B12] 跳出多层循环
来源：http://ls.panjiajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://dd.hnjuh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ww.jianghongdianzi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rd.hahajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://we.asd995.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xl.nicolike.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tq.lnxyls.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bb.shtwfgs.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mj.panjiajie.cn

[B13] 判断是否为数字
来源：http://xy.huixiangedu.cn

Py:   isinstance(x, (int, float))
来源：http://kz.muxihuayi.cn

PHP:  is_numeric($x)
来源：http://va.huixiangedu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ka.szsharing.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qt.shxzskj.cn

Java: x instanceof Number
来源：http://nm.szsharing.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yt.hahajie.cn

Ruby: x.is_a?(Numeric)
来源：http://mb.asd995.cn

C#:   x is int or double or decimal
来源：http://tx.shxzukj.cn

[B14] 判断值是否在集合内
来源：http://vv.szxytkj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ta.nicolike.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ih.nszjky.cn

JS:   [1, 2, 3].includes(x)
来源：http://oh.colortex.cn

TS:   [1, 2, 3].includes(x)
来源：http://fz.szxytkj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://zn.panjiajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ts.hnjuh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qd.shxzskj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rz.521024.cn

[B15] 布尔运算与取反
来源：http://jf.nszjky.cn

Py:   a and b or not c
来源：http://gf.bookmarksfly.cn

PHP:  $a && $b || !$c
来源：http://jy.bookmarksfly.cn

JS:   a && b || !c
来源：http://zs.bookmarksfly.cn

TS:   a && b || !c
来源：http://pz.nicolike.cn

Java: a && b || !c
来源：http://rk.huixiangedu.cn

Go:   a && b || !c
来源：http://ks.shtwfgs.cn

Ruby: a && b || !c
来源：http://bp.lnxyls.cn

C#:   a && b || !c
来源：http://ks.bjjhwx.cn

[B16] 卫语句：不满足条件提前返回
来源：http://tg.nszjky.cn

Py:   if not data: return
来源：http://iy.lnxyls.cn

PHP:  if (!$data) { return; }
来源：http://cf.nszjky.cn

JS:   if (!data) return;
来源：http://iw.panjiajie.cn

TS:   if (!data) return;
来源：http://yh.hnjuh.cn

Java: if (data == null) return;
来源：http://rp.521024.cn

Go:   if data == nil { return }
来源：http://vb.haigaiapp.cn

Ruby: return if data.nil?
来源：http://ay.hahajie.cn

C#:   if (data == null) return;
来源：http://lc.hnjuh.cn

================================================================================
来源：http://df.huixinmuqiang.cn

C. 函数与作用域
来源：http://yq.521024.cn

================================================================================
来源：http://nw.nszjky.cn

[C01] 定义函数
来源：http://xr.yuntaijiaju.cn

Py:   def add(a, b): return a + b
来源：http://sl.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sq.jctech888.com.cn

JS:   function add(a, b) { return a + b; }
来源：http://lo.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uw.asd995.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zz.shxzukj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ji.haigaiapp.cn

Ruby: def add(a, b); a + b; end
来源：http://yq.hnjuh.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://li.521024.cn

[C02] 默认参数
来源：http://bx.szsharing.cn

Py:   def greet(name="World"): return name
来源：http://jl.szxytkj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://rh.newstarts.cn

JS:   function greet(name = "World") { return name; }
来源：http://nt.yuexingan06.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bh.bookmarksfly.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://mm.gzmigu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vt.shxzukj.cn

Ruby: def greet(name = "World") = name
来源：http://cq.shxzukj.cn

C#:   string Greet(string name = "World") => name;
来源：http://ro.haigaiapp.cn

[C03] 可变参数
来源：http://yg.nicolike.cn

Py:   def total(*args): return sum(args)
来源：http://dd.jianghongdianzi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ds.chemitech.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kp.huanxung.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mv.wgjwhj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://se.gzmigu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gd.lnxyls.cn

Ruby: def total(*nums); nums.sum; end
来源：http://iy.wgjwhj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ak.panjiajie.cn

[C04] 命名参数 / 关键字参数
来源：http://zu.9csxet.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fh.hnjuh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vp.colortex.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ck.asd995.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qc.huanxung.cn

Java: // 无：用 Builder 模式或 record
来源：http://kq.yuntaijiaju.cn

Go:   // 无：用配置结构体参数
来源：http://vw.huixiangedu.cn

Ruby: f(a: 1, b: 2)
来源：http://ts.shxzskj.cn

C#:   f(a: 1, b: 2)
来源：http://db.bookmarksfly.cn

[C05] 返回多个值
来源：http://yx.huanxung.cn

Py:   return a, b
来源：http://kb.gzmigu.cn

PHP:  return [$a, $b];
来源：http://qo.bjjhwx.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pf.wgjwhj.cn

TS:   return { a, b };
来源：http://ds.nicolike.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yc.gzmigu.cn

Go:   return a, b
来源：http://yx.huanxung.cn

Ruby: return a, b
来源：http://xz.huixiangedu.cn

C#:   return (a, b);              // ValueTuple
来源：http://nx.muxihuayi.cn

[C06] 匿名函数 / lambda
来源：http://xt.szsharing.cn

Py:   square = lambda x: x * x
来源：http://ah.shxzskj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fi.szsharing.cn

JS:   const square = x => x * x;
来源：http://ii.wgjwhj.cn

TS:   const square = (x: number): number => x * x;
来源：http://av.yuexingan06.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jo.9csxet.cn

Go:   sq := func(x int) int { return x * x }
来源：http://lj.nszjky.cn

Ruby: square = ->(x) { x * x }
来源：http://qa.gzmigu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://sr.bookmarksfly.cn

[C07] 把函数作为参数传入
来源：http://fc.yuntaijiaju.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ar.hahajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vj.huanxung.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://oc.hahajie.cn

TS:   arr.map(String)
来源：http://hg.shxzskj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pi.bookmarksfly.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vm.muxihuayi.cn

Ruby: arr.map(&:upcase)
来源：http://qd.huanxung.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xa.nicolike.cn

[C08] 闭包
来源：http://yj.shtwfgs.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://im.colortex.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ow.yuntaijiaju.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://px.wgjwhj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://br.bookmarksfly.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ub.chemitech.net.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gn.huanxung.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vu.yuexingan06.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://iy.yuexingan06.cn

[C09] 递归
来源：http://zc.asd995.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jr.521024.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uf.haigaiapp.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cf.huanxung.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ek.shxzskj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://oh.shxzukj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tm.yuntaijiaju.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ak.9csxet.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ui.shxzukj.cn

[C10] 变量作用域
来源：http://gx.hahajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nt.jianghongdianzi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xz.bjjhwx.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rg.shxzskj.cn

TS:   同 JS
来源：http://ef.szsharing.cn

Java: 方法内为块级作用域
来源：http://ly.shxzskj.cn

Go:   花括号块级作用域
来源：http://ik.panjiajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qs.nszjky.cn

C#:   块级作用域
来源：http://je.lnxyls.cn

[C11] 模块导入与导出
来源：http://fy.bookmarksfly.cn

Py:   from module import func
来源：http://yl.chemitech.net.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tq.nszjky.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kr.newstarts.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rm.panjiajie.cn

Java: import java.util.List;
来源：http://tk.yuexingan06.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zz.newstarts.cn

Ruby: require "json"; require_relative "./util"
来源：http://nw.newstarts.cn

C#:   using System.Text;
来源：http://bm.lnxyls.cn

[C12] 立即执行函数 IIFE
来源：http://pa.nicolike.cn

Py:   (lambda: print("run"))()
来源：http://xa.bookmarksfly.cn


<!-- 参考信息 -->