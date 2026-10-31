代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://pq.colortex.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dl.szsharing.cn

TS:   // Node.js：readline 模块
来源：http://kh.shtwfgs.cn

Java: new Scanner(System.in).nextLine()
来源：http://rd.yuntaijiaju.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://yr.newstarts.cn

Ruby: gets.chomp
来源：http://zd.muxihuayi.cn

C#:   Console.ReadLine();
来源：http://xx.szsharing.cn

[A21] 保留指定小数位输出
来源：http://xx.521024.cn

Py:   f"{3.14159:.2f}"
来源：http://to.szxytkj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://sm.shtwfgs.cn

JS:   (3.14159).toFixed(2)
来源：http://iu.hnjuh.cn

TS:   (3.14159).toFixed(2)
来源：http://gq.lnxyls.cn

Java: String.format("%.2f", 3.14159)
来源：http://us.hnjuh.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lc.huixinmuqiang.cn

Ruby: format("%.2f", 3.14159)
来源：http://gd.shxzukj.cn

C#:   3.14159.ToString("F2")
来源：http://xo.bjjhwx.cn

[A22] 获取字符串长度
来源：http://ra.hnjuh.cn

Py:   len(s)
来源：http://vn.chemitech.net.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rx.gzmigu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://sb.jctech888.com.cn

TS:   s.length
来源：http://xv.jianghongdianzi.cn

Java: s.length()
来源：http://jc.szxytkj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pd.gzmigu.cn

Ruby: s.length
来源：http://gx.panjiajie.cn

C#:   s.Length
来源：http://gm.newstarts.cn

[A23] 大小写转换
来源：http://la.shxzukj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://uq.lnxyls.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wb.9csxet.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://og.9csxet.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xr.jctech888.com.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nf.haigaiapp.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wd.nicolike.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zv.asd995.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://su.chemitech.net.cn

[A24] 去除首尾空白
来源：http://cu.newstarts.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jj.lnxyls.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://du.gzmigu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yj.gzmigu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mu.asd995.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fr.shtwfgs.cn

Go:   strings.TrimSpace(s)
来源：http://rv.colortex.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rl.521024.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://on.muxihuayi.cn

[A25] 字符串比较
来源：http://fc.nszjky.cn

Py:   s1 == s2; s1 != s2
来源：http://dn.9csxet.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zi.colortex.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://am.jctech888.com.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jw.wgjwhj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ci.shtwfgs.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cf.nicolike.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://sq.asd995.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ir.nszjky.cn

[A26] 类型转换总览
来源：http://rw.521024.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mt.yuexingan06.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zr.nszjky.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zy.szxytkj.cn

TS:   Number() String() Boolean() x as number
来源：http://uv.shxzukj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ba.521024.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xk.yuntaijiaju.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mu.newstarts.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ap.panjiajie.cn

================================================================================
来源：http://tp.9csxet.cn

B. 流程控制
来源：http://ar.muxihuayi.cn

================================================================================
来源：http://vd.9csxet.cn

[B01] 条件判断 if / else
来源：http://lv.shxzukj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://pc.9csxet.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qk.colortex.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hw.shxzukj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://st.shtwfgs.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://sr.muxihuayi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wx.shtwfgs.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ip.hnjuh.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vd.shxzukj.cn

[B02] 多分支 else if / elif
来源：http://uu.bjjhwx.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gr.huanxung.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ei.chemitech.net.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jk.newstarts.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hx.nicolike.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rs.yuntaijiaju.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ug.szsharing.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ep.szsharing.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nh.shxzskj.cn

[B03] switch / match / case
来源：http://gf.szsharing.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xj.huixinmuqiang.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ko.huixinmuqiang.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jk.nszjky.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qw.szxytkj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://az.huixiangedu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://du.hahajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xv.newstarts.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mj.jianghongdianzi.cn

[B04] for 计数循环
来源：http://nm.hnjuh.cn

Py:   for i in range(10): print(i)
来源：http://qw.huanxung.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mi.colortex.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yh.haigaiapp.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fv.hahajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zo.newstarts.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fq.wgjwhj.cn

Ruby: 10.times { |i| puts i }
来源：http://vy.nszjky.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bv.colortex.cn

[B05] 遍历数组 / 列表
来源：http://zd.newstarts.cn

Py:   for item in arr: print(item)
来源：http://cf.huixinmuqiang.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ib.lnxyls.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://tq.shxzskj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://cn.yuexingan06.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vq.huanxung.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dr.panjiajie.cn

Ruby: arr.each { |item| puts item }
来源：http://tq.hahajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dd.bookmarksfly.cn

[B06] 遍历字典 / 对象
来源：http://cm.nicolike.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://jn.wgjwhj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tn.colortex.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oh.panjiajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ad.521024.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xr.yuntaijiaju.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://us.huixinmuqiang.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dj.nicolike.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nv.shtwfgs.cn

