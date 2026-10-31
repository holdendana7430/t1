代发 wailian999

TS:   s.length
来源：http://aq.haigaiapp.cn

Java: s.length()
来源：http://co.asd995.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mo.jianghongdianzi.cn

Ruby: s.length
来源：http://yq.nicolike.cn

C#:   s.Length
来源：http://ek.muxihuayi.cn

[A23] 大小写转换
来源：http://fq.nicolike.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://gd.panjiajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lv.hahajie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://co.chemitech.net.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ds.szxytkj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zj.huixiangedu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hu.nszjky.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tz.jianghongdianzi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://nr.szxytkj.cn

[A24] 去除首尾空白
来源：http://vw.hahajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hl.huixinmuqiang.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sr.shtwfgs.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ih.panjiajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mw.colortex.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://if.hnjuh.cn

Go:   strings.TrimSpace(s)
来源：http://xb.szxytkj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qj.9csxet.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tb.yuexingan06.cn

[A25] 字符串比较
来源：http://ah.yuntaijiaju.cn

Py:   s1 == s2; s1 != s2
来源：http://km.hahajie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ld.bookmarksfly.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jw.bookmarksfly.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://va.jianghongdianzi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zr.hahajie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ax.hnjuh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://aj.yuntaijiaju.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://eb.nicolike.cn

[A26] 类型转换总览
来源：http://ge.shxzskj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rd.lnxyls.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jh.yuexingan06.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yq.huanxung.cn

TS:   Number() String() Boolean() x as number
来源：http://yl.gzmigu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ec.muxihuayi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ep.huixinmuqiang.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://cj.huixinmuqiang.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ns.muxihuayi.cn

================================================================================
来源：http://so.haigaiapp.cn

B. 流程控制
来源：http://kp.nszjky.cn

================================================================================
来源：http://wd.lnxyls.cn

[B01] 条件判断 if / else
来源：http://lc.chemitech.net.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://sp.hnjuh.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://as.newstarts.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bm.yuexingan06.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://te.hnjuh.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://gf.yuntaijiaju.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tu.colortex.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zp.muxihuayi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jl.hahajie.cn

[B02] 多分支 else if / elif
来源：http://ym.9csxet.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://os.shxzskj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cl.hnjuh.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cq.521024.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fr.yuexingan06.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cr.chemitech.net.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gr.shxzukj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qm.newstarts.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cz.shxzukj.cn

[B03] switch / match / case
来源：http://vn.muxihuayi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nd.shtwfgs.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gk.huixiangedu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mk.gzmigu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mi.muxihuayi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://is.shxzskj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rw.newstarts.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wk.newstarts.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hg.szxytkj.cn

[B04] for 计数循环
来源：http://yt.lnxyls.cn

Py:   for i in range(10): print(i)
来源：http://ez.nszjky.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cc.huixiangedu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lz.asd995.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gf.shtwfgs.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bx.shtwfgs.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yd.shxzukj.cn

Ruby: 10.times { |i| puts i }
来源：http://fv.yuexingan06.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://iv.hahajie.cn

[B05] 遍历数组 / 列表
来源：http://hx.shxzskj.cn

Py:   for item in arr: print(item)
来源：http://ok.shxzukj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tt.muxihuayi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fp.yuexingan06.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ia.jctech888.com.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://kw.chemitech.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rz.wgjwhj.cn

Ruby: arr.each { |item| puts item }
来源：http://bw.muxihuayi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ce.huanxung.cn

[B06] 遍历字典 / 对象
来源：http://kl.huanxung.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zg.jianghongdianzi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ct.chemitech.net.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xp.yuntaijiaju.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ku.szxytkj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://at.huixiangedu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gx.nszjky.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://td.nicolike.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://by.panjiajie.cn

[B07] while 循环
来源：http://uo.asd995.cn

Py:   while i < 10: i += 1
来源：http://ir.wgjwhj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://sf.jctech888.com.cn

JS:   while (i < 10) { i++; }
来源：http://jo.bookmarksfly.cn

TS:   while (i < 10) { i++; }
来源：http://rm.yuntaijiaju.cn

Java: while (i < 10) { i++; }
来源：http://an.asd995.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vh.hahajie.cn

Ruby: while i < 10; i += 1; end
来源：http://ep.nszjky.cn

C#:   while (i < 10) { i++; }
来源：http://cu.shxzskj.cn

[B08] do-while（至少执行一次）
来源：http://zg.panjiajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://ic.huanxung.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xe.chemitech.net.cn

JS:   do { i++; } while (i < 10);
来源：http://zi.lnxyls.cn

TS:   do { i++; } while (i < 10);
来源：http://ps.huanxung.cn

Java: do { i++; } while (i < 10);
来源：http://ua.gzmigu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gp.9csxet.cn

