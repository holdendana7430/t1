代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://og.szsharing.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nv.nicolike.cn

TS:   // Node.js：readline 模块
来源：http://nf.huanxung.cn

Java: new Scanner(System.in).nextLine()
来源：http://ys.shxzukj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jd.hnjuh.cn

Ruby: gets.chomp
来源：http://ww.521024.cn

C#:   Console.ReadLine();
来源：http://bt.gzmigu.cn

[A21] 保留指定小数位输出
来源：http://uw.newstarts.cn

Py:   f"{3.14159:.2f}"
来源：http://rw.muxihuayi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ed.szxytkj.cn

JS:   (3.14159).toFixed(2)
来源：http://ta.huanxung.cn

TS:   (3.14159).toFixed(2)
来源：http://wg.shxzskj.cn

Java: String.format("%.2f", 3.14159)
来源：http://cf.nszjky.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fu.gzmigu.cn

Ruby: format("%.2f", 3.14159)
来源：http://kl.jianghongdianzi.cn

C#:   3.14159.ToString("F2")
来源：http://yu.yuntaijiaju.cn

[A22] 获取字符串长度
来源：http://ee.colortex.cn

Py:   len(s)
来源：http://wg.huanxung.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cr.chemitech.net.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://sf.panjiajie.cn

TS:   s.length
来源：http://hc.nicolike.cn

Java: s.length()
来源：http://zk.bookmarksfly.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xk.chemitech.net.cn

Ruby: s.length
来源：http://am.szxytkj.cn

C#:   s.Length
来源：http://gi.colortex.cn

[A23] 大小写转换
来源：http://rp.asd995.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://in.asd995.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.muxihuayi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mg.yuntaijiaju.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dt.nszjky.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://sn.nszjky.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nn.yuexingan06.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yn.hnjuh.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qt.lnxyls.cn

[A24] 去除首尾空白
来源：http://mh.szsharing.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://px.haigaiapp.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ye.9csxet.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dp.haigaiapp.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ne.nszjky.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vo.colortex.cn

Go:   strings.TrimSpace(s)
来源：http://va.lnxyls.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://sg.bookmarksfly.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nh.9csxet.cn

[A25] 字符串比较
来源：http://hx.jctech888.com.cn

Py:   s1 == s2; s1 != s2
来源：http://vq.newstarts.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://lp.huixiangedu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wg.haigaiapp.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gx.huixiangedu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ej.hnjuh.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wo.521024.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://na.bjjhwx.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://oa.szxytkj.cn

[A26] 类型转换总览
来源：http://qd.huanxung.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://np.bjjhwx.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jn.lnxyls.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ca.jctech888.com.cn

TS:   Number() String() Boolean() x as number
来源：http://du.nicolike.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vr.gzmigu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hg.yuntaijiaju.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ex.wgjwhj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mk.shtwfgs.cn

================================================================================
来源：http://uc.yuntaijiaju.cn

B. 流程控制
来源：http://xg.panjiajie.cn

================================================================================
来源：http://zl.shxzukj.cn

[B01] 条件判断 if / else
来源：http://or.nicolike.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://cw.hahajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ni.yuntaijiaju.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ay.szsharing.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ma.nszjky.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ae.yuntaijiaju.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fn.nicolike.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fr.bookmarksfly.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://aj.yuntaijiaju.cn

[B02] 多分支 else if / elif
来源：http://ni.shtwfgs.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ji.jianghongdianzi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lu.muxihuayi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yu.muxihuayi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gp.nicolike.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ks.lnxyls.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://in.wgjwhj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ue.huixinmuqiang.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vs.huixinmuqiang.cn

[B03] switch / match / case
来源：http://by.521024.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jv.hnjuh.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xv.huixinmuqiang.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tq.szxytkj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cs.chemitech.net.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vq.wgjwhj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tx.shtwfgs.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mq.haigaiapp.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zp.521024.cn

[B04] for 计数循环
来源：http://ev.bookmarksfly.cn

Py:   for i in range(10): print(i)
来源：http://tn.shxzskj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wj.muxihuayi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hg.wgjwhj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tr.haigaiapp.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lk.wgjwhj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zc.yuntaijiaju.cn

Ruby: 10.times { |i| puts i }
来源：http://bk.yuntaijiaju.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yd.9csxet.cn

[B05] 遍历数组 / 列表
来源：http://ky.panjiajie.cn

Py:   for item in arr: print(item)
来源：http://xk.gzmigu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yd.yuexingan06.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://uz.haigaiapp.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://vg.asd995.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ae.gzmigu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ru.wgjwhj.cn

Ruby: arr.each { |item| puts item }
来源：http://ch.colortex.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hh.muxihuayi.cn

