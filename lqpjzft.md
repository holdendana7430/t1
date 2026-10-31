代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lo.gzmigu.cn

Ruby: gets.chomp
来源：http://ye.szxytkj.cn

C#:   Console.ReadLine();
来源：http://wt.hnjuh.cn

[A21] 保留指定小数位输出
来源：http://mt.shxzskj.cn

Py:   f"{3.14159:.2f}"
来源：http://dr.wgjwhj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dw.szxytkj.cn

JS:   (3.14159).toFixed(2)
来源：http://mm.haigaiapp.cn

TS:   (3.14159).toFixed(2)
来源：http://nm.bookmarksfly.cn

Java: String.format("%.2f", 3.14159)
来源：http://ds.bookmarksfly.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://bg.shxzskj.cn

Ruby: format("%.2f", 3.14159)
来源：http://wr.lnxyls.cn

C#:   3.14159.ToString("F2")
来源：http://as.haigaiapp.cn

[A22] 获取字符串长度
来源：http://on.jianghongdianzi.cn

Py:   len(s)
来源：http://fs.nszjky.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://un.huixiangedu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://by.huixinmuqiang.cn

TS:   s.length
来源：http://ub.bjjhwx.cn

Java: s.length()
来源：http://rk.yuexingan06.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://my.nszjky.cn

Ruby: s.length
来源：http://ne.huanxung.cn

C#:   s.Length
来源：http://pm.shxzukj.cn

[A23] 大小写转换
来源：http://ts.yuexingan06.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://eq.newstarts.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hp.9csxet.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wb.bjjhwx.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bm.chemitech.net.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://uh.huixiangedu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wb.colortex.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://db.nszjky.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://vb.wgjwhj.cn

[A24] 去除首尾空白
来源：http://jf.szxytkj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ku.szsharing.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lv.gzmigu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rp.shxzukj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cp.chemitech.net.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qc.hahajie.cn

Go:   strings.TrimSpace(s)
来源：http://ft.panjiajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tu.hnjuh.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ur.nszjky.cn

[A25] 字符串比较
来源：http://sv.nszjky.cn

Py:   s1 == s2; s1 != s2
来源：http://hk.colortex.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ra.9csxet.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ms.panjiajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://sk.szxytkj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cc.colortex.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kz.haigaiapp.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hr.panjiajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ml.bjjhwx.cn

[A26] 类型转换总览
来源：http://sn.nszjky.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://po.521024.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jm.yuexingan06.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://uq.hnjuh.cn

TS:   Number() String() Boolean() x as number
来源：http://wp.bookmarksfly.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://uq.haigaiapp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ok.huixinmuqiang.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://kp.huanxung.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kz.nszjky.cn

================================================================================
来源：http://gk.szxytkj.cn

B. 流程控制
来源：http://hv.shxzskj.cn

================================================================================
来源：http://se.yuntaijiaju.cn

[B01] 条件判断 if / else
来源：http://uv.huixinmuqiang.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vn.jianghongdianzi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vl.hahajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://iw.newstarts.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hc.bookmarksfly.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://mf.shxzukj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ii.lnxyls.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ii.yuexingan06.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lp.shtwfgs.cn

[B02] 多分支 else if / elif
来源：http://lh.panjiajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kb.muxihuayi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ps.hahajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zx.hnjuh.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xt.jianghongdianzi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dc.newstarts.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fw.colortex.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mz.hnjuh.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nh.9csxet.cn

[B03] switch / match / case
来源：http://ol.huanxung.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hs.chemitech.net.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jd.nszjky.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://in.521024.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zh.haigaiapp.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cn.chemitech.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zh.wgjwhj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://oe.gzmigu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vo.bookmarksfly.cn

[B04] for 计数循环
来源：http://vg.huanxung.cn

Py:   for i in range(10): print(i)
来源：http://xy.yuntaijiaju.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ym.huanxung.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://di.gzmigu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nc.shtwfgs.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xf.muxihuayi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wl.jianghongdianzi.cn

Ruby: 10.times { |i| puts i }
来源：http://zc.panjiajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gd.panjiajie.cn

[B05] 遍历数组 / 列表
来源：http://to.nszjky.cn

Py:   for item in arr: print(item)
来源：http://pg.yuntaijiaju.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yw.chemitech.net.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ul.shxzskj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://dd.szsharing.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sd.shxzskj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lv.gzmigu.cn

Ruby: arr.each { |item| puts item }
来源：http://cr.asd995.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zl.szxytkj.cn

[B06] 遍历字典 / 对象
来源：http://yt.lnxyls.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mg.muxihuayi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pk.hnjuh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ig.yuntaijiaju.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cv.colortex.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fo.huixinmuqiang.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bi.colortex.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fm.huanxung.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://en.muxihuayi.cn

