代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://ql.521024.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ku.bjjhwx.cn

JS:   (3.14159).toFixed(2)
来源：http://ms.lnxyls.cn

TS:   (3.14159).toFixed(2)
来源：http://nf.szsharing.cn

Java: String.format("%.2f", 3.14159)
来源：http://tb.huanxung.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pu.shtwfgs.cn

Ruby: format("%.2f", 3.14159)
来源：http://mz.yuntaijiaju.cn

C#:   3.14159.ToString("F2")
来源：http://qh.yuexingan06.cn

[A22] 获取字符串长度
来源：http://pc.szxytkj.cn

Py:   len(s)
来源：http://wr.bjjhwx.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qu.muxihuayi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ri.jianghongdianzi.cn

TS:   s.length
来源：http://ww.9csxet.cn

Java: s.length()
来源：http://it.521024.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cq.haigaiapp.cn

Ruby: s.length
来源：http://gq.panjiajie.cn

C#:   s.Length
来源：http://ar.haigaiapp.cn

[A23] 大小写转换
来源：http://lh.huixinmuqiang.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://xb.shxzskj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ly.huixinmuqiang.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pf.asd995.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tp.shxzukj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://eq.hahajie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rr.nszjky.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wh.panjiajie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qa.haigaiapp.cn

[A24] 去除首尾空白
来源：http://hi.muxihuayi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vb.gzmigu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kg.521024.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pb.nszjky.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hf.bookmarksfly.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bv.haigaiapp.cn

Go:   strings.TrimSpace(s)
来源：http://fh.wgjwhj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qy.szsharing.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hi.shtwfgs.cn

[A25] 字符串比较
来源：http://es.muxihuayi.cn

Py:   s1 == s2; s1 != s2
来源：http://yl.jianghongdianzi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qf.newstarts.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yp.chemitech.net.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pg.shtwfgs.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yo.chemitech.net.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xp.muxihuayi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://iv.hahajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fp.yuntaijiaju.cn

[A26] 类型转换总览
来源：http://sf.huixiangedu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gj.jctech888.com.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://it.hahajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bx.nszjky.cn

TS:   Number() String() Boolean() x as number
来源：http://xs.jctech888.com.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ss.szsharing.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nc.nicolike.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rg.szsharing.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cx.hahajie.cn

================================================================================
来源：http://co.huixiangedu.cn

B. 流程控制
来源：http://xp.huixiangedu.cn

================================================================================
来源：http://fo.chemitech.net.cn

[B01] 条件判断 if / else
来源：http://me.asd995.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ee.yuntaijiaju.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ye.muxihuayi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cn.hahajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tx.nszjky.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qe.9csxet.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://is.gzmigu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cx.shxzukj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://oo.panjiajie.cn

[B02] 多分支 else if / elif
来源：http://gf.jctech888.com.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gu.huixiangedu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qx.asd995.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ni.nszjky.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://il.bjjhwx.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pn.newstarts.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gs.muxihuayi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wm.bjjhwx.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ei.bookmarksfly.cn

[B03] switch / match / case
来源：http://yb.szsharing.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cn.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://so.huixinmuqiang.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zw.shtwfgs.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ck.bjjhwx.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bi.hahajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://um.nicolike.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://eh.shtwfgs.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fh.newstarts.cn

[B04] for 计数循环
来源：http://uq.huixiangedu.cn

Py:   for i in range(10): print(i)
来源：http://cv.huixinmuqiang.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rr.muxihuayi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hi.521024.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ue.shxzskj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://aa.szxytkj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rl.521024.cn

Ruby: 10.times { |i| puts i }
来源：http://jb.newstarts.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ap.huixinmuqiang.cn

[B05] 遍历数组 / 列表
来源：http://nk.9csxet.cn

Py:   for item in arr: print(item)
来源：http://zv.521024.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fg.bookmarksfly.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fg.szsharing.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://pp.hnjuh.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wy.muxihuayi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cy.szxytkj.cn

Ruby: arr.each { |item| puts item }
来源：http://qu.yuexingan06.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jq.shxzukj.cn

[B06] 遍历字典 / 对象
来源：http://gp.nszjky.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://je.gzmigu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pe.gzmigu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uy.shtwfgs.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hf.jctech888.com.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yx.bookmarksfly.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vf.szsharing.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://po.shxzukj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://du.huanxung.cn

[B07] while 循环
来源：http://gp.gzmigu.cn

Py:   while i < 10: i += 1
来源：http://jy.nszjky.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hw.haigaiapp.cn

JS:   while (i < 10) { i++; }
来源：http://xh.lnxyls.cn

