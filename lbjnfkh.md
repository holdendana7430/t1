代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pc.muxihuayi.cn

Ruby: gets.chomp
来源：http://qu.yuntaijiaju.cn

C#:   Console.ReadLine();
来源：http://gq.yuexingan06.cn

[A21] 保留指定小数位输出
来源：http://kf.shxzukj.cn

Py:   f"{3.14159:.2f}"
来源：http://ll.chemitech.net.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fp.lnxyls.cn

JS:   (3.14159).toFixed(2)
来源：http://wu.asd995.cn

TS:   (3.14159).toFixed(2)
来源：http://nw.shxzukj.cn

Java: String.format("%.2f", 3.14159)
来源：http://oz.shtwfgs.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tk.huanxung.cn

Ruby: format("%.2f", 3.14159)
来源：http://eu.yuntaijiaju.cn

C#:   3.14159.ToString("F2")
来源：http://ww.wgjwhj.cn

[A22] 获取字符串长度
来源：http://gm.shxzukj.cn

Py:   len(s)
来源：http://az.huixiangedu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dz.9csxet.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cg.yuntaijiaju.cn

TS:   s.length
来源：http://gl.colortex.cn

Java: s.length()
来源：http://pv.huanxung.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://at.lnxyls.cn

Ruby: s.length
来源：http://rw.jianghongdianzi.cn

C#:   s.Length
来源：http://ir.shtwfgs.cn

[A23] 大小写转换
来源：http://pb.panjiajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ic.shtwfgs.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://im.nicolike.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ma.nszjky.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yi.muxihuayi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://em.huanxung.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mv.lnxyls.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mv.9csxet.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://dl.yuexingan06.cn

[A24] 去除首尾空白
来源：http://oi.hahajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cc.yuexingan06.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cj.9csxet.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qa.bjjhwx.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hl.huanxung.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fn.nszjky.cn

Go:   strings.TrimSpace(s)
来源：http://qu.shxzukj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rb.bookmarksfly.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sy.huixinmuqiang.cn

[A25] 字符串比较
来源：http://zn.jctech888.com.cn

Py:   s1 == s2; s1 != s2
来源：http://it.bookmarksfly.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ou.huixinmuqiang.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tq.huixiangedu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gp.lnxyls.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rv.bjjhwx.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xf.nicolike.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://bs.hahajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rm.yuexingan06.cn

[A26] 类型转换总览
来源：http://ta.shxzukj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cs.shxzskj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vp.hahajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vh.hahajie.cn

TS:   Number() String() Boolean() x as number
来源：http://wm.9csxet.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nr.jianghongdianzi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nk.bookmarksfly.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://it.colortex.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lz.521024.cn

================================================================================
来源：http://sh.colortex.cn

B. 流程控制
来源：http://sx.chemitech.net.cn

================================================================================
来源：http://ur.haigaiapp.cn

[B01] 条件判断 if / else
来源：http://qk.gzmigu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://if.yuntaijiaju.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gg.jianghongdianzi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kl.nszjky.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ho.lnxyls.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://uj.gzmigu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://in.lnxyls.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gc.colortex.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cw.colortex.cn

[B02] 多分支 else if / elif
来源：http://jv.colortex.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ng.shtwfgs.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lu.huixinmuqiang.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kw.jianghongdianzi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ob.hnjuh.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fr.huixiangedu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ij.hahajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yd.chemitech.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://el.hahajie.cn

[B03] switch / match / case
来源：http://ec.nicolike.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vb.huixinmuqiang.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vd.muxihuayi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wu.bjjhwx.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uv.yuntaijiaju.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zd.nicolike.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dh.bookmarksfly.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yc.jctech888.com.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://em.shxzskj.cn

[B04] for 计数循环
来源：http://cm.huixinmuqiang.cn

Py:   for i in range(10): print(i)
来源：http://it.shxzukj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lh.521024.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ya.haigaiapp.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rf.shxzukj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ix.asd995.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://iy.shxzskj.cn

Ruby: 10.times { |i| puts i }
来源：http://zl.nicolike.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rb.yuexingan06.cn

[B05] 遍历数组 / 列表
来源：http://gm.huixiangedu.cn

Py:   for item in arr: print(item)
来源：http://oj.jianghongdianzi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://te.shtwfgs.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://bn.muxihuayi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://nv.yuntaijiaju.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hk.yuntaijiaju.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dm.szxytkj.cn

Ruby: arr.each { |item| puts item }
来源：http://wc.nszjky.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sk.shxzukj.cn

[B06] 遍历字典 / 对象
来源：http://wk.muxihuayi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://lf.muxihuayi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://it.yuexingan06.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mf.szxytkj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qb.huanxung.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wt.hnjuh.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ta.hahajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vy.haigaiapp.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vk.muxihuayi.cn

