代发 wailian999

[A22] 获取字符串长度
来源：http://iw.szsharing.cn

Py:   len(s)
来源：http://ea.hahajie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gr.jianghongdianzi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://us.shxzskj.cn

TS:   s.length
来源：http://xh.colortex.cn

Java: s.length()
来源：http://av.9csxet.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hx.hahajie.cn

Ruby: s.length
来源：http://oe.lnxyls.cn

C#:   s.Length
来源：http://gp.hnjuh.cn

[A23] 大小写转换
来源：http://md.gzmigu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://za.shxzukj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fo.yuntaijiaju.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ky.wgjwhj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://uy.yuexingan06.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ja.szxytkj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qq.lnxyls.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lg.bookmarksfly.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ln.chemitech.net.cn

[A24] 去除首尾空白
来源：http://pa.nicolike.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zd.gzmigu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://td.chemitech.net.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cw.shtwfgs.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kr.jctech888.com.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qd.521024.cn

Go:   strings.TrimSpace(s)
来源：http://gt.newstarts.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tf.nicolike.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vh.chemitech.net.cn

[A25] 字符串比较
来源：http://or.huanxung.cn

Py:   s1 == s2; s1 != s2
来源：http://yg.521024.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ev.hnjuh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jx.bookmarksfly.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jk.colortex.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://eb.wgjwhj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rb.hnjuh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://qb.nicolike.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kd.nszjky.cn

[A26] 类型转换总览
来源：http://in.shxzukj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sq.chemitech.net.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pb.panjiajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gq.wgjwhj.cn

TS:   Number() String() Boolean() x as number
来源：http://nr.huixiangedu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bg.huixiangedu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mo.shxzskj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zl.shxzukj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yd.huixinmuqiang.cn

================================================================================
来源：http://sj.shxzskj.cn

B. 流程控制
来源：http://kq.9csxet.cn

================================================================================
来源：http://oq.bjjhwx.cn

[B01] 条件判断 if / else
来源：http://rn.jianghongdianzi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://qb.shxzskj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gy.huanxung.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ks.wgjwhj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wb.muxihuayi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://fi.yuexingan06.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ae.jctech888.com.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ol.bjjhwx.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mp.chemitech.net.cn

[B02] 多分支 else if / elif
来源：http://aa.521024.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ya.nicolike.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ek.521024.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zr.gzmigu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tf.szsharing.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pc.521024.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://og.asd995.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wd.chemitech.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ha.jianghongdianzi.cn

[B03] switch / match / case
来源：http://rs.shxzukj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hg.nszjky.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uh.shtwfgs.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eb.bjjhwx.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rv.chemitech.net.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uj.szsharing.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ml.szxytkj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://to.9csxet.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ys.yuexingan06.cn

[B04] for 计数循环
来源：http://vf.shxzskj.cn

Py:   for i in range(10): print(i)
来源：http://hw.shtwfgs.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://oy.bookmarksfly.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zi.wgjwhj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vb.shxzukj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yp.jctech888.com.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pp.chemitech.net.cn

Ruby: 10.times { |i| puts i }
来源：http://kb.yuntaijiaju.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ox.521024.cn

[B05] 遍历数组 / 列表
来源：http://dy.yuntaijiaju.cn

Py:   for item in arr: print(item)
来源：http://aq.hnjuh.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rx.newstarts.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://tg.shtwfgs.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://oi.chemitech.net.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yp.jianghongdianzi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vk.yuntaijiaju.cn

Ruby: arr.each { |item| puts item }
来源：http://sc.hnjuh.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vq.huixiangedu.cn

[B06] 遍历字典 / 对象
来源：http://qn.nszjky.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ou.nszjky.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ye.newstarts.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ce.panjiajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sh.muxihuayi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ox.szsharing.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jo.szxytkj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lx.huanxung.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tg.szxytkj.cn

[B07] while 循环
来源：http://ny.chemitech.net.cn

Py:   while i < 10: i += 1
来源：http://kv.huixinmuqiang.cn

PHP:  while ($i < 10) { $i++; }
来源：http://op.colortex.cn

JS:   while (i < 10) { i++; }
来源：http://wj.shtwfgs.cn

TS:   while (i < 10) { i++; }
来源：http://sj.bjjhwx.cn

Java: while (i < 10) { i++; }
来源：http://mk.szxytkj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rr.yuexingan06.cn

Ruby: while i < 10; i += 1; end
来源：http://hk.hahajie.cn

C#:   while (i < 10) { i++; }
来源：http://ba.gzmigu.cn

[B08] do-while（至少执行一次）
来源：http://zc.chemitech.net.cn

Py:   # 无 do-while：用 while True + break
来源：http://zi.bjjhwx.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ka.yuexingan06.cn

