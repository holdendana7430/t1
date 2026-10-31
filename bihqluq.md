代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://qy.chemitech.net.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tv.newstarts.cn

Ruby: format("%.2f", 3.14159)
来源：http://am.szsharing.cn

C#:   3.14159.ToString("F2")
来源：http://ox.lnxyls.cn

[A22] 获取字符串长度
来源：http://oi.bjjhwx.cn

Py:   len(s)
来源：http://ow.bjjhwx.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ea.jianghongdianzi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://za.yuexingan06.cn

TS:   s.length
来源：http://vy.huixiangedu.cn

Java: s.length()
来源：http://rb.jianghongdianzi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hu.nszjky.cn

Ruby: s.length
来源：http://tx.9csxet.cn

C#:   s.Length
来源：http://bq.shxzskj.cn

[A23] 大小写转换
来源：http://na.jianghongdianzi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://py.jctech888.com.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rx.huanxung.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qt.nszjky.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xk.shxzskj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://uo.chemitech.net.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mi.gzmigu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hp.9csxet.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zk.szsharing.cn

[A24] 去除首尾空白
来源：http://tn.huixiangedu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://kp.shxzskj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bn.huixinmuqiang.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hc.wgjwhj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tg.wgjwhj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kd.shxzskj.cn

Go:   strings.TrimSpace(s)
来源：http://et.muxihuayi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hp.shtwfgs.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cb.gzmigu.cn

[A25] 字符串比较
来源：http://ba.hahajie.cn

Py:   s1 == s2; s1 != s2
来源：http://ei.nszjky.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://be.shxzukj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ka.gzmigu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wz.9csxet.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jl.huixinmuqiang.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ky.szsharing.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://cr.shxzskj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xi.bjjhwx.cn

[A26] 类型转换总览
来源：http://fv.521024.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rh.szsharing.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gg.wgjwhj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rx.nicolike.cn

TS:   Number() String() Boolean() x as number
来源：http://xx.jctech888.com.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://oi.huanxung.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sj.shtwfgs.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://yu.huixinmuqiang.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hl.hnjuh.cn

================================================================================
来源：http://qg.huixiangedu.cn

B. 流程控制
来源：http://uq.yuntaijiaju.cn

================================================================================
来源：http://qx.huixinmuqiang.cn

[B01] 条件判断 if / else
来源：http://rn.bookmarksfly.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://gx.yuexingan06.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://al.9csxet.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jg.newstarts.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://io.bookmarksfly.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://wm.521024.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ru.colortex.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://oy.nszjky.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bm.shtwfgs.cn

[B02] 多分支 else if / elif
来源：http://nd.newstarts.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://uv.huanxung.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ag.hahajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tr.chemitech.net.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cb.521024.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://we.bjjhwx.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xx.jctech888.com.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xx.shxzukj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jm.asd995.cn

[B03] switch / match / case
来源：http://fc.asd995.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pn.huixinmuqiang.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yt.haigaiapp.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bd.shxzskj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hl.shtwfgs.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://is.bjjhwx.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ah.szxytkj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lj.9csxet.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ip.huixinmuqiang.cn

[B04] for 计数循环
来源：http://sv.nszjky.cn

Py:   for i in range(10): print(i)
来源：http://rh.521024.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xw.yuntaijiaju.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zz.bjjhwx.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kx.panjiajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zn.szsharing.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://oa.muxihuayi.cn

Ruby: 10.times { |i| puts i }
来源：http://wl.gzmigu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://px.lnxyls.cn

[B05] 遍历数组 / 列表
来源：http://zs.shxzskj.cn

Py:   for item in arr: print(item)
来源：http://zu.shxzukj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ba.colortex.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://jz.colortex.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://km.shtwfgs.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hh.colortex.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vu.shxzskj.cn

Ruby: arr.each { |item| puts item }
来源：http://ws.muxihuayi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nr.huixiangedu.cn

[B06] 遍历字典 / 对象
来源：http://tc.hahajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qb.chemitech.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wx.muxihuayi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lf.hahajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jf.yuexingan06.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://li.newstarts.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kv.hahajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://av.wgjwhj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ri.jctech888.com.cn

[B07] while 循环
来源：http://jg.521024.cn

Py:   while i < 10: i += 1
来源：http://qs.wgjwhj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://om.huixinmuqiang.cn

JS:   while (i < 10) { i++; }
来源：http://hi.wgjwhj.cn

TS:   while (i < 10) { i++; }
来源：http://nq.yuexingan06.cn

Java: while (i < 10) { i++; }
来源：http://pi.hnjuh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vh.gzmigu.cn

Ruby: while i < 10; i += 1; end
来源：http://kz.colortex.cn

