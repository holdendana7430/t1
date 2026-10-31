代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://ud.yuntaijiaju.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zy.shtwfgs.cn

JS:   (3.14159).toFixed(2)
来源：http://mi.shxzskj.cn

TS:   (3.14159).toFixed(2)
来源：http://ng.newstarts.cn

Java: String.format("%.2f", 3.14159)
来源：http://go.shtwfgs.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vb.521024.cn

Ruby: format("%.2f", 3.14159)
来源：http://pw.colortex.cn

C#:   3.14159.ToString("F2")
来源：http://fy.bjjhwx.cn

[A22] 获取字符串长度
来源：http://iw.yuexingan06.cn

Py:   len(s)
来源：http://ze.shxzskj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ml.shxzukj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cw.gzmigu.cn

TS:   s.length
来源：http://xa.wgjwhj.cn

Java: s.length()
来源：http://vj.szxytkj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ye.szsharing.cn

Ruby: s.length
来源：http://yd.9csxet.cn

C#:   s.Length
来源：http://hk.nszjky.cn

[A23] 大小写转换
来源：http://or.bjjhwx.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://id.lnxyls.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fy.nszjky.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fx.hahajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ho.asd995.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bd.wgjwhj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yu.newstarts.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tw.szxytkj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://cj.wgjwhj.cn

[A24] 去除首尾空白
来源：http://zk.haigaiapp.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xm.chemitech.net.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://yz.bookmarksfly.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wy.huanxung.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fq.jianghongdianzi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ed.shxzskj.cn

Go:   strings.TrimSpace(s)
来源：http://ic.shtwfgs.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tn.gzmigu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hb.colortex.cn

[A25] 字符串比较
来源：http://oq.colortex.cn

Py:   s1 == s2; s1 != s2
来源：http://kj.colortex.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wu.huixinmuqiang.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://uh.newstarts.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kq.huixinmuqiang.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://el.newstarts.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://im.lnxyls.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://he.huixiangedu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lh.9csxet.cn

[A26] 类型转换总览
来源：http://jx.gzmigu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ma.jctech888.com.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lh.huixiangedu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zx.shxzukj.cn

TS:   Number() String() Boolean() x as number
来源：http://cy.nszjky.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://uh.newstarts.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pj.newstarts.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://gm.bookmarksfly.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://db.newstarts.cn

================================================================================
来源：http://lo.yuexingan06.cn

B. 流程控制
来源：http://bk.chemitech.net.cn

================================================================================
来源：http://sm.nszjky.cn

[B01] 条件判断 if / else
来源：http://ok.jctech888.com.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://np.huixiangedu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vu.gzmigu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jc.jctech888.com.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jf.521024.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qz.nicolike.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zb.hnjuh.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ku.nicolike.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ui.yuntaijiaju.cn

[B02] 多分支 else if / elif
来源：http://ry.chemitech.net.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wu.521024.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wx.shtwfgs.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qc.wgjwhj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ct.bjjhwx.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lm.panjiajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vb.lnxyls.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bs.huixiangedu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ep.panjiajie.cn

[B03] switch / match / case
来源：http://nf.shxzskj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fl.colortex.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://va.nszjky.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xs.nszjky.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nh.lnxyls.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://iu.panjiajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zi.wgjwhj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dw.huixinmuqiang.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://an.yuexingan06.cn

[B04] for 计数循环
来源：http://ah.huixiangedu.cn

Py:   for i in range(10): print(i)
来源：http://hl.nicolike.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kt.chemitech.net.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nr.huixinmuqiang.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://id.bjjhwx.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vb.bjjhwx.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kk.colortex.cn

Ruby: 10.times { |i| puts i }
来源：http://uk.jianghongdianzi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hs.bookmarksfly.cn

[B05] 遍历数组 / 列表
来源：http://va.nszjky.cn

Py:   for item in arr: print(item)
来源：http://tl.jianghongdianzi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://px.newstarts.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://io.shxzukj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://dd.panjiajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://bw.hnjuh.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ww.wgjwhj.cn

Ruby: arr.each { |item| puts item }
来源：http://ez.muxihuayi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fl.jianghongdianzi.cn

[B06] 遍历字典 / 对象
来源：http://rq.huixinmuqiang.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ur.nszjky.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://og.gzmigu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sp.jianghongdianzi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://aj.panjiajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jp.bjjhwx.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xm.colortex.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cj.szxytkj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ik.shxzskj.cn

[B07] while 循环
来源：http://ak.szsharing.cn

Py:   while i < 10: i += 1
来源：http://vx.huixinmuqiang.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mn.yuntaijiaju.cn

JS:   while (i < 10) { i++; }
来源：http://lq.shxzukj.cn

