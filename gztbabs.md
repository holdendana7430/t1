代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://tp.huixinmuqiang.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bd.shxzskj.cn

TS:   // Node.js：readline 模块
来源：http://or.huixinmuqiang.cn

Java: new Scanner(System.in).nextLine()
来源：http://ko.wgjwhj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ce.521024.cn

Ruby: gets.chomp
来源：http://ox.shtwfgs.cn

C#:   Console.ReadLine();
来源：http://bh.bjjhwx.cn

[A21] 保留指定小数位输出
来源：http://sl.lnxyls.cn

Py:   f"{3.14159:.2f}"
来源：http://jb.panjiajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://uz.huixinmuqiang.cn

JS:   (3.14159).toFixed(2)
来源：http://ji.jctech888.com.cn

TS:   (3.14159).toFixed(2)
来源：http://hi.muxihuayi.cn

Java: String.format("%.2f", 3.14159)
来源：http://am.chemitech.net.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pn.jianghongdianzi.cn

Ruby: format("%.2f", 3.14159)
来源：http://tu.huixiangedu.cn

C#:   3.14159.ToString("F2")
来源：http://av.szxytkj.cn

[A22] 获取字符串长度
来源：http://pd.yuntaijiaju.cn

Py:   len(s)
来源：http://aq.hahajie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://iz.wgjwhj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ya.jianghongdianzi.cn

TS:   s.length
来源：http://zr.hnjuh.cn

Java: s.length()
来源：http://wy.hahajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ol.nszjky.cn

Ruby: s.length
来源：http://ev.9csxet.cn

C#:   s.Length
来源：http://bh.jianghongdianzi.cn

[A23] 大小写转换
来源：http://sd.panjiajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://tm.huanxung.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xc.bjjhwx.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dl.hnjuh.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://go.chemitech.net.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cq.hahajie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xf.shxzukj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bl.jctech888.com.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://en.gzmigu.cn

[A24] 去除首尾空白
来源：http://zd.shxzukj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://yo.hnjuh.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://om.haigaiapp.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://aw.chemitech.net.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oj.colortex.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cf.huanxung.cn

Go:   strings.TrimSpace(s)
来源：http://fu.asd995.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fz.haigaiapp.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ol.shxzskj.cn

[A25] 字符串比较
来源：http://fs.nszjky.cn

Py:   s1 == s2; s1 != s2
来源：http://fa.newstarts.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vt.521024.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pi.nicolike.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ec.9csxet.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://az.yuexingan06.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rt.nszjky.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://dm.nszjky.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://je.9csxet.cn

[A26] 类型转换总览
来源：http://zr.asd995.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xn.shxzskj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vr.szxytkj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zu.bookmarksfly.cn

TS:   Number() String() Boolean() x as number
来源：http://rv.yuntaijiaju.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kb.panjiajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pp.panjiajie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ba.chemitech.net.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://el.9csxet.cn

================================================================================
来源：http://zk.shxzskj.cn

B. 流程控制
来源：http://wu.wgjwhj.cn

================================================================================
来源：http://ac.jctech888.com.cn

[B01] 条件判断 if / else
来源：http://fx.colortex.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://br.panjiajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bu.yuexingan06.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pw.chemitech.net.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://op.huixinmuqiang.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://mf.huanxung.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wb.colortex.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yy.lnxyls.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hs.hnjuh.cn

[B02] 多分支 else if / elif
来源：http://pp.huixinmuqiang.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pq.bjjhwx.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://on.haigaiapp.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wt.newstarts.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://na.panjiajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cp.chemitech.net.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fv.szsharing.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zi.asd995.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vr.hahajie.cn

[B03] switch / match / case
来源：http://bs.hahajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ym.lnxyls.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cj.lnxyls.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kt.huanxung.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://va.nszjky.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kr.gzmigu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cg.shxzukj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ct.yuntaijiaju.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kv.lnxyls.cn

[B04] for 计数循环
来源：http://dv.szxytkj.cn

Py:   for i in range(10): print(i)
来源：http://um.lnxyls.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pb.huixinmuqiang.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tc.haigaiapp.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ky.hahajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fh.nicolike.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kq.shxzskj.cn

Ruby: 10.times { |i| puts i }
来源：http://vh.nicolike.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vx.newstarts.cn

[B05] 遍历数组 / 列表
来源：http://dn.nszjky.cn

Py:   for item in arr: print(item)
来源：http://od.shtwfgs.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ag.asd995.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gj.muxihuayi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://je.colortex.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://tq.huixiangedu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://is.colortex.cn

Ruby: arr.each { |item| puts item }
来源：http://pb.szsharing.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rw.shtwfgs.cn

