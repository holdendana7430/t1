代发 wailian999

C#:   (int)'A'; (char)65
来源：http://dc.asd995.cn

[A19] 交换两个变量
来源：http://xq.haigaiapp.cn

Py:   a, b = b, a
来源：http://pd.colortex.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://oc.chemitech.net.cn

JS:   [a, b] = [b, a];
来源：http://hp.hahajie.cn

TS:   [a, b] = [b, a];
来源：http://cm.asd995.cn

Java: int t = a; a = b; b = t;
来源：http://xb.gzmigu.cn

Go:   a, b = b, a
来源：http://kt.panjiajie.cn

Ruby: a, b = b, a
来源：http://uv.huixiangedu.cn

C#:   (a, b) = (b, a);
来源：http://lc.muxihuayi.cn

[A20] 读取标准输入
来源：http://pa.gzmigu.cn

Py:   name = input("请输入：")
来源：http://ub.jianghongdianzi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://th.nicolike.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://sm.nszjky.cn

TS:   // Node.js：readline 模块
来源：http://iy.gzmigu.cn

Java: new Scanner(System.in).nextLine()
来源：http://gq.huixiangedu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dr.nicolike.cn

Ruby: gets.chomp
来源：http://uj.wgjwhj.cn

C#:   Console.ReadLine();
来源：http://oa.521024.cn

[A21] 保留指定小数位输出
来源：http://kh.bookmarksfly.cn

Py:   f"{3.14159:.2f}"
来源：http://ge.yuntaijiaju.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://lo.szsharing.cn

JS:   (3.14159).toFixed(2)
来源：http://cv.yuntaijiaju.cn

TS:   (3.14159).toFixed(2)
来源：http://tk.bjjhwx.cn

Java: String.format("%.2f", 3.14159)
来源：http://qj.haigaiapp.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ny.huixiangedu.cn

Ruby: format("%.2f", 3.14159)
来源：http://qr.nicolike.cn

C#:   3.14159.ToString("F2")
来源：http://vr.hahajie.cn

[A22] 获取字符串长度
来源：http://iy.hahajie.cn

Py:   len(s)
来源：http://sa.asd995.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cc.shxzskj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wi.gzmigu.cn

TS:   s.length
来源：http://rv.muxihuayi.cn

Java: s.length()
来源：http://lo.521024.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mx.hahajie.cn

Ruby: s.length
来源：http://ht.jctech888.com.cn

C#:   s.Length
来源：http://qh.wgjwhj.cn

[A23] 大小写转换
来源：http://zq.nszjky.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://on.huixinmuqiang.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gj.huixiangedu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nm.521024.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hs.shtwfgs.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fk.shxzukj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ia.muxihuayi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lo.hahajie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zy.chemitech.net.cn

[A24] 去除首尾空白
来源：http://ce.newstarts.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://yg.panjiajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://oa.yuntaijiaju.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jk.wgjwhj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ih.jianghongdianzi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fw.gzmigu.cn

Go:   strings.TrimSpace(s)
来源：http://az.shtwfgs.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xr.panjiajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hj.huixiangedu.cn

[A25] 字符串比较
来源：http://sy.hnjuh.cn

Py:   s1 == s2; s1 != s2
来源：http://ib.szxytkj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wa.asd995.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ji.colortex.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hv.huanxung.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nf.muxihuayi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qc.haigaiapp.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hp.bjjhwx.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tv.wgjwhj.cn

[A26] 类型转换总览
来源：http://af.shxzskj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xc.521024.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ln.muxihuayi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ws.szxytkj.cn

TS:   Number() String() Boolean() x as number
来源：http://lx.nicolike.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ot.9csxet.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pb.haigaiapp.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://pq.colortex.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pp.newstarts.cn

================================================================================
来源：http://dr.hahajie.cn

B. 流程控制
来源：http://ez.shxzskj.cn

================================================================================
来源：http://ro.bookmarksfly.cn

[B01] 条件判断 if / else
来源：http://oe.hnjuh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ym.shtwfgs.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xc.gzmigu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qe.shxzskj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://iu.szxytkj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ow.szxytkj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fv.hnjuh.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vj.colortex.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vv.asd995.cn

[B02] 多分支 else if / elif
来源：http://ap.jctech888.com.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tq.bookmarksfly.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nt.jianghongdianzi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kq.wgjwhj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ij.yuntaijiaju.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kj.bookmarksfly.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://oj.panjiajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ah.shtwfgs.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dm.yuexingan06.cn

[B03] switch / match / case
来源：http://rg.yuntaijiaju.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mt.colortex.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tw.521024.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://og.jctech888.com.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rx.szxytkj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://md.huanxung.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nf.asd995.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gx.bjjhwx.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://is.huanxung.cn

[B04] for 计数循环
来源：http://hz.chemitech.net.cn

