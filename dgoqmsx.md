代发 wailian999

[A22] 获取字符串长度
来源：http://ma.hnjuh.cn

Py:   len(s)
来源：http://zl.gzmigu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xw.muxihuayi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qu.huixiangedu.cn

TS:   s.length
来源：http://kk.wgjwhj.cn

Java: s.length()
来源：http://yv.huixinmuqiang.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hy.huixiangedu.cn

Ruby: s.length
来源：http://yf.szsharing.cn

C#:   s.Length
来源：http://uy.chemitech.net.cn

[A23] 大小写转换
来源：http://rv.szxytkj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://gc.nszjky.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qa.nicolike.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tq.521024.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://aq.bookmarksfly.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cb.bjjhwx.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dw.bjjhwx.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vi.yuntaijiaju.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://vw.colortex.cn

[A24] 去除首尾空白
来源：http://kd.bookmarksfly.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gu.muxihuayi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wl.panjiajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tv.521024.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fo.bookmarksfly.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pr.huixiangedu.cn

Go:   strings.TrimSpace(s)
来源：http://oe.wgjwhj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qd.hnjuh.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zc.chemitech.net.cn

[A25] 字符串比较
来源：http://tn.nszjky.cn

Py:   s1 == s2; s1 != s2
来源：http://cu.asd995.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nd.huixiangedu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yq.colortex.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jt.9csxet.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qm.lnxyls.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vc.gzmigu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ur.huixiangedu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nx.wgjwhj.cn

[A26] 类型转换总览
来源：http://vt.newstarts.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dj.haigaiapp.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://po.newstarts.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ph.nicolike.cn

TS:   Number() String() Boolean() x as number
来源：http://dy.jianghongdianzi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://sa.szsharing.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xg.szxytkj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://er.jianghongdianzi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ti.lnxyls.cn

================================================================================
来源：http://mi.9csxet.cn

B. 流程控制
来源：http://eh.nszjky.cn

================================================================================
来源：http://fz.asd995.cn

[B01] 条件判断 if / else
来源：http://me.nicolike.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://yc.panjiajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jc.wgjwhj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cs.gzmigu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://py.nszjky.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://yf.nicolike.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://eb.shxzskj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fl.yuntaijiaju.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zk.521024.cn

[B02] 多分支 else if / elif
来源：http://jd.newstarts.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jx.huanxung.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://df.wgjwhj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uh.bjjhwx.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ec.haigaiapp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zf.hahajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yu.9csxet.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vt.hnjuh.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fl.huixinmuqiang.cn

[B03] switch / match / case
来源：http://gi.colortex.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ql.newstarts.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://by.lnxyls.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ao.wgjwhj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uv.huanxung.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ds.newstarts.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cs.jctech888.com.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qg.shtwfgs.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cg.gzmigu.cn

[B04] for 计数循环
来源：http://xw.panjiajie.cn

Py:   for i in range(10): print(i)
来源：http://dh.521024.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cn.hnjuh.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sm.jctech888.com.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ip.huanxung.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ie.jctech888.com.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tl.lnxyls.cn

Ruby: 10.times { |i| puts i }
来源：http://bv.521024.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tl.szsharing.cn

[B05] 遍历数组 / 列表
来源：http://rf.nicolike.cn

Py:   for item in arr: print(item)
来源：http://zt.yuexingan06.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fq.bjjhwx.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://oe.szsharing.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://dn.gzmigu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fw.gzmigu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ll.shxzukj.cn

Ruby: arr.each { |item| puts item }
来源：http://ky.wgjwhj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hk.chemitech.net.cn

[B06] 遍历字典 / 对象
来源：http://qg.nszjky.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://bi.jctech888.com.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xp.huixiangedu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lh.newstarts.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cx.shxzukj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://as.chemitech.net.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gc.huixiangedu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ax.nicolike.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ex.haigaiapp.cn

[B07] while 循环
来源：http://uo.bjjhwx.cn

Py:   while i < 10: i += 1
来源：http://aq.huixiangedu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gg.colortex.cn

JS:   while (i < 10) { i++; }
来源：http://ry.huanxung.cn

TS:   while (i < 10) { i++; }
来源：http://rb.bjjhwx.cn

Java: while (i < 10) { i++; }
来源：http://iv.muxihuayi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ar.shxzukj.cn

Ruby: while i < 10; i += 1; end
来源：http://ur.panjiajie.cn

C#:   while (i < 10) { i++; }
来源：http://hg.nszjky.cn

[B08] do-while（至少执行一次）
来源：http://dd.9csxet.cn

Py:   # 无 do-while：用 while True + break
来源：http://nn.521024.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://he.gzmigu.cn