TS:   while (i < 10) { i++; }
来源：http://vd.hahajie.cn

Java: while (i < 10) { i++; }
来源：http://yo.panjiajie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yv.gzmigu.cn

Ruby: while i < 10; i += 1; end
来源：http://gs.nszjky.cn

C#:   while (i < 10) { i++; }
来源：http://nm.panjiajie.cn

[B08] do-while（至少执行一次）
来源：http://za.nszjky.cn

Py:   # 无 do-while：用 while True + break
来源：http://ka.haigaiapp.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ob.shxzukj.cn

JS:   do { i++; } while (i < 10);
来源：http://ei.newstarts.cn

TS:   do { i++; } while (i < 10);
来源：http://km.yuntaijiaju.cn

Java: do { i++; } while (i < 10);
来源：http://xl.huanxung.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mw.jctech888.com.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ib.muxihuayi.cn

C#:   do { i++; } while (i < 10);
来源：http://tl.hnjuh.cn

[B09] break 与 continue
来源：http://iz.szxytkj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://td.huixinmuqiang.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mj.panjiajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sj.yuexingan06.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zh.jctech888.com.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://om.lnxyls.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ez.huixinmuqiang.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tr.panjiajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hr.nszjky.cn

[B10] 遍历同时拿索引
来源：http://ho.wgjwhj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://va.szsharing.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ii.colortex.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fv.panjiajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ic.9csxet.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://up.bjjhwx.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nl.lnxyls.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xo.hnjuh.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ss.gzmigu.cn

[B11] 生成数字序列 / 区间
来源：http://nu.jianghongdianzi.cn

Py:   list(range(0, 10, 2))
来源：http://uq.wgjwhj.cn

PHP:  range(0, 10, 2);
来源：http://ec.huixiangedu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jz.szxytkj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gj.shtwfgs.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xi.shtwfgs.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yw.shtwfgs.cn

Ruby: (0...10).step(2).to_a
来源：http://ih.hahajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kf.jianghongdianzi.cn

[B12] 跳出多层循环
来源：http://wr.haigaiapp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://cx.shxzskj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ug.chemitech.net.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yu.chemitech.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://du.nicolike.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://iv.jctech888.com.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ft.9csxet.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xm.panjiajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dd.521024.cn

[B13] 判断是否为数字
来源：http://mu.yuntaijiaju.cn

Py:   isinstance(x, (int, float))
来源：http://vf.nszjky.cn

PHP:  is_numeric($x)
来源：http://xq.nszjky.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iv.newstarts.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zp.newstarts.cn

Java: x instanceof Number
来源：http://ot.huixinmuqiang.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mn.521024.cn

Ruby: x.is_a?(Numeric)
来源：http://vb.haigaiapp.cn

C#:   x is int or double or decimal
来源：http://hl.szsharing.cn

[B14] 判断值是否在集合内
来源：http://lk.gzmigu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vj.bjjhwx.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://at.panjiajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://fi.szxytkj.cn

TS:   [1, 2, 3].includes(x)
来源：http://xn.yuexingan06.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hv.yuntaijiaju.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yk.asd995.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ak.asd995.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hu.huanxung.cn

[B15] 布尔运算与取反
来源：http://ox.521024.cn

Py:   a and b or not c
来源：http://hc.bookmarksfly.cn

PHP:  $a && $b || !$c
来源：http://rc.bookmarksfly.cn

JS:   a && b || !c
来源：http://hm.shxzukj.cn

TS:   a && b || !c
来源：http://qq.bookmarksfly.cn

Java: a && b || !c
来源：http://co.yuntaijiaju.cn

Go:   a && b || !c
来源：http://oa.nicolike.cn

Ruby: a && b || !c
来源：http://tq.huixiangedu.cn

C#:   a && b || !c
来源：http://zr.newstarts.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hx.shxzukj.cn

Py:   if not data: return
来源：http://lb.asd995.cn

PHP:  if (!$data) { return; }
来源：http://ax.521024.cn

JS:   if (!data) return;
来源：http://lr.colortex.cn

TS:   if (!data) return;
来源：http://gh.haigaiapp.cn

Java: if (data == null) return;
来源：http://af.yuntaijiaju.cn

Go:   if data == nil { return }
来源：http://gi.nicolike.cn

Ruby: return if data.nil?
来源：http://fv.colortex.cn

C#:   if (data == null) return;
来源：http://ek.newstarts.cn

================================================================================
来源：http://bs.nszjky.cn

C. 函数与作用域
来源：http://ho.nicolike.cn

================================================================================
来源：http://zr.szxytkj.cn

[C01] 定义函数
来源：http://ta.chemitech.net.cn