JS:   do { i++; } while (i < 10);
来源：http://ei.haigaiapp.cn

TS:   do { i++; } while (i < 10);
来源：http://bc.huixinmuqiang.cn

Java: do { i++; } while (i < 10);
来源：http://ni.asd995.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vt.hahajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fr.huanxung.cn

C#:   do { i++; } while (i < 10);
来源：http://ww.bjjhwx.cn

[B09] break 与 continue
来源：http://hw.huixinmuqiang.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fq.szxytkj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ac.shxzskj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aj.huixinmuqiang.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ts.521024.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nv.huixinmuqiang.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jt.yuntaijiaju.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fn.muxihuayi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hu.lnxyls.cn

[B10] 遍历同时拿索引
来源：http://ue.szxytkj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://go.panjiajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://st.wgjwhj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sq.gzmigu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lt.shtwfgs.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kg.chemitech.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qd.shtwfgs.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cc.521024.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jj.shtwfgs.cn

[B11] 生成数字序列 / 区间
来源：http://mn.lnxyls.cn

Py:   list(range(0, 10, 2))
来源：http://aq.huanxung.cn

PHP:  range(0, 10, 2);
来源：http://lj.newstarts.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ta.newstarts.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lz.yuexingan06.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://so.colortex.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hh.asd995.cn

Ruby: (0...10).step(2).to_a
来源：http://va.newstarts.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kw.gzmigu.cn

[B12] 跳出多层循环
来源：http://ss.9csxet.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yv.bjjhwx.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://qp.shtwfgs.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tf.wgjwhj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.bookmarksfly.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qf.shtwfgs.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zm.lnxyls.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://di.lnxyls.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vs.bjjhwx.cn

[B13] 判断是否为数字
来源：http://oi.shxzskj.cn

Py:   isinstance(x, (int, float))
来源：http://qm.nszjky.cn

PHP:  is_numeric($x)
来源：http://av.shtwfgs.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xp.huixiangedu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ft.nszjky.cn

Java: x instanceof Number
来源：http://bc.lnxyls.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ic.lnxyls.cn

Ruby: x.is_a?(Numeric)
来源：http://em.hnjuh.cn

C#:   x is int or double or decimal
来源：http://cb.wgjwhj.cn

[B14] 判断值是否在集合内
来源：http://em.szxytkj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hg.muxihuayi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qq.521024.cn

JS:   [1, 2, 3].includes(x)
来源：http://dg.lnxyls.cn

TS:   [1, 2, 3].includes(x)
来源：http://wc.gzmigu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://my.9csxet.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cc.chemitech.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fc.colortex.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://es.chemitech.net.cn

[B15] 布尔运算与取反
来源：http://jp.bookmarksfly.cn

Py:   a and b or not c
来源：http://hj.yuntaijiaju.cn

PHP:  $a && $b || !$c
来源：http://oh.huanxung.cn

JS:   a && b || !c
来源：http://hm.panjiajie.cn

TS:   a && b || !c
来源：http://cf.chemitech.net.cn

Java: a && b || !c
来源：http://ws.szxytkj.cn

Go:   a && b || !c
来源：http://go.huixiangedu.cn

Ruby: a && b || !c
来源：http://di.lnxyls.cn

C#:   a && b || !c
来源：http://um.nszjky.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jf.jianghongdianzi.cn

Py:   if not data: return
来源：http://wu.newstarts.cn

PHP:  if (!$data) { return; }
来源：http://gr.yuntaijiaju.cn

JS:   if (!data) return;
来源：http://nb.huanxung.cn

TS:   if (!data) return;
来源：http://mg.shxzskj.cn

Java: if (data == null) return;
来源：http://zh.jctech888.com.cn

Go:   if data == nil { return }
来源：http://av.newstarts.cn

Ruby: return if data.nil?
来源：http://ue.lnxyls.cn

C#:   if (data == null) return;
来源：http://hz.szsharing.cn

================================================================================
来源：http://br.colortex.cn

C. 函数与作用域
来源：http://cb.huixinmuqiang.cn

================================================================================
来源：http://ot.jianghongdianzi.cn

[C01] 定义函数
来源：http://mf.hnjuh.cn

Py:   def add(a, b): return a + b
来源：http://vz.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zc.colortex.cn

JS:   function add(a, b) { return a + b; }
来源：http://cy.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vm.bookmarksfly.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://cl.jctech888.com.cn

Go:   func add(a, b int) int { return a + b }
来源：http://fk.jianghongdianzi.cn

Ruby: def add(a, b); a + b; end
来源：http://jt.haigaiapp.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bp.hahajie.cn

[C02] 默认参数
来源：http://fq.nszjky.cn

Py:   def greet(name="World"): return name
来源：http://eo.asd995.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fi.9csxet.cn

