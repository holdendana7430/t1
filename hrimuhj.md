代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zm.nicolike.cn

Ruby: gets.chomp
来源：http://ao.muxihuayi.cn

C#:   Console.ReadLine();
来源：http://ah.bjjhwx.cn

[A21] 保留指定小数位输出
来源：http://xm.bookmarksfly.cn

Py:   f"{3.14159:.2f}"
来源：http://sd.panjiajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dp.chemitech.net.cn

JS:   (3.14159).toFixed(2)
来源：http://ra.szsharing.cn

TS:   (3.14159).toFixed(2)
来源：http://rz.nicolike.cn

Java: String.format("%.2f", 3.14159)
来源：http://ao.shtwfgs.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qk.shxzskj.cn

Ruby: format("%.2f", 3.14159)
来源：http://ph.lnxyls.cn

C#:   3.14159.ToString("F2")
来源：http://vm.521024.cn

[A22] 获取字符串长度
来源：http://ax.jctech888.com.cn

Py:   len(s)
来源：http://el.huixiangedu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mx.nicolike.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://oe.huixinmuqiang.cn

TS:   s.length
来源：http://is.9csxet.cn

Java: s.length()
来源：http://em.shxzskj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ye.shtwfgs.cn

Ruby: s.length
来源：http://jh.haigaiapp.cn

C#:   s.Length
来源：http://jt.jianghongdianzi.cn

[A23] 大小写转换
来源：http://bz.hahajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ms.yuntaijiaju.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://iq.jianghongdianzi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bj.hahajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gg.shxzukj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kr.asd995.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pp.gzmigu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zt.jianghongdianzi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qw.muxihuayi.cn

[A24] 去除首尾空白
来源：http://my.huixiangedu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jw.asd995.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://er.yuexingan06.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vl.9csxet.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eq.hnjuh.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ts.yuexingan06.cn

Go:   strings.TrimSpace(s)
来源：http://jc.shxzskj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ki.shtwfgs.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rr.jianghongdianzi.cn

[A25] 字符串比较
来源：http://bt.szxytkj.cn

Py:   s1 == s2; s1 != s2
来源：http://yb.bjjhwx.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rq.9csxet.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ki.gzmigu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nc.yuexingan06.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://am.nicolike.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ue.huanxung.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://uf.huanxung.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zo.colortex.cn

[A26] 类型转换总览
来源：http://bc.jianghongdianzi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ce.colortex.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jk.szsharing.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://lh.hnjuh.cn

TS:   Number() String() Boolean() x as number
来源：http://ju.asd995.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ar.haigaiapp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://uu.shxzskj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ce.muxihuayi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gd.huixiangedu.cn

================================================================================
来源：http://ic.newstarts.cn

B. 流程控制
来源：http://we.chemitech.net.cn

================================================================================
来源：http://oo.9csxet.cn

[B01] 条件判断 if / else
来源：http://br.hnjuh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://yk.shxzskj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yh.wgjwhj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cc.asd995.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bg.521024.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://cx.shtwfgs.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://na.yuexingan06.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vq.haigaiapp.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://st.colortex.cn

[B02] 多分支 else if / elif
来源：http://fr.gzmigu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ax.bookmarksfly.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zf.szxytkj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rk.521024.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ll.chemitech.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ri.szxytkj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zw.asd995.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nw.yuexingan06.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kn.gzmigu.cn

[B03] switch / match / case
来源：http://sk.hnjuh.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sp.colortex.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sa.521024.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hd.colortex.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ri.huixinmuqiang.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://co.muxihuayi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rt.chemitech.net.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://af.colortex.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gp.huixiangedu.cn

[B04] for 计数循环
来源：http://ji.huixiangedu.cn

Py:   for i in range(10): print(i)
来源：http://bw.haigaiapp.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rh.newstarts.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lb.huixinmuqiang.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hn.yuntaijiaju.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mv.huixinmuqiang.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rj.521024.cn

Ruby: 10.times { |i| puts i }
来源：http://er.yuntaijiaju.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://um.newstarts.cn

[B05] 遍历数组 / 列表
来源：http://ff.panjiajie.cn

Py:   for item in arr: print(item)
来源：http://nk.shxzukj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yn.wgjwhj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://my.muxihuayi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tl.yuexingan06.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hv.yuntaijiaju.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qq.9csxet.cn

Ruby: arr.each { |item| puts item }
来源：http://dp.bjjhwx.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ke.chemitech.net.cn

[B06] 遍历字典 / 对象
来源：http://ep.colortex.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ez.gzmigu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rb.wgjwhj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qu.szsharing.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pv.huixinmuqiang.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gk.shxzskj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mf.yuntaijiaju.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ol.shxzukj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gt.szsharing.cn