C#:   while (i < 10) { i++; }
来源：http://tu.szsharing.cn

[B08] do-while（至少执行一次）
来源：http://zv.jianghongdianzi.cn

Py:   # 无 do-while：用 while True + break
来源：http://tw.huixinmuqiang.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://no.jctech888.com.cn

JS:   do { i++; } while (i < 10);
来源：http://xm.wgjwhj.cn

TS:   do { i++; } while (i < 10);
来源：http://ki.bjjhwx.cn

Java: do { i++; } while (i < 10);
来源：http://lt.hnjuh.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sk.panjiajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://bi.bookmarksfly.cn

C#:   do { i++; } while (i < 10);
来源：http://hk.szsharing.cn

[B09] break 与 continue
来源：http://nr.colortex.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pz.yuexingan06.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ru.haigaiapp.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bn.nicolike.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://za.szxytkj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tu.szsharing.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mj.jianghongdianzi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ou.hahajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ye.shtwfgs.cn

[B10] 遍历同时拿索引
来源：http://yz.haigaiapp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zv.gzmigu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ij.colortex.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ox.hahajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qr.huanxung.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wx.521024.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yz.bjjhwx.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://np.hahajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zb.jctech888.com.cn

[B11] 生成数字序列 / 区间
来源：http://lc.panjiajie.cn

Py:   list(range(0, 10, 2))
来源：http://xg.jctech888.com.cn

PHP:  range(0, 10, 2);
来源：http://kv.hahajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zw.jianghongdianzi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cn.lnxyls.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uz.newstarts.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cb.nicolike.cn

Ruby: (0...10).step(2).to_a
来源：http://ep.hnjuh.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gr.521024.cn

[B12] 跳出多层循环
来源：http://lb.lnxyls.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ms.szsharing.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mx.jctech888.com.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ki.huanxung.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qv.bookmarksfly.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gp.lnxyls.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qo.panjiajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qf.panjiajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ul.asd995.cn

[B13] 判断是否为数字
来源：http://dh.szsharing.cn

Py:   isinstance(x, (int, float))
来源：http://id.chemitech.net.cn

PHP:  is_numeric($x)
来源：http://zc.muxihuayi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oj.jianghongdianzi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vj.huixinmuqiang.cn

Java: x instanceof Number
来源：http://re.newstarts.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zw.huanxung.cn

Ruby: x.is_a?(Numeric)
来源：http://ql.shtwfgs.cn

C#:   x is int or double or decimal
来源：http://dc.hahajie.cn

[B14] 判断值是否在集合内
来源：http://wv.huixiangedu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zu.hnjuh.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mm.jianghongdianzi.cn

JS:   [1, 2, 3].includes(x)
来源：http://dt.bjjhwx.cn

TS:   [1, 2, 3].includes(x)
来源：http://co.asd995.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ah.colortex.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fq.bjjhwx.cn

Ruby: [1, 2, 3].include?(x)
来源：http://sz.huixinmuqiang.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dm.9csxet.cn

[B15] 布尔运算与取反
来源：http://oz.asd995.cn

Py:   a and b or not c
来源：http://eb.muxihuayi.cn

PHP:  $a && $b || !$c
来源：http://en.bjjhwx.cn

JS:   a && b || !c
来源：http://fi.shxzukj.cn

TS:   a && b || !c
来源：http://pk.wgjwhj.cn

Java: a && b || !c
来源：http://hf.shtwfgs.cn

Go:   a && b || !c
来源：http://en.shxzskj.cn

Ruby: a && b || !c
来源：http://sx.9csxet.cn

C#:   a && b || !c
来源：http://or.chemitech.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hw.yuntaijiaju.cn

Py:   if not data: return
来源：http://sw.jianghongdianzi.cn

PHP:  if (!$data) { return; }
来源：http://oc.shxzskj.cn

JS:   if (!data) return;
来源：http://rw.lnxyls.cn

TS:   if (!data) return;
来源：http://ee.asd995.cn

Java: if (data == null) return;
来源：http://cq.9csxet.cn

Go:   if data == nil { return }
来源：http://mk.9csxet.cn

Ruby: return if data.nil?
来源：http://ki.nicolike.cn

C#:   if (data == null) return;
来源：http://sb.shxzskj.cn

================================================================================
来源：http://oj.newstarts.cn

C. 函数与作用域
来源：http://yr.9csxet.cn

================================================================================
来源：http://yr.nicolike.cn

[C01] 定义函数
来源：http://az.jctech888.com.cn

Py:   def add(a, b): return a + b
来源：http://ea.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mr.colortex.cn

JS:   function add(a, b) { return a + b; }
来源：http://em.huixinmuqiang.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://me.nszjky.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://cw.shtwfgs.cn

