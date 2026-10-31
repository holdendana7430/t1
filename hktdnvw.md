代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://im.yuntaijiaju.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kw.bookmarksfly.cn

Ruby: format("%.2f", 3.14159)
来源：http://ke.muxihuayi.cn

C#:   3.14159.ToString("F2")
来源：http://jv.muxihuayi.cn

[A22] 获取字符串长度
来源：http://bx.asd995.cn

Py:   len(s)
来源：http://cp.shxzskj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zc.yuntaijiaju.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://if.haigaiapp.cn

TS:   s.length
来源：http://wz.lnxyls.cn

Java: s.length()
来源：http://np.yuexingan06.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mm.shxzskj.cn

Ruby: s.length
来源：http://va.jctech888.com.cn

C#:   s.Length
来源：http://kh.yuexingan06.cn

[A23] 大小写转换
来源：http://ov.jianghongdianzi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ef.hahajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://tk.chemitech.net.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vl.muxihuayi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hg.gzmigu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://sg.jctech888.com.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hd.asd995.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hg.yuexingan06.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://hb.bookmarksfly.cn

[A24] 去除首尾空白
来源：http://ad.huanxung.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ex.muxihuayi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pn.shxzukj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bu.gzmigu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hn.muxihuayi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jo.colortex.cn

Go:   strings.TrimSpace(s)
来源：http://ss.jianghongdianzi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://eu.jianghongdianzi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://od.huixinmuqiang.cn

[A25] 字符串比较
来源：http://fg.bjjhwx.cn

Py:   s1 == s2; s1 != s2
来源：http://xc.wgjwhj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hd.wgjwhj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gp.hnjuh.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ig.shxzskj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vr.szsharing.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ah.jianghongdianzi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://us.shtwfgs.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gg.huixinmuqiang.cn

[A26] 类型转换总览
来源：http://kd.hnjuh.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vm.yuntaijiaju.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uz.bjjhwx.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gp.521024.cn

TS:   Number() String() Boolean() x as number
来源：http://zd.nszjky.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vs.gzmigu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fx.jctech888.com.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://yi.huixiangedu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://df.panjiajie.cn

================================================================================
来源：http://tk.shxzukj.cn

B. 流程控制
来源：http://cr.szxytkj.cn

================================================================================
来源：http://nl.9csxet.cn

[B01] 条件判断 if / else
来源：http://ob.shxzskj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://zi.yuexingan06.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://uz.shtwfgs.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kx.nszjky.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qn.yuntaijiaju.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://nx.panjiajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hd.wgjwhj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zc.yuntaijiaju.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wg.yuexingan06.cn

[B02] 多分支 else if / elif
来源：http://va.521024.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://uu.nszjky.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://to.hahajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yu.newstarts.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://va.newstarts.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ph.colortex.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://st.nicolike.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ie.jianghongdianzi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yk.huixiangedu.cn

[B03] switch / match / case
来源：http://ny.newstarts.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ls.jianghongdianzi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cf.yuexingan06.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jn.muxihuayi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qw.521024.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hp.gzmigu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ux.huixinmuqiang.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pv.muxihuayi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bi.nszjky.cn

[B04] for 计数循环
来源：http://qa.gzmigu.cn

Py:   for i in range(10): print(i)
来源：http://rf.newstarts.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://eb.huixiangedu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uy.panjiajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://id.521024.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kj.huixiangedu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vh.nicolike.cn

Ruby: 10.times { |i| puts i }
来源：http://la.haigaiapp.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yk.jianghongdianzi.cn

[B05] 遍历数组 / 列表
来源：http://gh.newstarts.cn

Py:   for item in arr: print(item)
来源：http://xt.nszjky.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vx.yuexingan06.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://jl.chemitech.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://to.panjiajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://nb.nszjky.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xp.chemitech.net.cn

Ruby: arr.each { |item| puts item }
来源：http://mn.szxytkj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dq.szxytkj.cn

[B06] 遍历字典 / 对象
来源：http://er.chemitech.net.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://rt.huixinmuqiang.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mn.nszjky.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://et.nicolike.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hw.huixinmuqiang.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ke.nicolike.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ir.colortex.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ls.nicolike.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kk.colortex.cn

[B07] while 循环
来源：http://kr.chemitech.net.cn

Py:   while i < 10: i += 1
来源：http://id.wgjwhj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vk.nszjky.cn

JS:   while (i < 10) { i++; }
来源：http://nr.szsharing.cn

TS:   while (i < 10) { i++; }
来源：http://mw.chemitech.net.cn

Java: while (i < 10) { i++; }
来源：http://qs.jianghongdianzi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ix.huixiangedu.cn