[B06] 遍历字典 / 对象
来源：http://tb.wgjwhj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://gq.szxytkj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://np.muxihuayi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kx.yuexingan06.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oc.huixiangedu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://av.bookmarksfly.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zp.yuexingan06.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zi.szsharing.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jo.colortex.cn

[B07] while 循环
来源：http://tc.panjiajie.cn

Py:   while i < 10: i += 1
来源：http://ly.bjjhwx.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ow.muxihuayi.cn

JS:   while (i < 10) { i++; }
来源：http://ns.lnxyls.cn

TS:   while (i < 10) { i++; }
来源：http://pp.bjjhwx.cn

Java: while (i < 10) { i++; }
来源：http://ya.colortex.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ni.hahajie.cn

Ruby: while i < 10; i += 1; end
来源：http://mb.521024.cn

C#:   while (i < 10) { i++; }
来源：http://jx.nicolike.cn

[B08] do-while（至少执行一次）
来源：http://nz.szsharing.cn

Py:   # 无 do-while：用 while True + break
来源：http://uv.jctech888.com.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ip.muxihuayi.cn

JS:   do { i++; } while (i < 10);
来源：http://ji.shtwfgs.cn

TS:   do { i++; } while (i < 10);
来源：http://ad.bjjhwx.cn

Java: do { i++; } while (i < 10);
来源：http://nw.shtwfgs.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://in.9csxet.cn

Ruby: begin; i += 1; end while i < 10
来源：http://lp.bookmarksfly.cn

C#:   do { i++; } while (i < 10);
来源：http://dd.huixiangedu.cn

[B09] break 与 continue
来源：http://sr.shxzukj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ur.szsharing.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dk.lnxyls.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nd.muxihuayi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cr.yuexingan06.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://er.haigaiapp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yr.jianghongdianzi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ss.gzmigu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hq.nszjky.cn

[B10] 遍历同时拿索引
来源：http://hv.9csxet.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bt.colortex.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://js.szsharing.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://au.jianghongdianzi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ab.szsharing.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://er.yuexingan06.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tt.muxihuayi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fb.521024.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mh.jianghongdianzi.cn

[B11] 生成数字序列 / 区间
来源：http://gl.shtwfgs.cn

Py:   list(range(0, 10, 2))
来源：http://um.huixiangedu.cn

PHP:  range(0, 10, 2);
来源：http://jb.yuntaijiaju.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yx.jianghongdianzi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pz.lnxyls.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ei.jctech888.com.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cg.yuexingan06.cn

Ruby: (0...10).step(2).to_a
来源：http://sa.9csxet.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ae.szxytkj.cn

[B12] 跳出多层循环
来源：http://ib.muxihuayi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://um.nicolike.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ht.521024.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wp.szxytkj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://my.shxzskj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wt.huanxung.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ag.colortex.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://uv.bookmarksfly.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dm.jianghongdianzi.cn

[B13] 判断是否为数字
来源：http://aw.shtwfgs.cn

Py:   isinstance(x, (int, float))
来源：http://sb.9csxet.cn

PHP:  is_numeric($x)
来源：http://aq.bjjhwx.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://td.szxytkj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://el.muxihuayi.cn

Java: x instanceof Number
来源：http://hz.hahajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pc.huixinmuqiang.cn

Ruby: x.is_a?(Numeric)
来源：http://ih.szxytkj.cn

C#:   x is int or double or decimal
来源：http://wd.szxytkj.cn

[B14] 判断值是否在集合内
来源：http://nv.nicolike.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://iw.szxytkj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://eh.hnjuh.cn

JS:   [1, 2, 3].includes(x)
来源：http://mr.huixinmuqiang.cn

TS:   [1, 2, 3].includes(x)
来源：http://aj.szsharing.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://sb.shtwfgs.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zl.muxihuayi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://hb.asd995.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ei.9csxet.cn

[B15] 布尔运算与取反
来源：http://xf.yuntaijiaju.cn

Py:   a and b or not c
来源：http://uy.haigaiapp.cn

PHP:  $a && $b || !$c
来源：http://ut.asd995.cn

JS:   a && b || !c
来源：http://lz.9csxet.cn

TS:   a && b || !c
来源：http://bm.jianghongdianzi.cn

Java: a && b || !c
来源：http://ye.nicolike.cn

Go:   a && b || !c
来源：http://in.9csxet.cn

Ruby: a && b || !c
来源：http://jq.bjjhwx.cn

C#:   a && b || !c
来源：http://je.9csxet.cn

[B16] 卫语句：不满足条件提前返回
来源：http://nn.wgjwhj.cn

Py:   if not data: return
来源：http://hc.huanxung.cn

PHP:  if (!$data) { return; }
来源：http://kx.wgjwhj.cn

JS:   if (!data) return;
来源：http://hi.jianghongdianzi.cn

TS:   if (!data) return;
来源：http://ca.lnxyls.cn

