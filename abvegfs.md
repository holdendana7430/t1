代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://kg.shxzskj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fj.colortex.cn

Ruby: format("%.2f", 3.14159)
来源：http://sg.lnxyls.cn

C#:   3.14159.ToString("F2")
来源：http://aq.shxzskj.cn

[A22] 获取字符串长度
来源：http://jd.huixiangedu.cn

Py:   len(s)
来源：http://ny.shtwfgs.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ai.wgjwhj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://if.jianghongdianzi.cn

TS:   s.length
来源：http://un.muxihuayi.cn

Java: s.length()
来源：http://qv.huixinmuqiang.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://sf.szsharing.cn

Ruby: s.length
来源：http://wl.newstarts.cn

C#:   s.Length
来源：http://qv.jctech888.com.cn

[A23] 大小写转换
来源：http://tr.chemitech.net.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ic.hahajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mw.yuntaijiaju.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ti.bookmarksfly.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kq.jctech888.com.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://yx.huixiangedu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zd.hahajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pn.newstarts.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://nm.shxzskj.cn

[A24] 去除首尾空白
来源：http://me.yuexingan06.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://an.chemitech.net.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ez.9csxet.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cz.bjjhwx.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gu.9csxet.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ut.lnxyls.cn

Go:   strings.TrimSpace(s)
来源：http://ic.huixinmuqiang.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://at.hahajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fq.nicolike.cn

[A25] 字符串比较
来源：http://ov.yuexingan06.cn

Py:   s1 == s2; s1 != s2
来源：http://vi.szxytkj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qk.newstarts.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nd.szxytkj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nq.newstarts.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pp.huixiangedu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zf.huixiangedu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://cf.chemitech.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hn.szxytkj.cn

[A26] 类型转换总览
来源：http://lt.huanxung.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zs.newstarts.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vs.hahajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fi.szsharing.cn

TS:   Number() String() Boolean() x as number
来源：http://sl.bookmarksfly.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rb.hahajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ej.chemitech.net.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://du.chemitech.net.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://am.hahajie.cn

================================================================================
来源：http://zx.jianghongdianzi.cn

B. 流程控制
来源：http://nd.jianghongdianzi.cn

================================================================================
来源：http://xs.haigaiapp.cn

[B01] 条件判断 if / else
来源：http://st.wgjwhj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ln.nicolike.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fu.hnjuh.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dy.lnxyls.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vo.huixinmuqiang.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://jc.jctech888.com.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bv.newstarts.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zz.haigaiapp.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wx.yuexingan06.cn

[B02] 多分支 else if / elif
来源：http://fe.shxzskj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sr.nicolike.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ok.haigaiapp.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zm.shtwfgs.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ex.9csxet.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ed.bjjhwx.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://em.huanxung.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://oe.huanxung.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bx.panjiajie.cn

[B03] switch / match / case
来源：http://ne.jianghongdianzi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vr.colortex.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nh.521024.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bl.szsharing.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qr.panjiajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xb.shxzskj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kh.gzmigu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zd.nicolike.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jo.szxytkj.cn

[B04] for 计数循环
来源：http://yd.szxytkj.cn

Py:   for i in range(10): print(i)
来源：http://xg.bookmarksfly.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ub.haigaiapp.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ti.521024.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mn.nszjky.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ij.yuexingan06.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wn.bookmarksfly.cn

Ruby: 10.times { |i| puts i }
来源：http://jf.lnxyls.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jr.huixiangedu.cn

[B05] 遍历数组 / 列表
来源：http://bs.panjiajie.cn

Py:   for item in arr: print(item)
来源：http://bx.nicolike.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gr.asd995.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://mr.shxzukj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://oa.hnjuh.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://tg.chemitech.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vp.bjjhwx.cn

Ruby: arr.each { |item| puts item }
来源：http://wc.jianghongdianzi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://im.jctech888.com.cn

[B06] 遍历字典 / 对象
来源：http://jv.colortex.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://bo.szxytkj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rb.hahajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jx.shxzukj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dt.panjiajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vl.muxihuayi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://va.colortex.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xp.wgjwhj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://so.muxihuayi.cn

[B07] while 循环
来源：http://hu.shxzskj.cn

Py:   while i < 10: i += 1
来源：http://fc.lnxyls.cn

PHP:  while ($i < 10) { $i++; }
来源：http://dk.panjiajie.cn

JS:   while (i < 10) { i++; }
来源：http://yi.szxytkj.cn

TS:   while (i < 10) { i++; }
来源：http://ye.yuexingan06.cn

Java: while (i < 10) { i++; }
来源：http://nj.nszjky.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nu.bjjhwx.cn

Ruby: while i < 10; i += 1; end
来源：http://lk.szxytkj.cn

C#:   while (i < 10) { i++; }
来源：http://km.hahajie.cn

