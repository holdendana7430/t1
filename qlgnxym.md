代发 wailian999

JS:   [a, b] = [b, a];
来源：http://as.asd995.cn

TS:   [a, b] = [b, a];
来源：http://aj.szsharing.cn

Java: int t = a; a = b; b = t;
来源：http://rc.muxihuayi.cn

Go:   a, b = b, a
来源：http://cu.hahajie.cn

Ruby: a, b = b, a
来源：http://ni.huixinmuqiang.cn

C#:   (a, b) = (b, a);
来源：http://zz.szsharing.cn

[A20] 读取标准输入
来源：http://ed.huixinmuqiang.cn

Py:   name = input("请输入：")
来源：http://do.521024.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://dy.haigaiapp.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://at.chemitech.net.cn

TS:   // Node.js：readline 模块
来源：http://ih.huixiangedu.cn

Java: new Scanner(System.in).nextLine()
来源：http://ja.haigaiapp.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://tl.bookmarksfly.cn

Ruby: gets.chomp
来源：http://wd.bookmarksfly.cn

C#:   Console.ReadLine();
来源：http://gy.lnxyls.cn

[A21] 保留指定小数位输出
来源：http://wd.colortex.cn

Py:   f"{3.14159:.2f}"
来源：http://kq.jctech888.com.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xo.huixiangedu.cn

JS:   (3.14159).toFixed(2)
来源：http://pg.huixiangedu.cn

TS:   (3.14159).toFixed(2)
来源：http://vm.chemitech.net.cn

Java: String.format("%.2f", 3.14159)
来源：http://yy.bookmarksfly.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xe.hnjuh.cn

Ruby: format("%.2f", 3.14159)
来源：http://au.newstarts.cn

C#:   3.14159.ToString("F2")
来源：http://zx.jianghongdianzi.cn

[A22] 获取字符串长度
来源：http://mf.bjjhwx.cn

Py:   len(s)
来源：http://sh.szxytkj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://sh.haigaiapp.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bq.huixinmuqiang.cn

TS:   s.length
来源：http://np.wgjwhj.cn

Java: s.length()
来源：http://pe.lnxyls.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bk.521024.cn

Ruby: s.length
来源：http://kt.nicolike.cn

C#:   s.Length
来源：http://lw.muxihuayi.cn

[A23] 大小写转换
来源：http://wb.huanxung.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://nx.hahajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://av.asd995.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ue.muxihuayi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qn.szsharing.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lj.shtwfgs.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mt.hahajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://if.yuexingan06.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qn.yuntaijiaju.cn

[A24] 去除首尾空白
来源：http://lf.bookmarksfly.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rg.asd995.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fc.chemitech.net.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sv.huanxung.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ss.shtwfgs.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ow.yuexingan06.cn

Go:   strings.TrimSpace(s)
来源：http://mu.9csxet.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gb.yuntaijiaju.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ew.bookmarksfly.cn

[A25] 字符串比较
来源：http://wy.hnjuh.cn

Py:   s1 == s2; s1 != s2
来源：http://on.hahajie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hu.huanxung.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ma.yuntaijiaju.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qp.hnjuh.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nx.szsharing.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://or.newstarts.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hl.shtwfgs.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bc.jianghongdianzi.cn

[A26] 类型转换总览
来源：http://eq.gzmigu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://em.9csxet.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qs.9csxet.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mq.szsharing.cn

TS:   Number() String() Boolean() x as number
来源：http://zr.shxzukj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zo.shxzukj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gx.shxzukj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://cv.asd995.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dl.lnxyls.cn

================================================================================
来源：http://ew.jctech888.com.cn

B. 流程控制
来源：http://ax.jianghongdianzi.cn

================================================================================
来源：http://cd.jctech888.com.cn

[B01] 条件判断 if / else
来源：http://mq.jctech888.com.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vy.9csxet.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://oa.szxytkj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dv.szsharing.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://no.szsharing.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://zj.huixiangedu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ek.bookmarksfly.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rr.huanxung.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tj.szxytkj.cn

[B02] 多分支 else if / elif
来源：http://kw.shtwfgs.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ui.jianghongdianzi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pm.yuexingan06.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gr.wgjwhj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ne.muxihuayi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kd.muxihuayi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ki.newstarts.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://of.jianghongdianzi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ha.colortex.cn

[B03] switch / match / case
来源：http://rl.bjjhwx.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kw.lnxyls.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ez.haigaiapp.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cc.shxzukj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eg.szsharing.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://is.nicolike.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xs.chemitech.net.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ab.yuexingan06.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hg.colortex.cn

[B04] for 计数循环
来源：http://gj.newstarts.cn

Py:   for i in range(10): print(i)
来源：http://ay.hahajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ow.huixiangedu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ap.huixinmuqiang.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lb.lnxyls.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ut.huixiangedu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://co.szxytkj.cn

