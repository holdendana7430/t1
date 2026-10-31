代发 wailian999

Ruby: a, b = b, a
来源：http://yr.jianghongdianzi.cn

C#:   (a, b) = (b, a);
来源：http://vg.muxihuayi.cn

[A20] 读取标准输入
来源：http://qd.panjiajie.cn

Py:   name = input("请输入：")
来源：http://lw.huixiangedu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.yuntaijiaju.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ks.huanxung.cn

TS:   // Node.js：readline 模块
来源：http://au.shtwfgs.cn

Java: new Scanner(System.in).nextLine()
来源：http://rv.yuntaijiaju.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fg.shxzskj.cn

Ruby: gets.chomp
来源：http://bl.huanxung.cn

C#:   Console.ReadLine();
来源：http://zb.chemitech.net.cn

[A21] 保留指定小数位输出
来源：http://ir.shxzskj.cn

Py:   f"{3.14159:.2f}"
来源：http://ol.jctech888.com.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xo.9csxet.cn

JS:   (3.14159).toFixed(2)
来源：http://xu.szxytkj.cn

TS:   (3.14159).toFixed(2)
来源：http://gm.9csxet.cn

Java: String.format("%.2f", 3.14159)
来源：http://gv.panjiajie.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gm.shxzukj.cn

Ruby: format("%.2f", 3.14159)
来源：http://dq.szxytkj.cn

C#:   3.14159.ToString("F2")
来源：http://nd.huixiangedu.cn

[A22] 获取字符串长度
来源：http://ym.shtwfgs.cn

Py:   len(s)
来源：http://lc.wgjwhj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hw.shxzskj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pt.wgjwhj.cn

TS:   s.length
来源：http://nq.521024.cn

Java: s.length()
来源：http://px.yuntaijiaju.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xk.yuntaijiaju.cn

Ruby: s.length
来源：http://qh.shtwfgs.cn

C#:   s.Length
来源：http://pv.yuexingan06.cn

[A23] 大小写转换
来源：http://hb.hahajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://it.jctech888.com.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ja.hnjuh.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dd.lnxyls.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hk.hnjuh.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gf.shxzukj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jb.shxzukj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://di.chemitech.net.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://yz.newstarts.cn

[A24] 去除首尾空白
来源：http://op.gzmigu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://br.panjiajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://id.9csxet.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mf.chemitech.net.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xg.chemitech.net.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://le.521024.cn

Go:   strings.TrimSpace(s)
来源：http://pa.shtwfgs.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hw.shxzskj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lb.gzmigu.cn

[A25] 字符串比较
来源：http://qb.gzmigu.cn

Py:   s1 == s2; s1 != s2
来源：http://lg.nszjky.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xr.huixiangedu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hn.yuntaijiaju.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ip.yuntaijiaju.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zp.jianghongdianzi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gf.lnxyls.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://qo.gzmigu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wn.shxzukj.cn

[A26] 类型转换总览
来源：http://hl.asd995.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vx.jctech888.com.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cb.huanxung.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gd.9csxet.cn

TS:   Number() String() Boolean() x as number
来源：http://al.yuntaijiaju.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pt.lnxyls.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sz.szxytkj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://cv.bjjhwx.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zp.shtwfgs.cn

================================================================================
来源：http://qp.szxytkj.cn

B. 流程控制
来源：http://lm.muxihuayi.cn

================================================================================
来源：http://xy.521024.cn

[B01] 条件判断 if / else
来源：http://yq.hahajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vc.hahajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ge.hnjuh.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ys.jianghongdianzi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nx.jctech888.com.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qi.haigaiapp.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://aa.newstarts.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ay.521024.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mv.hnjuh.cn

[B02] 多分支 else if / elif
来源：http://ad.newstarts.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hs.huixiangedu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rf.szsharing.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dq.bookmarksfly.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mm.jianghongdianzi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nx.hahajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gm.bookmarksfly.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qi.huixinmuqiang.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tm.lnxyls.cn

[B03] switch / match / case
来源：http://ms.nicolike.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wn.hnjuh.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pl.shxzskj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hu.haigaiapp.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qx.9csxet.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hm.hahajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hv.jctech888.com.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://up.nszjky.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dt.huixiangedu.cn

[B04] for 计数循环
来源：http://uk.jctech888.com.cn

Py:   for i in range(10): print(i)
来源：http://fc.shtwfgs.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wb.bookmarksfly.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oy.wgjwhj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vq.shtwfgs.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vk.asd995.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ik.huanxung.cn

Ruby: 10.times { |i| puts i }
来源：http://cj.haigaiapp.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ih.muxihuayi.cn

[B05] 遍历数组 / 列表
来源：http://uu.huixiangedu.cn

Py:   for item in arr: print(item)
来源：http://bb.nszjky.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://eh.hnjuh.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://su.yuntaijiaju.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ig.szsharing.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://cu.shxzukj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kq.nicolike.cn

