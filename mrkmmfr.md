代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://ml.szsharing.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fw.szsharing.cn

TS:   // Node.js：readline 模块
来源：http://lk.muxihuayi.cn

Java: new Scanner(System.in).nextLine()
来源：http://oo.wgjwhj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://tj.newstarts.cn

Ruby: gets.chomp
来源：http://ar.yuntaijiaju.cn

C#:   Console.ReadLine();
来源：http://ls.huixiangedu.cn

[A21] 保留指定小数位输出
来源：http://ay.huixinmuqiang.cn

Py:   f"{3.14159:.2f}"
来源：http://to.nszjky.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://nm.huixinmuqiang.cn

JS:   (3.14159).toFixed(2)
来源：http://mb.huixiangedu.cn

TS:   (3.14159).toFixed(2)
来源：http://if.asd995.cn

Java: String.format("%.2f", 3.14159)
来源：http://jo.nszjky.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jn.szsharing.cn

Ruby: format("%.2f", 3.14159)
来源：http://cw.yuexingan06.cn

C#:   3.14159.ToString("F2")
来源：http://or.panjiajie.cn

[A22] 获取字符串长度
来源：http://de.haigaiapp.cn

Py:   len(s)
来源：http://jm.wgjwhj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jp.jctech888.com.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ff.huixinmuqiang.cn

TS:   s.length
来源：http://gc.huixiangedu.cn

Java: s.length()
来源：http://hf.9csxet.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://yn.bjjhwx.cn

Ruby: s.length
来源：http://gu.szsharing.cn

C#:   s.Length
来源：http://kh.panjiajie.cn

[A23] 大小写转换
来源：http://ha.9csxet.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.hnjuh.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kn.szxytkj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://sd.9csxet.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gm.szxytkj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lw.shxzukj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ud.hahajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://go.521024.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://tk.shxzukj.cn

[A24] 去除首尾空白
来源：http://ch.nicolike.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vy.haigaiapp.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://po.jianghongdianzi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mt.jctech888.com.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nr.nicolike.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://po.asd995.cn

Go:   strings.TrimSpace(s)
来源：http://rf.shxzukj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xm.jianghongdianzi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fl.shxzskj.cn

[A25] 字符串比较
来源：http://fs.newstarts.cn

Py:   s1 == s2; s1 != s2
来源：http://db.jianghongdianzi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qj.bookmarksfly.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rq.huixiangedu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nn.gzmigu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mz.jctech888.com.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://oy.shtwfgs.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://wa.colortex.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ui.bookmarksfly.cn

[A26] 类型转换总览
来源：http://yv.haigaiapp.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gq.chemitech.net.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zv.jianghongdianzi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bx.haigaiapp.cn

TS:   Number() String() Boolean() x as number
来源：http://xx.hnjuh.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://li.shxzskj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ei.panjiajie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://dq.newstarts.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xn.jctech888.com.cn

================================================================================
来源：http://ay.yuntaijiaju.cn

B. 流程控制
来源：http://ov.asd995.cn

================================================================================
来源：http://bg.jctech888.com.cn

[B01] 条件判断 if / else
来源：http://ye.521024.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ng.panjiajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ze.haigaiapp.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zt.shxzskj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://iu.huixiangedu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ug.asd995.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ob.haigaiapp.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gs.gzmigu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mv.shxzskj.cn

[B02] 多分支 else if / elif
来源：http://tv.huanxung.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qo.yuntaijiaju.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ar.hnjuh.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xw.hahajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nt.huanxung.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mu.yuexingan06.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gy.szxytkj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ps.9csxet.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ej.yuntaijiaju.cn

[B03] switch / match / case
来源：http://az.huanxung.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vl.521024.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yu.shxzskj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sq.521024.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xt.hahajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nd.newstarts.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gv.newstarts.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xl.muxihuayi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hn.shtwfgs.cn

[B04] for 计数循环
来源：http://wg.huixinmuqiang.cn

Py:   for i in range(10): print(i)
来源：http://sc.521024.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mx.9csxet.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kq.panjiajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bi.haigaiapp.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ur.jctech888.com.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gz.gzmigu.cn

Ruby: 10.times { |i| puts i }
来源：http://xz.muxihuayi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qg.521024.cn

[B05] 遍历数组 / 列表
来源：http://yc.bjjhwx.cn

Py:   for item in arr: print(item)
来源：http://ti.huixinmuqiang.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dc.jctech888.com.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://pp.bjjhwx.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://dz.wgjwhj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lf.521024.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ol.chemitech.net.cn

Ruby: arr.each { |item| puts item }
来源：http://au.521024.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ba.bjjhwx.cn

