代发 wailian999

Ruby: a, b = b, a
来源：http://ia.shxzskj.cn

C#:   (a, b) = (b, a);
来源：http://ki.wgjwhj.cn

[A20] 读取标准输入
来源：http://oz.jianghongdianzi.cn

Py:   name = input("请输入：")
来源：http://gc.huixinmuqiang.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://vv.haigaiapp.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://uu.9csxet.cn

TS:   // Node.js：readline 模块
来源：http://rl.nszjky.cn

Java: new Scanner(System.in).nextLine()
来源：http://pu.asd995.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://na.hahajie.cn

Ruby: gets.chomp
来源：http://mr.hahajie.cn

C#:   Console.ReadLine();
来源：http://qz.huixinmuqiang.cn

[A21] 保留指定小数位输出
来源：http://jx.yuntaijiaju.cn

Py:   f"{3.14159:.2f}"
来源：http://wz.yuntaijiaju.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jz.hnjuh.cn

JS:   (3.14159).toFixed(2)
来源：http://zr.shxzukj.cn

TS:   (3.14159).toFixed(2)
来源：http://yy.jianghongdianzi.cn

Java: String.format("%.2f", 3.14159)
来源：http://bd.shxzskj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yo.hnjuh.cn

Ruby: format("%.2f", 3.14159)
来源：http://fs.newstarts.cn

C#:   3.14159.ToString("F2")
来源：http://ss.9csxet.cn

[A22] 获取字符串长度
来源：http://wk.jianghongdianzi.cn

Py:   len(s)
来源：http://ah.yuexingan06.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://uh.szsharing.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://af.lnxyls.cn

TS:   s.length
来源：http://jj.wgjwhj.cn

Java: s.length()
来源：http://kt.shtwfgs.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fq.yuexingan06.cn

Ruby: s.length
来源：http://nh.jianghongdianzi.cn

C#:   s.Length
来源：http://nb.bookmarksfly.cn

[A23] 大小写转换
来源：http://uj.huanxung.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://md.asd995.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lp.shtwfgs.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://uj.yuntaijiaju.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ld.hnjuh.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://iq.panjiajie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://se.jianghongdianzi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://sm.asd995.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://sz.haigaiapp.cn

[A24] 去除首尾空白
来源：http://kb.9csxet.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bo.jctech888.com.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wo.wgjwhj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yl.yuexingan06.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xe.colortex.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ro.nicolike.cn

Go:   strings.TrimSpace(s)
来源：http://nw.shtwfgs.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xd.shtwfgs.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dh.shtwfgs.cn

[A25] 字符串比较
来源：http://gj.asd995.cn

Py:   s1 == s2; s1 != s2
来源：http://up.lnxyls.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://aq.szxytkj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bw.yuntaijiaju.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tt.asd995.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ya.jctech888.com.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://up.colortex.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://bm.huixiangedu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ib.asd995.cn

[A26] 类型转换总览
来源：http://mh.hnjuh.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ai.lnxyls.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://il.bjjhwx.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bb.shxzukj.cn

TS:   Number() String() Boolean() x as number
来源：http://pk.9csxet.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vo.asd995.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ct.panjiajie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://yp.9csxet.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uj.newstarts.cn

================================================================================
来源：http://yw.jianghongdianzi.cn

B. 流程控制
来源：http://kv.shxzukj.cn

================================================================================
来源：http://wj.huixinmuqiang.cn

[B01] 条件判断 if / else
来源：http://lz.hnjuh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ba.colortex.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mw.nszjky.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cp.nszjky.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ne.chemitech.net.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://jk.yuexingan06.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zx.jianghongdianzi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mt.hahajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rr.muxihuayi.cn

[B02] 多分支 else if / elif
来源：http://ku.szsharing.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kx.gzmigu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tk.gzmigu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ta.bjjhwx.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qw.colortex.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lw.huixinmuqiang.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bn.hnjuh.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fp.szsharing.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zu.huanxung.cn

[B03] switch / match / case
来源：http://rm.9csxet.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vp.newstarts.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://se.muxihuayi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ea.panjiajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sk.huixinmuqiang.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nl.muxihuayi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pc.asd995.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tm.nszjky.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tr.hnjuh.cn

[B04] for 计数循环
来源：http://ep.colortex.cn

Py:   for i in range(10): print(i)
来源：http://xv.szxytkj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pj.szsharing.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gv.huanxung.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yl.muxihuayi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fe.szxytkj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yv.nicolike.cn

Ruby: 10.times { |i| puts i }
来源：http://yl.shtwfgs.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bz.haigaiapp.cn

[B05] 遍历数组 / 列表
来源：http://lh.shxzskj.cn

Py:   for item in arr: print(item)
来源：http://lb.yuntaijiaju.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mp.colortex.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://on.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fi.nszjky.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xh.nszjky.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nw.chemitech.net.cn