[B07] while 循环
来源：http://rs.yuntaijiaju.cn

Py:   while i < 10: i += 1
来源：http://ma.yuntaijiaju.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vc.hnjuh.cn

JS:   while (i < 10) { i++; }
来源：http://et.shxzukj.cn

TS:   while (i < 10) { i++; }
来源：http://og.lnxyls.cn

Java: while (i < 10) { i++; }
来源：http://rp.panjiajie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mu.shxzskj.cn

Ruby: while i < 10; i += 1; end
来源：http://bl.bookmarksfly.cn

C#:   while (i < 10) { i++; }
来源：http://yc.panjiajie.cn

[B08] do-while（至少执行一次）
来源：http://ya.panjiajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://yy.hahajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://oe.bookmarksfly.cn

JS:   do { i++; } while (i < 10);
来源：http://sd.huixiangedu.cn

TS:   do { i++; } while (i < 10);
来源：http://uo.shtwfgs.cn

Java: do { i++; } while (i < 10);
来源：http://fw.hnjuh.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://hi.newstarts.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ms.hahajie.cn

C#:   do { i++; } while (i < 10);
来源：http://wn.jianghongdianzi.cn

[B09] break 与 continue
来源：http://ke.shtwfgs.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qz.hnjuh.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gb.huixiangedu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://so.bjjhwx.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ll.szsharing.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uz.shxzskj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zf.muxihuayi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zv.jianghongdianzi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pj.colortex.cn

[B10] 遍历同时拿索引
来源：http://tc.szxytkj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fm.huixinmuqiang.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dx.szxytkj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mq.lnxyls.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ar.chemitech.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ja.nicolike.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sl.huixiangedu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qe.muxihuayi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jl.panjiajie.cn

[B11] 生成数字序列 / 区间
来源：http://dj.shxzskj.cn

Py:   list(range(0, 10, 2))
来源：http://zz.haigaiapp.cn

PHP:  range(0, 10, 2);
来源：http://km.wgjwhj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yk.521024.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cl.gzmigu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zg.yuntaijiaju.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yf.9csxet.cn

Ruby: (0...10).step(2).to_a
来源：http://bw.szsharing.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gg.colortex.cn

[B12] 跳出多层循环
来源：http://ag.bookmarksfly.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://cf.panjiajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://eb.gzmigu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hc.shtwfgs.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bg.bjjhwx.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ik.9csxet.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mx.szxytkj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fq.haigaiapp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fk.huixinmuqiang.cn

[B13] 判断是否为数字
来源：http://gu.haigaiapp.cn

Py:   isinstance(x, (int, float))
来源：http://sn.hahajie.cn

PHP:  is_numeric($x)
来源：http://fm.colortex.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ac.9csxet.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bx.nicolike.cn

Java: x instanceof Number
来源：http://dt.bjjhwx.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kr.bookmarksfly.cn

Ruby: x.is_a?(Numeric)
来源：http://ms.nszjky.cn

C#:   x is int or double or decimal
来源：http://uq.yuntaijiaju.cn

[B14] 判断值是否在集合内
来源：http://vl.colortex.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fw.shxzskj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oc.bookmarksfly.cn

JS:   [1, 2, 3].includes(x)
来源：http://fd.jctech888.com.cn

TS:   [1, 2, 3].includes(x)
来源：http://um.wgjwhj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qh.521024.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://oo.shxzskj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://dt.chemitech.net.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vn.shxzukj.cn

[B15] 布尔运算与取反
来源：http://yj.huanxung.cn

Py:   a and b or not c
来源：http://xw.jianghongdianzi.cn

PHP:  $a && $b || !$c
来源：http://gf.jianghongdianzi.cn

JS:   a && b || !c
来源：http://hj.bjjhwx.cn

TS:   a && b || !c
来源：http://gj.colortex.cn

Java: a && b || !c
来源：http://ox.colortex.cn

Go:   a && b || !c
来源：http://wd.chemitech.net.cn

Ruby: a && b || !c
来源：http://xl.521024.cn

C#:   a && b || !c
来源：http://vw.panjiajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ss.chemitech.net.cn

Py:   if not data: return
来源：http://wf.huixiangedu.cn

PHP:  if (!$data) { return; }
来源：http://ia.panjiajie.cn

JS:   if (!data) return;
来源：http://ak.bjjhwx.cn

TS:   if (!data) return;
来源：http://wr.huanxung.cn

Java: if (data == null) return;
来源：http://mt.szxytkj.cn

Go:   if data == nil { return }
来源：http://sg.colortex.cn

Ruby: return if data.nil?
来源：http://cl.newstarts.cn

C#:   if (data == null) return;
来源：http://nd.shxzskj.cn

