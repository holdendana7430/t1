代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://yw.gzmigu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ka.521024.cn

TS:   // Node.js：readline 模块
来源：http://vm.521024.cn

Java: new Scanner(System.in).nextLine()
来源：http://pc.huixinmuqiang.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ta.huixiangedu.cn

Ruby: gets.chomp
来源：http://xh.chemitech.net.cn

C#:   Console.ReadLine();
来源：http://ol.asd995.cn

[A21] 保留指定小数位输出
来源：http://ks.nicolike.cn

Py:   f"{3.14159:.2f}"
来源：http://xn.huixinmuqiang.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vi.szxytkj.cn

JS:   (3.14159).toFixed(2)
来源：http://hr.9csxet.cn

TS:   (3.14159).toFixed(2)
来源：http://fx.nicolike.cn

Java: String.format("%.2f", 3.14159)
来源：http://di.panjiajie.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jo.gzmigu.cn

Ruby: format("%.2f", 3.14159)
来源：http://uu.9csxet.cn

C#:   3.14159.ToString("F2")
来源：http://mm.colortex.cn

[A22] 获取字符串长度
来源：http://sf.yuexingan06.cn

Py:   len(s)
来源：http://xh.shxzskj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://is.shtwfgs.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://og.hnjuh.cn

TS:   s.length
来源：http://qi.newstarts.cn

Java: s.length()
来源：http://ki.panjiajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ya.gzmigu.cn

Ruby: s.length
来源：http://qq.chemitech.net.cn

C#:   s.Length
来源：http://ps.huixinmuqiang.cn

[A23] 大小写转换
来源：http://cl.panjiajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://lg.newstarts.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hu.muxihuayi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jw.521024.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gg.hahajie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wv.wgjwhj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://af.szxytkj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bg.jianghongdianzi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://mz.asd995.cn

[A24] 去除首尾空白
来源：http://lt.jianghongdianzi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hc.shxzskj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ia.gzmigu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ct.shxzukj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xr.yuntaijiaju.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jy.muxihuayi.cn

Go:   strings.TrimSpace(s)
来源：http://we.gzmigu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://oo.9csxet.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cz.asd995.cn

[A25] 字符串比较
来源：http://zc.jctech888.com.cn

Py:   s1 == s2; s1 != s2
来源：http://zz.shxzskj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://lr.haigaiapp.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fb.nicolike.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bw.521024.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ut.yuexingan06.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://od.jctech888.com.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ly.lnxyls.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ln.muxihuayi.cn

[A26] 类型转换总览
来源：http://xg.shxzukj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ph.yuexingan06.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fh.jianghongdianzi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mt.muxihuayi.cn

TS:   Number() String() Boolean() x as number
来源：http://of.huanxung.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nu.szsharing.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pm.hahajie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://pg.szxytkj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cp.shxzukj.cn

================================================================================
来源：http://hc.shxzukj.cn

B. 流程控制
来源：http://aw.hahajie.cn

================================================================================
来源：http://pj.lnxyls.cn

[B01] 条件判断 if / else
来源：http://qf.asd995.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://kt.huanxung.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://je.yuntaijiaju.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://up.nszjky.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xx.wgjwhj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://uw.nszjky.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wi.jctech888.com.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mz.jianghongdianzi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vs.nszjky.cn

[B02] 多分支 else if / elif
来源：http://jc.521024.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zd.huixinmuqiang.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rb.wgjwhj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ae.wgjwhj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pg.lnxyls.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fq.chemitech.net.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hy.nicolike.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://br.haigaiapp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://of.colortex.cn

[B03] switch / match / case
来源：http://bu.huixinmuqiang.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://iz.shxzskj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sg.szsharing.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lv.newstarts.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oi.jctech888.com.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ua.nszjky.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ka.huanxung.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ar.shxzskj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dq.chemitech.net.cn

[B04] for 计数循环
来源：http://lq.szsharing.cn

Py:   for i in range(10): print(i)
来源：http://bb.521024.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pv.huixinmuqiang.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sd.huixinmuqiang.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mt.gzmigu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://km.bjjhwx.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://um.nszjky.cn

Ruby: 10.times { |i| puts i }
来源：http://ut.haigaiapp.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lm.hahajie.cn

[B05] 遍历数组 / 列表
来源：http://hc.hahajie.cn

Py:   for item in arr: print(item)
来源：http://cu.lnxyls.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pa.chemitech.net.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yr.jianghongdianzi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ts.huixinmuqiang.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://cj.521024.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ko.lnxyls.cn

Ruby: arr.each { |item| puts item }
来源：http://wp.bjjhwx.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yx.shtwfgs.cn

