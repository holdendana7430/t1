代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xf.muxihuayi.cn

Ruby: gets.chomp
来源：http://io.9csxet.cn

C#:   Console.ReadLine();
来源：http://lg.szsharing.cn

[A21] 保留指定小数位输出
来源：http://tc.newstarts.cn

Py:   f"{3.14159:.2f}"
来源：http://ju.hahajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vo.chemitech.net.cn

JS:   (3.14159).toFixed(2)
来源：http://ml.yuntaijiaju.cn

TS:   (3.14159).toFixed(2)
来源：http://lb.hnjuh.cn

Java: String.format("%.2f", 3.14159)
来源：http://xj.szxytkj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://uq.huixinmuqiang.cn

Ruby: format("%.2f", 3.14159)
来源：http://cm.jctech888.com.cn

C#:   3.14159.ToString("F2")
来源：http://bu.9csxet.cn

[A22] 获取字符串长度
来源：http://hg.gzmigu.cn

Py:   len(s)
来源：http://va.wgjwhj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zx.521024.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tl.hnjuh.cn

TS:   s.length
来源：http://kg.jianghongdianzi.cn

Java: s.length()
来源：http://qo.hahajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jo.yuexingan06.cn

Ruby: s.length
来源：http://fs.newstarts.cn

C#:   s.Length
来源：http://eo.hnjuh.cn

[A23] 大小写转换
来源：http://tx.9csxet.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://cy.newstarts.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://si.gzmigu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cw.haigaiapp.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hi.muxihuayi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tu.yuexingan06.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://go.panjiajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ps.nszjky.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ue.nszjky.cn

[A24] 去除首尾空白
来源：http://fp.huixiangedu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qp.muxihuayi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qz.lnxyls.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jd.hahajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ji.shtwfgs.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vm.huanxung.cn

Go:   strings.TrimSpace(s)
来源：http://lz.asd995.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rc.szxytkj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qm.yuexingan06.cn

[A25] 字符串比较
来源：http://vu.shxzukj.cn

Py:   s1 == s2; s1 != s2
来源：http://du.huixiangedu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qh.hahajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://is.shxzskj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yk.gzmigu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dn.haigaiapp.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gn.panjiajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://jk.jctech888.com.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nk.huanxung.cn

[A26] 类型转换总览
来源：http://aq.hahajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zh.gzmigu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fd.panjiajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://it.gzmigu.cn

TS:   Number() String() Boolean() x as number
来源：http://no.nszjky.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ov.gzmigu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sy.shxzskj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://qd.shxzskj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xn.yuexingan06.cn

================================================================================
来源：http://jg.521024.cn

B. 流程控制
来源：http://pn.yuexingan06.cn

================================================================================
来源：http://da.chemitech.net.cn

[B01] 条件判断 if / else
来源：http://yk.shxzukj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vo.panjiajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gw.chemitech.net.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://av.szsharing.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://at.bjjhwx.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://mf.szxytkj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ls.shxzukj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kq.szsharing.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ky.huanxung.cn

[B02] 多分支 else if / elif
来源：http://ck.colortex.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ka.jctech888.com.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cg.szsharing.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://on.huixinmuqiang.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ay.521024.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tn.jianghongdianzi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bl.huixinmuqiang.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ow.jianghongdianzi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fd.hnjuh.cn

[B03] switch / match / case
来源：http://el.asd995.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zs.newstarts.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yt.huanxung.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tu.huixiangedu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://de.wgjwhj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://oa.muxihuayi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ds.521024.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lj.nicolike.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ym.huanxung.cn

[B04] for 计数循环
来源：http://tc.shtwfgs.cn

Py:   for i in range(10): print(i)
来源：http://sz.szsharing.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ij.wgjwhj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ko.chemitech.net.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zv.gzmigu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ex.hnjuh.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://iq.colortex.cn

Ruby: 10.times { |i| puts i }
来源：http://dp.wgjwhj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fp.szxytkj.cn

[B05] 遍历数组 / 列表
来源：http://ec.huixinmuqiang.cn

Py:   for item in arr: print(item)
来源：http://qs.huixinmuqiang.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ji.yuntaijiaju.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://sf.muxihuayi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ga.huanxung.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vo.lnxyls.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mo.gzmigu.cn

Ruby: arr.each { |item| puts item }
来源：http://nv.haigaiapp.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xa.shxzskj.cn

[B06] 遍历字典 / 对象
来源：http://zb.huixinmuqiang.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tk.huanxung.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kl.muxihuayi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vh.yuexingan06.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vp.nicolike.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mb.asd995.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pp.yuntaijiaju.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://js.yuexingan06.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sq.nicolike.cn