Ruby: 10.times { |i| puts i }
来源：http://uo.nszjky.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ei.huanxung.cn

[B05] 遍历数组 / 列表
来源：http://mm.521024.cn

Py:   for item in arr: print(item)
来源：http://dk.panjiajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://eg.muxihuayi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://sf.huixiangedu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ah.yuexingan06.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://rm.shtwfgs.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wg.haigaiapp.cn

Ruby: arr.each { |item| puts item }
来源：http://ox.huixiangedu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ex.lnxyls.cn

[B06] 遍历字典 / 对象
来源：http://qd.bjjhwx.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://op.yuexingan06.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pz.newstarts.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ae.yuexingan06.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ev.jctech888.com.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cb.gzmigu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rb.muxihuayi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mm.hnjuh.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gs.chemitech.net.cn

[B07] while 循环
来源：http://ug.hnjuh.cn

Py:   while i < 10: i += 1
来源：http://ef.huixinmuqiang.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zr.huixinmuqiang.cn

JS:   while (i < 10) { i++; }
来源：http://sp.yuntaijiaju.cn

TS:   while (i < 10) { i++; }
来源：http://gh.521024.cn

Java: while (i < 10) { i++; }
来源：http://sz.shtwfgs.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ge.gzmigu.cn

Ruby: while i < 10; i += 1; end
来源：http://ew.jctech888.com.cn

C#:   while (i < 10) { i++; }
来源：http://ao.szsharing.cn

[B08] do-while（至少执行一次）
来源：http://uh.szsharing.cn

Py:   # 无 do-while：用 while True + break
来源：http://zd.bookmarksfly.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://dn.yuntaijiaju.cn

JS:   do { i++; } while (i < 10);
来源：http://rr.asd995.cn

TS:   do { i++; } while (i < 10);
来源：http://mz.jctech888.com.cn

Java: do { i++; } while (i < 10);
来源：http://fy.nszjky.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://li.shxzskj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ee.nszjky.cn

C#:   do { i++; } while (i < 10);
来源：http://mu.newstarts.cn

[B09] break 与 continue
来源：http://qv.jianghongdianzi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cx.lnxyls.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://et.asd995.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ft.jctech888.com.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bm.jctech888.com.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gz.chemitech.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sq.521024.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://df.nicolike.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jo.haigaiapp.cn

[B10] 遍历同时拿索引
来源：http://rs.colortex.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rp.jctech888.com.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yb.newstarts.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wt.jctech888.com.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vj.colortex.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mp.muxihuayi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://er.muxihuayi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wz.newstarts.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://es.521024.cn

[B11] 生成数字序列 / 区间
来源：http://mc.chemitech.net.cn

Py:   list(range(0, 10, 2))
来源：http://oz.521024.cn

PHP:  range(0, 10, 2);
来源：http://gf.shtwfgs.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://be.yuexingan06.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://le.jctech888.com.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tc.huixiangedu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ol.yuexingan06.cn

Ruby: (0...10).step(2).to_a
来源：http://dc.huanxung.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xt.haigaiapp.cn

[B12] 跳出多层循环
来源：http://db.colortex.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hj.yuexingan06.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://yq.lnxyls.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wq.yuntaijiaju.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wp.jctech888.com.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rw.colortex.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mb.yuntaijiaju.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vs.9csxet.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://oe.asd995.cn

[B13] 判断是否为数字
来源：http://bf.colortex.cn

Py:   isinstance(x, (int, float))
来源：http://tc.huixiangedu.cn

PHP:  is_numeric($x)
来源：http://hh.shtwfgs.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://al.chemitech.net.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ho.bjjhwx.cn

Java: x instanceof Number
来源：http://gy.gzmigu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ln.jianghongdianzi.cn

Ruby: x.is_a?(Numeric)
来源：http://mt.asd995.cn

C#:   x is int or double or decimal
来源：http://ve.jctech888.com.cn

[B14] 判断值是否在集合内
来源：http://fb.yuexingan06.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zb.521024.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nh.lnxyls.cn

JS:   [1, 2, 3].includes(x)
来源：http://mj.haigaiapp.cn

TS:   [1, 2, 3].includes(x)
来源：http://ng.chemitech.net.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rn.521024.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pg.nicolike.cn

Ruby: [1, 2, 3].include?(x)
来源：http://hq.chemitech.net.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ln.nicolike.cn

[B15] 布尔运算与取反
来源：http://sw.shtwfgs.cn

Py:   a and b or not c
来源：http://nh.hahajie.cn

PHP:  $a && $b || !$c
来源：http://gh.521024.cn

JS:   a && b || !c
来源：http://zi.bookmarksfly.cn

TS:   a && b || !c
来源：http://ig.hnjuh.cn

Java: a && b || !c
来源：http://rf.chemitech.net.cn

Go:   a && b || !c
来源：http://qb.huixiangedu.cn

Ruby: a && b || !c
来源：http://kx.gzmigu.cn