[B07] while 循环
来源：http://wd.yuexingan06.cn

Py:   while i < 10: i += 1
来源：http://nl.shxzskj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ah.szsharing.cn

JS:   while (i < 10) { i++; }
来源：http://wt.gzmigu.cn

TS:   while (i < 10) { i++; }
来源：http://nx.szsharing.cn

Java: while (i < 10) { i++; }
来源：http://kp.asd995.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jh.wgjwhj.cn

Ruby: while i < 10; i += 1; end
来源：http://xx.jianghongdianzi.cn

C#:   while (i < 10) { i++; }
来源：http://ay.muxihuayi.cn

[B08] do-while（至少执行一次）
来源：http://tc.gzmigu.cn

Py:   # 无 do-while：用 while True + break
来源：http://kd.hnjuh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://hw.nicolike.cn

JS:   do { i++; } while (i < 10);
来源：http://ph.haigaiapp.cn

TS:   do { i++; } while (i < 10);
来源：http://dc.jctech888.com.cn

Java: do { i++; } while (i < 10);
来源：http://aq.nszjky.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xf.asd995.cn

Ruby: begin; i += 1; end while i < 10
来源：http://if.colortex.cn

C#:   do { i++; } while (i < 10);
来源：http://mh.panjiajie.cn

[B09] break 与 continue
来源：http://mr.jctech888.com.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fb.huanxung.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fh.gzmigu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uv.wgjwhj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vt.9csxet.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mv.szsharing.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dz.asd995.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ak.muxihuayi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bl.yuntaijiaju.cn

[B10] 遍历同时拿索引
来源：http://fl.szxytkj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pw.newstarts.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://px.huanxung.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cw.hnjuh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ro.9csxet.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ti.chemitech.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://np.panjiajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ea.szsharing.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rw.haigaiapp.cn

[B11] 生成数字序列 / 区间
来源：http://fa.colortex.cn

Py:   list(range(0, 10, 2))
来源：http://mv.szxytkj.cn

PHP:  range(0, 10, 2);
来源：http://pv.521024.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fz.szxytkj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yn.jctech888.com.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dr.bookmarksfly.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ln.jianghongdianzi.cn

Ruby: (0...10).step(2).to_a
来源：http://yl.shxzskj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kh.huanxung.cn

[B12] 跳出多层循环
来源：http://yq.shxzskj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://vu.muxihuayi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ka.huixiangedu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zt.lnxyls.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ai.wgjwhj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nm.bjjhwx.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zt.521024.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gt.yuntaijiaju.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://oe.hnjuh.cn

[B13] 判断是否为数字
来源：http://bc.shxzukj.cn

Py:   isinstance(x, (int, float))
来源：http://ed.asd995.cn

PHP:  is_numeric($x)
来源：http://xx.nszjky.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oa.lnxyls.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gf.colortex.cn

Java: x instanceof Number
来源：http://oe.haigaiapp.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hg.bookmarksfly.cn

Ruby: x.is_a?(Numeric)
来源：http://yw.yuntaijiaju.cn

C#:   x is int or double or decimal
来源：http://lb.muxihuayi.cn

[B14] 判断值是否在集合内
来源：http://ev.haigaiapp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kb.yuntaijiaju.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ra.bookmarksfly.cn

JS:   [1, 2, 3].includes(x)
来源：http://il.nicolike.cn

TS:   [1, 2, 3].includes(x)
来源：http://ye.wgjwhj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dr.wgjwhj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://og.wgjwhj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xt.szsharing.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yv.bjjhwx.cn

[B15] 布尔运算与取反
来源：http://bi.huanxung.cn

Py:   a and b or not c
来源：http://pc.yuntaijiaju.cn

PHP:  $a && $b || !$c
来源：http://xh.yuntaijiaju.cn

JS:   a && b || !c
来源：http://ny.yuexingan06.cn

TS:   a && b || !c
来源：http://si.szsharing.cn

Java: a && b || !c
来源：http://mt.jianghongdianzi.cn

Go:   a && b || !c
来源：http://ru.gzmigu.cn

Ruby: a && b || !c
来源：http://dd.chemitech.net.cn

C#:   a && b || !c
来源：http://wa.haigaiapp.cn

[B16] 卫语句：不满足条件提前返回
来源：http://rc.hahajie.cn

Py:   if not data: return
来源：http://lx.bookmarksfly.cn

PHP:  if (!$data) { return; }
来源：http://jq.muxihuayi.cn

JS:   if (!data) return;
来源：http://he.gzmigu.cn

TS:   if (!data) return;
来源：http://sd.hahajie.cn

Java: if (data == null) return;
来源：http://rc.hahajie.cn

Go:   if data == nil { return }
来源：http://fb.huixiangedu.cn

Ruby: return if data.nil?
来源：http://zx.szxytkj.cn

