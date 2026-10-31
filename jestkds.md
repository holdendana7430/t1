代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://cj.szsharing.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ef.huixinmuqiang.cn

TS:   // Node.js：readline 模块
来源：http://ur.hahajie.cn

Java: new Scanner(System.in).nextLine()
来源：http://pt.huixinmuqiang.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ov.shxzskj.cn

Ruby: gets.chomp
来源：http://id.9csxet.cn

C#:   Console.ReadLine();
来源：http://dd.shtwfgs.cn

[A21] 保留指定小数位输出
来源：http://cp.nszjky.cn

Py:   f"{3.14159:.2f}"
来源：http://ki.bjjhwx.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cj.wgjwhj.cn

JS:   (3.14159).toFixed(2)
来源：http://wz.asd995.cn

TS:   (3.14159).toFixed(2)
来源：http://pg.huixiangedu.cn

Java: String.format("%.2f", 3.14159)
来源：http://ib.haigaiapp.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lg.shxzukj.cn

Ruby: format("%.2f", 3.14159)
来源：http://ig.shtwfgs.cn

C#:   3.14159.ToString("F2")
来源：http://am.9csxet.cn

[A22] 获取字符串长度
来源：http://fh.newstarts.cn

Py:   len(s)
来源：http://uh.yuexingan06.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cb.bjjhwx.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zx.muxihuayi.cn

TS:   s.length
来源：http://py.huanxung.cn

Java: s.length()
来源：http://ps.muxihuayi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://aj.jianghongdianzi.cn

Ruby: s.length
来源：http://up.gzmigu.cn

C#:   s.Length
来源：http://vy.panjiajie.cn

[A23] 大小写转换
来源：http://qz.jctech888.com.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://xd.szsharing.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://da.bookmarksfly.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kw.wgjwhj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zo.hahajie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jd.muxihuayi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sg.gzmigu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ae.chemitech.net.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://sn.szxytkj.cn

[A24] 去除首尾空白
来源：http://tr.shtwfgs.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xp.yuexingan06.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gn.wgjwhj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hp.muxihuayi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qt.shxzukj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://uw.chemitech.net.cn

Go:   strings.TrimSpace(s)
来源：http://vn.gzmigu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fp.szsharing.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kf.haigaiapp.cn

[A25] 字符串比较
来源：http://vj.hahajie.cn

Py:   s1 == s2; s1 != s2
来源：http://dk.yuntaijiaju.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fm.nszjky.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gb.shxzukj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fg.jianghongdianzi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://et.jctech888.com.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://di.shxzukj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://fm.nicolike.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gc.yuntaijiaju.cn

[A26] 类型转换总览
来源：http://cl.panjiajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ym.szsharing.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://am.jctech888.com.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://uv.521024.cn

TS:   Number() String() Boolean() x as number
来源：http://lc.lnxyls.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://am.shtwfgs.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://id.nicolike.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://us.wgjwhj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mb.hahajie.cn

================================================================================
来源：http://sr.huanxung.cn

B. 流程控制
来源：http://ba.huixiangedu.cn

================================================================================
来源：http://ff.jianghongdianzi.cn

[B01] 条件判断 if / else
来源：http://ew.521024.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ty.bookmarksfly.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vs.521024.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://la.shxzukj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://cc.shxzukj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xg.nicolike.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ga.shxzskj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://uz.bjjhwx.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tu.yuexingan06.cn

[B02] 多分支 else if / elif
来源：http://rv.shxzskj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://el.huixiangedu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ew.lnxyls.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vs.gzmigu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dh.nicolike.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yn.shxzskj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gv.jctech888.com.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://np.jctech888.com.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vd.yuexingan06.cn

[B03] switch / match / case
来源：http://ri.newstarts.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ax.szxytkj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bn.asd995.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pl.shtwfgs.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eq.szxytkj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mf.huixiangedu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hw.nszjky.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://me.huanxung.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wl.shtwfgs.cn

[B04] for 计数循环
来源：http://fd.szxytkj.cn

Py:   for i in range(10): print(i)
来源：http://pb.haigaiapp.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ma.shtwfgs.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qn.shxzskj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vk.hahajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xc.jctech888.com.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ab.asd995.cn

Ruby: 10.times { |i| puts i }
来源：http://sg.chemitech.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qy.9csxet.cn

[B05] 遍历数组 / 列表
来源：http://jq.shtwfgs.cn

Py:   for item in arr: print(item)
来源：http://ch.panjiajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yi.yuntaijiaju.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://br.shxzskj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://sj.nszjky.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://og.huixinmuqiang.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zd.jianghongdianzi.cn

Ruby: arr.each { |item| puts item }
来源：http://id.panjiajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qd.lnxyls.cn