TS:   while (i < 10) { i++; }
来源：http://uu.nszjky.cn

Java: while (i < 10) { i++; }
来源：http://vh.huixiangedu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mz.lnxyls.cn

Ruby: while i < 10; i += 1; end
来源：http://iu.huanxung.cn

C#:   while (i < 10) { i++; }
来源：http://ws.yuntaijiaju.cn

[B08] do-while（至少执行一次）
来源：http://zc.lnxyls.cn

Py:   # 无 do-while：用 while True + break
来源：http://pt.asd995.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://po.szsharing.cn

JS:   do { i++; } while (i < 10);
来源：http://aj.lnxyls.cn

TS:   do { i++; } while (i < 10);
来源：http://tn.521024.cn

Java: do { i++; } while (i < 10);
来源：http://wy.huixiangedu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://hu.hnjuh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://kg.muxihuayi.cn

C#:   do { i++; } while (i < 10);
来源：http://gf.hnjuh.cn

[B09] break 与 continue
来源：http://sh.wgjwhj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dx.lnxyls.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xt.jianghongdianzi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zg.asd995.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lt.gzmigu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gf.hnjuh.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ma.shxzukj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mf.bjjhwx.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ck.nszjky.cn

[B10] 遍历同时拿索引
来源：http://th.yuexingan06.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tz.nszjky.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gr.chemitech.net.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ip.521024.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yz.wgjwhj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ge.nszjky.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://au.asd995.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ie.jianghongdianzi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rs.colortex.cn

[B11] 生成数字序列 / 区间
来源：http://go.521024.cn

Py:   list(range(0, 10, 2))
来源：http://aq.szsharing.cn

PHP:  range(0, 10, 2);
来源：http://nt.yuexingan06.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://db.hnjuh.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cw.hahajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mr.nicolike.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zy.huixiangedu.cn

Ruby: (0...10).step(2).to_a
来源：http://vw.nszjky.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dv.huixiangedu.cn

[B12] 跳出多层循环
来源：http://sc.gzmigu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ny.haigaiapp.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ae.wgjwhj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ux.nicolike.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pf.nicolike.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vc.521024.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ca.521024.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sg.hahajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tp.521024.cn

[B13] 判断是否为数字
来源：http://no.muxihuayi.cn

Py:   isinstance(x, (int, float))
来源：http://hu.521024.cn

PHP:  is_numeric($x)
来源：http://tr.9csxet.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://to.chemitech.net.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://si.szxytkj.cn

Java: x instanceof Number
来源：http://nb.szsharing.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://oc.szxytkj.cn

Ruby: x.is_a?(Numeric)
来源：http://dy.szxytkj.cn

C#:   x is int or double or decimal
来源：http://ce.hahajie.cn

[B14] 判断值是否在集合内
来源：http://gh.newstarts.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hv.bjjhwx.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cc.9csxet.cn

JS:   [1, 2, 3].includes(x)
来源：http://eu.shxzskj.cn

TS:   [1, 2, 3].includes(x)
来源：http://ex.chemitech.net.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://on.muxihuayi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ln.bookmarksfly.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vt.lnxyls.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rs.shxzskj.cn

[B15] 布尔运算与取反
来源：http://pc.chemitech.net.cn

Py:   a and b or not c
来源：http://lo.shtwfgs.cn

PHP:  $a && $b || !$c
来源：http://pl.bjjhwx.cn

JS:   a && b || !c
来源：http://ww.gzmigu.cn

TS:   a && b || !c
来源：http://co.nicolike.cn

Java: a && b || !c
来源：http://up.lnxyls.cn

Go:   a && b || !c
来源：http://ji.jctech888.com.cn

Ruby: a && b || !c
来源：http://lx.jianghongdianzi.cn

C#:   a && b || !c
来源：http://xs.jianghongdianzi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ni.nszjky.cn

Py:   if not data: return
来源：http://ad.9csxet.cn

PHP:  if (!$data) { return; }
来源：http://fo.hnjuh.cn

JS:   if (!data) return;
来源：http://ul.hahajie.cn

TS:   if (!data) return;
来源：http://td.nszjky.cn

Java: if (data == null) return;
来源：http://ob.yuexingan06.cn

Go:   if data == nil { return }
来源：http://ie.haigaiapp.cn

Ruby: return if data.nil?
来源：http://fp.colortex.cn

C#:   if (data == null) return;
来源：http://cj.wgjwhj.cn

================================================================================
来源：http://mq.szsharing.cn

C. 函数与作用域
来源：http://js.shtwfgs.cn

================================================================================
来源：http://hy.wgjwhj.cn

[C01] 定义函数
来源：http://bb.bjjhwx.cn