Ruby: begin; i += 1; end while i < 10
来源：http://lv.nszjky.cn

C#:   do { i++; } while (i < 10);
来源：http://ec.chemitech.net.cn

[B09] break 与 continue
来源：http://hk.chemitech.net.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://uj.yuntaijiaju.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qs.szxytkj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ir.szsharing.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pl.bjjhwx.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zn.szsharing.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pe.shtwfgs.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xa.szxytkj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ww.huanxung.cn

[B10] 遍历同时拿索引
来源：http://ss.shxzukj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mw.panjiajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://to.szxytkj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://es.colortex.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mn.gzmigu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ng.hnjuh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://we.shxzukj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uf.muxihuayi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xe.shxzukj.cn

[B11] 生成数字序列 / 区间
来源：http://yq.chemitech.net.cn

Py:   list(range(0, 10, 2))
来源：http://mc.hnjuh.cn

PHP:  range(0, 10, 2);
来源：http://xd.jctech888.com.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fk.bookmarksfly.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ma.shxzukj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vz.hahajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gp.panjiajie.cn

Ruby: (0...10).step(2).to_a
来源：http://ca.jianghongdianzi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xf.colortex.cn

[B12] 跳出多层循环
来源：http://lx.jctech888.com.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://gr.haigaiapp.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ey.haigaiapp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gh.lnxyls.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://uu.shtwfgs.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dl.521024.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zs.huanxung.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rb.huixinmuqiang.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hw.gzmigu.cn

[B13] 判断是否为数字
来源：http://lk.yuntaijiaju.cn

Py:   isinstance(x, (int, float))
来源：http://gs.9csxet.cn

PHP:  is_numeric($x)
来源：http://cs.shtwfgs.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lu.yuexingan06.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://za.huanxung.cn

Java: x instanceof Number
来源：http://zx.newstarts.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sy.yuntaijiaju.cn

Ruby: x.is_a?(Numeric)
来源：http://pw.asd995.cn

C#:   x is int or double or decimal
来源：http://yh.colortex.cn

[B14] 判断值是否在集合内
来源：http://jv.panjiajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://na.shtwfgs.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gn.bjjhwx.cn

JS:   [1, 2, 3].includes(x)
来源：http://fg.yuntaijiaju.cn

TS:   [1, 2, 3].includes(x)
来源：http://ze.shxzskj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://bg.yuntaijiaju.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lk.yuntaijiaju.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ey.panjiajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://an.bjjhwx.cn

[B15] 布尔运算与取反
来源：http://kd.szxytkj.cn

Py:   a and b or not c
来源：http://qq.szsharing.cn

PHP:  $a && $b || !$c
来源：http://be.521024.cn

JS:   a && b || !c
来源：http://zg.shtwfgs.cn

TS:   a && b || !c
来源：http://lx.nszjky.cn

Java: a && b || !c
来源：http://qn.muxihuayi.cn

Go:   a && b || !c
来源：http://az.jianghongdianzi.cn

Ruby: a && b || !c
来源：http://fw.shtwfgs.cn

C#:   a && b || !c
来源：http://ak.shxzskj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hg.yuexingan06.cn

Py:   if not data: return
来源：http://fv.newstarts.cn

PHP:  if (!$data) { return; }
来源：http://wf.huixinmuqiang.cn

JS:   if (!data) return;
来源：http://no.shxzukj.cn

TS:   if (!data) return;
来源：http://pv.shxzukj.cn

Java: if (data == null) return;
来源：http://ov.nszjky.cn

Go:   if data == nil { return }
来源：http://mi.panjiajie.cn

Ruby: return if data.nil?
来源：http://ss.szsharing.cn

C#:   if (data == null) return;
来源：http://sp.haigaiapp.cn

================================================================================
来源：http://uj.jianghongdianzi.cn

C. 函数与作用域
来源：http://od.huixiangedu.cn

================================================================================
来源：http://xg.yuexingan06.cn

[C01] 定义函数
来源：http://ip.hahajie.cn

Py:   def add(a, b): return a + b
来源：http://bn.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qd.shtwfgs.cn

JS:   function add(a, b) { return a + b; }
来源：http://nv.szxytkj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kd.shtwfgs.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://sg.yuexingan06.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ij.nszjky.cn

Ruby: def add(a, b); a + b; end
来源：http://fm.newstarts.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fl.haigaiapp.cn

[C02] 默认参数
来源：http://wd.shxzskj.cn

Py:   def greet(name="World"): return name
来源：http://zc.bookmarksfly.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zp.newstarts.cn

JS:   function greet(name = "World") { return name; }
来源：http://nt.szsharing.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qz.colortex.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rn.nszjky.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kh.shtwfgs.cn

Ruby: def greet(name = "World") = name
来源：http://df.shxzukj.cn