[B06] 遍历字典 / 对象
来源：http://jj.nszjky.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://lp.colortex.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://um.521024.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uk.hahajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bz.newstarts.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://oi.shtwfgs.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hv.gzmigu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ye.shtwfgs.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jv.bjjhwx.cn

[B07] while 循环
来源：http://pl.shxzukj.cn

Py:   while i < 10: i += 1
来源：http://mh.bookmarksfly.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bw.bookmarksfly.cn

JS:   while (i < 10) { i++; }
来源：http://md.jianghongdianzi.cn

TS:   while (i < 10) { i++; }
来源：http://jd.asd995.cn

Java: while (i < 10) { i++; }
来源：http://oe.muxihuayi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lg.bookmarksfly.cn

Ruby: while i < 10; i += 1; end
来源：http://qi.huanxung.cn

C#:   while (i < 10) { i++; }
来源：http://ll.shxzukj.cn

[B08] do-while（至少执行一次）
来源：http://yu.bjjhwx.cn

Py:   # 无 do-while：用 while True + break
来源：http://yl.shxzukj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mu.panjiajie.cn

JS:   do { i++; } while (i < 10);
来源：http://lr.521024.cn

TS:   do { i++; } while (i < 10);
来源：http://xq.hahajie.cn

Java: do { i++; } while (i < 10);
来源：http://te.huixinmuqiang.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://qs.szsharing.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ys.bookmarksfly.cn

C#:   do { i++; } while (i < 10);
来源：http://xc.panjiajie.cn

[B09] break 与 continue
来源：http://qx.nicolike.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ls.521024.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ah.wgjwhj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yh.szsharing.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qj.hnjuh.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rm.yuexingan06.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fm.nszjky.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tm.szsharing.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uy.muxihuayi.cn

[B10] 遍历同时拿索引
来源：http://hq.jctech888.com.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ap.newstarts.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pk.bookmarksfly.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ff.panjiajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bz.nszjky.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wh.muxihuayi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sz.nicolike.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gs.nszjky.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kw.asd995.cn

[B11] 生成数字序列 / 区间
来源：http://kh.bookmarksfly.cn

Py:   list(range(0, 10, 2))
来源：http://wo.chemitech.net.cn

PHP:  range(0, 10, 2);
来源：http://lx.szxytkj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://id.wgjwhj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iz.shxzskj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nu.hahajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lt.colortex.cn

Ruby: (0...10).step(2).to_a
来源：http://pk.jianghongdianzi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vu.szsharing.cn

[B12] 跳出多层循环
来源：http://wm.haigaiapp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://nu.hahajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gd.shxzskj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fo.nszjky.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rk.huixinmuqiang.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://aq.gzmigu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yv.szxytkj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://aw.shtwfgs.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pd.lnxyls.cn

[B13] 判断是否为数字
来源：http://fw.colortex.cn

Py:   isinstance(x, (int, float))
来源：http://rp.jctech888.com.cn

PHP:  is_numeric($x)
来源：http://tu.yuexingan06.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kt.huixinmuqiang.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xd.lnxyls.cn

Java: x instanceof Number
来源：http://ml.asd995.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wu.huanxung.cn

Ruby: x.is_a?(Numeric)
来源：http://vc.bookmarksfly.cn

C#:   x is int or double or decimal
来源：http://fc.huixiangedu.cn

[B14] 判断值是否在集合内
来源：http://po.szsharing.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ry.hnjuh.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jh.huixinmuqiang.cn

JS:   [1, 2, 3].includes(x)
来源：http://xc.szsharing.cn

TS:   [1, 2, 3].includes(x)
来源：http://zq.huanxung.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hw.shxzskj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sn.hnjuh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zt.hahajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jf.yuntaijiaju.cn

[B15] 布尔运算与取反
来源：http://lc.haigaiapp.cn

Py:   a and b or not c
来源：http://qi.nszjky.cn

PHP:  $a && $b || !$c
来源：http://pw.asd995.cn

JS:   a && b || !c
来源：http://ko.chemitech.net.cn

TS:   a && b || !c
来源：http://ea.huixiangedu.cn

Java: a && b || !c
来源：http://zm.szxytkj.cn

Go:   a && b || !c
来源：http://dl.bjjhwx.cn

Ruby: a && b || !c
来源：http://gq.lnxyls.cn

C#:   a && b || !c
来源：http://tp.bjjhwx.cn

[B16] 卫语句：不满足条件提前返回
来源：http://td.nicolike.cn

Py:   if not data: return
来源：http://bq.huanxung.cn

PHP:  if (!$data) { return; }
来源：http://sd.panjiajie.cn

JS:   if (!data) return;
来源：http://pi.haigaiapp.cn

TS:   if (!data) return;
来源：http://oa.chemitech.net.cn