Java: if (data == null) return;
来源：http://wj.wgjwhj.cn

Go:   if data == nil { return }
来源：http://cx.colortex.cn

Ruby: return if data.nil?
来源：http://fo.asd995.cn

C#:   if (data == null) return;
来源：http://ci.nicolike.cn

================================================================================
来源：http://co.hnjuh.cn

C. 函数与作用域
来源：http://cp.panjiajie.cn

================================================================================
来源：http://py.521024.cn

[C01] 定义函数
来源：http://ve.colortex.cn

Py:   def add(a, b): return a + b
来源：http://ss.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wo.bjjhwx.cn

JS:   function add(a, b) { return a + b; }
来源：http://wl.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://in.huixiangedu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://by.yuntaijiaju.cn

Go:   func add(a, b int) int { return a + b }
来源：http://uo.colortex.cn

Ruby: def add(a, b); a + b; end
来源：http://gc.colortex.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://le.lnxyls.cn

[C02] 默认参数
来源：http://lm.asd995.cn

Py:   def greet(name="World"): return name
来源：http://uu.panjiajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://kt.bookmarksfly.cn

JS:   function greet(name = "World") { return name; }
来源：http://bq.hahajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://eo.lnxyls.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://lg.huixiangedu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hg.yuntaijiaju.cn

Ruby: def greet(name = "World") = name
来源：http://sa.shxzukj.cn

C#:   string Greet(string name = "World") => name;
来源：http://cy.bjjhwx.cn

[C03] 可变参数
来源：http://uy.shtwfgs.cn

Py:   def total(*args): return sum(args)
来源：http://be.gzmigu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://by.szxytkj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gl.szsharing.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cp.nszjky.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mb.szxytkj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zj.asd995.cn

Ruby: def total(*nums); nums.sum; end
来源：http://cy.newstarts.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pu.nszjky.cn

[C04] 命名参数 / 关键字参数
来源：http://qp.shxzukj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hn.hnjuh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tr.jctech888.com.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wd.jctech888.com.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://iu.colortex.cn

Java: // 无：用 Builder 模式或 record
来源：http://zi.gzmigu.cn

Go:   // 无：用配置结构体参数
来源：http://wh.hnjuh.cn

Ruby: f(a: 1, b: 2)
来源：http://dj.shtwfgs.cn

C#:   f(a: 1, b: 2)
来源：http://ss.haigaiapp.cn

[C05] 返回多个值
来源：http://ij.gzmigu.cn

Py:   return a, b
来源：http://lx.hnjuh.cn

PHP:  return [$a, $b];
来源：http://qv.nszjky.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://oi.hahajie.cn

TS:   return { a, b };
来源：http://xp.hnjuh.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://km.newstarts.cn

Go:   return a, b
来源：http://bf.jianghongdianzi.cn

Ruby: return a, b
来源：http://bw.9csxet.cn

C#:   return (a, b);              // ValueTuple
来源：http://ig.bookmarksfly.cn

[C06] 匿名函数 / lambda
来源：http://od.hahajie.cn

Py:   square = lambda x: x * x
来源：http://za.colortex.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ep.asd995.cn

JS:   const square = x => x * x;
来源：http://ya.yuntaijiaju.cn

TS:   const square = (x: number): number => x * x;
来源：http://sb.jianghongdianzi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ij.hahajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ew.hnjuh.cn

Ruby: square = ->(x) { x * x }
来源：http://aq.szsharing.cn

C#:   Func<int, int> square = x => x * x;
来源：http://uj.nicolike.cn

[C07] 把函数作为参数传入
来源：http://xf.lnxyls.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gu.panjiajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://iu.521024.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mb.colortex.cn

TS:   arr.map(String)
来源：http://bi.wgjwhj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ze.gzmigu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jk.bjjhwx.cn

Ruby: arr.map(&:upcase)
来源：http://pl.hahajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gf.chemitech.net.cn

[C08] 闭包
来源：http://at.huixiangedu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wk.muxihuayi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pb.colortex.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jp.hahajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nt.521024.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wi.9csxet.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pq.hahajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://au.521024.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ui.hnjuh.cn

[C09] 递归
来源：http://lp.jianghongdianzi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tj.szsharing.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ri.chemitech.net.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://us.hahajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bl.gzmigu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yj.jianghongdianzi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ya.nszjky.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zx.shxzukj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xw.hnjuh.cn

[C10] 变量作用域
来源：http://mf.muxihuayi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jo.hahajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ax.jianghongdianzi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kz.szsharing.cn

TS:   同 JS
来源：http://iu.haigaiapp.cn

Java: 方法内为块级作用域
来源：http://la.panjiajie.cn

Go:   花括号块级作用域
来源：http://vd.gzmigu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lr.shxzukj.cn


<!-- 参考信息 -->