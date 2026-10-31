代发 wailian999

JS:   [a, b] = [b, a];
来源：http://nl.huixiangedu.cn

TS:   [a, b] = [b, a];
来源：http://up.huixiangedu.cn

Java: int t = a; a = b; b = t;
来源：http://gs.yuexingan06.cn

Go:   a, b = b, a
来源：http://fi.gzmigu.cn

Ruby: a, b = b, a
来源：http://rr.shtwfgs.cn

C#:   (a, b) = (b, a);
来源：http://mc.chemitech.net.cn

[A20] 读取标准输入
来源：http://tz.gzmigu.cn

Py:   name = input("请输入：")
来源：http://lx.szxytkj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ky.nicolike.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qb.shxzskj.cn

TS:   // Node.js：readline 模块
来源：http://xv.szxytkj.cn

Java: new Scanner(System.in).nextLine()
来源：http://as.nicolike.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ft.wgjwhj.cn

Ruby: gets.chomp
来源：http://lo.huixinmuqiang.cn

C#:   Console.ReadLine();
来源：http://gu.muxihuayi.cn

[A21] 保留指定小数位输出
来源：http://hu.huanxung.cn

Py:   f"{3.14159:.2f}"
来源：http://jh.haigaiapp.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qb.muxihuayi.cn

JS:   (3.14159).toFixed(2)
来源：http://fx.gzmigu.cn

TS:   (3.14159).toFixed(2)
来源：http://ux.wgjwhj.cn

Java: String.format("%.2f", 3.14159)
来源：http://qe.hnjuh.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ty.wgjwhj.cn

Ruby: format("%.2f", 3.14159)
来源：http://qn.jctech888.com.cn

C#:   3.14159.ToString("F2")
来源：http://tj.lnxyls.cn

[A22] 获取字符串长度
来源：http://es.huanxung.cn

Py:   len(s)
来源：http://cz.bjjhwx.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ni.newstarts.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nj.gzmigu.cn

TS:   s.length
来源：http://sv.9csxet.cn

Java: s.length()
来源：http://qo.asd995.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://uf.haigaiapp.cn

Ruby: s.length
来源：http://le.asd995.cn

C#:   s.Length
来源：http://ml.szsharing.cn

[A23] 大小写转换
来源：http://ah.yuexingan06.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://cq.szsharing.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bn.yuexingan06.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xo.szsharing.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tf.shtwfgs.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lf.bjjhwx.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cr.hahajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tm.shxzskj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qm.huanxung.cn

[A24] 去除首尾空白
来源：http://xt.newstarts.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vu.muxihuayi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ws.muxihuayi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yi.huixiangedu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mc.chemitech.net.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kq.nicolike.cn

Go:   strings.TrimSpace(s)
来源：http://ui.panjiajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://yn.hahajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ab.jctech888.com.cn

[A25] 字符串比较
来源：http://vz.haigaiapp.cn

Py:   s1 == s2; s1 != s2
来源：http://yw.jianghongdianzi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dx.asd995.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bb.huanxung.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ix.gzmigu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mm.hahajie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cv.haigaiapp.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://te.muxihuayi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ff.colortex.cn

[A26] 类型转换总览
来源：http://mo.gzmigu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yf.chemitech.net.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dc.hahajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sm.521024.cn

TS:   Number() String() Boolean() x as number
来源：http://wu.yuntaijiaju.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kg.jianghongdianzi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ha.huixiangedu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://wd.nszjky.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://eb.panjiajie.cn

================================================================================
来源：http://gq.hnjuh.cn

B. 流程控制
来源：http://qf.hahajie.cn

================================================================================
来源：http://hg.nicolike.cn

[B01] 条件判断 if / else
来源：http://kd.colortex.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://fh.asd995.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gn.shxzukj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lg.huanxung.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bd.yuexingan06.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://wd.jianghongdianzi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vf.jianghongdianzi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yv.lnxyls.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vc.521024.cn

[B02] 多分支 else if / elif
来源：http://em.shxzukj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sl.yuntaijiaju.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bt.szsharing.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sw.colortex.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gi.haigaiapp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cm.muxihuayi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xa.yuexingan06.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pq.nicolike.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hx.szsharing.cn

[B03] switch / match / case
来源：http://rk.asd995.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cj.szsharing.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bp.9csxet.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tt.huixiangedu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ms.nicolike.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://si.chemitech.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yj.huixinmuqiang.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kx.nicolike.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ve.shxzukj.cn

[B04] for 计数循环
来源：http://bt.yuexingan06.cn

Py:   for i in range(10): print(i)
来源：http://hz.jianghongdianzi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mh.huanxung.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hu.shxzukj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ba.asd995.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ow.jianghongdianzi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://iq.9csxet.cn

Ruby: 10.times { |i| puts i }
来源：http://er.521024.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tf.yuntaijiaju.cn