Ruby: while i < 10; i += 1; end
来源：http://ev.jianghongdianzi.cn

C#:   while (i < 10) { i++; }
来源：http://dk.asd995.cn

[B08] do-while（至少执行一次）
来源：http://ay.yuexingan06.cn

Py:   # 无 do-while：用 while True + break
来源：http://xg.huanxung.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://kd.9csxet.cn

JS:   do { i++; } while (i < 10);
来源：http://iv.yuntaijiaju.cn

TS:   do { i++; } while (i < 10);
来源：http://hw.jianghongdianzi.cn

Java: do { i++; } while (i < 10);
来源：http://aa.yuexingan06.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mg.bookmarksfly.cn

Ruby: begin; i += 1; end while i < 10
来源：http://in.nszjky.cn

C#:   do { i++; } while (i < 10);
来源：http://af.panjiajie.cn

[B09] break 与 continue
来源：http://jg.jctech888.com.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jz.bjjhwx.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cc.asd995.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://il.colortex.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xo.wgjwhj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jd.bjjhwx.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hu.hahajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ot.hahajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nq.haigaiapp.cn

[B10] 遍历同时拿索引
来源：http://lm.shxzskj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ch.huixinmuqiang.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gm.shxzukj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mu.hahajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ec.9csxet.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ip.hnjuh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mk.szsharing.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fe.bjjhwx.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dl.shxzskj.cn

[B11] 生成数字序列 / 区间
来源：http://mt.szsharing.cn

Py:   list(range(0, 10, 2))
来源：http://hk.szxytkj.cn

PHP:  range(0, 10, 2);
来源：http://ne.hnjuh.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pd.hahajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fu.gzmigu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gy.asd995.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gn.jctech888.com.cn

Ruby: (0...10).step(2).to_a
来源：http://co.gzmigu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xv.panjiajie.cn

[B12] 跳出多层循环
来源：http://qz.hnjuh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pm.bookmarksfly.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fs.bookmarksfly.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ho.newstarts.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pl.bookmarksfly.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sa.huixiangedu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sj.asd995.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pi.lnxyls.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ls.nicolike.cn

[B13] 判断是否为数字
来源：http://ao.asd995.cn

Py:   isinstance(x, (int, float))
来源：http://bn.lnxyls.cn

PHP:  is_numeric($x)
来源：http://da.huanxung.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lm.yuexingan06.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iz.newstarts.cn

Java: x instanceof Number
来源：http://fk.hnjuh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://aa.nszjky.cn

Ruby: x.is_a?(Numeric)
来源：http://wk.nszjky.cn

C#:   x is int or double or decimal
来源：http://pj.nicolike.cn

[B14] 判断值是否在集合内
来源：http://ft.yuntaijiaju.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hh.bookmarksfly.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://za.huixinmuqiang.cn

JS:   [1, 2, 3].includes(x)
来源：http://st.panjiajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://cg.jctech888.com.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xf.yuexingan06.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qf.bjjhwx.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zt.hahajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ii.hnjuh.cn

[B15] 布尔运算与取反
来源：http://vd.szsharing.cn

Py:   a and b or not c
来源：http://vy.szsharing.cn

PHP:  $a && $b || !$c
来源：http://kq.wgjwhj.cn

JS:   a && b || !c
来源：http://km.nicolike.cn

TS:   a && b || !c
来源：http://rs.521024.cn

Java: a && b || !c
来源：http://qs.colortex.cn

Go:   a && b || !c
来源：http://zt.lnxyls.cn

Ruby: a && b || !c
来源：http://yp.huixinmuqiang.cn

C#:   a && b || !c
来源：http://kc.bjjhwx.cn

[B16] 卫语句：不满足条件提前返回
来源：http://sy.huanxung.cn

Py:   if not data: return
来源：http://ck.huixiangedu.cn

PHP:  if (!$data) { return; }
来源：http://fg.haigaiapp.cn

JS:   if (!data) return;
来源：http://xk.yuntaijiaju.cn

TS:   if (!data) return;
来源：http://zk.yuexingan06.cn

Java: if (data == null) return;
来源：http://no.colortex.cn

Go:   if data == nil { return }
来源：http://da.shxzskj.cn

Ruby: return if data.nil?
来源：http://rz.jianghongdianzi.cn

C#:   if (data == null) return;
来源：http://yi.newstarts.cn

================================================================================
来源：http://yv.huanxung.cn

C. 函数与作用域
来源：http://ws.9csxet.cn

================================================================================
来源：http://ol.szsharing.cn

[C01] 定义函数
来源：http://cq.hahajie.cn

Py:   def add(a, b): return a + b
来源：http://rl.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dq.bjjhwx.cn