Go:   func add(a, b int) int { return a + b }
来源：http://uj.shtwfgs.cn

Ruby: def add(a, b); a + b; end
来源：http://xx.9csxet.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ga.shxzskj.cn

[C02] 默认参数
来源：http://nu.jctech888.com.cn

Py:   def greet(name="World"): return name
来源：http://gu.nszjky.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://gv.shtwfgs.cn

JS:   function greet(name = "World") { return name; }
来源：http://gy.panjiajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hr.hnjuh.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dk.nszjky.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://it.gzmigu.cn

Ruby: def greet(name = "World") = name
来源：http://ut.huixinmuqiang.cn

C#:   string Greet(string name = "World") => name;
来源：http://ax.colortex.cn

[C03] 可变参数
来源：http://pb.shxzukj.cn

Py:   def total(*args): return sum(args)
来源：http://yb.shxzukj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vi.yuntaijiaju.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rh.chemitech.net.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zo.jctech888.com.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ig.hahajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://oq.muxihuayi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://df.huixiangedu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bl.wgjwhj.cn

[C04] 命名参数 / 关键字参数
来源：http://ua.nszjky.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mj.yuntaijiaju.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tu.9csxet.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gz.hnjuh.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jk.wgjwhj.cn

Java: // 无：用 Builder 模式或 record
来源：http://zr.huixinmuqiang.cn

Go:   // 无：用配置结构体参数
来源：http://bp.panjiajie.cn

Ruby: f(a: 1, b: 2)
来源：http://fs.jctech888.com.cn

C#:   f(a: 1, b: 2)
来源：http://qj.colortex.cn

[C05] 返回多个值
来源：http://lz.newstarts.cn

Py:   return a, b
来源：http://sh.huanxung.cn

PHP:  return [$a, $b];
来源：http://wh.yuexingan06.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ke.huanxung.cn

TS:   return { a, b };
来源：http://uq.lnxyls.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nf.hnjuh.cn

Go:   return a, b
来源：http://eb.asd995.cn

Ruby: return a, b
来源：http://di.szsharing.cn

C#:   return (a, b);              // ValueTuple
来源：http://yq.521024.cn

[C06] 匿名函数 / lambda
来源：http://nb.szxytkj.cn

Py:   square = lambda x: x * x
来源：http://zt.szsharing.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://nc.gzmigu.cn

JS:   const square = x => x * x;
来源：http://cg.hnjuh.cn

TS:   const square = (x: number): number => x * x;
来源：http://ev.chemitech.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://px.wgjwhj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://na.shxzskj.cn

Ruby: square = ->(x) { x * x }
来源：http://il.jctech888.com.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ow.bjjhwx.cn

[C07] 把函数作为参数传入
来源：http://df.nszjky.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tb.shxzukj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xn.hnjuh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pe.nszjky.cn

TS:   arr.map(String)
来源：http://pd.szsharing.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://eh.yuntaijiaju.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ik.huanxung.cn

Ruby: arr.map(&:upcase)
来源：http://vn.chemitech.net.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://io.huanxung.cn

[C08] 闭包
来源：http://pr.huixiangedu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ic.jctech888.com.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ah.shtwfgs.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xs.haigaiapp.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://iq.jianghongdianzi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xk.hnjuh.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pc.panjiajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jq.chemitech.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://la.9csxet.cn

[C09] 递归
来源：http://ys.9csxet.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://iq.hnjuh.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xh.lnxyls.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zg.jianghongdianzi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ui.asd995.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ni.wgjwhj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qx.wgjwhj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://up.bjjhwx.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rc.9csxet.cn

[C10] 变量作用域
来源：http://vi.huixiangedu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xj.muxihuayi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ym.chemitech.net.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sj.jctech888.com.cn

TS:   同 JS
来源：http://ua.9csxet.cn

Java: 方法内为块级作用域
来源：http://zt.jianghongdianzi.cn

Go:   花括号块级作用域
来源：http://au.huanxung.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ha.wgjwhj.cn

C#:   块级作用域
来源：http://jk.yuexingan06.cn

[C11] 模块导入与导出
来源：http://rb.huanxung.cn

Py:   from module import func
来源：http://ke.nszjky.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hr.wgjwhj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ud.shtwfgs.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zn.lnxyls.cn

Java: import java.util.List;
来源：http://ve.gzmigu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://it.shxzukj.cn

Ruby: require "json"; require_relative "./util"
来源：http://wx.nszjky.cn

C#:   using System.Text;
来源：http://vr.yuntaijiaju.cn

[C12] 立即执行函数 IIFE
来源：http://ff.huixinmuqiang.cn

Py:   (lambda: print("run"))()
来源：http://ji.gzmigu.cn


<!-- 参考信息 -->