Ruby: arr.each { |item| puts item }
来源：http://gr.nicolike.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zl.panjiajie.cn

[B06] 遍历字典 / 对象
来源：http://kw.huixiangedu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://uc.bjjhwx.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ek.huixinmuqiang.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://na.hnjuh.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ke.nicolike.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gq.yuexingan06.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jj.huixiangedu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rg.huanxung.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zd.bookmarksfly.cn

[B07] while 循环
来源：http://yv.521024.cn

Py:   while i < 10: i += 1
来源：http://ro.huanxung.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ac.huixiangedu.cn

JS:   while (i < 10) { i++; }
来源：http://zt.haigaiapp.cn

TS:   while (i < 10) { i++; }
来源：http://xk.yuexingan06.cn

Java: while (i < 10) { i++; }
来源：http://tn.yuexingan06.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ne.haigaiapp.cn

Ruby: while i < 10; i += 1; end
来源：http://sd.shxzskj.cn

C#:   while (i < 10) { i++; }
来源：http://ai.nszjky.cn

[B08] do-while（至少执行一次）
来源：http://ga.shxzukj.cn

Py:   # 无 do-while：用 while True + break
来源：http://yw.lnxyls.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://aj.chemitech.net.cn

JS:   do { i++; } while (i < 10);
来源：http://dv.newstarts.cn

TS:   do { i++; } while (i < 10);
来源：http://sr.yuexingan06.cn

Java: do { i++; } while (i < 10);
来源：http://ec.521024.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ra.jctech888.com.cn

Ruby: begin; i += 1; end while i < 10
来源：http://aq.panjiajie.cn

C#:   do { i++; } while (i < 10);
来源：http://am.lnxyls.cn

[B09] break 与 continue
来源：http://oh.yuntaijiaju.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://og.shxzskj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rr.shxzskj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ss.yuntaijiaju.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dn.nicolike.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dl.gzmigu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qg.yuntaijiaju.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://un.hahajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wf.asd995.cn

[B10] 遍历同时拿索引
来源：http://am.nicolike.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mu.huixiangedu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zi.bjjhwx.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vg.hahajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pd.huixiangedu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qf.shxzukj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://td.huixinmuqiang.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cc.hahajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://on.nszjky.cn

[B11] 生成数字序列 / 区间
来源：http://oo.szsharing.cn

Py:   list(range(0, 10, 2))
来源：http://vu.9csxet.cn

PHP:  range(0, 10, 2);
来源：http://nz.yuexingan06.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qp.asd995.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xc.colortex.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://th.szxytkj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://os.9csxet.cn

Ruby: (0...10).step(2).to_a
来源：http://jd.newstarts.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uq.yuexingan06.cn

[B12] 跳出多层循环
来源：http://yg.lnxyls.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://kn.yuexingan06.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ew.wgjwhj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jy.huixiangedu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://md.muxihuayi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xs.jctech888.com.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ag.bookmarksfly.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ws.haigaiapp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kn.jianghongdianzi.cn

[B13] 判断是否为数字
来源：http://ta.shxzskj.cn

Py:   isinstance(x, (int, float))
来源：http://qd.shxzskj.cn

PHP:  is_numeric($x)
来源：http://ul.jianghongdianzi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bk.huixinmuqiang.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://eg.szxytkj.cn

Java: x instanceof Number
来源：http://ln.nszjky.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cm.521024.cn

Ruby: x.is_a?(Numeric)
来源：http://hm.huanxung.cn

C#:   x is int or double or decimal
来源：http://qx.shxzskj.cn

[B14] 判断值是否在集合内
来源：http://ke.yuntaijiaju.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rn.chemitech.net.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ui.jctech888.com.cn

JS:   [1, 2, 3].includes(x)
来源：http://jl.yuntaijiaju.cn

TS:   [1, 2, 3].includes(x)
来源：http://jw.bjjhwx.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://yj.shxzukj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qx.521024.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gx.bjjhwx.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ti.hnjuh.cn

[B15] 布尔运算与取反
来源：http://dc.huixiangedu.cn

Py:   a and b or not c
来源：http://wm.yuntaijiaju.cn

PHP:  $a && $b || !$c
来源：http://ms.newstarts.cn

JS:   a && b || !c
来源：http://dv.szxytkj.cn

TS:   a && b || !c
来源：http://my.hnjuh.cn

Java: a && b || !c
来源：http://do.9csxet.cn

Go:   a && b || !c
来源：http://vv.huixiangedu.cn

Ruby: a && b || !c
来源：http://xx.shxzukj.cn

C#:   a && b || !c
来源：http://bg.nszjky.cn

[B16] 卫语句：不满足条件提前返回
来源：http://yp.panjiajie.cn

Py:   if not data: return
来源：http://yl.shxzskj.cn