[B07] while 循环
来源：http://iq.wgjwhj.cn

Py:   while i < 10: i += 1
来源：http://rr.yuntaijiaju.cn

PHP:  while ($i < 10) { $i++; }
来源：http://tu.szxytkj.cn

JS:   while (i < 10) { i++; }
来源：http://vd.lnxyls.cn

TS:   while (i < 10) { i++; }
来源：http://dp.szsharing.cn

Java: while (i < 10) { i++; }
来源：http://qb.szsharing.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wl.szsharing.cn

Ruby: while i < 10; i += 1; end
来源：http://vv.yuexingan06.cn

C#:   while (i < 10) { i++; }
来源：http://te.nszjky.cn

[B08] do-while（至少执行一次）
来源：http://ma.szsharing.cn

Py:   # 无 do-while：用 while True + break
来源：http://dr.huixiangedu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://uy.chemitech.net.cn

JS:   do { i++; } while (i < 10);
来源：http://ke.haigaiapp.cn

TS:   do { i++; } while (i < 10);
来源：http://hh.muxihuayi.cn

Java: do { i++; } while (i < 10);
来源：http://bk.huanxung.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xr.panjiajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pk.9csxet.cn

C#:   do { i++; } while (i < 10);
来源：http://gq.huixiangedu.cn

[B09] break 与 continue
来源：http://et.521024.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jg.yuntaijiaju.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zu.chemitech.net.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://na.szsharing.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zv.yuntaijiaju.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zg.wgjwhj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kq.wgjwhj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fv.nicolike.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ms.shxzukj.cn

[B10] 遍历同时拿索引
来源：http://jd.shtwfgs.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://de.newstarts.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bz.newstarts.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pm.newstarts.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yq.jianghongdianzi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yl.haigaiapp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bo.nicolike.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://iw.shxzskj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://aa.jianghongdianzi.cn

[B11] 生成数字序列 / 区间
来源：http://jj.huanxung.cn

Py:   list(range(0, 10, 2))
来源：http://cc.hahajie.cn

PHP:  range(0, 10, 2);
来源：http://js.huanxung.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vv.9csxet.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pj.panjiajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://on.bjjhwx.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tr.szsharing.cn

Ruby: (0...10).step(2).to_a
来源：http://bc.huanxung.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wc.shxzukj.cn

[B12] 跳出多层循环
来源：http://dr.asd995.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ip.szxytkj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ch.hahajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xs.bjjhwx.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://op.chemitech.net.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zm.newstarts.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mn.yuexingan06.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tp.jctech888.com.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hs.nicolike.cn

[B13] 判断是否为数字
来源：http://kj.jctech888.com.cn

Py:   isinstance(x, (int, float))
来源：http://st.muxihuayi.cn

PHP:  is_numeric($x)
来源：http://vf.jianghongdianzi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://go.asd995.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://me.bjjhwx.cn

Java: x instanceof Number
来源：http://fw.shxzskj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jm.bjjhwx.cn

Ruby: x.is_a?(Numeric)
来源：http://la.asd995.cn

C#:   x is int or double or decimal
来源：http://ok.chemitech.net.cn

[B14] 判断值是否在集合内
来源：http://lx.panjiajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pc.gzmigu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://au.panjiajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://nd.yuexingan06.cn

TS:   [1, 2, 3].includes(x)
来源：http://fi.yuexingan06.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://pb.chemitech.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://if.wgjwhj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cq.nszjky.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rp.521024.cn

[B15] 布尔运算与取反
来源：http://do.wgjwhj.cn

Py:   a and b or not c
来源：http://gr.muxihuayi.cn

PHP:  $a && $b || !$c
来源：http://kl.newstarts.cn

JS:   a && b || !c
来源：http://fm.9csxet.cn

TS:   a && b || !c
来源：http://sr.jctech888.com.cn

Java: a && b || !c
来源：http://kw.colortex.cn

Go:   a && b || !c
来源：http://kj.hahajie.cn

Ruby: a && b || !c
来源：http://fa.newstarts.cn

C#:   a && b || !c
来源：http://ri.szxytkj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zh.jctech888.com.cn

Py:   if not data: return
来源：http://go.bjjhwx.cn

PHP:  if (!$data) { return; }
来源：http://hy.szsharing.cn

JS:   if (!data) return;
来源：http://oe.nszjky.cn

TS:   if (!data) return;
来源：http://si.jianghongdianzi.cn

Java: if (data == null) return;
来源：http://yi.chemitech.net.cn

Go:   if data == nil { return }
来源：http://be.huixiangedu.cn

Ruby: return if data.nil?
来源：http://sv.panjiajie.cn