[B06] 遍历字典 / 对象
来源：http://eh.521024.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tc.panjiajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mf.muxihuayi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rl.nicolike.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rs.chemitech.net.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bk.szxytkj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ci.huixiangedu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xc.yuexingan06.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kj.jianghongdianzi.cn

[B07] while 循环
来源：http://kx.muxihuayi.cn

Py:   while i < 10: i += 1
来源：http://og.szxytkj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://cn.jctech888.com.cn

JS:   while (i < 10) { i++; }
来源：http://pi.bookmarksfly.cn

TS:   while (i < 10) { i++; }
来源：http://zl.gzmigu.cn

Java: while (i < 10) { i++; }
来源：http://fc.gzmigu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ie.panjiajie.cn

Ruby: while i < 10; i += 1; end
来源：http://ih.bjjhwx.cn

C#:   while (i < 10) { i++; }
来源：http://ja.gzmigu.cn

[B08] do-while（至少执行一次）
来源：http://go.jctech888.com.cn

Py:   # 无 do-while：用 while True + break
来源：http://rh.szsharing.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://dt.muxihuayi.cn

JS:   do { i++; } while (i < 10);
来源：http://mz.haigaiapp.cn

TS:   do { i++; } while (i < 10);
来源：http://hw.szsharing.cn

Java: do { i++; } while (i < 10);
来源：http://km.hnjuh.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://it.jctech888.com.cn

Ruby: begin; i += 1; end while i < 10
来源：http://dc.szxytkj.cn

C#:   do { i++; } while (i < 10);
来源：http://yf.shtwfgs.cn

[B09] break 与 continue
来源：http://ws.szxytkj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://do.nszjky.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gl.nicolike.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sa.lnxyls.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xl.yuntaijiaju.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rx.jianghongdianzi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zq.muxihuayi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rx.yuexingan06.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ct.nszjky.cn

[B10] 遍历同时拿索引
来源：http://wl.muxihuayi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fd.nicolike.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://po.521024.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zx.yuntaijiaju.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dv.wgjwhj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fj.hahajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://km.colortex.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rz.lnxyls.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vr.jctech888.com.cn

[B11] 生成数字序列 / 区间
来源：http://jp.hnjuh.cn

Py:   list(range(0, 10, 2))
来源：http://mb.nszjky.cn

PHP:  range(0, 10, 2);
来源：http://ra.panjiajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wl.huixiangedu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ua.yuntaijiaju.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gn.gzmigu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hv.panjiajie.cn

Ruby: (0...10).step(2).to_a
来源：http://zn.yuexingan06.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yd.shxzskj.cn

[B12] 跳出多层循环
来源：http://ib.bookmarksfly.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://un.haigaiapp.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://cq.hahajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vy.jianghongdianzi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ek.chemitech.net.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nq.asd995.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qh.shxzukj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kz.newstarts.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yw.yuexingan06.cn

[B13] 判断是否为数字
来源：http://ku.shtwfgs.cn

Py:   isinstance(x, (int, float))
来源：http://bh.szxytkj.cn

PHP:  is_numeric($x)
来源：http://ni.asd995.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qp.bookmarksfly.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://se.huanxung.cn

Java: x instanceof Number
来源：http://bg.nicolike.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kp.521024.cn

Ruby: x.is_a?(Numeric)
来源：http://ng.szsharing.cn

C#:   x is int or double or decimal
来源：http://qy.shxzskj.cn

[B14] 判断值是否在集合内
来源：http://sz.yuntaijiaju.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ou.bjjhwx.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fs.panjiajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://ji.nicolike.cn

TS:   [1, 2, 3].includes(x)
来源：http://kz.huixinmuqiang.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://yg.bookmarksfly.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ro.wgjwhj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://hv.szsharing.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gt.chemitech.net.cn

[B15] 布尔运算与取反
来源：http://pw.lnxyls.cn

Py:   a and b or not c
来源：http://lw.bookmarksfly.cn

PHP:  $a && $b || !$c
来源：http://wn.shtwfgs.cn

JS:   a && b || !c
来源：http://xj.yuntaijiaju.cn

TS:   a && b || !c
来源：http://vr.bjjhwx.cn

Java: a && b || !c
来源：http://sr.hahajie.cn

Go:   a && b || !c
来源：http://ar.szxytkj.cn

Ruby: a && b || !c
来源：http://dj.lnxyls.cn

C#:   a && b || !c
来源：http://tv.lnxyls.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lh.szxytkj.cn

Py:   if not data: return
来源：http://ts.jctech888.com.cn

PHP:  if (!$data) { return; }
来源：http://xm.shtwfgs.cn

JS:   if (!data) return;
来源：http://yo.hnjuh.cn

TS:   if (!data) return;
来源：http://dy.huanxung.cn