JS:   function add(a, b) { return a + b; }
来源：http://yr.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://we.panjiajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://rt.hahajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://np.nszjky.cn

Ruby: def add(a, b); a + b; end
来源：http://wx.9csxet.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ot.nszjky.cn

[C02] 默认参数
来源：http://hv.nicolike.cn

Py:   def greet(name="World"): return name
来源：http://fd.yuntaijiaju.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://se.gzmigu.cn

JS:   function greet(name = "World") { return name; }
来源：http://df.jctech888.com.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yp.wgjwhj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ai.yuexingan06.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://af.jianghongdianzi.cn

Ruby: def greet(name = "World") = name
来源：http://ex.bookmarksfly.cn

C#:   string Greet(string name = "World") => name;
来源：http://as.521024.cn

[C03] 可变参数
来源：http://jv.bjjhwx.cn

Py:   def total(*args): return sum(args)
来源：http://zj.chemitech.net.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lx.asd995.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sc.bookmarksfly.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nz.huanxung.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nq.muxihuayi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gd.shxzskj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fd.colortex.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://by.huanxung.cn

[C04] 命名参数 / 关键字参数
来源：http://aa.nicolike.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://al.yuexingan06.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lt.szxytkj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pe.huanxung.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qw.asd995.cn

Java: // 无：用 Builder 模式或 record
来源：http://hi.9csxet.cn

Go:   // 无：用配置结构体参数
来源：http://gd.shxzukj.cn

Ruby: f(a: 1, b: 2)
来源：http://na.shxzukj.cn

C#:   f(a: 1, b: 2)
来源：http://vc.haigaiapp.cn

[C05] 返回多个值
来源：http://vu.szsharing.cn

Py:   return a, b
来源：http://st.panjiajie.cn

PHP:  return [$a, $b];
来源：http://aw.jianghongdianzi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://lv.panjiajie.cn

TS:   return { a, b };
来源：http://xr.yuntaijiaju.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ki.bookmarksfly.cn

Go:   return a, b
来源：http://wc.yuexingan06.cn

Ruby: return a, b
来源：http://zb.yuexingan06.cn

C#:   return (a, b);              // ValueTuple
来源：http://qd.huixinmuqiang.cn

[C06] 匿名函数 / lambda
来源：http://cf.asd995.cn

Py:   square = lambda x: x * x
来源：http://om.szsharing.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://mi.yuexingan06.cn

JS:   const square = x => x * x;
来源：http://cv.jianghongdianzi.cn

TS:   const square = (x: number): number => x * x;
来源：http://uk.huanxung.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tp.nszjky.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rk.newstarts.cn

Ruby: square = ->(x) { x * x }
来源：http://lc.yuexingan06.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ph.bjjhwx.cn

[C07] 把函数作为参数传入
来源：http://is.lnxyls.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jo.panjiajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://an.muxihuayi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xj.huixiangedu.cn

TS:   arr.map(String)
来源：http://km.yuexingan06.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rp.hnjuh.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wy.wgjwhj.cn

Ruby: arr.map(&:upcase)
来源：http://eg.nszjky.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gm.szsharing.cn

[C08] 闭包
来源：http://gr.nszjky.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jp.wgjwhj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fq.szsharing.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qh.muxihuayi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hi.huanxung.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tx.gzmigu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xa.nszjky.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mw.huixinmuqiang.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bw.jianghongdianzi.cn

[C09] 递归
来源：http://id.yuntaijiaju.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ih.panjiajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wj.jianghongdianzi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ee.colortex.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dg.colortex.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qg.521024.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zp.hahajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vq.panjiajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uh.wgjwhj.cn

[C10] 变量作用域
来源：http://fd.hnjuh.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ho.chemitech.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ui.lnxyls.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xz.wgjwhj.cn

TS:   同 JS
来源：http://ag.hnjuh.cn

Java: 方法内为块级作用域
来源：http://mo.nszjky.cn

Go:   花括号块级作用域
来源：http://nw.hahajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pi.szxytkj.cn

C#:   块级作用域
来源：http://qu.9csxet.cn

[C11] 模块导入与导出
来源：http://wy.huanxung.cn

Py:   from module import func
来源：http://tk.9csxet.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ck.jianghongdianzi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ib.jctech888.com.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gp.huanxung.cn

Java: import java.util.List;
来源：http://mm.shxzukj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ys.haigaiapp.cn

Ruby: require "json"; require_relative "./util"
来源：http://ba.asd995.cn

C#:   using System.Text;
来源：http://hv.yuexingan06.cn

[C12] 立即执行函数 IIFE
来源：http://xo.chemitech.net.cn

Py:   (lambda: print("run"))()
来源：http://dw.shxzukj.cn


<!-- 参考信息 -->