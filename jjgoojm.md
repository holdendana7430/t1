代发 wailian999

[A22] 获取字符串长度
来源：http://fa.yuntaijiaju.cn

Py:   len(s)
来源：http://yc.bookmarksfly.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://so.huanxung.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gy.nicolike.cn

TS:   s.length
来源：http://nx.yuntaijiaju.cn

Java: s.length()
来源：http://oi.chemitech.net.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://iz.szxytkj.cn

Ruby: s.length
来源：http://yx.szsharing.cn

C#:   s.Length
来源：http://mw.9csxet.cn

[A23] 大小写转换
来源：http://qu.newstarts.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ak.shtwfgs.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gu.colortex.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xd.jctech888.com.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gb.newstarts.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fa.asd995.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lw.szxytkj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xq.muxihuayi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://es.bjjhwx.cn

[A24] 去除首尾空白
来源：http://zu.huixinmuqiang.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qf.yuntaijiaju.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gx.jctech888.com.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rk.hahajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lq.chemitech.net.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jh.shxzskj.cn

Go:   strings.TrimSpace(s)
来源：http://ii.lnxyls.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zt.gzmigu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wa.chemitech.net.cn

[A25] 字符串比较
来源：http://qh.shxzskj.cn

Py:   s1 == s2; s1 != s2
来源：http://eb.szsharing.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rs.jctech888.com.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://br.shxzskj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dj.panjiajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tw.muxihuayi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ns.yuntaijiaju.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://bn.chemitech.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zh.newstarts.cn

[A26] 类型转换总览
来源：http://jf.newstarts.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gr.lnxyls.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hj.nicolike.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vf.szsharing.cn

TS:   Number() String() Boolean() x as number
来源：http://am.colortex.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ye.nicolike.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://za.colortex.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://uc.huixinmuqiang.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ks.jianghongdianzi.cn

================================================================================
来源：http://ff.szxytkj.cn

B. 流程控制
来源：http://hp.bookmarksfly.cn

================================================================================
来源：http://qw.asd995.cn

[B01] 条件判断 if / else
来源：http://ph.521024.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://es.chemitech.net.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ka.lnxyls.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ic.jianghongdianzi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xt.shxzskj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://di.yuexingan06.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://av.shxzukj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cr.bookmarksfly.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bz.521024.cn

[B02] 多分支 else if / elif
来源：http://jp.jianghongdianzi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yc.huixiangedu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qd.huixiangedu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aw.colortex.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://es.panjiajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uu.panjiajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yu.nicolike.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xt.jctech888.com.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qb.huixinmuqiang.cn

[B03] switch / match / case
来源：http://so.huanxung.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fg.szsharing.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gg.bjjhwx.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vn.nicolike.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zz.chemitech.net.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jg.gzmigu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pr.huixiangedu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lz.szxytkj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ai.lnxyls.cn

[B04] for 计数循环
来源：http://qq.huanxung.cn

Py:   for i in range(10): print(i)
来源：http://fs.shxzskj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pb.shxzukj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ii.lnxyls.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ay.hnjuh.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yp.shxzskj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://iy.shtwfgs.cn

Ruby: 10.times { |i| puts i }
来源：http://ll.szsharing.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yb.panjiajie.cn

[B05] 遍历数组 / 列表
来源：http://ot.wgjwhj.cn

Py:   for item in arr: print(item)
来源：http://li.lnxyls.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hb.bjjhwx.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ig.chemitech.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ch.huixinmuqiang.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://cs.muxihuayi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fr.panjiajie.cn

Ruby: arr.each { |item| puts item }
来源：http://lb.521024.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dw.huixiangedu.cn

[B06] 遍历字典 / 对象
来源：http://dy.haigaiapp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://iz.hahajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bs.jianghongdianzi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pe.asd995.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://da.gzmigu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nh.nszjky.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://uw.asd995.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lp.shxzskj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dw.bookmarksfly.cn

[B07] while 循环
来源：http://sv.9csxet.cn

Py:   while i < 10: i += 1
来源：http://zi.jianghongdianzi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://jj.jianghongdianzi.cn

JS:   while (i < 10) { i++; }
来源：http://np.chemitech.net.cn

TS:   while (i < 10) { i++; }
来源：http://en.lnxyls.cn

Java: while (i < 10) { i++; }
来源：http://mv.panjiajie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lu.jianghongdianzi.cn

Ruby: while i < 10; i += 1; end
来源：http://ny.nszjky.cn

C#:   while (i < 10) { i++; }
来源：http://fo.muxihuayi.cn

[B08] do-while（至少执行一次）
来源：http://mx.hahajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://ov.chemitech.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pd.nszjky.cn