Py:   def add(a, b): return a + b
来源：http://lf.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vy.jctech888.com.cn

JS:   function add(a, b) { return a + b; }
来源：http://dw.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oa.yuntaijiaju.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ma.hnjuh.cn

Go:   func add(a, b int) int { return a + b }
来源：http://yr.shtwfgs.cn

Ruby: def add(a, b); a + b; end
来源：http://xu.bookmarksfly.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xn.hnjuh.cn

[C02] 默认参数
来源：http://cp.asd995.cn

Py:   def greet(name="World"): return name
来源：http://ut.colortex.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vq.wgjwhj.cn

JS:   function greet(name = "World") { return name; }
来源：http://gm.huixinmuqiang.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qr.jianghongdianzi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://oj.521024.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vj.hahajie.cn

Ruby: def greet(name = "World") = name
来源：http://yo.haigaiapp.cn

C#:   string Greet(string name = "World") => name;
来源：http://vp.panjiajie.cn

[C03] 可变参数
来源：http://pt.bjjhwx.cn

Py:   def total(*args): return sum(args)
来源：http://ye.huanxung.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xb.shxzukj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ug.szsharing.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://md.gzmigu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jx.shxzukj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nu.shxzukj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://oa.lnxyls.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sk.colortex.cn

[C04] 命名参数 / 关键字参数
来源：http://mw.bjjhwx.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ir.gzmigu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gp.wgjwhj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hc.jctech888.com.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gb.bookmarksfly.cn

Java: // 无：用 Builder 模式或 record
来源：http://yw.hnjuh.cn

Go:   // 无：用配置结构体参数
来源：http://yh.521024.cn

Ruby: f(a: 1, b: 2)
来源：http://ug.asd995.cn

C#:   f(a: 1, b: 2)
来源：http://xb.lnxyls.cn

[C05] 返回多个值
来源：http://ar.shtwfgs.cn

Py:   return a, b
来源：http://wy.haigaiapp.cn

PHP:  return [$a, $b];
来源：http://be.muxihuayi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://oo.shxzskj.cn

TS:   return { a, b };
来源：http://ru.huanxung.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ae.shxzskj.cn

Go:   return a, b
来源：http://jk.chemitech.net.cn

Ruby: return a, b
来源：http://gj.gzmigu.cn

C#:   return (a, b);              // ValueTuple
来源：http://ei.asd995.cn

[C06] 匿名函数 / lambda
来源：http://is.huixinmuqiang.cn

Py:   square = lambda x: x * x
来源：http://wz.asd995.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://md.nicolike.cn

JS:   const square = x => x * x;
来源：http://cp.szsharing.cn

TS:   const square = (x: number): number => x * x;
来源：http://ad.shxzskj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ee.nicolike.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gc.nicolike.cn

Ruby: square = ->(x) { x * x }
来源：http://ah.bookmarksfly.cn

C#:   Func<int, int> square = x => x * x;
来源：http://jg.yuntaijiaju.cn

[C07] 把函数作为参数传入
来源：http://dm.nszjky.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vs.nszjky.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jm.521024.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jj.huixiangedu.cn

TS:   arr.map(String)
来源：http://zs.yuexingan06.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://if.jianghongdianzi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://is.shtwfgs.cn

Ruby: arr.map(&:upcase)
来源：http://rt.newstarts.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://el.lnxyls.cn

[C08] 闭包
来源：http://ze.bjjhwx.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zu.nicolike.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xg.colortex.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hg.shxzskj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mq.lnxyls.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yv.huanxung.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://np.huixiangedu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gb.jctech888.com.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jm.panjiajie.cn

[C09] 递归
来源：http://ie.haigaiapp.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nm.jctech888.com.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vk.haigaiapp.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nl.huanxung.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ju.szxytkj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ma.yuntaijiaju.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://yu.gzmigu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hw.hahajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yf.jctech888.com.cn

[C10] 变量作用域
来源：http://ci.huixiangedu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://it.jctech888.com.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ft.wgjwhj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qg.wgjwhj.cn

TS:   同 JS
来源：http://af.shxzskj.cn

Java: 方法内为块级作用域
来源：http://lm.jianghongdianzi.cn

Go:   花括号块级作用域
来源：http://nl.wgjwhj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wa.huixinmuqiang.cn

C#:   块级作用域
来源：http://nn.nszjky.cn

[C11] 模块导入与导出
来源：http://zz.bjjhwx.cn

Py:   from module import func
来源：http://rw.huixiangedu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://es.nszjky.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://cr.colortex.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tq.muxihuayi.cn

Java: import java.util.List;
来源：http://er.yuexingan06.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ul.chemitech.net.cn


<!-- 参考信息 -->