Ruby: arr.each { |item| puts item }
来源：http://rx.shtwfgs.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qw.jctech888.com.cn

[B06] 遍历字典 / 对象
来源：http://vs.bookmarksfly.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://jy.hahajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ec.huanxung.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pv.jianghongdianzi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sx.9csxet.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zj.haigaiapp.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://po.lnxyls.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qt.huanxung.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zg.asd995.cn

[B07] while 循环
来源：http://iv.wgjwhj.cn

Py:   while i < 10: i += 1
来源：http://cf.szsharing.cn

PHP:  while ($i < 10) { $i++; }
来源：http://so.hnjuh.cn

JS:   while (i < 10) { i++; }
来源：http://dd.shxzukj.cn

TS:   while (i < 10) { i++; }
来源：http://tk.lnxyls.cn

Java: while (i < 10) { i++; }
来源：http://wq.huixiangedu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ad.yuntaijiaju.cn

Ruby: while i < 10; i += 1; end
来源：http://ur.szsharing.cn

C#:   while (i < 10) { i++; }
来源：http://fv.nicolike.cn

[B08] do-while（至少执行一次）
来源：http://zs.hahajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://xf.yuntaijiaju.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vb.newstarts.cn

JS:   do { i++; } while (i < 10);
来源：http://ot.huixiangedu.cn

TS:   do { i++; } while (i < 10);
来源：http://ib.nszjky.cn

Java: do { i++; } while (i < 10);
来源：http://ii.lnxyls.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://id.szxytkj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wy.bookmarksfly.cn

C#:   do { i++; } while (i < 10);
来源：http://gz.bjjhwx.cn

[B09] break 与 continue
来源：http://ej.huixiangedu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ii.huixiangedu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qy.shxzukj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bk.bookmarksfly.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://du.huixinmuqiang.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sm.haigaiapp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wx.huixinmuqiang.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qj.nicolike.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vg.yuexingan06.cn

[B10] 遍历同时拿索引
来源：http://rj.hnjuh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mu.yuexingan06.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://aw.lnxyls.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fz.chemitech.net.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ww.nszjky.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pm.haigaiapp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yt.shxzukj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gn.yuexingan06.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mc.newstarts.cn

[B11] 生成数字序列 / 区间
来源：http://qb.lnxyls.cn

Py:   list(range(0, 10, 2))
来源：http://xe.hahajie.cn

PHP:  range(0, 10, 2);
来源：http://pk.hahajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mm.muxihuayi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uq.bookmarksfly.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dn.lnxyls.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hs.muxihuayi.cn

Ruby: (0...10).step(2).to_a
来源：http://la.nicolike.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vt.lnxyls.cn

[B12] 跳出多层循环
来源：http://uv.newstarts.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://on.shxzskj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://tz.newstarts.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nu.huixiangedu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kj.szsharing.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nh.asd995.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ay.szsharing.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mp.chemitech.net.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tc.panjiajie.cn

[B13] 判断是否为数字
来源：http://lg.yuntaijiaju.cn

Py:   isinstance(x, (int, float))
来源：http://qx.jctech888.com.cn

PHP:  is_numeric($x)
来源：http://vt.haigaiapp.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qf.huanxung.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zo.hahajie.cn

Java: x instanceof Number
来源：http://os.hnjuh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fc.nszjky.cn

Ruby: x.is_a?(Numeric)
来源：http://so.szxytkj.cn

C#:   x is int or double or decimal
来源：http://qx.yuexingan06.cn

[B14] 判断值是否在集合内
来源：http://cw.jianghongdianzi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gp.bjjhwx.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://iu.bookmarksfly.cn

JS:   [1, 2, 3].includes(x)
来源：http://ty.haigaiapp.cn

TS:   [1, 2, 3].includes(x)
来源：http://dp.colortex.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kl.bookmarksfly.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://uz.9csxet.cn

Ruby: [1, 2, 3].include?(x)
来源：http://lm.haigaiapp.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://oa.panjiajie.cn

[B15] 布尔运算与取反
来源：http://st.shtwfgs.cn

Py:   a and b or not c
来源：http://wo.asd995.cn

PHP:  $a && $b || !$c
来源：http://pd.yuexingan06.cn

JS:   a && b || !c
来源：http://ur.wgjwhj.cn

TS:   a && b || !c
来源：http://fk.9csxet.cn

Java: a && b || !c
来源：http://tq.huanxung.cn

Go:   a && b || !c
来源：http://gs.jianghongdianzi.cn

Ruby: a && b || !c
来源：http://ej.jianghongdianzi.cn

C#:   a && b || !c
来源：http://jy.nszjky.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lf.shtwfgs.cn

Py:   if not data: return
来源：http://fj.nicolike.cn