JS:   do { i++; } while (i < 10);
来源：http://gm.haigaiapp.cn

TS:   do { i++; } while (i < 10);
来源：http://fn.521024.cn

Java: do { i++; } while (i < 10);
来源：http://zc.bookmarksfly.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://op.szxytkj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xs.szsharing.cn

C#:   do { i++; } while (i < 10);
来源：http://vv.chemitech.net.cn

[B09] break 与 continue
来源：http://tn.hnjuh.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zz.szxytkj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wv.muxihuayi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oo.haigaiapp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ox.shtwfgs.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ur.szxytkj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ub.gzmigu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xq.9csxet.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hb.huixiangedu.cn

[B10] 遍历同时拿索引
来源：http://vp.huanxung.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ev.521024.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bz.jianghongdianzi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://on.bjjhwx.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xb.jianghongdianzi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://do.yuntaijiaju.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uz.asd995.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ud.gzmigu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cl.9csxet.cn

[B11] 生成数字序列 / 区间
来源：http://au.muxihuayi.cn

Py:   list(range(0, 10, 2))
来源：http://nm.nicolike.cn

PHP:  range(0, 10, 2);
来源：http://pm.bjjhwx.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qa.bjjhwx.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qp.chemitech.net.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qu.bjjhwx.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tw.huanxung.cn

Ruby: (0...10).step(2).to_a
来源：http://th.shxzskj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bs.nszjky.cn

[B12] 跳出多层循环
来源：http://zs.521024.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bo.521024.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://xa.panjiajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bm.hahajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wh.szxytkj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vt.lnxyls.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ce.9csxet.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dw.gzmigu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zd.nicolike.cn

[B13] 判断是否为数字
来源：http://bu.szsharing.cn

Py:   isinstance(x, (int, float))
来源：http://ii.huixiangedu.cn

PHP:  is_numeric($x)
来源：http://ku.colortex.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jw.9csxet.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bu.asd995.cn

Java: x instanceof Number
来源：http://st.nicolike.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bx.huixiangedu.cn

Ruby: x.is_a?(Numeric)
来源：http://ce.szxytkj.cn

C#:   x is int or double or decimal
来源：http://jc.colortex.cn

[B14] 判断值是否在集合内
来源：http://gl.lnxyls.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://my.huanxung.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bq.jctech888.com.cn

JS:   [1, 2, 3].includes(x)
来源：http://ky.haigaiapp.cn

TS:   [1, 2, 3].includes(x)
来源：http://oc.szsharing.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://zw.lnxyls.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://av.yuexingan06.cn

Ruby: [1, 2, 3].include?(x)
来源：http://re.haigaiapp.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gu.muxihuayi.cn

[B15] 布尔运算与取反
来源：http://ru.haigaiapp.cn

Py:   a and b or not c
来源：http://zi.jianghongdianzi.cn

PHP:  $a && $b || !$c
来源：http://xo.yuntaijiaju.cn

JS:   a && b || !c
来源：http://nt.huixinmuqiang.cn

TS:   a && b || !c
来源：http://zg.szxytkj.cn

Java: a && b || !c
来源：http://gh.gzmigu.cn

Go:   a && b || !c
来源：http://jz.shxzukj.cn

Ruby: a && b || !c
来源：http://uj.asd995.cn

C#:   a && b || !c
来源：http://ah.shtwfgs.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hp.newstarts.cn

Py:   if not data: return
来源：http://fb.chemitech.net.cn

PHP:  if (!$data) { return; }
来源：http://us.shxzskj.cn

JS:   if (!data) return;
来源：http://cy.chemitech.net.cn

TS:   if (!data) return;
来源：http://bl.yuntaijiaju.cn

Java: if (data == null) return;
来源：http://xq.newstarts.cn

Go:   if data == nil { return }
来源：http://jy.yuntaijiaju.cn

Ruby: return if data.nil?
来源：http://bj.huanxung.cn

C#:   if (data == null) return;
来源：http://of.9csxet.cn

================================================================================
来源：http://nq.haigaiapp.cn

C. 函数与作用域
来源：http://jd.9csxet.cn

================================================================================
来源：http://kc.jctech888.com.cn

[C01] 定义函数
来源：http://sq.lnxyls.cn

Py:   def add(a, b): return a + b
来源：http://us.muxihuayi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xp.hnjuh.cn

JS:   function add(a, b) { return a + b; }
来源：http://fe.huixinmuqiang.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zh.szxytkj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zq.shxzukj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://kv.szxytkj.cn

Ruby: def add(a, b); a + b; end
来源：http://qh.bookmarksfly.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://si.szsharing.cn

[C02] 默认参数
来源：http://gw.colortex.cn

