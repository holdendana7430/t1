代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://sp.colortex.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wo.huixinmuqiang.cn

TS:   // Node.js：readline 模块
来源：http://bh.huanxung.cn

Java: new Scanner(System.in).nextLine()
来源：http://xs.bookmarksfly.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wx.lnxyls.cn

Ruby: gets.chomp
来源：http://nv.colortex.cn

C#:   Console.ReadLine();
来源：http://qp.hnjuh.cn

[A21] 保留指定小数位输出
来源：http://xs.9csxet.cn

Py:   f"{3.14159:.2f}"
来源：http://cm.muxihuayi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fs.nszjky.cn

JS:   (3.14159).toFixed(2)
来源：http://jq.bookmarksfly.cn

TS:   (3.14159).toFixed(2)
来源：http://jq.newstarts.cn

Java: String.format("%.2f", 3.14159)
来源：http://qq.521024.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yg.bookmarksfly.cn

Ruby: format("%.2f", 3.14159)
来源：http://ht.yuntaijiaju.cn

C#:   3.14159.ToString("F2")
来源：http://ix.colortex.cn

[A22] 获取字符串长度
来源：http://dx.huixiangedu.cn

Py:   len(s)
来源：http://qg.jctech888.com.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pz.bookmarksfly.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vm.bookmarksfly.cn

TS:   s.length
来源：http://ac.521024.cn

Java: s.length()
来源：http://lh.nicolike.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://oh.muxihuayi.cn

Ruby: s.length
来源：http://ya.szxytkj.cn

C#:   s.Length
来源：http://to.jctech888.com.cn

[A23] 大小写转换
来源：http://bu.bookmarksfly.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://nr.521024.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://tb.asd995.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fo.asd995.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qh.haigaiapp.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hm.huixiangedu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kd.wgjwhj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tb.bookmarksfly.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://op.yuntaijiaju.cn

[A24] 去除首尾空白
来源：http://fk.huanxung.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ko.hnjuh.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bh.haigaiapp.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jk.huixinmuqiang.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mb.szsharing.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vo.jianghongdianzi.cn

Go:   strings.TrimSpace(s)
来源：http://oz.nicolike.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://iu.newstarts.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ap.haigaiapp.cn

[A25] 字符串比较
来源：http://bl.521024.cn

Py:   s1 == s2; s1 != s2
来源：http://yn.bookmarksfly.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ni.jctech888.com.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://sx.muxihuayi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lj.hahajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yn.hahajie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://js.lnxyls.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://wf.lnxyls.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hh.bjjhwx.cn

[A26] 类型转换总览
来源：http://ql.jctech888.com.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zh.gzmigu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tf.szxytkj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jf.yuntaijiaju.cn

TS:   Number() String() Boolean() x as number
来源：http://ju.wgjwhj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wn.wgjwhj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jx.huanxung.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://gg.szsharing.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ea.shxzukj.cn

================================================================================
来源：http://uk.panjiajie.cn

B. 流程控制
来源：http://eq.hnjuh.cn

================================================================================
来源：http://ok.hnjuh.cn

[B01] 条件判断 if / else
来源：http://rz.haigaiapp.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vq.shxzukj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hc.nicolike.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ve.muxihuayi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lb.521024.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://iw.bjjhwx.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xq.shxzukj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gm.panjiajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pv.lnxyls.cn

[B02] 多分支 else if / elif
来源：http://za.521024.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jv.muxihuayi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qf.muxihuayi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ux.yuexingan06.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yl.jctech888.com.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tw.9csxet.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ps.shxzukj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://sm.gzmigu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vd.colortex.cn

[B03] switch / match / case
来源：http://xb.yuexingan06.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pv.9csxet.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cd.jianghongdianzi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xs.haigaiapp.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://to.lnxyls.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ik.newstarts.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wc.nszjky.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dk.panjiajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bu.haigaiapp.cn

[B04] for 计数循环
来源：http://lk.9csxet.cn

Py:   for i in range(10): print(i)
来源：http://gt.bjjhwx.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://da.nszjky.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iq.yuntaijiaju.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fo.huixinmuqiang.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yh.huixinmuqiang.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ig.yuntaijiaju.cn

Ruby: 10.times { |i| puts i }
来源：http://fq.szsharing.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://iu.huixinmuqiang.cn

[B05] 遍历数组 / 列表
来源：http://in.hnjuh.cn

Py:   for item in arr: print(item)
来源：http://ef.huanxung.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mz.yuexingan06.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qn.nszjky.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mh.huixiangedu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://mo.huixinmuqiang.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ua.yuntaijiaju.cn

Ruby: arr.each { |item| puts item }
来源：http://pl.gzmigu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ne.hahajie.cn