PHP:  if (!$data) { return; }
来源：http://tw.9csxet.cn

JS:   if (!data) return;
来源：http://ct.asd995.cn

TS:   if (!data) return;
来源：http://bh.jianghongdianzi.cn

Java: if (data == null) return;
来源：http://cz.panjiajie.cn

Go:   if data == nil { return }
来源：http://bw.chemitech.net.cn

Ruby: return if data.nil?
来源：http://se.bookmarksfly.cn

C#:   if (data == null) return;
来源：http://jp.9csxet.cn

================================================================================
来源：http://ei.shxzukj.cn

C. 函数与作用域
来源：http://if.huanxung.cn

================================================================================
来源：http://rc.bookmarksfly.cn

[C01] 定义函数
来源：http://vo.hnjuh.cn

Py:   def add(a, b): return a + b
来源：http://mf.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ae.yuntaijiaju.cn

JS:   function add(a, b) { return a + b; }
来源：http://uq.szxytkj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ts.bjjhwx.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vl.szsharing.cn

Go:   func add(a, b int) int { return a + b }
来源：http://lu.haigaiapp.cn

Ruby: def add(a, b); a + b; end
来源：http://ui.asd995.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://am.521024.cn

[C02] 默认参数
来源：http://re.szxytkj.cn

Py:   def greet(name="World"): return name
来源：http://xi.jianghongdianzi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://kp.nszjky.cn

JS:   function greet(name = "World") { return name; }
来源：http://qn.shxzskj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wd.bookmarksfly.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://tw.bookmarksfly.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jj.yuexingan06.cn

Ruby: def greet(name = "World") = name
来源：http://wn.huanxung.cn

C#:   string Greet(string name = "World") => name;
来源：http://cm.haigaiapp.cn

[C03] 可变参数
来源：http://zx.chemitech.net.cn

Py:   def total(*args): return sum(args)
来源：http://kp.yuntaijiaju.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ba.jianghongdianzi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fa.jctech888.com.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ln.yuntaijiaju.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jh.jctech888.com.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yz.muxihuayi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ih.muxihuayi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://px.shxzskj.cn

[C04] 命名参数 / 关键字参数
来源：http://mq.521024.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ac.hahajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ip.lnxyls.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vq.bjjhwx.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sl.huanxung.cn

Java: // 无：用 Builder 模式或 record
来源：http://uj.gzmigu.cn

Go:   // 无：用配置结构体参数
来源：http://uy.szsharing.cn

Ruby: f(a: 1, b: 2)
来源：http://fx.yuexingan06.cn

C#:   f(a: 1, b: 2)
来源：http://hb.hahajie.cn

[C05] 返回多个值
来源：http://fp.muxihuayi.cn

Py:   return a, b
来源：http://nv.yuexingan06.cn

PHP:  return [$a, $b];
来源：http://gm.jctech888.com.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ij.hahajie.cn

TS:   return { a, b };
来源：http://vh.huanxung.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nv.521024.cn

Go:   return a, b
来源：http://xl.521024.cn

Ruby: return a, b
来源：http://jw.wgjwhj.cn

C#:   return (a, b);              // ValueTuple
来源：http://pv.yuntaijiaju.cn

[C06] 匿名函数 / lambda
来源：http://yj.huixinmuqiang.cn

Py:   square = lambda x: x * x
来源：http://cd.shxzskj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://va.nszjky.cn

JS:   const square = x => x * x;
来源：http://xa.lnxyls.cn

TS:   const square = (x: number): number => x * x;
来源：http://lr.shxzukj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ks.haigaiapp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://al.yuexingan06.cn

Ruby: square = ->(x) { x * x }
来源：http://kn.newstarts.cn

C#:   Func<int, int> square = x => x * x;
来源：http://jl.panjiajie.cn

[C07] 把函数作为参数传入
来源：http://hs.chemitech.net.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zr.szxytkj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://pe.shxzukj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://in.huanxung.cn

TS:   arr.map(String)
来源：http://np.nicolike.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cr.chemitech.net.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://va.shxzukj.cn

Ruby: arr.map(&:upcase)
来源：http://sl.bjjhwx.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://nu.lnxyls.cn

[C08] 闭包
来源：http://yl.hnjuh.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lc.hahajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lm.huanxung.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mh.szxytkj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fv.shtwfgs.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dh.nszjky.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pe.bookmarksfly.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ai.nszjky.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uh.asd995.cn

[C09] 递归
来源：http://qt.colortex.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vn.wgjwhj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xm.huixinmuqiang.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hd.jianghongdianzi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cm.yuexingan06.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ip.huixiangedu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tz.haigaiapp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://iz.nszjky.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mh.muxihuayi.cn

[C10] 变量作用域
来源：http://nk.nicolike.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sv.gzmigu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://oa.yuntaijiaju.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://as.shxzukj.cn


<!-- 参考信息 -->