Java: if (data == null) return;
来源：http://dh.shtwfgs.cn

Go:   if data == nil { return }
来源：http://re.shxzskj.cn

Ruby: return if data.nil?
来源：http://ui.shxzskj.cn

C#:   if (data == null) return;
来源：http://es.9csxet.cn

================================================================================
来源：http://wq.panjiajie.cn

C. 函数与作用域
来源：http://xf.colortex.cn

================================================================================
来源：http://nq.bjjhwx.cn

[C01] 定义函数
来源：http://fr.nicolike.cn

Py:   def add(a, b): return a + b
来源：http://ww.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ax.panjiajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://yw.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vy.shxzskj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fe.bjjhwx.cn

Go:   func add(a, b int) int { return a + b }
来源：http://tx.colortex.cn

Ruby: def add(a, b); a + b; end
来源：http://ms.muxihuayi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mc.jianghongdianzi.cn

[C02] 默认参数
来源：http://tp.chemitech.net.cn

Py:   def greet(name="World"): return name
来源：http://jo.chemitech.net.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://sc.wgjwhj.cn

JS:   function greet(name = "World") { return name; }
来源：http://po.szxytkj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fy.9csxet.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ee.panjiajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vq.huixiangedu.cn

Ruby: def greet(name = "World") = name
来源：http://zz.bookmarksfly.cn

C#:   string Greet(string name = "World") => name;
来源：http://vm.shxzukj.cn

[C03] 可变参数
来源：http://sf.huixiangedu.cn

Py:   def total(*args): return sum(args)
来源：http://bm.lnxyls.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zo.haigaiapp.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mx.wgjwhj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xn.panjiajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vo.hahajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mw.jianghongdianzi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wt.bjjhwx.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xg.shxzskj.cn

[C04] 命名参数 / 关键字参数
来源：http://pw.jianghongdianzi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ot.shtwfgs.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ki.bjjhwx.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pn.lnxyls.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dx.bjjhwx.cn

Java: // 无：用 Builder 模式或 record
来源：http://et.shtwfgs.cn

Go:   // 无：用配置结构体参数
来源：http://ti.shtwfgs.cn

Ruby: f(a: 1, b: 2)
来源：http://wi.panjiajie.cn

C#:   f(a: 1, b: 2)
来源：http://zv.newstarts.cn

[C05] 返回多个值
来源：http://tf.panjiajie.cn

Py:   return a, b
来源：http://rw.yuexingan06.cn

PHP:  return [$a, $b];
来源：http://ec.szxytkj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ho.9csxet.cn

TS:   return { a, b };
来源：http://yh.newstarts.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dz.hnjuh.cn

Go:   return a, b
来源：http://xh.gzmigu.cn

Ruby: return a, b
来源：http://ko.huanxung.cn

C#:   return (a, b);              // ValueTuple
来源：http://yw.newstarts.cn

[C06] 匿名函数 / lambda
来源：http://uk.lnxyls.cn

Py:   square = lambda x: x * x
来源：http://fc.huixiangedu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fp.chemitech.net.cn

JS:   const square = x => x * x;
来源：http://hw.szsharing.cn

TS:   const square = (x: number): number => x * x;
来源：http://uf.hnjuh.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ip.chemitech.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://tg.9csxet.cn

Ruby: square = ->(x) { x * x }
来源：http://cm.yuexingan06.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ri.yuntaijiaju.cn

[C07] 把函数作为参数传入
来源：http://mw.shxzskj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cl.yuntaijiaju.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kk.521024.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://th.nicolike.cn

TS:   arr.map(String)
来源：http://wn.hahajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ao.hahajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cs.wgjwhj.cn

Ruby: arr.map(&:upcase)
来源：http://ok.hahajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://tk.huixiangedu.cn

[C08] 闭包
来源：http://pi.szsharing.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xx.asd995.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://oh.panjiajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bx.bookmarksfly.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mb.haigaiapp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qs.wgjwhj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qf.bjjhwx.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ia.muxihuayi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bw.hnjuh.cn

[C09] 递归
来源：http://wb.bookmarksfly.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://io.yuexingan06.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://om.hnjuh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tl.bjjhwx.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dk.521024.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://aj.szsharing.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zr.nicolike.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rv.huixiangedu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ci.9csxet.cn

[C10] 变量作用域
来源：http://mq.nszjky.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tp.shxzskj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://sn.jianghongdianzi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mm.hahajie.cn

TS:   同 JS
来源：http://ve.muxihuayi.cn

Java: 方法内为块级作用域
来源：http://jr.hahajie.cn

Go:   花括号块级作用域
来源：http://vf.wgjwhj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cr.jianghongdianzi.cn


<!-- 参考信息 -->