[B06] 遍历字典 / 对象
来源：http://sa.hnjuh.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pg.hnjuh.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.gzmigu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zd.shxzskj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wa.hnjuh.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cf.hahajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pv.hnjuh.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ar.muxihuayi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xd.huanxung.cn

[B07] while 循环
来源：http://xg.shxzskj.cn

Py:   while i < 10: i += 1
来源：http://lk.shxzukj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://pb.jianghongdianzi.cn

JS:   while (i < 10) { i++; }
来源：http://ob.newstarts.cn

TS:   while (i < 10) { i++; }
来源：http://mw.lnxyls.cn

Java: while (i < 10) { i++; }
来源：http://iw.huixiangedu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mw.wgjwhj.cn

Ruby: while i < 10; i += 1; end
来源：http://hs.wgjwhj.cn

C#:   while (i < 10) { i++; }
来源：http://pu.szxytkj.cn

[B08] do-while（至少执行一次）
来源：http://rd.huixinmuqiang.cn

Py:   # 无 do-while：用 while True + break
来源：http://js.shxzukj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://wl.jctech888.com.cn

JS:   do { i++; } while (i < 10);
来源：http://hu.521024.cn

TS:   do { i++; } while (i < 10);
来源：http://vq.muxihuayi.cn

Java: do { i++; } while (i < 10);
来源：http://zm.bjjhwx.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://tp.wgjwhj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xi.bookmarksfly.cn

C#:   do { i++; } while (i < 10);
来源：http://xy.gzmigu.cn

[B09] break 与 continue
来源：http://jj.huanxung.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gc.bjjhwx.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ix.nszjky.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ko.szxytkj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tn.yuntaijiaju.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ni.colortex.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qk.bookmarksfly.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zf.muxihuayi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zj.huixinmuqiang.cn

[B10] 遍历同时拿索引
来源：http://hg.asd995.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hc.bookmarksfly.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ue.bjjhwx.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pg.9csxet.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pw.nicolike.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yl.huixiangedu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://se.yuntaijiaju.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pn.nszjky.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yb.shxzskj.cn

[B11] 生成数字序列 / 区间
来源：http://oz.shxzukj.cn

Py:   list(range(0, 10, 2))
来源：http://ip.521024.cn

PHP:  range(0, 10, 2);
来源：http://zv.chemitech.net.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ol.lnxyls.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wn.huanxung.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gu.panjiajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ua.huanxung.cn

Ruby: (0...10).step(2).to_a
来源：http://cr.shxzukj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://oa.shxzskj.cn

[B12] 跳出多层循环
来源：http://uc.szxytkj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bz.wgjwhj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wt.bjjhwx.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tf.yuntaijiaju.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wm.521024.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dr.yuntaijiaju.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gp.huixinmuqiang.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gi.9csxet.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kz.chemitech.net.cn

[B13] 判断是否为数字
来源：http://op.yuntaijiaju.cn

Py:   isinstance(x, (int, float))
来源：http://al.colortex.cn

PHP:  is_numeric($x)
来源：http://vv.yuexingan06.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gk.gzmigu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zm.huanxung.cn

Java: x instanceof Number
来源：http://cd.9csxet.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ds.chemitech.net.cn

Ruby: x.is_a?(Numeric)
来源：http://vr.shtwfgs.cn

C#:   x is int or double or decimal
来源：http://ic.szxytkj.cn

[B14] 判断值是否在集合内
来源：http://nb.asd995.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nu.shxzskj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ha.wgjwhj.cn

JS:   [1, 2, 3].includes(x)
来源：http://ly.jctech888.com.cn

TS:   [1, 2, 3].includes(x)
来源：http://kw.hahajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gb.bookmarksfly.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ia.huanxung.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xx.lnxyls.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dn.asd995.cn

[B15] 布尔运算与取反
来源：http://xw.chemitech.net.cn

Py:   a and b or not c
来源：http://bu.muxihuayi.cn

PHP:  $a && $b || !$c
来源：http://sj.shtwfgs.cn

JS:   a && b || !c
来源：http://pg.shxzskj.cn

TS:   a && b || !c
来源：http://ql.panjiajie.cn

Java: a && b || !c
来源：http://qi.jianghongdianzi.cn

Go:   a && b || !c
来源：http://sy.nszjky.cn

Ruby: a && b || !c
来源：http://ha.colortex.cn

C#:   a && b || !c
来源：http://np.wgjwhj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ay.bjjhwx.cn

Py:   if not data: return
来源：http://ra.hnjuh.cn

PHP:  if (!$data) { return; }
来源：http://ar.nszjky.cn

JS:   if (!data) return;
来源：http://yd.9csxet.cn

TS:   if (!data) return;
来源：http://oj.shxzskj.cn