[B06] 遍历字典 / 对象
来源：http://wt.bjjhwx.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://rz.bjjhwx.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rr.jianghongdianzi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vr.bjjhwx.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yw.muxihuayi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hr.bjjhwx.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://uj.lnxyls.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qn.szsharing.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lr.nszjky.cn

[B07] while 循环
来源：http://ny.hnjuh.cn

Py:   while i < 10: i += 1
来源：http://qv.huixinmuqiang.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lu.shxzukj.cn

JS:   while (i < 10) { i++; }
来源：http://vo.yuntaijiaju.cn

TS:   while (i < 10) { i++; }
来源：http://zn.huixiangedu.cn

Java: while (i < 10) { i++; }
来源：http://ti.yuexingan06.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kn.colortex.cn

Ruby: while i < 10; i += 1; end
来源：http://xb.huanxung.cn

C#:   while (i < 10) { i++; }
来源：http://vq.muxihuayi.cn

[B08] do-while（至少执行一次）
来源：http://lj.chemitech.net.cn

Py:   # 无 do-while：用 while True + break
来源：http://jr.szsharing.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qv.bookmarksfly.cn

JS:   do { i++; } while (i < 10);
来源：http://pt.asd995.cn

TS:   do { i++; } while (i < 10);
来源：http://co.521024.cn

Java: do { i++; } while (i < 10);
来源：http://ei.szsharing.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vi.521024.cn

Ruby: begin; i += 1; end while i < 10
来源：http://gr.hahajie.cn

C#:   do { i++; } while (i < 10);
来源：http://wo.haigaiapp.cn

[B09] break 与 continue
来源：http://ss.huixinmuqiang.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rr.shxzskj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ar.yuexingan06.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sx.gzmigu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://do.yuntaijiaju.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bk.newstarts.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gs.gzmigu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ts.shxzskj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sf.bookmarksfly.cn

[B10] 遍历同时拿索引
来源：http://fe.huanxung.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mn.yuntaijiaju.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rc.szsharing.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pv.huixinmuqiang.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ob.szxytkj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vv.huixinmuqiang.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yu.haigaiapp.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wr.shtwfgs.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hh.nicolike.cn

[B11] 生成数字序列 / 区间
来源：http://mc.bjjhwx.cn

Py:   list(range(0, 10, 2))
来源：http://qd.colortex.cn

PHP:  range(0, 10, 2);
来源：http://fv.shtwfgs.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qz.bjjhwx.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dn.szsharing.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lw.huixiangedu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nb.hahajie.cn

Ruby: (0...10).step(2).to_a
来源：http://zi.haigaiapp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fh.asd995.cn

[B12] 跳出多层循环
来源：http://hy.hahajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://oo.newstarts.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://kn.bookmarksfly.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mh.bookmarksfly.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rb.521024.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wx.hnjuh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bf.huixinmuqiang.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ww.yuntaijiaju.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wk.shtwfgs.cn

[B13] 判断是否为数字
来源：http://pk.lnxyls.cn

Py:   isinstance(x, (int, float))
来源：http://ab.panjiajie.cn

PHP:  is_numeric($x)
来源：http://hm.huanxung.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gm.chemitech.net.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ob.chemitech.net.cn

Java: x instanceof Number
来源：http://uw.9csxet.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rb.szxytkj.cn

Ruby: x.is_a?(Numeric)
来源：http://wx.jctech888.com.cn

C#:   x is int or double or decimal
来源：http://zf.colortex.cn

[B14] 判断值是否在集合内
来源：http://ts.shtwfgs.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uw.shxzskj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dh.muxihuayi.cn

JS:   [1, 2, 3].includes(x)
来源：http://ou.huanxung.cn

TS:   [1, 2, 3].includes(x)
来源：http://yj.bookmarksfly.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ey.nszjky.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jk.nszjky.cn

Ruby: [1, 2, 3].include?(x)
来源：http://wv.hahajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sj.hnjuh.cn

[B15] 布尔运算与取反
来源：http://vh.jianghongdianzi.cn

Py:   a and b or not c
来源：http://nd.huixiangedu.cn

PHP:  $a && $b || !$c
来源：http://ka.hahajie.cn

JS:   a && b || !c
来源：http://ny.szsharing.cn

TS:   a && b || !c
来源：http://uy.huanxung.cn

Java: a && b || !c
来源：http://an.newstarts.cn

Go:   a && b || !c
来源：http://jl.szsharing.cn

Ruby: a && b || !c
来源：http://am.szsharing.cn

C#:   a && b || !c
来源：http://zo.lnxyls.cn

[B16] 卫语句：不满足条件提前返回
来源：http://rz.jctech888.com.cn

Py:   if not data: return
来源：http://hh.lnxyls.cn

PHP:  if (!$data) { return; }
来源：http://uw.jianghongdianzi.cn

JS:   if (!data) return;
来源：http://bc.bjjhwx.cn

TS:   if (!data) return;
来源：http://ja.shxzskj.cn