[B07] while 循环
来源：http://sn.wgjwhj.cn

Py:   while i < 10: i += 1
来源：http://cg.wgjwhj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ca.lnxyls.cn

JS:   while (i < 10) { i++; }
来源：http://ri.yuntaijiaju.cn

TS:   while (i < 10) { i++; }
来源：http://jr.nszjky.cn

Java: while (i < 10) { i++; }
来源：http://kn.newstarts.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cp.gzmigu.cn

Ruby: while i < 10; i += 1; end
来源：http://kn.nicolike.cn

C#:   while (i < 10) { i++; }
来源：http://ns.chemitech.net.cn

[B08] do-while（至少执行一次）
来源：http://ie.colortex.cn

Py:   # 无 do-while：用 while True + break
来源：http://pt.bookmarksfly.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://eg.521024.cn

JS:   do { i++; } while (i < 10);
来源：http://yo.hahajie.cn

TS:   do { i++; } while (i < 10);
来源：http://mx.panjiajie.cn

Java: do { i++; } while (i < 10);
来源：http://ex.colortex.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jv.hahajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://yu.jctech888.com.cn

C#:   do { i++; } while (i < 10);
来源：http://eu.nicolike.cn

[B09] break 与 continue
来源：http://dm.szsharing.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sg.huanxung.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pg.yuntaijiaju.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lu.panjiajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xg.bookmarksfly.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fc.jctech888.com.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fq.hnjuh.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ok.gzmigu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wi.wgjwhj.cn

[B10] 遍历同时拿索引
来源：http://qn.yuexingan06.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jw.shtwfgs.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mx.muxihuayi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ya.szxytkj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://iw.shxzukj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zj.yuntaijiaju.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://in.haigaiapp.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nx.szsharing.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ob.nicolike.cn

[B11] 生成数字序列 / 区间
来源：http://qv.shxzskj.cn

Py:   list(range(0, 10, 2))
来源：http://kj.chemitech.net.cn

PHP:  range(0, 10, 2);
来源：http://ez.shxzskj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://db.bjjhwx.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://se.lnxyls.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nt.szsharing.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://us.hnjuh.cn

Ruby: (0...10).step(2).to_a
来源：http://sz.chemitech.net.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.gzmigu.cn

[B12] 跳出多层循环
来源：http://iw.jctech888.com.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zm.newstarts.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://lw.colortex.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sd.huixinmuqiang.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kg.szsharing.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://db.hahajie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qq.shxzukj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://na.hnjuh.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pw.panjiajie.cn

[B13] 判断是否为数字
来源：http://tn.lnxyls.cn

Py:   isinstance(x, (int, float))
来源：http://nb.9csxet.cn

PHP:  is_numeric($x)
来源：http://xp.newstarts.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vw.shtwfgs.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://me.gzmigu.cn

Java: x instanceof Number
来源：http://dr.bookmarksfly.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hn.gzmigu.cn

Ruby: x.is_a?(Numeric)
来源：http://iq.muxihuayi.cn

C#:   x is int or double or decimal
来源：http://dr.yuntaijiaju.cn

[B14] 判断值是否在集合内
来源：http://zv.yuntaijiaju.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cu.shxzukj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bw.bookmarksfly.cn

JS:   [1, 2, 3].includes(x)
来源：http://jb.muxihuayi.cn

TS:   [1, 2, 3].includes(x)
来源：http://nl.521024.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rp.jctech888.com.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lz.hnjuh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vi.newstarts.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://er.szxytkj.cn

[B15] 布尔运算与取反
来源：http://di.szxytkj.cn

Py:   a and b or not c
来源：http://ck.jctech888.com.cn

PHP:  $a && $b || !$c
来源：http://bb.huixinmuqiang.cn

JS:   a && b || !c
来源：http://rz.shtwfgs.cn

TS:   a && b || !c
来源：http://kf.shtwfgs.cn

Java: a && b || !c
来源：http://vz.yuntaijiaju.cn

Go:   a && b || !c
来源：http://pl.panjiajie.cn

Ruby: a && b || !c
来源：http://uh.shxzukj.cn

C#:   a && b || !c
来源：http://bl.huanxung.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zf.huanxung.cn

Py:   if not data: return
来源：http://ig.hahajie.cn

PHP:  if (!$data) { return; }
来源：http://ft.bookmarksfly.cn

JS:   if (!data) return;
来源：http://vs.shxzukj.cn

TS:   if (!data) return;
来源：http://td.asd995.cn

Java: if (data == null) return;
来源：http://ae.jctech888.com.cn

Go:   if data == nil { return }
来源：http://ly.jianghongdianzi.cn

Ruby: return if data.nil?
来源：http://uw.szxytkj.cn