C#:   a && b || !c
来源：http://so.jianghongdianzi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fi.521024.cn

Py:   if not data: return
来源：http://kh.haigaiapp.cn

PHP:  if (!$data) { return; }
来源：http://db.bjjhwx.cn

JS:   if (!data) return;
来源：http://nk.wgjwhj.cn

TS:   if (!data) return;
来源：http://ky.chemitech.net.cn

Java: if (data == null) return;
来源：http://xi.muxihuayi.cn

Go:   if data == nil { return }
来源：http://jn.bookmarksfly.cn

Ruby: return if data.nil?
来源：http://hr.hnjuh.cn

C#:   if (data == null) return;
来源：http://va.bjjhwx.cn

================================================================================
来源：http://md.chemitech.net.cn

C. 函数与作用域
来源：http://lv.yuntaijiaju.cn

================================================================================
来源：http://fd.hnjuh.cn

[C01] 定义函数
来源：http://xu.9csxet.cn

Py:   def add(a, b): return a + b
来源：http://he.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eg.yuntaijiaju.cn

JS:   function add(a, b) { return a + b; }
来源：http://ic.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ok.chemitech.net.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mv.asd995.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dd.hnjuh.cn

Ruby: def add(a, b); a + b; end
来源：http://fy.bjjhwx.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sq.wgjwhj.cn

[C02] 默认参数
来源：http://tk.jianghongdianzi.cn

Py:   def greet(name="World"): return name
来源：http://fz.nszjky.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://mt.jctech888.com.cn

JS:   function greet(name = "World") { return name; }
来源：http://zf.yuntaijiaju.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://au.shxzukj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://pt.chemitech.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jr.jianghongdianzi.cn

Ruby: def greet(name = "World") = name
来源：http://gs.yuexingan06.cn

C#:   string Greet(string name = "World") => name;
来源：http://li.huixiangedu.cn

[C03] 可变参数
来源：http://ts.wgjwhj.cn

Py:   def total(*args): return sum(args)
来源：http://sd.haigaiapp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gi.szsharing.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pv.nicolike.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rf.9csxet.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jz.yuexingan06.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nd.hnjuh.cn

Ruby: def total(*nums); nums.sum; end
来源：http://oa.panjiajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rw.hahajie.cn

[C04] 命名参数 / 关键字参数
来源：http://xd.nszjky.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yh.gzmigu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qk.shtwfgs.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gr.yuexingan06.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://eq.newstarts.cn

Java: // 无：用 Builder 模式或 record
来源：http://fx.chemitech.net.cn

Go:   // 无：用配置结构体参数
来源：http://sr.szsharing.cn

Ruby: f(a: 1, b: 2)
来源：http://dw.hnjuh.cn

C#:   f(a: 1, b: 2)
来源：http://tz.9csxet.cn

[C05] 返回多个值
来源：http://es.szsharing.cn

Py:   return a, b
来源：http://fh.bookmarksfly.cn

PHP:  return [$a, $b];
来源：http://ya.huixinmuqiang.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://kd.shtwfgs.cn

TS:   return { a, b };
来源：http://mg.haigaiapp.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zu.huixiangedu.cn

Go:   return a, b
来源：http://mk.asd995.cn

Ruby: return a, b
来源：http://ns.wgjwhj.cn

C#:   return (a, b);              // ValueTuple
来源：http://nr.nszjky.cn

[C06] 匿名函数 / lambda
来源：http://ui.shxzskj.cn

Py:   square = lambda x: x * x
来源：http://na.szxytkj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://cq.szsharing.cn

JS:   const square = x => x * x;
来源：http://sm.huixinmuqiang.cn

TS:   const square = (x: number): number => x * x;
来源：http://vm.nszjky.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cj.asd995.cn

Go:   sq := func(x int) int { return x * x }
来源：http://vx.huixinmuqiang.cn

Ruby: square = ->(x) { x * x }
来源：http://mz.panjiajie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://oz.wgjwhj.cn

[C07] 把函数作为参数传入
来源：http://ga.huanxung.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ko.bookmarksfly.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bs.nszjky.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://an.huanxung.cn

TS:   arr.map(String)
来源：http://mi.9csxet.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ur.muxihuayi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ei.yuntaijiaju.cn

Ruby: arr.map(&:upcase)
来源：http://ky.521024.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cw.jianghongdianzi.cn

[C08] 闭包
来源：http://to.huixinmuqiang.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yd.asd995.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fu.asd995.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ks.bjjhwx.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hg.shtwfgs.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mm.521024.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zd.muxihuayi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hl.yuexingan06.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ki.shxzukj.cn

[C09] 递归
来源：http://fy.chemitech.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hg.asd995.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pp.huixinmuqiang.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://py.asd995.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sr.chemitech.net.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ih.huanxung.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sa.szsharing.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xb.hnjuh.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ox.chemitech.net.cn


<!-- 参考信息 -->