[B06] 遍历字典 / 对象
来源：http://rv.gzmigu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xh.nicolike.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vc.gzmigu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hg.jctech888.com.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rj.szsharing.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kb.gzmigu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://aa.shtwfgs.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gp.jianghongdianzi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ru.asd995.cn

[B07] while 循环
来源：http://nb.521024.cn

Py:   while i < 10: i += 1
来源：http://ov.hahajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://dj.gzmigu.cn

JS:   while (i < 10) { i++; }
来源：http://qn.hnjuh.cn

TS:   while (i < 10) { i++; }
来源：http://mx.hahajie.cn

Java: while (i < 10) { i++; }
来源：http://iz.shtwfgs.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ix.panjiajie.cn

Ruby: while i < 10; i += 1; end
来源：http://fo.lnxyls.cn

C#:   while (i < 10) { i++; }
来源：http://mc.521024.cn

[B08] do-while（至少执行一次）
来源：http://qk.muxihuayi.cn

Py:   # 无 do-while：用 while True + break
来源：http://vn.panjiajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://fp.colortex.cn

JS:   do { i++; } while (i < 10);
来源：http://qf.haigaiapp.cn

TS:   do { i++; } while (i < 10);
来源：http://cm.colortex.cn

Java: do { i++; } while (i < 10);
来源：http://wp.nicolike.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://zz.huanxung.cn

Ruby: begin; i += 1; end while i < 10
来源：http://da.szsharing.cn

C#:   do { i++; } while (i < 10);
来源：http://xc.9csxet.cn

[B09] break 与 continue
来源：http://th.asd995.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://de.haigaiapp.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kb.yuexingan06.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jb.newstarts.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yl.jctech888.com.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jg.jctech888.com.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qq.hahajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hr.jianghongdianzi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sx.jianghongdianzi.cn

[B10] 遍历同时拿索引
来源：http://lq.lnxyls.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rm.chemitech.net.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ri.wgjwhj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uw.szxytkj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cv.lnxyls.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qv.haigaiapp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xg.shxzskj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://df.nszjky.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jz.newstarts.cn

[B11] 生成数字序列 / 区间
来源：http://jx.shtwfgs.cn

Py:   list(range(0, 10, 2))
来源：http://no.bjjhwx.cn

PHP:  range(0, 10, 2);
来源：http://ut.9csxet.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kq.huixiangedu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aw.gzmigu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wb.hnjuh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mt.huixinmuqiang.cn

Ruby: (0...10).step(2).to_a
来源：http://jq.gzmigu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qr.muxihuayi.cn

[B12] 跳出多层循环
来源：http://pz.yuntaijiaju.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://cb.panjiajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://nr.huixinmuqiang.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zc.haigaiapp.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sl.haigaiapp.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ok.shtwfgs.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ya.9csxet.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cq.521024.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vb.gzmigu.cn

[B13] 判断是否为数字
来源：http://cl.bookmarksfly.cn

Py:   isinstance(x, (int, float))
来源：http://ei.newstarts.cn

PHP:  is_numeric($x)
来源：http://wg.hnjuh.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ld.newstarts.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sh.yuexingan06.cn

Java: x instanceof Number
来源：http://dt.muxihuayi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lo.lnxyls.cn

Ruby: x.is_a?(Numeric)
来源：http://ss.panjiajie.cn

C#:   x is int or double or decimal
来源：http://gs.jctech888.com.cn

[B14] 判断值是否在集合内
来源：http://ja.muxihuayi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ln.muxihuayi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nm.huanxung.cn

JS:   [1, 2, 3].includes(x)
来源：http://ld.shtwfgs.cn

TS:   [1, 2, 3].includes(x)
来源：http://ad.gzmigu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dp.haigaiapp.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hc.newstarts.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ci.wgjwhj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xo.shxzskj.cn

[B15] 布尔运算与取反
来源：http://wq.gzmigu.cn

Py:   a and b or not c
来源：http://pp.huanxung.cn

PHP:  $a && $b || !$c
来源：http://nw.yuntaijiaju.cn

JS:   a && b || !c
来源：http://vh.szsharing.cn

TS:   a && b || !c
来源：http://iw.panjiajie.cn

Java: a && b || !c
来源：http://vz.colortex.cn

Go:   a && b || !c
来源：http://xk.yuexingan06.cn

Ruby: a && b || !c
来源：http://vp.hnjuh.cn

C#:   a && b || !c
来源：http://ss.chemitech.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ey.szsharing.cn

Py:   if not data: return
来源：http://gm.hnjuh.cn

PHP:  if (!$data) { return; }
来源：http://gf.yuexingan06.cn

JS:   if (!data) return;
来源：http://rr.bjjhwx.cn