C#:   if (data == null) return;
来源：http://jp.chemitech.net.cn

================================================================================
来源：http://az.huanxung.cn

C. 函数与作用域
来源：http://tq.haigaiapp.cn

================================================================================
来源：http://su.huixiangedu.cn

[C01] 定义函数
来源：http://qj.asd995.cn

Py:   def add(a, b): return a + b
来源：http://dl.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fr.shxzskj.cn

JS:   function add(a, b) { return a + b; }
来源：http://sz.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jz.nicolike.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://sf.wgjwhj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://bd.shtwfgs.cn

Ruby: def add(a, b); a + b; end
来源：http://ra.shxzukj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ja.hahajie.cn

[C02] 默认参数
来源：http://ty.asd995.cn

Py:   def greet(name="World"): return name
来源：http://ld.panjiajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://te.jctech888.com.cn

JS:   function greet(name = "World") { return name; }
来源：http://ya.wgjwhj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yu.shxzukj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ve.nicolike.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://br.panjiajie.cn

Ruby: def greet(name = "World") = name
来源：http://uh.bookmarksfly.cn

C#:   string Greet(string name = "World") => name;
来源：http://tn.szxytkj.cn

[C03] 可变参数
来源：http://oh.lnxyls.cn

Py:   def total(*args): return sum(args)
来源：http://wd.colortex.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ki.yuexingan06.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://al.szsharing.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hd.yuntaijiaju.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zx.bookmarksfly.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wz.newstarts.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ml.szsharing.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dx.521024.cn

[C04] 命名参数 / 关键字参数
来源：http://bc.szsharing.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://km.newstarts.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xw.newstarts.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://go.nszjky.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qa.jianghongdianzi.cn

Java: // 无：用 Builder 模式或 record
来源：http://qc.colortex.cn

Go:   // 无：用配置结构体参数
来源：http://xq.newstarts.cn

Ruby: f(a: 1, b: 2)
来源：http://qg.nszjky.cn

C#:   f(a: 1, b: 2)
来源：http://vs.huanxung.cn

[C05] 返回多个值
来源：http://hc.wgjwhj.cn

Py:   return a, b
来源：http://sw.lnxyls.cn

PHP:  return [$a, $b];
来源：http://qq.chemitech.net.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://kl.bookmarksfly.cn

TS:   return { a, b };
来源：http://fm.yuexingan06.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zc.yuexingan06.cn

Go:   return a, b
来源：http://eu.nszjky.cn

Ruby: return a, b
来源：http://yo.muxihuayi.cn

C#:   return (a, b);              // ValueTuple
来源：http://zd.hahajie.cn

[C06] 匿名函数 / lambda
来源：http://pi.9csxet.cn

Py:   square = lambda x: x * x
来源：http://qy.szsharing.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://yn.wgjwhj.cn

JS:   const square = x => x * x;
来源：http://ns.szsharing.cn

TS:   const square = (x: number): number => x * x;
来源：http://fb.chemitech.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://uv.shxzukj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hf.521024.cn

Ruby: square = ->(x) { x * x }
来源：http://vb.hahajie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://um.huixiangedu.cn

[C07] 把函数作为参数传入
来源：http://ad.bookmarksfly.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yz.yuntaijiaju.cn

PHP:  array_map("strtoupper", $arr);
来源：http://tn.lnxyls.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xy.wgjwhj.cn

TS:   arr.map(String)
来源：http://ka.nszjky.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jf.szsharing.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sl.haigaiapp.cn

Ruby: arr.map(&:upcase)
来源：http://hh.szxytkj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://vo.gzmigu.cn

[C08] 闭包
来源：http://bc.newstarts.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ah.huixiangedu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wu.wgjwhj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mn.bjjhwx.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qq.hahajie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ah.9csxet.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hv.szxytkj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bs.jctech888.com.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ib.chemitech.net.cn

[C09] 递归
来源：http://at.nicolike.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gn.lnxyls.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qh.lnxyls.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cy.colortex.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fo.huixinmuqiang.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vc.gzmigu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ot.huanxung.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://og.jianghongdianzi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ll.lnxyls.cn

[C10] 变量作用域
来源：http://bp.yuexingan06.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://uq.shtwfgs.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ra.jianghongdianzi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://le.bookmarksfly.cn

TS:   同 JS
来源：http://kh.521024.cn

Java: 方法内为块级作用域
来源：http://qb.hahajie.cn

Go:   花括号块级作用域
来源：http://vy.panjiajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fx.shtwfgs.cn

C#:   块级作用域
来源：http://ow.yuexingan06.cn

[C11] 模块导入与导出
来源：http://jg.bookmarksfly.cn

Py:   from module import func
来源：http://ls.colortex.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zn.shxzukj.cn


<!-- 参考信息 -->