================================================================================
来源：http://qo.haigaiapp.cn

C. 函数与作用域
来源：http://kw.9csxet.cn

================================================================================
来源：http://jk.szsharing.cn

[C01] 定义函数
来源：http://ij.jctech888.com.cn

Py:   def add(a, b): return a + b
来源：http://mc.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qu.9csxet.cn

JS:   function add(a, b) { return a + b; }
来源：http://uh.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lu.shtwfgs.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ly.newstarts.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vn.szsharing.cn

Ruby: def add(a, b); a + b; end
来源：http://at.muxihuayi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jh.newstarts.cn

[C02] 默认参数
来源：http://ju.asd995.cn

Py:   def greet(name="World"): return name
来源：http://om.huanxung.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://kk.bookmarksfly.cn

JS:   function greet(name = "World") { return name; }
来源：http://ig.colortex.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://eb.huixinmuqiang.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qi.jctech888.com.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vp.521024.cn

Ruby: def greet(name = "World") = name
来源：http://ca.muxihuayi.cn

C#:   string Greet(string name = "World") => name;
来源：http://al.nicolike.cn

[C03] 可变参数
来源：http://fw.asd995.cn

Py:   def total(*args): return sum(args)
来源：http://zs.asd995.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://og.asd995.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://da.nicolike.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://my.muxihuayi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gj.yuntaijiaju.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rn.bookmarksfly.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hl.szsharing.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lu.lnxyls.cn

[C04] 命名参数 / 关键字参数
来源：http://zb.yuexingan06.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://un.huanxung.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yc.9csxet.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uo.szxytkj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qr.gzmigu.cn

Java: // 无：用 Builder 模式或 record
来源：http://gn.lnxyls.cn

Go:   // 无：用配置结构体参数
来源：http://lz.nszjky.cn

Ruby: f(a: 1, b: 2)
来源：http://uy.nicolike.cn

C#:   f(a: 1, b: 2)
来源：http://ny.shtwfgs.cn

[C05] 返回多个值
来源：http://xp.huixinmuqiang.cn

Py:   return a, b
来源：http://ab.shxzukj.cn

PHP:  return [$a, $b];
来源：http://wc.yuntaijiaju.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://gx.hahajie.cn

TS:   return { a, b };
来源：http://du.521024.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rq.bjjhwx.cn

Go:   return a, b
来源：http://al.shxzukj.cn

Ruby: return a, b
来源：http://bt.haigaiapp.cn

C#:   return (a, b);              // ValueTuple
来源：http://dh.huixinmuqiang.cn

[C06] 匿名函数 / lambda
来源：http://ft.shtwfgs.cn

Py:   square = lambda x: x * x
来源：http://ns.szxytkj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fq.yuntaijiaju.cn

JS:   const square = x => x * x;
来源：http://bc.yuntaijiaju.cn

TS:   const square = (x: number): number => x * x;
来源：http://ag.jianghongdianzi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ct.nicolike.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ie.chemitech.net.cn

Ruby: square = ->(x) { x * x }
来源：http://ob.huixiangedu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dg.nicolike.cn

[C07] 把函数作为参数传入
来源：http://bb.chemitech.net.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yw.newstarts.cn

PHP:  array_map("strtoupper", $arr);
来源：http://pi.nszjky.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rf.szxytkj.cn

TS:   arr.map(String)
来源：http://qy.9csxet.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://id.shtwfgs.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sw.yuntaijiaju.cn

Ruby: arr.map(&:upcase)
来源：http://kx.jctech888.com.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://yj.lnxyls.cn

[C08] 闭包
来源：http://sx.nicolike.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pe.newstarts.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gt.wgjwhj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uu.bookmarksfly.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ph.chemitech.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uf.chemitech.net.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dj.yuexingan06.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lu.colortex.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lm.haigaiapp.cn

[C09] 递归
来源：http://aa.shxzukj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uy.chemitech.net.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://oh.asd995.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jf.shxzukj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jr.colortex.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ss.wgjwhj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vp.yuntaijiaju.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uv.jianghongdianzi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hh.gzmigu.cn

[C10] 变量作用域
来源：http://mr.lnxyls.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rv.newstarts.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tw.wgjwhj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pt.huixinmuqiang.cn

TS:   同 JS
来源：http://er.colortex.cn

Java: 方法内为块级作用域
来源：http://dm.chemitech.net.cn

Go:   花括号块级作用域
来源：http://hi.jianghongdianzi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://oo.jctech888.com.cn

C#:   块级作用域
来源：http://vi.jianghongdianzi.cn

[C11] 模块导入与导出
来源：http://md.huixiangedu.cn

Py:   from module import func
来源：http://lq.huanxung.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://uh.yuexingan06.cn


<!-- 参考信息 -->