Py:   for i in range(10): print(i)
来源：http://ox.nszjky.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jd.shtwfgs.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jp.huixinmuqiang.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pv.huixinmuqiang.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lm.huixiangedu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hd.shxzskj.cn

Ruby: 10.times { |i| puts i }
来源：http://eu.lnxyls.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wd.wgjwhj.cn

[B05] 遍历数组 / 列表
来源：http://ql.shxzskj.cn

Py:   for item in arr: print(item)
来源：http://fe.colortex.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://no.jianghongdianzi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://mb.wgjwhj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://nh.nszjky.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ks.hnjuh.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tx.jctech888.com.cn

Ruby: arr.each { |item| puts item }
来源：http://ls.yuntaijiaju.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://au.colortex.cn

[B06] 遍历字典 / 对象
来源：http://ys.haigaiapp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://uu.haigaiapp.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://up.bjjhwx.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xa.jctech888.com.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ab.szxytkj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://et.newstarts.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qi.lnxyls.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ha.bjjhwx.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yp.jctech888.com.cn

[B07] while 循环
来源：http://rb.colortex.cn

Py:   while i < 10: i += 1
来源：http://ny.szsharing.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qq.nszjky.cn

JS:   while (i < 10) { i++; }
来源：http://sa.jianghongdianzi.cn

TS:   while (i < 10) { i++; }
来源：http://lf.nicolike.cn

Java: while (i < 10) { i++; }
来源：http://ih.colortex.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jb.haigaiapp.cn

Ruby: while i < 10; i += 1; end
来源：http://kt.jctech888.com.cn

C#:   while (i < 10) { i++; }
来源：http://gf.shtwfgs.cn

[B08] do-while（至少执行一次）
来源：http://ig.jianghongdianzi.cn

Py:   # 无 do-while：用 while True + break
来源：http://cc.jctech888.com.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://lx.nszjky.cn

JS:   do { i++; } while (i < 10);
来源：http://qq.jianghongdianzi.cn

TS:   do { i++; } while (i < 10);
来源：http://on.asd995.cn

Java: do { i++; } while (i < 10);
来源：http://rx.shxzukj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ks.hnjuh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cx.yuntaijiaju.cn

C#:   do { i++; } while (i < 10);
来源：http://ap.asd995.cn

[B09] break 与 continue
来源：http://oc.bjjhwx.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ym.szsharing.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://as.hahajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mz.nicolike.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gz.panjiajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tx.9csxet.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wg.lnxyls.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fc.bookmarksfly.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zv.yuexingan06.cn

[B10] 遍历同时拿索引
来源：http://vp.bookmarksfly.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://uk.haigaiapp.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fo.521024.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jl.huanxung.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vr.szxytkj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kr.yuexingan06.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jj.colortex.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ol.bookmarksfly.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pe.newstarts.cn

[B11] 生成数字序列 / 区间
来源：http://on.wgjwhj.cn

Py:   list(range(0, 10, 2))
来源：http://sn.hahajie.cn

PHP:  range(0, 10, 2);
来源：http://lc.muxihuayi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hu.huixinmuqiang.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xp.hahajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://eq.chemitech.net.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hv.shxzukj.cn

Ruby: (0...10).step(2).to_a
来源：http://gc.hnjuh.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sf.huixiangedu.cn

[B12] 跳出多层循环
来源：http://nz.gzmigu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ui.huixiangedu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://pq.jianghongdianzi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mq.haigaiapp.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://by.chemitech.net.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wr.haigaiapp.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ma.gzmigu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dy.colortex.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gc.lnxyls.cn

[B13] 判断是否为数字
来源：http://xz.shtwfgs.cn

Py:   isinstance(x, (int, float))
来源：http://ta.newstarts.cn

PHP:  is_numeric($x)
来源：http://xd.shxzukj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dd.shtwfgs.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kg.yuntaijiaju.cn

Java: x instanceof Number
来源：http://su.wgjwhj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qu.jianghongdianzi.cn

Ruby: x.is_a?(Numeric)
来源：http://hu.shtwfgs.cn

C#:   x is int or double or decimal
来源：http://mi.jctech888.com.cn

[B14] 判断值是否在集合内
来源：http://ri.huixinmuqiang.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wr.panjiajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yn.shxzukj.cn

JS:   [1, 2, 3].includes(x)
来源：http://it.hnjuh.cn

TS:   [1, 2, 3].includes(x)
来源：http://oq.huixiangedu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dg.bookmarksfly.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jy.newstarts.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rr.huixinmuqiang.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dj.newstarts.cn

[B15] 布尔运算与取反
来源：http://xy.9csxet.cn

Py:   a and b or not c
来源：http://qu.asd995.cn

PHP:  $a && $b || !$c
来源：http://wa.haigaiapp.cn

JS:   a && b || !c
来源：http://ik.jctech888.com.cn

TS:   a && b || !c
来源：http://iu.huixinmuqiang.cn