Java: if (data == null) return;
来源：http://nt.521024.cn

Go:   if data == nil { return }
来源：http://zq.bjjhwx.cn

Ruby: return if data.nil?
来源：http://tz.huanxung.cn

C#:   if (data == null) return;
来源：http://ep.shtwfgs.cn

================================================================================
来源：http://uv.shxzukj.cn

C. 函数与作用域
来源：http://an.shtwfgs.cn

================================================================================
来源：http://dy.chemitech.net.cn

[C01] 定义函数
来源：http://xh.haigaiapp.cn

Py:   def add(a, b): return a + b
来源：http://cc.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rr.hnjuh.cn

JS:   function add(a, b) { return a + b; }
来源：http://co.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://en.yuntaijiaju.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ml.wgjwhj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://lo.shxzukj.cn

Ruby: def add(a, b); a + b; end
来源：http://bt.lnxyls.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zy.asd995.cn

[C02] 默认参数
来源：http://qp.jctech888.com.cn

Py:   def greet(name="World"): return name
来源：http://kd.jianghongdianzi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ln.lnxyls.cn

JS:   function greet(name = "World") { return name; }
来源：http://ry.hahajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://mm.newstarts.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jg.gzmigu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://is.wgjwhj.cn

Ruby: def greet(name = "World") = name
来源：http://ao.yuexingan06.cn

C#:   string Greet(string name = "World") => name;
来源：http://fd.shtwfgs.cn

[C03] 可变参数
来源：http://wx.asd995.cn

Py:   def total(*args): return sum(args)
来源：http://pb.jctech888.com.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fu.bjjhwx.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ar.nicolike.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bh.asd995.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ay.chemitech.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lq.bookmarksfly.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zf.huixiangedu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jx.nszjky.cn

[C04] 命名参数 / 关键字参数
来源：http://cx.jctech888.com.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yu.szsharing.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fw.haigaiapp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mg.szsharing.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://aq.muxihuayi.cn

Java: // 无：用 Builder 模式或 record
来源：http://oj.nicolike.cn

Go:   // 无：用配置结构体参数
来源：http://jy.lnxyls.cn

Ruby: f(a: 1, b: 2)
来源：http://fv.panjiajie.cn

C#:   f(a: 1, b: 2)
来源：http://zs.nszjky.cn

[C05] 返回多个值
来源：http://mk.bookmarksfly.cn

Py:   return a, b
来源：http://ux.lnxyls.cn

PHP:  return [$a, $b];
来源：http://qu.shxzskj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ik.colortex.cn

TS:   return { a, b };
来源：http://zd.hnjuh.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bu.shxzskj.cn

Go:   return a, b
来源：http://jv.nicolike.cn

Ruby: return a, b
来源：http://wo.nicolike.cn

C#:   return (a, b);              // ValueTuple
来源：http://fe.huanxung.cn

[C06] 匿名函数 / lambda
来源：http://oq.shxzukj.cn

Py:   square = lambda x: x * x
来源：http://fs.muxihuayi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://yg.asd995.cn

JS:   const square = x => x * x;
来源：http://bc.chemitech.net.cn

TS:   const square = (x: number): number => x * x;
来源：http://ng.szxytkj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fl.szxytkj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jp.yuexingan06.cn

Ruby: square = ->(x) { x * x }
来源：http://tt.yuntaijiaju.cn

C#:   Func<int, int> square = x => x * x;
来源：http://oh.lnxyls.cn

[C07] 把函数作为参数传入
来源：http://vl.hahajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yz.yuntaijiaju.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ly.gzmigu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lg.gzmigu.cn

TS:   arr.map(String)
来源：http://nv.szsharing.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zy.szxytkj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bn.shxzukj.cn

Ruby: arr.map(&:upcase)
来源：http://gr.bookmarksfly.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ax.colortex.cn

[C08] 闭包
来源：http://ed.bookmarksfly.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tr.haigaiapp.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fe.nszjky.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://du.yuexingan06.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cx.hnjuh.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://os.newstarts.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gl.hnjuh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kc.hahajie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yy.colortex.cn

[C09] 递归
来源：http://ch.haigaiapp.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wp.nicolike.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ea.shxzskj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ab.lnxyls.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gz.shxzskj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ga.hahajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vd.9csxet.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ow.bjjhwx.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xh.lnxyls.cn

[C10] 变量作用域
来源：http://xz.szxytkj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://la.asd995.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://sf.huixiangedu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kp.wgjwhj.cn

TS:   同 JS
来源：http://gh.muxihuayi.cn

Java: 方法内为块级作用域
来源：http://ku.huixiangedu.cn

Go:   花括号块级作用域
来源：http://pw.521024.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://iu.szxytkj.cn


<!-- 参考信息 -->