PHP:  if (!$data) { return; }
来源：http://mk.shxzskj.cn

JS:   if (!data) return;
来源：http://qt.wgjwhj.cn

TS:   if (!data) return;
来源：http://gi.bjjhwx.cn

Java: if (data == null) return;
来源：http://vo.huixiangedu.cn

Go:   if data == nil { return }
来源：http://pi.newstarts.cn

Ruby: return if data.nil?
来源：http://wt.chemitech.net.cn

C#:   if (data == null) return;
来源：http://tk.huixiangedu.cn

================================================================================
来源：http://mp.chemitech.net.cn

C. 函数与作用域
来源：http://xp.shtwfgs.cn

================================================================================
来源：http://bb.gzmigu.cn

[C01] 定义函数
来源：http://co.bjjhwx.cn

Py:   def add(a, b): return a + b
来源：http://gp.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ig.shxzukj.cn

JS:   function add(a, b) { return a + b; }
来源：http://ij.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hu.wgjwhj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ht.haigaiapp.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vm.shtwfgs.cn

Ruby: def add(a, b); a + b; end
来源：http://xs.hahajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lu.gzmigu.cn

[C02] 默认参数
来源：http://le.asd995.cn

Py:   def greet(name="World"): return name
来源：http://bz.newstarts.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ez.colortex.cn

JS:   function greet(name = "World") { return name; }
来源：http://ll.shtwfgs.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ij.huixiangedu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ry.shxzukj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cb.szxytkj.cn

Ruby: def greet(name = "World") = name
来源：http://gr.panjiajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://vv.szxytkj.cn

[C03] 可变参数
来源：http://ht.shxzukj.cn

Py:   def total(*args): return sum(args)
来源：http://um.nszjky.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mx.nszjky.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xp.shtwfgs.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ma.nicolike.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ta.hahajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nu.huanxung.cn

Ruby: def total(*nums); nums.sum; end
来源：http://de.huixinmuqiang.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lr.shxzukj.cn

[C04] 命名参数 / 关键字参数
来源：http://va.huanxung.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qy.9csxet.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://id.bookmarksfly.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cm.muxihuayi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bs.yuntaijiaju.cn

Java: // 无：用 Builder 模式或 record
来源：http://qf.huanxung.cn

Go:   // 无：用配置结构体参数
来源：http://sq.muxihuayi.cn

Ruby: f(a: 1, b: 2)
来源：http://ik.colortex.cn

C#:   f(a: 1, b: 2)
来源：http://bu.yuexingan06.cn

[C05] 返回多个值
来源：http://yk.muxihuayi.cn

Py:   return a, b
来源：http://fl.szsharing.cn

PHP:  return [$a, $b];
来源：http://up.521024.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://no.nicolike.cn

TS:   return { a, b };
来源：http://is.shxzukj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rw.wgjwhj.cn

Go:   return a, b
来源：http://cd.hahajie.cn

Ruby: return a, b
来源：http://tw.lnxyls.cn

C#:   return (a, b);              // ValueTuple
来源：http://an.hahajie.cn

[C06] 匿名函数 / lambda
来源：http://mm.bookmarksfly.cn

Py:   square = lambda x: x * x
来源：http://bl.huanxung.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ih.shxzskj.cn

JS:   const square = x => x * x;
来源：http://nq.shxzukj.cn

TS:   const square = (x: number): number => x * x;
来源：http://aw.szsharing.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ge.szxytkj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jn.asd995.cn

Ruby: square = ->(x) { x * x }
来源：http://fg.yuexingan06.cn

C#:   Func<int, int> square = x => x * x;
来源：http://cp.huixinmuqiang.cn

[C07] 把函数作为参数传入
来源：http://ar.wgjwhj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ug.bookmarksfly.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ax.bookmarksfly.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cl.shxzskj.cn

TS:   arr.map(String)
来源：http://ax.chemitech.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ou.lnxyls.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tr.huixiangedu.cn

Ruby: arr.map(&:upcase)
来源：http://zi.haigaiapp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://zm.huixinmuqiang.cn

[C08] 闭包
来源：http://ty.chemitech.net.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pj.huanxung.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bk.panjiajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pi.9csxet.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bv.hahajie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://as.521024.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://om.yuntaijiaju.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ab.nszjky.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fa.colortex.cn

[C09] 递归
来源：http://xq.huixinmuqiang.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vp.yuntaijiaju.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ks.521024.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://il.yuntaijiaju.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xy.yuexingan06.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pt.gzmigu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ka.panjiajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rc.huixiangedu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ms.huixiangedu.cn

[C10] 变量作用域
来源：http://xo.szsharing.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ga.jctech888.com.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lz.huixinmuqiang.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ja.newstarts.cn


<!-- 参考信息 -->