C#:   if (data == null) return;
来源：http://sg.chemitech.net.cn

================================================================================
来源：http://vr.jianghongdianzi.cn

C. 函数与作用域
来源：http://gi.muxihuayi.cn

================================================================================
来源：http://xp.nicolike.cn

[C01] 定义函数
来源：http://df.lnxyls.cn

Py:   def add(a, b): return a + b
来源：http://nu.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cm.lnxyls.cn

JS:   function add(a, b) { return a + b; }
来源：http://qx.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nj.521024.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://pv.lnxyls.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ya.9csxet.cn

Ruby: def add(a, b); a + b; end
来源：http://fi.chemitech.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bq.yuexingan06.cn

[C02] 默认参数
来源：http://ew.yuexingan06.cn

Py:   def greet(name="World"): return name
来源：http://td.newstarts.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://df.nicolike.cn

JS:   function greet(name = "World") { return name; }
来源：http://yg.bookmarksfly.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lx.gzmigu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://iv.muxihuayi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zl.521024.cn

Ruby: def greet(name = "World") = name
来源：http://hw.newstarts.cn

C#:   string Greet(string name = "World") => name;
来源：http://cb.colortex.cn

[C03] 可变参数
来源：http://bu.szsharing.cn

Py:   def total(*args): return sum(args)
来源：http://ap.huanxung.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wg.shxzskj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://uv.521024.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tn.chemitech.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gq.huixinmuqiang.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fu.hahajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gd.521024.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fw.yuntaijiaju.cn

[C04] 命名参数 / 关键字参数
来源：http://ct.bjjhwx.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hw.yuexingan06.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xz.szxytkj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ri.wgjwhj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zw.shxzukj.cn

Java: // 无：用 Builder 模式或 record
来源：http://zp.newstarts.cn

Go:   // 无：用配置结构体参数
来源：http://nf.yuexingan06.cn

Ruby: f(a: 1, b: 2)
来源：http://fe.muxihuayi.cn

C#:   f(a: 1, b: 2)
来源：http://xy.gzmigu.cn

[C05] 返回多个值
来源：http://em.lnxyls.cn

Py:   return a, b
来源：http://pa.colortex.cn

PHP:  return [$a, $b];
来源：http://ia.bjjhwx.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dh.lnxyls.cn

TS:   return { a, b };
来源：http://xz.huixiangedu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pk.yuntaijiaju.cn

Go:   return a, b
来源：http://hi.jctech888.com.cn

Ruby: return a, b
来源：http://sm.panjiajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://db.colortex.cn

[C06] 匿名函数 / lambda
来源：http://yr.szsharing.cn

Py:   square = lambda x: x * x
来源：http://rd.szxytkj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pi.nicolike.cn

JS:   const square = x => x * x;
来源：http://yc.huanxung.cn

TS:   const square = (x: number): number => x * x;
来源：http://zn.huixinmuqiang.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gz.haigaiapp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ps.huanxung.cn

Ruby: square = ->(x) { x * x }
来源：http://xi.521024.cn

C#:   Func<int, int> square = x => x * x;
来源：http://jz.asd995.cn

[C07] 把函数作为参数传入
来源：http://xt.huixinmuqiang.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lv.hahajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ck.shxzskj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ex.shxzskj.cn

TS:   arr.map(String)
来源：http://pn.shxzskj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rb.shxzukj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qo.jianghongdianzi.cn

Ruby: arr.map(&:upcase)
来源：http://jk.newstarts.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://bb.gzmigu.cn

[C08] 闭包
来源：http://pm.shxzukj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kj.panjiajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ai.huanxung.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ty.szxytkj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sb.szsharing.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tq.haigaiapp.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ye.hnjuh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ii.huixinmuqiang.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://up.hahajie.cn

[C09] 递归
来源：http://ix.yuexingan06.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xz.huixiangedu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lc.shxzukj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ta.szsharing.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yj.shxzukj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kt.haigaiapp.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uw.hnjuh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://aq.bjjhwx.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ul.shxzukj.cn

[C10] 变量作用域
来源：http://gq.nicolike.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://so.newstarts.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dq.hnjuh.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wc.bjjhwx.cn

TS:   同 JS
来源：http://ot.muxihuayi.cn

Java: 方法内为块级作用域
来源：http://ml.gzmigu.cn

Go:   花括号块级作用域
来源：http://yz.huanxung.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gh.lnxyls.cn

C#:   块级作用域
来源：http://ft.yuntaijiaju.cn

[C11] 模块导入与导出
来源：http://tp.panjiajie.cn

Py:   from module import func
来源：http://bv.shtwfgs.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bv.nszjky.cn


<!-- 参考信息 -->