[B05] 遍历数组 / 列表
来源：http://rk.chemitech.net.cn

Py:   for item in arr: print(item)
来源：http://wh.chemitech.net.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ir.nszjky.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://pd.huixiangedu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ey.lnxyls.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ym.jianghongdianzi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://eq.shtwfgs.cn

Ruby: arr.each { |item| puts item }
来源：http://ag.huixinmuqiang.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gy.huixiangedu.cn

[B06] 遍历字典 / 对象
来源：http://ov.szsharing.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://dn.szxytkj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wc.panjiajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ui.huixinmuqiang.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qr.yuntaijiaju.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ic.bookmarksfly.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ch.nszjky.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tf.muxihuayi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dj.yuexingan06.cn

[B07] while 循环
来源：http://vr.chemitech.net.cn

Py:   while i < 10: i += 1
来源：http://fm.huanxung.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fx.asd995.cn

JS:   while (i < 10) { i++; }
来源：http://fu.hahajie.cn

TS:   while (i < 10) { i++; }
来源：http://wy.newstarts.cn

Java: while (i < 10) { i++; }
来源：http://ku.521024.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qf.jianghongdianzi.cn

Ruby: while i < 10; i += 1; end
来源：http://of.lnxyls.cn

C#:   while (i < 10) { i++; }
来源：http://xc.haigaiapp.cn

[B08] do-while（至少执行一次）
来源：http://hb.shxzukj.cn

Py:   # 无 do-while：用 while True + break
来源：http://cv.nszjky.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vs.hnjuh.cn

JS:   do { i++; } while (i < 10);
来源：http://qk.nicolike.cn

TS:   do { i++; } while (i < 10);
来源：http://jl.lnxyls.cn

Java: do { i++; } while (i < 10);
来源：http://xd.chemitech.net.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mx.bookmarksfly.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pm.shxzukj.cn

C#:   do { i++; } while (i < 10);
来源：http://qi.hnjuh.cn

[B09] break 与 continue
来源：http://tv.huixiangedu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xk.bookmarksfly.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mw.hnjuh.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bk.haigaiapp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ej.hnjuh.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ml.shxzukj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qo.muxihuayi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gu.shtwfgs.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oh.shxzskj.cn

[B10] 遍历同时拿索引
来源：http://ef.yuntaijiaju.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rc.gzmigu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jt.huanxung.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://iy.huixiangedu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kl.shxzukj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ln.shtwfgs.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wv.9csxet.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bx.colortex.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://eq.huixiangedu.cn

[B11] 生成数字序列 / 区间
来源：http://ov.yuntaijiaju.cn

Py:   list(range(0, 10, 2))
来源：http://bu.newstarts.cn

PHP:  range(0, 10, 2);
来源：http://bo.huanxung.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zd.nszjky.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rd.9csxet.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fr.jianghongdianzi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ux.wgjwhj.cn

Ruby: (0...10).step(2).to_a
来源：http://ig.huixiangedu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://am.521024.cn

[B12] 跳出多层循环
来源：http://tp.hnjuh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://df.shtwfgs.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://dp.shxzukj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ic.asd995.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ug.jianghongdianzi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ow.bookmarksfly.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yk.shxzukj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fs.jianghongdianzi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pq.asd995.cn

[B13] 判断是否为数字
来源：http://rn.szsharing.cn

Py:   isinstance(x, (int, float))
来源：http://cv.hnjuh.cn

PHP:  is_numeric($x)
来源：http://qe.shxzskj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jy.szsharing.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pb.panjiajie.cn

Java: x instanceof Number
来源：http://el.szxytkj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xl.panjiajie.cn

Ruby: x.is_a?(Numeric)
来源：http://wv.yuntaijiaju.cn

C#:   x is int or double or decimal
来源：http://pg.muxihuayi.cn

[B14] 判断值是否在集合内
来源：http://be.yuexingan06.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wp.newstarts.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://op.521024.cn

JS:   [1, 2, 3].includes(x)
来源：http://gh.hnjuh.cn

TS:   [1, 2, 3].includes(x)
来源：http://ph.nszjky.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://li.asd995.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cl.szxytkj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://lp.jianghongdianzi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dx.nszjky.cn

[B15] 布尔运算与取反
来源：http://ct.panjiajie.cn

Py:   a and b or not c
来源：http://zc.bjjhwx.cn

PHP:  $a && $b || !$c
来源：http://jr.colortex.cn

JS:   a && b || !c
来源：http://dq.huanxung.cn

TS:   a && b || !c
来源：http://xr.shxzskj.cn

Java: a && b || !c
来源：http://oq.huixinmuqiang.cn

Go:   a && b || !c
来源：http://xv.szxytkj.cn

Ruby: a && b || !c
来源：http://vf.chemitech.net.cn