[B08] do-while（至少执行一次）
来源：http://sq.huixinmuqiang.cn

Py:   # 无 do-while：用 while True + break
来源：http://kl.huanxung.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://uv.bjjhwx.cn

JS:   do { i++; } while (i < 10);
来源：http://rn.yuntaijiaju.cn

TS:   do { i++; } while (i < 10);
来源：http://og.shxzukj.cn

Java: do { i++; } while (i < 10);
来源：http://sy.panjiajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://rp.szsharing.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vn.bjjhwx.cn

C#:   do { i++; } while (i < 10);
来源：http://lf.gzmigu.cn

[B09] break 与 continue
来源：http://zl.nszjky.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mi.lnxyls.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://my.shxzskj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pw.nicolike.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zt.colortex.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vc.huixinmuqiang.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ur.huanxung.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ys.jianghongdianzi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fh.521024.cn

[B10] 遍历同时拿索引
来源：http://iv.jianghongdianzi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yx.shxzukj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ik.panjiajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ys.jctech888.com.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://un.szxytkj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://si.shtwfgs.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dk.huixinmuqiang.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xa.yuexingan06.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cc.chemitech.net.cn

[B11] 生成数字序列 / 区间
来源：http://ke.shtwfgs.cn

Py:   list(range(0, 10, 2))
来源：http://zn.wgjwhj.cn

PHP:  range(0, 10, 2);
来源：http://mg.bjjhwx.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dw.szsharing.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lo.gzmigu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nv.newstarts.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ik.huixinmuqiang.cn

Ruby: (0...10).step(2).to_a
来源：http://hp.wgjwhj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gq.521024.cn

[B12] 跳出多层循环
来源：http://rq.hnjuh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://mb.yuexingan06.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://nk.yuntaijiaju.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://py.asd995.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ul.chemitech.net.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vq.jianghongdianzi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://py.shtwfgs.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cr.asd995.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dl.szsharing.cn

[B13] 判断是否为数字
来源：http://tx.chemitech.net.cn

Py:   isinstance(x, (int, float))
来源：http://gh.hnjuh.cn

PHP:  is_numeric($x)
来源：http://td.jctech888.com.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://up.shtwfgs.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vo.jctech888.com.cn

Java: x instanceof Number
来源：http://jp.bookmarksfly.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ir.bookmarksfly.cn

Ruby: x.is_a?(Numeric)
来源：http://pa.colortex.cn

C#:   x is int or double or decimal
来源：http://np.hahajie.cn

[B14] 判断值是否在集合内
来源：http://rg.shxzskj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zy.yuexingan06.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://af.huixinmuqiang.cn

JS:   [1, 2, 3].includes(x)
来源：http://kf.bookmarksfly.cn

TS:   [1, 2, 3].includes(x)
来源：http://zu.jianghongdianzi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ze.huanxung.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fd.bjjhwx.cn

Ruby: [1, 2, 3].include?(x)
来源：http://yt.bjjhwx.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://db.shxzskj.cn

[B15] 布尔运算与取反
来源：http://su.gzmigu.cn

Py:   a and b or not c
来源：http://mm.asd995.cn

PHP:  $a && $b || !$c
来源：http://eu.521024.cn

JS:   a && b || !c
来源：http://nc.colortex.cn

TS:   a && b || !c
来源：http://zc.yuntaijiaju.cn

Java: a && b || !c
来源：http://qz.lnxyls.cn

Go:   a && b || !c
来源：http://ns.shxzskj.cn

Ruby: a && b || !c
来源：http://ub.muxihuayi.cn

C#:   a && b || !c
来源：http://ne.jianghongdianzi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lt.asd995.cn

Py:   if not data: return
来源：http://sf.jianghongdianzi.cn

PHP:  if (!$data) { return; }
来源：http://zt.asd995.cn

JS:   if (!data) return;
来源：http://mo.bookmarksfly.cn

TS:   if (!data) return;
来源：http://rv.huanxung.cn

Java: if (data == null) return;
来源：http://ai.yuntaijiaju.cn

Go:   if data == nil { return }
来源：http://bq.haigaiapp.cn

Ruby: return if data.nil?
来源：http://hb.lnxyls.cn

C#:   if (data == null) return;
来源：http://fx.colortex.cn

================================================================================
来源：http://lr.colortex.cn

C. 函数与作用域
来源：http://yi.asd995.cn

================================================================================
来源：http://si.wgjwhj.cn

[C01] 定义函数
来源：http://po.bookmarksfly.cn

Py:   def add(a, b): return a + b
来源：http://nc.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://io.huixinmuqiang.cn

JS:   function add(a, b) { return a + b; }
来源：http://gb.hahajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ji.shxzukj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://oy.jctech888.com.cn