Py:   def greet(name="World"): return name
来源：http://gw.szxytkj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wr.panjiajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://dv.nszjky.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://aa.lnxyls.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fp.yuexingan06.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ll.szsharing.cn

Ruby: def greet(name = "World") = name
来源：http://jk.lnxyls.cn

C#:   string Greet(string name = "World") => name;
来源：http://ge.bookmarksfly.cn

[C03] 可变参数
来源：http://ex.shxzukj.cn

Py:   def total(*args): return sum(args)
来源：http://js.shxzskj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jb.bjjhwx.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pa.huixinmuqiang.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://oi.bjjhwx.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://np.lnxyls.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ub.nszjky.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ak.nicolike.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wy.521024.cn

[C04] 命名参数 / 关键字参数
来源：http://fw.muxihuayi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qe.nicolike.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dj.huixinmuqiang.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://oj.panjiajie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cz.jianghongdianzi.cn

Java: // 无：用 Builder 模式或 record
来源：http://xf.nicolike.cn

Go:   // 无：用配置结构体参数
来源：http://hc.nicolike.cn

Ruby: f(a: 1, b: 2)
来源：http://gj.szxytkj.cn

C#:   f(a: 1, b: 2)
来源：http://mp.haigaiapp.cn

[C05] 返回多个值
来源：http://uq.jctech888.com.cn

Py:   return a, b
来源：http://nu.wgjwhj.cn

PHP:  return [$a, $b];
来源：http://yh.haigaiapp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yi.chemitech.net.cn

TS:   return { a, b };
来源：http://df.9csxet.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yi.gzmigu.cn

Go:   return a, b
来源：http://zs.newstarts.cn

Ruby: return a, b
来源：http://vi.wgjwhj.cn

C#:   return (a, b);              // ValueTuple
来源：http://eo.wgjwhj.cn

[C06] 匿名函数 / lambda
来源：http://mu.9csxet.cn

Py:   square = lambda x: x * x
来源：http://iq.chemitech.net.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://hd.lnxyls.cn

JS:   const square = x => x * x;
来源：http://vx.9csxet.cn

TS:   const square = (x: number): number => x * x;
来源：http://hn.yuntaijiaju.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ke.huixinmuqiang.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zu.huixinmuqiang.cn

Ruby: square = ->(x) { x * x }
来源：http://ek.bjjhwx.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qr.9csxet.cn

[C07] 把函数作为参数传入
来源：http://rx.huixinmuqiang.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zb.szxytkj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ua.hnjuh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cd.szsharing.cn

TS:   arr.map(String)
来源：http://gr.hahajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ft.shtwfgs.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://iu.yuexingan06.cn

Ruby: arr.map(&:upcase)
来源：http://zx.bookmarksfly.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://vu.nicolike.cn

[C08] 闭包
来源：http://md.bjjhwx.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uk.lnxyls.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kl.huixinmuqiang.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sr.shxzukj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ru.huixiangedu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ik.wgjwhj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://eh.9csxet.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mg.lnxyls.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://je.nszjky.cn

[C09] 递归
来源：http://aa.yuntaijiaju.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://an.asd995.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xt.szxytkj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oz.shtwfgs.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yu.lnxyls.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ev.shxzskj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ld.bookmarksfly.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sp.521024.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pm.bjjhwx.cn

[C10] 变量作用域
来源：http://yk.yuexingan06.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yf.bjjhwx.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jl.shxzukj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lp.521024.cn

TS:   同 JS
来源：http://rs.9csxet.cn

Java: 方法内为块级作用域
来源：http://or.bjjhwx.cn

Go:   花括号块级作用域
来源：http://pz.shxzskj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://le.chemitech.net.cn

C#:   块级作用域
来源：http://bb.nicolike.cn

[C11] 模块导入与导出
来源：http://jc.huanxung.cn

Py:   from module import func
来源：http://tl.muxihuayi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ea.chemitech.net.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://nb.jctech888.com.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ns.nicolike.cn

Java: import java.util.List;
来源：http://mz.asd995.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qn.hnjuh.cn

Ruby: require "json"; require_relative "./util"
来源：http://uz.shtwfgs.cn

C#:   using System.Text;
来源：http://wy.muxihuayi.cn

[C12] 立即执行函数 IIFE
来源：http://zn.hahajie.cn

Py:   (lambda: print("run"))()
来源：http://bz.shxzskj.cn

PHP:  (function () { echo "run"; })();
来源：http://ya.panjiajie.cn

JS:   (() => { console.log("run"); })();
来源：http://sv.lnxyls.cn

TS:   (() => { console.log("run"); })();
来源：http://oc.szsharing.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nq.bookmarksfly.cn


<!-- 参考信息 -->