JS:   do { i++; } while (i < 10);
来源：http://kb.panjiajie.cn

TS:   do { i++; } while (i < 10);
来源：http://ui.jctech888.com.cn

Java: do { i++; } while (i < 10);
来源：http://ln.newstarts.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vt.gzmigu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fl.wgjwhj.cn

C#:   do { i++; } while (i < 10);
来源：http://av.9csxet.cn

[B09] break 与 continue
来源：http://le.huixiangedu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ym.shxzukj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://eb.chemitech.net.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cb.9csxet.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ud.jianghongdianzi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qz.szsharing.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://js.bookmarksfly.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cj.lnxyls.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ob.szsharing.cn

[B10] 遍历同时拿索引
来源：http://ji.haigaiapp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pi.huixiangedu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://br.yuntaijiaju.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lr.bjjhwx.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gz.hahajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bj.jianghongdianzi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wi.huanxung.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yu.colortex.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fx.muxihuayi.cn

[B11] 生成数字序列 / 区间
来源：http://qt.gzmigu.cn

Py:   list(range(0, 10, 2))
来源：http://jm.shxzskj.cn

PHP:  range(0, 10, 2);
来源：http://wi.asd995.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bk.lnxyls.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ku.nicolike.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ez.jctech888.com.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sw.nszjky.cn

Ruby: (0...10).step(2).to_a
来源：http://tw.gzmigu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sj.shxzskj.cn

[B12] 跳出多层循环
来源：http://fq.huanxung.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ld.nszjky.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://rq.colortex.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bf.szsharing.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yh.nszjky.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://aa.bjjhwx.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mk.lnxyls.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tr.9csxet.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bh.newstarts.cn

[B13] 判断是否为数字
来源：http://yv.shxzskj.cn

Py:   isinstance(x, (int, float))
来源：http://wf.shxzskj.cn

PHP:  is_numeric($x)
来源：http://bv.yuntaijiaju.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bv.panjiajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qo.hahajie.cn

Java: x instanceof Number
来源：http://lj.szxytkj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gg.nicolike.cn

Ruby: x.is_a?(Numeric)
来源：http://ed.9csxet.cn

C#:   x is int or double or decimal
来源：http://mw.huanxung.cn

[B14] 判断值是否在集合内
来源：http://li.hnjuh.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qt.shxzskj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wr.colortex.cn

JS:   [1, 2, 3].includes(x)
来源：http://hc.nicolike.cn

TS:   [1, 2, 3].includes(x)
来源：http://tw.hahajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://wv.shxzskj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zf.yuexingan06.cn

Ruby: [1, 2, 3].include?(x)
来源：http://lq.huixinmuqiang.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ir.shtwfgs.cn

[B15] 布尔运算与取反
来源：http://ro.szxytkj.cn

Py:   a and b or not c
来源：http://at.9csxet.cn

PHP:  $a && $b || !$c
来源：http://hw.nicolike.cn

JS:   a && b || !c
来源：http://bs.colortex.cn

TS:   a && b || !c
来源：http://oz.yuntaijiaju.cn

Java: a && b || !c
来源：http://bs.szsharing.cn

Go:   a && b || !c
来源：http://ne.huixinmuqiang.cn

Ruby: a && b || !c
来源：http://sp.wgjwhj.cn

C#:   a && b || !c
来源：http://ua.shxzskj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zv.bjjhwx.cn

Py:   if not data: return
来源：http://ns.huanxung.cn

PHP:  if (!$data) { return; }
来源：http://xe.521024.cn

JS:   if (!data) return;
来源：http://qm.asd995.cn

TS:   if (!data) return;
来源：http://jn.szsharing.cn

Java: if (data == null) return;
来源：http://lo.haigaiapp.cn

Go:   if data == nil { return }
来源：http://cs.shxzukj.cn

Ruby: return if data.nil?
来源：http://yg.jctech888.com.cn

C#:   if (data == null) return;
来源：http://bz.bjjhwx.cn

================================================================================
来源：http://bq.muxihuayi.cn

C. 函数与作用域
来源：http://vc.9csxet.cn

================================================================================
来源：http://ns.gzmigu.cn

[C01] 定义函数
来源：http://cy.nszjky.cn

Py:   def add(a, b): return a + b
来源：http://wv.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hp.szsharing.cn

JS:   function add(a, b) { return a + b; }
来源：http://ae.szxytkj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ce.hnjuh.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qo.szxytkj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://gm.521024.cn

Ruby: def add(a, b); a + b; end
来源：http://kf.asd995.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vs.bjjhwx.cn

[C02] 默认参数
来源：http://yq.nicolike.cn

Py:   def greet(name="World"): return name
来源：http://wb.nszjky.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ba.521024.cn