Java: a && b || !c
来源：http://hy.jctech888.com.cn

Go:   a && b || !c
来源：http://zm.lnxyls.cn

Ruby: a && b || !c
来源：http://qr.lnxyls.cn

C#:   a && b || !c
来源：http://uc.newstarts.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qa.bookmarksfly.cn

Py:   if not data: return
来源：http://we.huanxung.cn

PHP:  if (!$data) { return; }
来源：http://oi.jctech888.com.cn

JS:   if (!data) return;
来源：http://yn.shxzskj.cn

TS:   if (!data) return;
来源：http://hs.colortex.cn

Java: if (data == null) return;
来源：http://ym.asd995.cn

Go:   if data == nil { return }
来源：http://km.newstarts.cn

Ruby: return if data.nil?
来源：http://xh.newstarts.cn

C#:   if (data == null) return;
来源：http://yd.shxzukj.cn

================================================================================
来源：http://cx.huixiangedu.cn

C. 函数与作用域
来源：http://hs.muxihuayi.cn

================================================================================
来源：http://pi.gzmigu.cn

[C01] 定义函数
来源：http://ws.yuntaijiaju.cn

Py:   def add(a, b): return a + b
来源：http://ql.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zw.huanxung.cn

JS:   function add(a, b) { return a + b; }
来源：http://in.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zj.bookmarksfly.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://jt.muxihuayi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://bc.521024.cn

Ruby: def add(a, b); a + b; end
来源：http://mz.shxzskj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zn.521024.cn

[C02] 默认参数
来源：http://rh.521024.cn

Py:   def greet(name="World"): return name
来源：http://pq.newstarts.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qg.521024.cn

JS:   function greet(name = "World") { return name; }
来源：http://ra.haigaiapp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://mo.szsharing.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ya.huanxung.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vc.lnxyls.cn

Ruby: def greet(name = "World") = name
来源：http://bc.wgjwhj.cn

C#:   string Greet(string name = "World") => name;
来源：http://um.yuntaijiaju.cn

[C03] 可变参数
来源：http://jg.hnjuh.cn

Py:   def total(*args): return sum(args)
来源：http://ym.hahajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pt.hahajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zz.hnjuh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://op.newstarts.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sh.yuntaijiaju.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ea.lnxyls.cn

Ruby: def total(*nums); nums.sum; end
来源：http://na.haigaiapp.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pl.nszjky.cn

[C04] 命名参数 / 关键字参数
来源：http://dt.nszjky.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://op.huanxung.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ly.bjjhwx.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qr.szsharing.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zr.hahajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://hy.521024.cn

Go:   // 无：用配置结构体参数
来源：http://bn.9csxet.cn

Ruby: f(a: 1, b: 2)
来源：http://hn.huixinmuqiang.cn

C#:   f(a: 1, b: 2)
来源：http://no.szxytkj.cn

[C05] 返回多个值
来源：http://ro.asd995.cn

Py:   return a, b
来源：http://qp.nszjky.cn

PHP:  return [$a, $b];
来源：http://yj.panjiajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ov.newstarts.cn

TS:   return { a, b };
来源：http://ez.huanxung.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yf.huixinmuqiang.cn

Go:   return a, b
来源：http://um.9csxet.cn

Ruby: return a, b
来源：http://oc.colortex.cn

C#:   return (a, b);              // ValueTuple
来源：http://oa.panjiajie.cn

[C06] 匿名函数 / lambda
来源：http://ft.yuexingan06.cn

Py:   square = lambda x: x * x
来源：http://kq.shtwfgs.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ui.colortex.cn

JS:   const square = x => x * x;
来源：http://rs.gzmigu.cn

TS:   const square = (x: number): number => x * x;
来源：http://no.bookmarksfly.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fd.newstarts.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qq.9csxet.cn

Ruby: square = ->(x) { x * x }
来源：http://ao.asd995.cn

C#:   Func<int, int> square = x => x * x;
来源：http://kl.nicolike.cn

[C07] 把函数作为参数传入
来源：http://qy.yuntaijiaju.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tx.haigaiapp.cn

PHP:  array_map("strtoupper", $arr);
来源：http://dw.szsharing.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sb.9csxet.cn

TS:   arr.map(String)
来源：http://kb.yuntaijiaju.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qn.shxzukj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yv.muxihuayi.cn

Ruby: arr.map(&:upcase)
来源：http://em.bookmarksfly.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ri.shxzskj.cn

[C08] 闭包
来源：http://mt.shtwfgs.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gp.yuntaijiaju.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ad.colortex.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ew.haigaiapp.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ud.521024.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lo.yuntaijiaju.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ol.hahajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://im.haigaiapp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xm.jianghongdianzi.cn

[C09] 递归
来源：http://ya.panjiajie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jv.shxzskj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://go.huixinmuqiang.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://je.shxzukj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xa.hahajie.cn


<!-- 参考信息 -->