Py:   def add(a, b): return a + b
来源：http://cy.muxihuayi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wq.shxzskj.cn

JS:   function add(a, b) { return a + b; }
来源：http://ee.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ls.colortex.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ne.hahajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://kx.nszjky.cn

Ruby: def add(a, b); a + b; end
来源：http://fx.jctech888.com.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nz.bjjhwx.cn

[C02] 默认参数
来源：http://wa.muxihuayi.cn

Py:   def greet(name="World"): return name
来源：http://ih.wgjwhj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ha.szxytkj.cn

JS:   function greet(name = "World") { return name; }
来源：http://ko.shxzukj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gy.shxzukj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://aq.huixinmuqiang.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://un.yuntaijiaju.cn

Ruby: def greet(name = "World") = name
来源：http://me.shxzukj.cn

C#:   string Greet(string name = "World") => name;
来源：http://da.hahajie.cn

[C03] 可变参数
来源：http://lj.yuntaijiaju.cn

Py:   def total(*args): return sum(args)
来源：http://le.gzmigu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lg.szxytkj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://di.hnjuh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qm.huixinmuqiang.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://li.nicolike.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ba.lnxyls.cn

Ruby: def total(*nums); nums.sum; end
来源：http://nf.shtwfgs.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xm.huanxung.cn

[C04] 命名参数 / 关键字参数
来源：http://wk.newstarts.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ux.shxzskj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ig.jctech888.com.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.newstarts.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sy.lnxyls.cn

Java: // 无：用 Builder 模式或 record
来源：http://ui.huixiangedu.cn

Go:   // 无：用配置结构体参数
来源：http://pq.haigaiapp.cn

Ruby: f(a: 1, b: 2)
来源：http://kb.bookmarksfly.cn

C#:   f(a: 1, b: 2)
来源：http://xx.hnjuh.cn

[C05] 返回多个值
来源：http://lh.hnjuh.cn

Py:   return a, b
来源：http://ax.lnxyls.cn

PHP:  return [$a, $b];
来源：http://lh.huanxung.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xs.hahajie.cn

TS:   return { a, b };
来源：http://my.haigaiapp.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fq.bookmarksfly.cn

Go:   return a, b
来源：http://lo.szxytkj.cn

Ruby: return a, b
来源：http://hs.shxzskj.cn

C#:   return (a, b);              // ValueTuple
来源：http://kg.shxzskj.cn

[C06] 匿名函数 / lambda
来源：http://ue.yuntaijiaju.cn

Py:   square = lambda x: x * x
来源：http://mh.huixinmuqiang.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://nu.wgjwhj.cn

JS:   const square = x => x * x;
来源：http://sz.muxihuayi.cn

TS:   const square = (x: number): number => x * x;
来源：http://br.bjjhwx.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tw.yuntaijiaju.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fu.wgjwhj.cn

Ruby: square = ->(x) { x * x }
来源：http://rw.huixinmuqiang.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ql.nicolike.cn

[C07] 把函数作为参数传入
来源：http://mv.szxytkj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pe.colortex.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ml.nicolike.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xq.shxzskj.cn

TS:   arr.map(String)
来源：http://pr.wgjwhj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://px.hahajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kh.haigaiapp.cn

Ruby: arr.map(&:upcase)
来源：http://hd.jianghongdianzi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://nz.521024.cn

[C08] 闭包
来源：http://al.newstarts.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kw.asd995.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ez.jianghongdianzi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zx.9csxet.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sx.chemitech.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qj.szxytkj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dz.shxzskj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ou.shxzukj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://in.jianghongdianzi.cn

[C09] 递归
来源：http://gz.szxytkj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uk.yuexingan06.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dv.hahajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yv.jianghongdianzi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gp.newstarts.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zk.nicolike.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ur.wgjwhj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://po.521024.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nh.jianghongdianzi.cn

[C10] 变量作用域
来源：http://zm.bookmarksfly.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fw.nszjky.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cp.521024.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qp.huixiangedu.cn

TS:   同 JS
来源：http://lu.nicolike.cn

Java: 方法内为块级作用域
来源：http://is.chemitech.net.cn

Go:   花括号块级作用域
来源：http://ro.nicolike.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ag.colortex.cn

C#:   块级作用域
来源：http://xs.521024.cn

[C11] 模块导入与导出
来源：http://sz.yuntaijiaju.cn

Py:   from module import func
来源：http://sj.huixiangedu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://fo.asd995.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://iq.shxzukj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dl.yuexingan06.cn

Java: import java.util.List;
来源：http://ly.huanxung.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hg.asd995.cn


<!-- 参考信息 -->