JS:   function greet(name = "World") { return name; }
来源：http://py.colortex.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://oq.muxihuayi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hr.nszjky.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nx.shxzukj.cn

Ruby: def greet(name = "World") = name
来源：http://ir.shtwfgs.cn

C#:   string Greet(string name = "World") => name;
来源：http://ue.muxihuayi.cn

[C03] 可变参数
来源：http://sd.colortex.cn

Py:   def total(*args): return sum(args)
来源：http://ed.shtwfgs.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://su.panjiajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://an.panjiajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qs.yuexingan06.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cq.hnjuh.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://we.nicolike.cn

Ruby: def total(*nums); nums.sum; end
来源：http://bv.huixinmuqiang.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ca.asd995.cn

[C04] 命名参数 / 关键字参数
来源：http://hb.9csxet.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gs.haigaiapp.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jm.9csxet.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://li.szsharing.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ah.521024.cn

Java: // 无：用 Builder 模式或 record
来源：http://cc.gzmigu.cn

Go:   // 无：用配置结构体参数
来源：http://wf.muxihuayi.cn

Ruby: f(a: 1, b: 2)
来源：http://fz.huixinmuqiang.cn

C#:   f(a: 1, b: 2)
来源：http://ha.yuexingan06.cn

[C05] 返回多个值
来源：http://jg.shtwfgs.cn

Py:   return a, b
来源：http://bf.huixinmuqiang.cn

PHP:  return [$a, $b];
来源：http://qp.shtwfgs.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yx.lnxyls.cn

TS:   return { a, b };
来源：http://ux.huixiangedu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jv.haigaiapp.cn

Go:   return a, b
来源：http://lv.panjiajie.cn

Ruby: return a, b
来源：http://de.lnxyls.cn

C#:   return (a, b);              // ValueTuple
来源：http://yt.lnxyls.cn

[C06] 匿名函数 / lambda
来源：http://vu.lnxyls.cn

Py:   square = lambda x: x * x
来源：http://ma.lnxyls.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://di.colortex.cn

JS:   const square = x => x * x;
来源：http://hk.gzmigu.cn

TS:   const square = (x: number): number => x * x;
来源：http://by.haigaiapp.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://az.hahajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dc.muxihuayi.cn

Ruby: square = ->(x) { x * x }
来源：http://ko.huixiangedu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bz.huixiangedu.cn

[C07] 把函数作为参数传入
来源：http://sn.lnxyls.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yp.lnxyls.cn

PHP:  array_map("strtoupper", $arr);
来源：http://rd.huanxung.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ph.nicolike.cn

TS:   arr.map(String)
来源：http://dh.shxzskj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ol.nszjky.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yd.shxzskj.cn

Ruby: arr.map(&:upcase)
来源：http://sg.muxihuayi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://yb.521024.cn

[C08] 闭包
来源：http://mw.chemitech.net.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wf.szxytkj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ee.nszjky.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://do.wgjwhj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ly.panjiajie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qx.9csxet.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ri.huanxung.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jk.szxytkj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nv.nicolike.cn

[C09] 递归
来源：http://jv.asd995.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pa.hahajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fr.muxihuayi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fx.jctech888.com.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://go.newstarts.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gn.521024.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://yk.hahajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://on.nicolike.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ig.jctech888.com.cn

[C10] 变量作用域
来源：http://qq.bookmarksfly.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cs.wgjwhj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ln.chemitech.net.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qx.huixinmuqiang.cn

TS:   同 JS
来源：http://gl.nszjky.cn

Java: 方法内为块级作用域
来源：http://eq.nicolike.cn

Go:   花括号块级作用域
来源：http://pf.lnxyls.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jg.panjiajie.cn

C#:   块级作用域
来源：http://fe.haigaiapp.cn

[C11] 模块导入与导出
来源：http://pj.jctech888.com.cn

Py:   from module import func
来源：http://js.yuexingan06.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://fr.huixinmuqiang.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ho.hahajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tv.huixinmuqiang.cn

Java: import java.util.List;
来源：http://ij.muxihuayi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ia.jctech888.com.cn

Ruby: require "json"; require_relative "./util"
来源：http://ew.colortex.cn

C#:   using System.Text;
来源：http://gx.szsharing.cn

[C12] 立即执行函数 IIFE
来源：http://hx.hahajie.cn

Py:   (lambda: print("run"))()
来源：http://tj.shxzukj.cn

PHP:  (function () { echo "run"; })();
来源：http://at.huanxung.cn

JS:   (() => { console.log("run"); })();
来源：http://nz.wgjwhj.cn

TS:   (() => { console.log("run"); })();
来源：http://by.shtwfgs.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cv.jctech888.com.cn


<!-- 参考信息 -->