TS:   if (!data) return;
来源：http://nu.jianghongdianzi.cn

Java: if (data == null) return;
来源：http://wu.huixiangedu.cn

Go:   if data == nil { return }
来源：http://um.muxihuayi.cn

Ruby: return if data.nil?
来源：http://pl.wgjwhj.cn

C#:   if (data == null) return;
来源：http://dk.bookmarksfly.cn

================================================================================
来源：http://vk.szxytkj.cn

C. 函数与作用域
来源：http://vq.jctech888.com.cn

================================================================================
来源：http://nq.shxzskj.cn

[C01] 定义函数
来源：http://su.huanxung.cn

Py:   def add(a, b): return a + b
来源：http://pd.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cg.huixinmuqiang.cn

JS:   function add(a, b) { return a + b; }
来源：http://la.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dg.gzmigu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://cx.huixiangedu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://lx.szxytkj.cn

Ruby: def add(a, b); a + b; end
来源：http://um.bookmarksfly.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dp.nszjky.cn

[C02] 默认参数
来源：http://zn.gzmigu.cn

Py:   def greet(name="World"): return name
来源：http://xn.colortex.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bd.szsharing.cn

JS:   function greet(name = "World") { return name; }
来源：http://dz.yuexingan06.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ja.yuntaijiaju.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://em.huanxung.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://at.bjjhwx.cn

Ruby: def greet(name = "World") = name
来源：http://cg.haigaiapp.cn

C#:   string Greet(string name = "World") => name;
来源：http://rg.huanxung.cn

[C03] 可变参数
来源：http://ma.9csxet.cn

Py:   def total(*args): return sum(args)
来源：http://fl.wgjwhj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nm.jianghongdianzi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ye.haigaiapp.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pm.szxytkj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gr.bjjhwx.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gp.521024.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vk.lnxyls.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ja.9csxet.cn

[C04] 命名参数 / 关键字参数
来源：http://ho.lnxyls.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dy.shtwfgs.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xl.shxzukj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://du.lnxyls.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hg.hahajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://mo.shtwfgs.cn

Go:   // 无：用配置结构体参数
来源：http://tg.521024.cn

Ruby: f(a: 1, b: 2)
来源：http://mq.asd995.cn

C#:   f(a: 1, b: 2)
来源：http://wg.yuexingan06.cn

[C05] 返回多个值
来源：http://ip.bjjhwx.cn

Py:   return a, b
来源：http://rs.newstarts.cn

PHP:  return [$a, $b];
来源：http://ce.wgjwhj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://mz.huanxung.cn

TS:   return { a, b };
来源：http://jy.lnxyls.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ew.521024.cn

Go:   return a, b
来源：http://tq.gzmigu.cn

Ruby: return a, b
来源：http://fv.shxzukj.cn

C#:   return (a, b);              // ValueTuple
来源：http://ah.chemitech.net.cn

[C06] 匿名函数 / lambda
来源：http://og.colortex.cn

Py:   square = lambda x: x * x
来源：http://iu.szsharing.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ue.hahajie.cn

JS:   const square = x => x * x;
来源：http://za.lnxyls.cn

TS:   const square = (x: number): number => x * x;
来源：http://sn.muxihuayi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mj.haigaiapp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://lv.shtwfgs.cn

Ruby: square = ->(x) { x * x }
来源：http://ek.jianghongdianzi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://pa.chemitech.net.cn

[C07] 把函数作为参数传入
来源：http://xu.shtwfgs.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sw.jctech888.com.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ki.yuntaijiaju.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ep.colortex.cn

TS:   arr.map(String)
来源：http://lb.hnjuh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nz.huixinmuqiang.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hw.lnxyls.cn

Ruby: arr.map(&:upcase)
来源：http://ws.bookmarksfly.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://yo.chemitech.net.cn

[C08] 闭包
来源：http://qz.nszjky.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://km.hahajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gl.bookmarksfly.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kb.wgjwhj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lb.panjiajie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://he.bjjhwx.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ee.yuntaijiaju.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tb.gzmigu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bp.asd995.cn

[C09] 递归
来源：http://ty.lnxyls.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ok.hahajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pv.nicolike.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oo.521024.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ll.jctech888.com.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ns.hahajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jt.nszjky.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bn.huixiangedu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hq.gzmigu.cn

[C10] 变量作用域
来源：http://rt.lnxyls.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zt.chemitech.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vk.lnxyls.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://aw.asd995.cn

TS:   同 JS
来源：http://it.muxihuayi.cn

Java: 方法内为块级作用域
来源：http://ix.shtwfgs.cn

Go:   花括号块级作用域
来源：http://vi.huixiangedu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nw.wgjwhj.cn


<!-- 参考信息 -->