Java: if (data == null) return;
来源：http://ju.nicolike.cn

Go:   if data == nil { return }
来源：http://mj.muxihuayi.cn

Ruby: return if data.nil?
来源：http://yk.newstarts.cn

C#:   if (data == null) return;
来源：http://lb.colortex.cn

================================================================================
来源：http://vk.huixiangedu.cn

C. 函数与作用域
来源：http://ew.shtwfgs.cn

================================================================================
来源：http://ks.nicolike.cn

[C01] 定义函数
来源：http://wi.muxihuayi.cn

Py:   def add(a, b): return a + b
来源：http://ic.haigaiapp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xk.huixiangedu.cn

JS:   function add(a, b) { return a + b; }
来源：http://am.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vp.jianghongdianzi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wz.shxzskj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://id.haigaiapp.cn

Ruby: def add(a, b); a + b; end
来源：http://du.asd995.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://aa.haigaiapp.cn

[C02] 默认参数
来源：http://hx.chemitech.net.cn

Py:   def greet(name="World"): return name
来源：http://id.haigaiapp.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://os.chemitech.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://ni.szsharing.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xv.newstarts.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vf.521024.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bp.hnjuh.cn

Ruby: def greet(name = "World") = name
来源：http://xg.nicolike.cn

C#:   string Greet(string name = "World") => name;
来源：http://tc.wgjwhj.cn

[C03] 可变参数
来源：http://tl.jianghongdianzi.cn

Py:   def total(*args): return sum(args)
来源：http://uh.hahajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gu.muxihuayi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lf.yuexingan06.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bo.huanxung.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ar.huixinmuqiang.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jw.bookmarksfly.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rw.newstarts.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kf.521024.cn

[C04] 命名参数 / 关键字参数
来源：http://ri.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vs.hnjuh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hm.muxihuayi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mr.newstarts.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dx.wgjwhj.cn

Java: // 无：用 Builder 模式或 record
来源：http://gg.jctech888.com.cn

Go:   // 无：用配置结构体参数
来源：http://xp.haigaiapp.cn

Ruby: f(a: 1, b: 2)
来源：http://eg.huixinmuqiang.cn

C#:   f(a: 1, b: 2)
来源：http://ig.9csxet.cn

[C05] 返回多个值
来源：http://jy.chemitech.net.cn

Py:   return a, b
来源：http://cl.hnjuh.cn

PHP:  return [$a, $b];
来源：http://rr.szxytkj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://sd.huixiangedu.cn

TS:   return { a, b };
来源：http://dp.nszjky.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://am.newstarts.cn

Go:   return a, b
来源：http://xv.asd995.cn

Ruby: return a, b
来源：http://re.hnjuh.cn

C#:   return (a, b);              // ValueTuple
来源：http://de.yuntaijiaju.cn

[C06] 匿名函数 / lambda
来源：http://hk.yuntaijiaju.cn

Py:   square = lambda x: x * x
来源：http://jy.nicolike.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://rb.9csxet.cn

JS:   const square = x => x * x;
来源：http://it.muxihuayi.cn

TS:   const square = (x: number): number => x * x;
来源：http://ez.9csxet.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jv.bookmarksfly.cn

Go:   sq := func(x int) int { return x * x }
来源：http://go.yuntaijiaju.cn

Ruby: square = ->(x) { x * x }
来源：http://nx.yuexingan06.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bb.gzmigu.cn

[C07] 把函数作为参数传入
来源：http://fz.hahajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qk.nicolike.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hv.newstarts.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wb.muxihuayi.cn

TS:   arr.map(String)
来源：http://pl.shtwfgs.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ed.muxihuayi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://av.muxihuayi.cn

Ruby: arr.map(&:upcase)
来源：http://ce.colortex.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hu.shxzskj.cn

[C08] 闭包
来源：http://ge.shtwfgs.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://om.gzmigu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pj.colortex.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://aa.szsharing.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rt.colortex.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ab.521024.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tc.nszjky.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jj.lnxyls.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qr.asd995.cn

[C09] 递归
来源：http://nh.9csxet.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wn.szsharing.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wu.gzmigu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bz.huixinmuqiang.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fp.nszjky.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cx.wgjwhj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wj.wgjwhj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uu.jctech888.com.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yl.huixinmuqiang.cn

[C10] 变量作用域
来源：http://xp.lnxyls.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://di.asd995.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zb.shxzskj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://up.bookmarksfly.cn

TS:   同 JS
来源：http://dw.bookmarksfly.cn

Java: 方法内为块级作用域
来源：http://no.asd995.cn

Go:   花括号块级作用域
来源：http://jy.nicolike.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rw.bookmarksfly.cn


<!-- 参考信息 -->