C#:   a && b || !c
来源：http://xc.shxzukj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://el.szxytkj.cn

Py:   if not data: return
来源：http://jd.shtwfgs.cn

PHP:  if (!$data) { return; }
来源：http://pz.shxzukj.cn

JS:   if (!data) return;
来源：http://zx.jianghongdianzi.cn

TS:   if (!data) return;
来源：http://pb.521024.cn

Java: if (data == null) return;
来源：http://oj.yuntaijiaju.cn

Go:   if data == nil { return }
来源：http://pg.9csxet.cn

Ruby: return if data.nil?
来源：http://kx.huixinmuqiang.cn

C#:   if (data == null) return;
来源：http://sd.yuntaijiaju.cn

================================================================================
来源：http://sp.huixinmuqiang.cn

C. 函数与作用域
来源：http://zu.bjjhwx.cn

================================================================================
来源：http://aa.521024.cn

[C01] 定义函数
来源：http://uz.huixinmuqiang.cn

Py:   def add(a, b): return a + b
来源：http://no.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ig.newstarts.cn

JS:   function add(a, b) { return a + b; }
来源：http://mp.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lp.gzmigu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://yt.jctech888.com.cn

Go:   func add(a, b int) int { return a + b }
来源：http://gu.wgjwhj.cn

Ruby: def add(a, b); a + b; end
来源：http://dq.9csxet.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ha.hahajie.cn

[C02] 默认参数
来源：http://ny.9csxet.cn

Py:   def greet(name="World"): return name
来源：http://xj.newstarts.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zl.szxytkj.cn

JS:   function greet(name = "World") { return name; }
来源：http://ob.muxihuayi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://eu.shxzskj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://yk.chemitech.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mc.huixinmuqiang.cn

Ruby: def greet(name = "World") = name
来源：http://zv.newstarts.cn

C#:   string Greet(string name = "World") => name;
来源：http://dh.gzmigu.cn

[C03] 可变参数
来源：http://bz.muxihuayi.cn

Py:   def total(*args): return sum(args)
来源：http://cj.bookmarksfly.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sk.jctech888.com.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://be.lnxyls.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mf.jctech888.com.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xn.wgjwhj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://oa.521024.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vj.shtwfgs.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vu.szxytkj.cn

[C04] 命名参数 / 关键字参数
来源：http://ub.jianghongdianzi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sq.shxzskj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mi.lnxyls.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bk.bjjhwx.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tq.muxihuayi.cn

Java: // 无：用 Builder 模式或 record
来源：http://ae.wgjwhj.cn

Go:   // 无：用配置结构体参数
来源：http://fx.hahajie.cn

Ruby: f(a: 1, b: 2)
来源：http://af.huixinmuqiang.cn

C#:   f(a: 1, b: 2)
来源：http://kd.bookmarksfly.cn

[C05] 返回多个值
来源：http://yg.muxihuayi.cn

Py:   return a, b
来源：http://ea.jianghongdianzi.cn

PHP:  return [$a, $b];
来源：http://py.nicolike.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ok.colortex.cn

TS:   return { a, b };
来源：http://ch.muxihuayi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xt.bjjhwx.cn

Go:   return a, b
来源：http://iz.shxzukj.cn

Ruby: return a, b
来源：http://hg.szsharing.cn

C#:   return (a, b);              // ValueTuple
来源：http://yv.shxzskj.cn

[C06] 匿名函数 / lambda
来源：http://os.newstarts.cn

Py:   square = lambda x: x * x
来源：http://qq.yuexingan06.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ea.szxytkj.cn

JS:   const square = x => x * x;
来源：http://om.gzmigu.cn

TS:   const square = (x: number): number => x * x;
来源：http://oh.chemitech.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cu.shxzukj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://nb.huixiangedu.cn

Ruby: square = ->(x) { x * x }
来源：http://tj.jianghongdianzi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xh.huixiangedu.cn

[C07] 把函数作为参数传入
来源：http://pv.jctech888.com.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wf.lnxyls.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vn.9csxet.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tc.jctech888.com.cn

TS:   arr.map(String)
来源：http://kn.hnjuh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ne.bookmarksfly.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xj.lnxyls.cn

Ruby: arr.map(&:upcase)
来源：http://mz.shxzukj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://tj.bjjhwx.cn

[C08] 闭包
来源：http://kj.nszjky.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://co.chemitech.net.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ib.nszjky.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vx.wgjwhj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bn.shxzskj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uf.shtwfgs.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yk.colortex.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xm.haigaiapp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xt.shxzukj.cn

[C09] 递归
来源：http://lg.huixiangedu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wh.hnjuh.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://so.gzmigu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ix.szsharing.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ua.yuntaijiaju.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qj.yuexingan06.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sd.jianghongdianzi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://oj.muxihuayi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rh.hnjuh.cn


<!-- 参考信息 -->