Go:   func add(a, b int) int { return a + b }
来源：http://md.shxzskj.cn

Ruby: def add(a, b); a + b; end
来源：http://bu.panjiajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kw.nszjky.cn

[C02] 默认参数
来源：http://mt.szsharing.cn

Py:   def greet(name="World"): return name
来源：http://qs.lnxyls.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://kn.nszjky.cn

JS:   function greet(name = "World") { return name; }
来源：http://bh.shxzskj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qx.szsharing.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cb.asd995.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fs.yuntaijiaju.cn

Ruby: def greet(name = "World") = name
来源：http://mf.gzmigu.cn

C#:   string Greet(string name = "World") => name;
来源：http://hu.9csxet.cn

[C03] 可变参数
来源：http://rd.huixinmuqiang.cn

Py:   def total(*args): return sum(args)
来源：http://ub.9csxet.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tn.bjjhwx.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ia.szsharing.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ut.huixinmuqiang.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xb.newstarts.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yf.jianghongdianzi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://mh.shxzukj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ge.shxzskj.cn

[C04] 命名参数 / 关键字参数
来源：http://xy.huanxung.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dh.bjjhwx.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://eh.lnxyls.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://eo.yuntaijiaju.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ym.chemitech.net.cn

Java: // 无：用 Builder 模式或 record
来源：http://ga.9csxet.cn

Go:   // 无：用配置结构体参数
来源：http://uh.wgjwhj.cn

Ruby: f(a: 1, b: 2)
来源：http://fb.nicolike.cn

C#:   f(a: 1, b: 2)
来源：http://oj.szxytkj.cn

[C05] 返回多个值
来源：http://ya.panjiajie.cn

Py:   return a, b
来源：http://vm.muxihuayi.cn

PHP:  return [$a, $b];
来源：http://nw.huixiangedu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ek.yuexingan06.cn

TS:   return { a, b };
来源：http://hb.shxzskj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ak.chemitech.net.cn

Go:   return a, b
来源：http://qc.gzmigu.cn

Ruby: return a, b
来源：http://ly.asd995.cn

C#:   return (a, b);              // ValueTuple
来源：http://wa.nszjky.cn

[C06] 匿名函数 / lambda
来源：http://sk.yuexingan06.cn

Py:   square = lambda x: x * x
来源：http://be.jianghongdianzi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zs.yuntaijiaju.cn

JS:   const square = x => x * x;
来源：http://vh.asd995.cn

TS:   const square = (x: number): number => x * x;
来源：http://iz.shxzskj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tc.jctech888.com.cn

Go:   sq := func(x int) int { return x * x }
来源：http://mj.haigaiapp.cn

Ruby: square = ->(x) { x * x }
来源：http://er.gzmigu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zh.hahajie.cn

[C07] 把函数作为参数传入
来源：http://dh.chemitech.net.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nb.newstarts.cn

PHP:  array_map("strtoupper", $arr);
来源：http://mg.hnjuh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sm.bookmarksfly.cn

TS:   arr.map(String)
来源：http://aj.huanxung.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yc.jctech888.com.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://eu.szsharing.cn

Ruby: arr.map(&:upcase)
来源：http://mj.hnjuh.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://np.panjiajie.cn

[C08] 闭包
来源：http://bp.szsharing.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tt.shtwfgs.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cy.chemitech.net.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cd.shtwfgs.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pj.9csxet.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qa.bookmarksfly.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mx.haigaiapp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nt.nicolike.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pa.asd995.cn

[C09] 递归
来源：http://ly.wgjwhj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cr.shxzukj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yd.yuexingan06.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nd.colortex.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hn.yuntaijiaju.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ox.lnxyls.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ig.521024.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uq.huixiangedu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ti.szsharing.cn

[C10] 变量作用域
来源：http://tb.huanxung.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wl.szsharing.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fr.hnjuh.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ft.wgjwhj.cn

TS:   同 JS
来源：http://sf.jctech888.com.cn

Java: 方法内为块级作用域
来源：http://la.asd995.cn

Go:   花括号块级作用域
来源：http://ee.jctech888.com.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gp.colortex.cn

C#:   块级作用域
来源：http://bu.521024.cn

[C11] 模块导入与导出
来源：http://rb.panjiajie.cn

Py:   from module import func
来源：http://ti.521024.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ey.haigaiapp.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hd.nicolike.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tq.newstarts.cn

Java: import java.util.List;
来源：http://lz.panjiajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wy.haigaiapp.cn

Ruby: require "json"; require_relative "./util"
来源：http://pg.huixiangedu.cn

C#:   using System.Text;
来源：http://ha.lnxyls.cn

[C12] 立即执行函数 IIFE
来源：http://yv.asd995.cn

Py:   (lambda: print("run"))()
来源：http://bi.lnxyls.cn


<!-- 参考信息 -->