C#:   string Greet(string name = "World") => name;
来源：http://xw.jianghongdianzi.cn

[C03] 可变参数
来源：http://tp.yuexingan06.cn

Py:   def total(*args): return sum(args)
来源：http://rn.yuntaijiaju.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pn.nicolike.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gq.colortex.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sp.wgjwhj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yk.colortex.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dp.shxzukj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vk.szsharing.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bi.yuntaijiaju.cn

[C04] 命名参数 / 关键字参数
来源：http://xi.nszjky.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mn.szxytkj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jf.panjiajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cx.521024.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://el.yuexingan06.cn

Java: // 无：用 Builder 模式或 record
来源：http://eb.panjiajie.cn

Go:   // 无：用配置结构体参数
来源：http://qf.yuexingan06.cn

Ruby: f(a: 1, b: 2)
来源：http://ws.wgjwhj.cn

C#:   f(a: 1, b: 2)
来源：http://wd.9csxet.cn

[C05] 返回多个值
来源：http://uf.colortex.cn

Py:   return a, b
来源：http://uf.huixiangedu.cn

PHP:  return [$a, $b];
来源：http://zb.shxzskj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dm.lnxyls.cn

TS:   return { a, b };
来源：http://ky.muxihuayi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ji.szxytkj.cn

Go:   return a, b
来源：http://fu.panjiajie.cn

Ruby: return a, b
来源：http://wj.chemitech.net.cn

C#:   return (a, b);              // ValueTuple
来源：http://fm.huixiangedu.cn

[C06] 匿名函数 / lambda
来源：http://qk.jctech888.com.cn

Py:   square = lambda x: x * x
来源：http://tn.nszjky.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://gj.shxzukj.cn

JS:   const square = x => x * x;
来源：http://fs.yuexingan06.cn

TS:   const square = (x: number): number => x * x;
来源：http://st.nicolike.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xy.yuntaijiaju.cn

Go:   sq := func(x int) int { return x * x }
来源：http://uc.gzmigu.cn

Ruby: square = ->(x) { x * x }
来源：http://pn.jianghongdianzi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dd.jianghongdianzi.cn

[C07] 把函数作为参数传入
来源：http://tb.shxzskj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dt.yuntaijiaju.cn

PHP:  array_map("strtoupper", $arr);
来源：http://uk.asd995.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wh.nszjky.cn

TS:   arr.map(String)
来源：http://vc.yuexingan06.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ov.szxytkj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ar.szsharing.cn

Ruby: arr.map(&:upcase)
来源：http://oo.panjiajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cd.wgjwhj.cn

[C08] 闭包
来源：http://km.9csxet.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uf.9csxet.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tv.nicolike.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://if.hahajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ja.szsharing.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nv.yuexingan06.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kv.jctech888.com.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ey.bookmarksfly.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lo.nicolike.cn

[C09] 递归
来源：http://fd.muxihuayi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wt.hnjuh.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fn.newstarts.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dp.shxzukj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ue.chemitech.net.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rn.bookmarksfly.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mi.hahajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ie.9csxet.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kg.asd995.cn

[C10] 变量作用域
来源：http://ja.9csxet.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ow.szxytkj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ni.shxzukj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nw.jctech888.com.cn

TS:   同 JS
来源：http://vn.asd995.cn

Java: 方法内为块级作用域
来源：http://sc.gzmigu.cn

Go:   花括号块级作用域
来源：http://ek.huixinmuqiang.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ss.yuexingan06.cn

C#:   块级作用域
来源：http://iw.nicolike.cn

[C11] 模块导入与导出
来源：http://lx.szsharing.cn

Py:   from module import func
来源：http://mg.chemitech.net.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wt.muxihuayi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://tg.huixinmuqiang.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wx.gzmigu.cn

Java: import java.util.List;
来源：http://fq.nicolike.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kc.huixinmuqiang.cn

Ruby: require "json"; require_relative "./util"
来源：http://yb.haigaiapp.cn

C#:   using System.Text;
来源：http://gx.521024.cn

[C12] 立即执行函数 IIFE
来源：http://xm.chemitech.net.cn

Py:   (lambda: print("run"))()
来源：http://nf.nszjky.cn

PHP:  (function () { echo "run"; })();
来源：http://op.newstarts.cn

JS:   (() => { console.log("run"); })();
来源：http://hk.newstarts.cn

TS:   (() => { console.log("run"); })();
来源：http://lb.wgjwhj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cq.szsharing.cn

Go:   func() { fmt.Println("run") }()
来源：http://nt.shtwfgs.cn

Ruby: -> { puts "run" }.call
来源：http://io.shxzskj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://dq.bookmarksfly.cn

[C13] 类型声明 / 类型注解
来源：http://hd.huanxung.cn


<!-- 参考信息 -->