[B07] while 循环
来源：http://lf.jianghongdianzi.cn

Py:   while i < 10: i += 1
来源：http://ny.huixinmuqiang.cn

PHP:  while ($i < 10) { $i++; }
来源：http://at.shtwfgs.cn

JS:   while (i < 10) { i++; }
来源：http://dk.huixiangedu.cn

TS:   while (i < 10) { i++; }
来源：http://td.bookmarksfly.cn

Java: while (i < 10) { i++; }
来源：http://hg.gzmigu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ll.shxzukj.cn

Ruby: while i < 10; i += 1; end
来源：http://ko.chemitech.net.cn

C#:   while (i < 10) { i++; }
来源：http://xf.newstarts.cn

[B08] do-while（至少执行一次）
来源：http://fj.jianghongdianzi.cn

Py:   # 无 do-while：用 while True + break
来源：http://ko.newstarts.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cx.bjjhwx.cn

JS:   do { i++; } while (i < 10);
来源：http://gr.wgjwhj.cn

TS:   do { i++; } while (i < 10);
来源：http://gg.huanxung.cn

Java: do { i++; } while (i < 10);
来源：http://go.haigaiapp.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sx.521024.cn

Ruby: begin; i += 1; end while i < 10
来源：http://up.chemitech.net.cn

C#:   do { i++; } while (i < 10);
来源：http://cx.chemitech.net.cn

[B09] break 与 continue
来源：http://zj.nszjky.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://co.asd995.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hf.panjiajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dv.szsharing.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oo.yuexingan06.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wn.muxihuayi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://oc.bjjhwx.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sw.nicolike.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zr.shtwfgs.cn

[B10] 遍历同时拿索引
来源：http://yf.colortex.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jk.huixiangedu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fp.huanxung.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://iz.huixiangedu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xk.lnxyls.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://px.bookmarksfly.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wa.szxytkj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://li.hahajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qw.wgjwhj.cn

[B11] 生成数字序列 / 区间
来源：http://du.huixinmuqiang.cn

Py:   list(range(0, 10, 2))
来源：http://yx.szsharing.cn

PHP:  range(0, 10, 2);
来源：http://df.szsharing.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uh.huixinmuqiang.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zw.lnxyls.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cg.lnxyls.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lb.yuntaijiaju.cn

Ruby: (0...10).step(2).to_a
来源：http://xm.lnxyls.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rl.szxytkj.cn

[B12] 跳出多层循环
来源：http://bb.huixinmuqiang.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://gj.hnjuh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://xe.bjjhwx.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ti.chemitech.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jq.asd995.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ok.asd995.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uz.haigaiapp.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jo.szxytkj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://up.lnxyls.cn

[B13] 判断是否为数字
来源：http://vc.huanxung.cn

Py:   isinstance(x, (int, float))
来源：http://au.bjjhwx.cn

PHP:  is_numeric($x)
来源：http://ve.hnjuh.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yb.huanxung.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ai.muxihuayi.cn

Java: x instanceof Number
来源：http://vn.huixiangedu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cu.newstarts.cn

Ruby: x.is_a?(Numeric)
来源：http://ia.521024.cn

C#:   x is int or double or decimal
来源：http://he.jianghongdianzi.cn

[B14] 判断值是否在集合内
来源：http://ls.gzmigu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fs.9csxet.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dw.szxytkj.cn

JS:   [1, 2, 3].includes(x)
来源：http://fu.huixinmuqiang.cn

TS:   [1, 2, 3].includes(x)
来源：http://yo.jctech888.com.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://eo.szsharing.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fa.hnjuh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://br.szxytkj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vw.shxzskj.cn

[B15] 布尔运算与取反
来源：http://pv.szxytkj.cn

Py:   a and b or not c
来源：http://wh.nszjky.cn

PHP:  $a && $b || !$c
来源：http://rh.jctech888.com.cn

JS:   a && b || !c
来源：http://or.newstarts.cn

TS:   a && b || !c
来源：http://ys.nszjky.cn

Java: a && b || !c
来源：http://sa.yuntaijiaju.cn

Go:   a && b || !c
来源：http://wk.huixiangedu.cn

Ruby: a && b || !c
来源：http://fi.asd995.cn

C#:   a && b || !c
来源：http://mp.lnxyls.cn

[B16] 卫语句：不满足条件提前返回
来源：http://nk.521024.cn

Py:   if not data: return
来源：http://bd.haigaiapp.cn

PHP:  if (!$data) { return; }
来源：http://gu.wgjwhj.cn

JS:   if (!data) return;
来源：http://vc.colortex.cn

TS:   if (!data) return;
来源：http://ua.jianghongdianzi.cn