C#:   if (data == null) return;
来源：http://nu.huixiangedu.cn

================================================================================
来源：http://hq.yuexingan06.cn

C. 函数与作用域
来源：http://mr.jianghongdianzi.cn

================================================================================
来源：http://rr.newstarts.cn

[C01] 定义函数
来源：http://pg.newstarts.cn

Py:   def add(a, b): return a + b
来源：http://qo.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lm.bjjhwx.cn

JS:   function add(a, b) { return a + b; }
来源：http://vz.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zm.muxihuayi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qg.yuntaijiaju.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ap.jianghongdianzi.cn

Ruby: def add(a, b); a + b; end
来源：http://dx.yuexingan06.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zp.bjjhwx.cn

[C02] 默认参数
来源：http://fj.bjjhwx.cn

Py:   def greet(name="World"): return name
来源：http://we.szsharing.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://sk.shxzskj.cn

JS:   function greet(name = "World") { return name; }
来源：http://wg.gzmigu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fa.wgjwhj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dn.shtwfgs.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ux.jianghongdianzi.cn

Ruby: def greet(name = "World") = name
来源：http://ww.szsharing.cn

C#:   string Greet(string name = "World") => name;
来源：http://ic.wgjwhj.cn

[C03] 可变参数
来源：http://yj.shxzukj.cn

Py:   def total(*args): return sum(args)
来源：http://io.521024.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://td.hnjuh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mw.huixiangedu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lu.nszjky.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rx.wgjwhj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hb.lnxyls.cn

Ruby: def total(*nums); nums.sum; end
来源：http://cr.hnjuh.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vl.nszjky.cn

[C04] 命名参数 / 关键字参数
来源：http://ir.shxzukj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ej.nicolike.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://es.bjjhwx.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zs.huixiangedu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rj.newstarts.cn

Java: // 无：用 Builder 模式或 record
来源：http://vz.jctech888.com.cn

Go:   // 无：用配置结构体参数
来源：http://dv.yuexingan06.cn

Ruby: f(a: 1, b: 2)
来源：http://ml.newstarts.cn

C#:   f(a: 1, b: 2)
来源：http://sf.haigaiapp.cn

[C05] 返回多个值
来源：http://fc.szsharing.cn

Py:   return a, b
来源：http://uf.jianghongdianzi.cn

PHP:  return [$a, $b];
来源：http://ni.huixiangedu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zk.haigaiapp.cn

TS:   return { a, b };
来源：http://wv.szxytkj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jp.521024.cn

Go:   return a, b
来源：http://nw.bookmarksfly.cn

Ruby: return a, b
来源：http://zx.hnjuh.cn

C#:   return (a, b);              // ValueTuple
来源：http://lq.nszjky.cn

[C06] 匿名函数 / lambda
来源：http://gm.shxzukj.cn

Py:   square = lambda x: x * x
来源：http://dt.szsharing.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://sf.szxytkj.cn

JS:   const square = x => x * x;
来源：http://sq.haigaiapp.cn

TS:   const square = (x: number): number => x * x;
来源：http://zn.521024.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://aq.chemitech.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://uo.panjiajie.cn

Ruby: square = ->(x) { x * x }
来源：http://ev.chemitech.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://is.haigaiapp.cn

[C07] 把函数作为参数传入
来源：http://mc.szxytkj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bl.shtwfgs.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kj.colortex.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vo.haigaiapp.cn

TS:   arr.map(String)
来源：http://ic.newstarts.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xz.wgjwhj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ys.9csxet.cn

Ruby: arr.map(&:upcase)
来源：http://ch.bjjhwx.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://no.muxihuayi.cn

[C08] 闭包
来源：http://pm.chemitech.net.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://az.jianghongdianzi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zv.hnjuh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gp.shtwfgs.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pm.haigaiapp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://iy.jctech888.com.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fm.newstarts.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nl.haigaiapp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://eo.bookmarksfly.cn

[C09] 递归
来源：http://nx.yuexingan06.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fj.bjjhwx.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jm.nicolike.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bi.muxihuayi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yk.newstarts.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jy.shxzskj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://aa.huanxung.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sa.jctech888.com.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ur.muxihuayi.cn

[C10] 变量作用域
来源：http://cz.lnxyls.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pz.gzmigu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ub.wgjwhj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wm.bjjhwx.cn

TS:   同 JS
来源：http://vz.szxytkj.cn

Java: 方法内为块级作用域
来源：http://il.newstarts.cn

Go:   花括号块级作用域
来源：http://dj.yuexingan06.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zk.haigaiapp.cn

C#:   块级作用域
来源：http://bv.hahajie.cn

[C11] 模块导入与导出
来源：http://vm.hnjuh.cn

Py:   from module import func
来源：http://uj.gzmigu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zv.bjjhwx.cn


<!-- 参考信息 -->