Java: if (data == null) return;
来源：http://lj.newstarts.cn

Go:   if data == nil { return }
来源：http://yp.jctech888.com.cn

Ruby: return if data.nil?
来源：http://mw.nicolike.cn

C#:   if (data == null) return;
来源：http://ea.521024.cn

================================================================================
来源：http://gj.muxihuayi.cn

C. 函数与作用域
来源：http://ff.hnjuh.cn

================================================================================
来源：http://kk.shxzukj.cn

[C01] 定义函数
来源：http://xp.shtwfgs.cn

Py:   def add(a, b): return a + b
来源：http://rw.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gp.bjjhwx.cn

JS:   function add(a, b) { return a + b; }
来源：http://jt.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xm.9csxet.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ib.yuntaijiaju.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xh.huixiangedu.cn

Ruby: def add(a, b); a + b; end
来源：http://ox.yuntaijiaju.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fb.asd995.cn

[C02] 默认参数
来源：http://qk.nszjky.cn

Py:   def greet(name="World"): return name
来源：http://dq.yuexingan06.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ns.newstarts.cn

JS:   function greet(name = "World") { return name; }
来源：http://zw.haigaiapp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ds.jianghongdianzi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qy.yuntaijiaju.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://uk.hnjuh.cn

Ruby: def greet(name = "World") = name
来源：http://pq.lnxyls.cn

C#:   string Greet(string name = "World") => name;
来源：http://cf.gzmigu.cn

[C03] 可变参数
来源：http://xr.nszjky.cn

Py:   def total(*args): return sum(args)
来源：http://al.hahajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kq.521024.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ga.hnjuh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ns.shtwfgs.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://uq.huanxung.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uk.lnxyls.cn

Ruby: def total(*nums); nums.sum; end
来源：http://em.muxihuayi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zc.jctech888.com.cn

[C04] 命名参数 / 关键字参数
来源：http://ki.nszjky.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://db.szxytkj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ug.gzmigu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ed.shxzukj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bj.jianghongdianzi.cn

Java: // 无：用 Builder 模式或 record
来源：http://ia.shtwfgs.cn

Go:   // 无：用配置结构体参数
来源：http://aj.gzmigu.cn

Ruby: f(a: 1, b: 2)
来源：http://kf.yuntaijiaju.cn

C#:   f(a: 1, b: 2)
来源：http://bc.colortex.cn

[C05] 返回多个值
来源：http://hr.muxihuayi.cn

Py:   return a, b
来源：http://xk.szxytkj.cn

PHP:  return [$a, $b];
来源：http://oo.huanxung.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://tk.haigaiapp.cn

TS:   return { a, b };
来源：http://oy.gzmigu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ys.shxzukj.cn

Go:   return a, b
来源：http://mu.jianghongdianzi.cn

Ruby: return a, b
来源：http://xy.bjjhwx.cn

C#:   return (a, b);              // ValueTuple
来源：http://sn.yuntaijiaju.cn

[C06] 匿名函数 / lambda
来源：http://ys.huixinmuqiang.cn

Py:   square = lambda x: x * x
来源：http://pp.nicolike.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ip.haigaiapp.cn

JS:   const square = x => x * x;
来源：http://zg.huixiangedu.cn

TS:   const square = (x: number): number => x * x;
来源：http://nw.jctech888.com.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lc.huanxung.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ko.hnjuh.cn

Ruby: square = ->(x) { x * x }
来源：http://lh.panjiajie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xb.521024.cn

[C07] 把函数作为参数传入
来源：http://lu.lnxyls.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sr.huixiangedu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wk.nszjky.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rw.jctech888.com.cn

TS:   arr.map(String)
来源：http://no.jctech888.com.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cy.shxzskj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rr.nszjky.cn

Ruby: arr.map(&:upcase)
来源：http://fg.szxytkj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ho.521024.cn

[C08] 闭包
来源：http://ul.shxzskj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qr.shtwfgs.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fw.hnjuh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://da.muxihuayi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sm.szsharing.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xf.huixinmuqiang.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ju.jctech888.com.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://am.yuntaijiaju.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jt.nicolike.cn

[C09] 递归
来源：http://sr.yuntaijiaju.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ak.shtwfgs.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ai.hahajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lw.panjiajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pd.shxzskj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ub.szsharing.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wg.gzmigu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://oy.szsharing.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cu.haigaiapp.cn

[C10] 变量作用域
来源：http://ac.shtwfgs.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sz.newstarts.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ee.wgjwhj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dt.jianghongdianzi.cn

TS:   同 JS
来源：http://nn.huixinmuqiang.cn

Java: 方法内为块级作用域
来源：http://mb.shxzskj.cn

Go:   花括号块级作用域
来源：http://lv.panjiajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vh.lnxyls.cn


<!-- 参考信息 -->