Java: if (data == null) return;
来源：http://nb.gzmigu.cn

Go:   if data == nil { return }
来源：http://jm.szsharing.cn

Ruby: return if data.nil?
来源：http://pk.bjjhwx.cn

C#:   if (data == null) return;
来源：http://gc.wgjwhj.cn

================================================================================
来源：http://cw.huixinmuqiang.cn

C. 函数与作用域
来源：http://ox.shxzskj.cn

================================================================================
来源：http://jb.szsharing.cn

[C01] 定义函数
来源：http://id.huixiangedu.cn

Py:   def add(a, b): return a + b
来源：http://ik.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zx.huixiangedu.cn

JS:   function add(a, b) { return a + b; }
来源：http://vk.yuexingan06.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ht.panjiajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mg.bookmarksfly.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xc.szxytkj.cn

Ruby: def add(a, b); a + b; end
来源：http://xt.bookmarksfly.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://om.bjjhwx.cn

[C02] 默认参数
来源：http://uc.hahajie.cn

Py:   def greet(name="World"): return name
来源：http://ae.gzmigu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ev.haigaiapp.cn

JS:   function greet(name = "World") { return name; }
来源：http://mx.nszjky.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gg.shtwfgs.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://kw.szxytkj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ap.gzmigu.cn

Ruby: def greet(name = "World") = name
来源：http://hc.gzmigu.cn

C#:   string Greet(string name = "World") => name;
来源：http://as.newstarts.cn

[C03] 可变参数
来源：http://ul.chemitech.net.cn

Py:   def total(*args): return sum(args)
来源：http://xu.szsharing.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dh.colortex.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yh.shxzskj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jl.chemitech.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gg.gzmigu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ix.huixinmuqiang.cn

Ruby: def total(*nums); nums.sum; end
来源：http://or.chemitech.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://af.shtwfgs.cn

[C04] 命名参数 / 关键字参数
来源：http://og.9csxet.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mv.huixiangedu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gr.szsharing.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ap.bjjhwx.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mu.hahajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://em.shxzukj.cn

Go:   // 无：用配置结构体参数
来源：http://bm.bookmarksfly.cn

Ruby: f(a: 1, b: 2)
来源：http://ti.9csxet.cn

C#:   f(a: 1, b: 2)
来源：http://aq.newstarts.cn

[C05] 返回多个值
来源：http://rz.hnjuh.cn

Py:   return a, b
来源：http://bh.bjjhwx.cn

PHP:  return [$a, $b];
来源：http://ws.haigaiapp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://db.szsharing.cn

TS:   return { a, b };
来源：http://fo.nszjky.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lz.yuexingan06.cn

Go:   return a, b
来源：http://ky.shxzskj.cn

Ruby: return a, b
来源：http://fw.haigaiapp.cn

C#:   return (a, b);              // ValueTuple
来源：http://us.yuexingan06.cn

[C06] 匿名函数 / lambda
来源：http://ea.haigaiapp.cn

Py:   square = lambda x: x * x
来源：http://ih.huixiangedu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://hy.hnjuh.cn

JS:   const square = x => x * x;
来源：http://ma.jianghongdianzi.cn

TS:   const square = (x: number): number => x * x;
来源：http://fx.yuntaijiaju.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nu.shxzskj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://th.huanxung.cn

Ruby: square = ->(x) { x * x }
来源：http://ei.huixiangedu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ga.hnjuh.cn

[C07] 把函数作为参数传入
来源：http://py.jianghongdianzi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mx.panjiajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://lw.newstarts.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pi.nszjky.cn

TS:   arr.map(String)
来源：http://js.bjjhwx.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mt.muxihuayi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wd.newstarts.cn

Ruby: arr.map(&:upcase)
来源：http://kx.szsharing.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://iy.muxihuayi.cn

[C08] 闭包
来源：http://jv.gzmigu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uu.newstarts.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mq.wgjwhj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ch.newstarts.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qk.jctech888.com.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jc.newstarts.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ag.shxzskj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ab.jianghongdianzi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cw.huixinmuqiang.cn

[C09] 递归
来源：http://cd.shtwfgs.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ll.bjjhwx.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ls.szsharing.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sv.szsharing.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bv.huanxung.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ny.huixinmuqiang.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vg.szsharing.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xl.chemitech.net.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cu.huixinmuqiang.cn

[C10] 变量作用域
来源：http://zn.yuexingan06.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ac.bjjhwx.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://my.nszjky.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qi.hahajie.cn

TS:   同 JS
来源：http://zc.bjjhwx.cn

Java: 方法内为块级作用域
来源：http://wq.haigaiapp.cn

Go:   花括号块级作用域
来源：http://cy.9csxet.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tz.nszjky.cn


<!-- 参考信息 -->