JS:   function greet(name = "World") { return name; }
来源：http://tr.muxihuayi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://tu.huixiangedu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ot.lnxyls.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nt.szsharing.cn

Ruby: def greet(name = "World") = name
来源：http://qv.jctech888.com.cn

C#:   string Greet(string name = "World") => name;
来源：http://ik.jianghongdianzi.cn

[C03] 可变参数
来源：http://oo.muxihuayi.cn

Py:   def total(*args): return sum(args)
来源：http://ad.wgjwhj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nq.huanxung.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fn.huixiangedu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ya.huixiangedu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ii.yuexingan06.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ny.gzmigu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://jh.hnjuh.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ts.haigaiapp.cn

[C04] 命名参数 / 关键字参数
来源：http://aa.huixiangedu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ii.huixinmuqiang.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ft.huixiangedu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dg.hnjuh.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vl.shtwfgs.cn

Java: // 无：用 Builder 模式或 record
来源：http://sm.szsharing.cn

Go:   // 无：用配置结构体参数
来源：http://mq.asd995.cn

Ruby: f(a: 1, b: 2)
来源：http://sj.chemitech.net.cn

C#:   f(a: 1, b: 2)
来源：http://gm.lnxyls.cn

[C05] 返回多个值
来源：http://ne.huixinmuqiang.cn

Py:   return a, b
来源：http://zc.hahajie.cn

PHP:  return [$a, $b];
来源：http://yv.newstarts.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://lk.huanxung.cn

TS:   return { a, b };
来源：http://lv.9csxet.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tn.hnjuh.cn

Go:   return a, b
来源：http://zv.521024.cn

Ruby: return a, b
来源：http://zi.hnjuh.cn

C#:   return (a, b);              // ValueTuple
来源：http://zl.bookmarksfly.cn

[C06] 匿名函数 / lambda
来源：http://zi.huanxung.cn

Py:   square = lambda x: x * x
来源：http://no.muxihuayi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://em.jctech888.com.cn

JS:   const square = x => x * x;
来源：http://xc.asd995.cn

TS:   const square = (x: number): number => x * x;
来源：http://ec.chemitech.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jh.colortex.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gi.shxzukj.cn

Ruby: square = ->(x) { x * x }
来源：http://dm.asd995.cn

C#:   Func<int, int> square = x => x * x;
来源：http://sc.nicolike.cn

[C07] 把函数作为参数传入
来源：http://se.nszjky.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gk.szxytkj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ip.hahajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ln.nszjky.cn

TS:   arr.map(String)
来源：http://gn.szsharing.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ji.521024.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xx.chemitech.net.cn

Ruby: arr.map(&:upcase)
来源：http://ks.521024.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://vq.yuexingan06.cn

[C08] 闭包
来源：http://dy.muxihuayi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ia.nicolike.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dv.haigaiapp.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jd.jianghongdianzi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ic.nicolike.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gq.hnjuh.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kh.panjiajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zs.shxzskj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tg.huixinmuqiang.cn

[C09] 递归
来源：http://oh.bookmarksfly.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jh.szsharing.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ga.wgjwhj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dx.nszjky.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xi.nicolike.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ua.bookmarksfly.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wh.gzmigu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hu.hahajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tv.shxzukj.cn

[C10] 变量作用域
来源：http://sy.shxzskj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sl.wgjwhj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://uh.shtwfgs.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ob.hnjuh.cn

TS:   同 JS
来源：http://ql.yuntaijiaju.cn

Java: 方法内为块级作用域
来源：http://ku.gzmigu.cn

Go:   花括号块级作用域
来源：http://ta.9csxet.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ox.colortex.cn

C#:   块级作用域
来源：http://yr.jctech888.com.cn

[C11] 模块导入与导出
来源：http://on.szxytkj.cn

Py:   from module import func
来源：http://sl.9csxet.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hl.jianghongdianzi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://yv.panjiajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ql.bjjhwx.cn

Java: import java.util.List;
来源：http://hz.huixinmuqiang.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hq.jctech888.com.cn

Ruby: require "json"; require_relative "./util"
来源：http://xg.shxzukj.cn

C#:   using System.Text;
来源：http://qh.asd995.cn

[C12] 立即执行函数 IIFE
来源：http://vz.chemitech.net.cn

Py:   (lambda: print("run"))()
来源：http://hs.wgjwhj.cn

PHP:  (function () { echo "run"; })();
来源：http://tc.asd995.cn

JS:   (() => { console.log("run"); })();
来源：http://dr.shtwfgs.cn

TS:   (() => { console.log("run"); })();
来源：http://vi.bookmarksfly.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qk.panjiajie.cn


<!-- 参考信息 -->