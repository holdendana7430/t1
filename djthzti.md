代发 wailian999

C#:   (int)'A'; (char)65
来源：http://tf.colortex.cn

[A19] 交换两个变量
来源：http://ti.szsharing.cn

Py:   a, b = b, a
来源：http://jv.9csxet.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://no.bjjhwx.cn

JS:   [a, b] = [b, a];
来源：http://kh.hnjuh.cn

TS:   [a, b] = [b, a];
来源：http://rk.huixiangedu.cn

Java: int t = a; a = b; b = t;
来源：http://gk.yuexingan06.cn

Go:   a, b = b, a
来源：http://rq.muxihuayi.cn

Ruby: a, b = b, a
来源：http://ah.huixiangedu.cn

C#:   (a, b) = (b, a);
来源：http://qy.gzmigu.cn

[A20] 读取标准输入
来源：http://nc.nicolike.cn

Py:   name = input("请输入：")
来源：http://tt.521024.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ze.bookmarksfly.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zd.yuexingan06.cn

TS:   // Node.js：readline 模块
来源：http://oa.newstarts.cn

Java: new Scanner(System.in).nextLine()
来源：http://gl.521024.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qu.bjjhwx.cn

Ruby: gets.chomp
来源：http://vo.nszjky.cn

C#:   Console.ReadLine();
来源：http://zx.hnjuh.cn

[A21] 保留指定小数位输出
来源：http://de.newstarts.cn

Py:   f"{3.14159:.2f}"
来源：http://ys.szxytkj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://lq.lnxyls.cn

JS:   (3.14159).toFixed(2)
来源：http://uh.nszjky.cn

TS:   (3.14159).toFixed(2)
来源：http://ev.yuntaijiaju.cn

Java: String.format("%.2f", 3.14159)
来源：http://ne.newstarts.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jm.bjjhwx.cn

Ruby: format("%.2f", 3.14159)
来源：http://xs.9csxet.cn

C#:   3.14159.ToString("F2")
来源：http://oj.bjjhwx.cn

[A22] 获取字符串长度
来源：http://on.jianghongdianzi.cn

Py:   len(s)
来源：http://ig.yuexingan06.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rc.nicolike.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bw.haigaiapp.cn

TS:   s.length
来源：http://er.colortex.cn

Java: s.length()
来源：http://xp.hahajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cp.panjiajie.cn

Ruby: s.length
来源：http://pa.hahajie.cn

C#:   s.Length
来源：http://hv.yuexingan06.cn

[A23] 大小写转换
来源：http://cb.hahajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://yb.bjjhwx.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qo.hahajie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qm.hahajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bx.wgjwhj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ad.nszjky.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kh.asd995.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ci.yuntaijiaju.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://bl.huanxung.cn

[A24] 去除首尾空白
来源：http://ia.colortex.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ln.colortex.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lu.asd995.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mt.muxihuayi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jz.muxihuayi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fd.panjiajie.cn

Go:   strings.TrimSpace(s)
来源：http://wk.bjjhwx.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vf.lnxyls.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vo.9csxet.cn

[A25] 字符串比较
来源：http://ei.bookmarksfly.cn

Py:   s1 == s2; s1 != s2
来源：http://lt.hnjuh.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xc.shxzukj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bw.yuntaijiaju.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bi.asd995.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ku.jctech888.com.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dv.chemitech.net.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://dd.jctech888.com.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ri.huixiangedu.cn

[A26] 类型转换总览
来源：http://la.chemitech.net.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mo.hahajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hk.jianghongdianzi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xn.szsharing.cn

TS:   Number() String() Boolean() x as number
来源：http://zq.yuexingan06.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rf.muxihuayi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ke.bjjhwx.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://bx.huanxung.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zq.muxihuayi.cn

================================================================================
来源：http://dv.wgjwhj.cn

B. 流程控制
来源：http://fu.colortex.cn

================================================================================
来源：http://te.jctech888.com.cn

[B01] 条件判断 if / else
来源：http://nj.panjiajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xa.panjiajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ha.chemitech.net.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mp.wgjwhj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mw.bookmarksfly.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ah.huixiangedu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nh.huixinmuqiang.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bb.lnxyls.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ku.shxzskj.cn

[B02] 多分支 else if / elif
来源：http://qp.shxzskj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nt.hnjuh.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zg.shxzukj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jg.colortex.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://un.jctech888.com.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fi.colortex.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pv.jctech888.com.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wh.nszjky.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wc.jctech888.com.cn

[B03] switch / match / case
来源：http://bu.panjiajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://uy.jianghongdianzi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ya.shtwfgs.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pa.hahajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fz.9csxet.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qe.hahajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ix.muxihuayi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cp.9csxet.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ij.lnxyls.cn

[B04] for 计数循环
来源：http://yr.shxzukj.cn

Py:   for i in range(10): print(i)
来源：http://yv.haigaiapp.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ak.shtwfgs.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nt.9csxet.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qq.bookmarksfly.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lx.yuntaijiaju.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nb.gzmigu.cn

Ruby: 10.times { |i| puts i }
来源：http://mv.haigaiapp.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rw.szxytkj.cn

[B05] 遍历数组 / 列表
来源：http://zu.jctech888.com.cn

Py:   for item in arr: print(item)
来源：http://lz.wgjwhj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://px.shtwfgs.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yj.yuntaijiaju.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rq.huixiangedu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xj.wgjwhj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gx.szxytkj.cn

Ruby: arr.each { |item| puts item }
来源：http://by.huixiangedu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hp.jianghongdianzi.cn

[B06] 遍历字典 / 对象
来源：http://hy.chemitech.net.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://cb.shxzskj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pv.newstarts.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nq.muxihuayi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://en.hnjuh.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bw.szsharing.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://la.hahajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fb.lnxyls.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://oa.bjjhwx.cn

[B07] while 循环
来源：http://my.yuntaijiaju.cn

Py:   while i < 10: i += 1
来源：http://zs.521024.cn

PHP:  while ($i < 10) { $i++; }
来源：http://pm.gzmigu.cn

JS:   while (i < 10) { i++; }
来源：http://cv.huixinmuqiang.cn

TS:   while (i < 10) { i++; }
来源：http://eg.nszjky.cn

Java: while (i < 10) { i++; }
来源：http://xj.shtwfgs.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rw.nicolike.cn

Ruby: while i < 10; i += 1; end
来源：http://uk.bjjhwx.cn

C#:   while (i < 10) { i++; }
来源：http://qy.szxytkj.cn

[B08] do-while（至少执行一次）
来源：http://wu.shtwfgs.cn

Py:   # 无 do-while：用 while True + break
来源：http://bb.huanxung.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ev.gzmigu.cn

JS:   do { i++; } while (i < 10);
来源：http://ha.jianghongdianzi.cn

TS:   do { i++; } while (i < 10);
来源：http://ed.colortex.cn

Java: do { i++; } while (i < 10);
来源：http://yq.haigaiapp.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xx.9csxet.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qu.521024.cn

C#:   do { i++; } while (i < 10);
来源：http://zw.wgjwhj.cn

[B09] break 与 continue
来源：http://oe.chemitech.net.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://un.yuntaijiaju.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lz.yuexingan06.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hg.newstarts.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xe.haigaiapp.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dx.asd995.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://an.bookmarksfly.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fb.hahajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wh.yuexingan06.cn

[B10] 遍历同时拿索引
来源：http://zz.jianghongdianzi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pu.haigaiapp.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yv.shxzukj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wt.shtwfgs.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pv.asd995.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bj.hnjuh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vz.jctech888.com.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cj.haigaiapp.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xo.huixiangedu.cn

[B11] 生成数字序列 / 区间
来源：http://xe.yuntaijiaju.cn

Py:   list(range(0, 10, 2))
来源：http://to.colortex.cn

PHP:  range(0, 10, 2);
来源：http://gu.shxzukj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ed.jctech888.com.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nu.muxihuayi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ih.hnjuh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gv.nicolike.cn

Ruby: (0...10).step(2).to_a
来源：http://ed.shxzskj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ga.bookmarksfly.cn

[B12] 跳出多层循环
来源：http://be.colortex.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://gg.shxzskj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://kd.gzmigu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://js.521024.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gi.szsharing.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zc.521024.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gt.szsharing.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://en.shxzskj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ci.hnjuh.cn

[B13] 判断是否为数字
来源：http://xe.hnjuh.cn

Py:   isinstance(x, (int, float))
来源：http://ug.jctech888.com.cn

PHP:  is_numeric($x)
来源：http://cc.szxytkj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wa.lnxyls.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wi.huixiangedu.cn

Java: x instanceof Number
来源：http://ad.shtwfgs.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qv.yuexingan06.cn

Ruby: x.is_a?(Numeric)
来源：http://zr.szsharing.cn

C#:   x is int or double or decimal
来源：http://ox.9csxet.cn

[B14] 判断值是否在集合内
来源：http://qw.shxzskj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ns.yuexingan06.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bp.colortex.cn

JS:   [1, 2, 3].includes(x)
来源：http://vm.shxzskj.cn

TS:   [1, 2, 3].includes(x)
来源：http://ty.hahajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ol.gzmigu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vw.wgjwhj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ck.shxzukj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ab.asd995.cn

[B15] 布尔运算与取反
来源：http://oa.jianghongdianzi.cn

Py:   a and b or not c
来源：http://eu.asd995.cn

PHP:  $a && $b || !$c
来源：http://bp.haigaiapp.cn

JS:   a && b || !c
来源：http://vq.shxzukj.cn

TS:   a && b || !c
来源：http://pn.yuexingan06.cn

Java: a && b || !c
来源：http://qp.asd995.cn

Go:   a && b || !c
来源：http://an.lnxyls.cn

Ruby: a && b || !c
来源：http://qt.huanxung.cn

C#:   a && b || !c
来源：http://qr.gzmigu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://cl.colortex.cn

Py:   if not data: return
来源：http://rp.szsharing.cn

PHP:  if (!$data) { return; }
来源：http://jo.huixinmuqiang.cn

JS:   if (!data) return;
来源：http://yh.hnjuh.cn

TS:   if (!data) return;
来源：http://oh.gzmigu.cn

Java: if (data == null) return;
来源：http://zm.521024.cn

Go:   if data == nil { return }
来源：http://nf.huixinmuqiang.cn

Ruby: return if data.nil?
来源：http://mz.huixinmuqiang.cn

C#:   if (data == null) return;
来源：http://ru.huanxung.cn

================================================================================
来源：http://gd.muxihuayi.cn

C. 函数与作用域
来源：http://wg.huanxung.cn

================================================================================
来源：http://cm.chemitech.net.cn

[C01] 定义函数
来源：http://ba.shtwfgs.cn

Py:   def add(a, b): return a + b
来源：http://va.haigaiapp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ru.hahajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://eg.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xo.nicolike.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fh.nicolike.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mv.gzmigu.cn

Ruby: def add(a, b); a + b; end
来源：http://ce.yuntaijiaju.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ez.lnxyls.cn

[C02] 默认参数
来源：http://gv.muxihuayi.cn

Py:   def greet(name="World"): return name
来源：http://rp.colortex.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vx.huixiangedu.cn

JS:   function greet(name = "World") { return name; }
来源：http://yy.wgjwhj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rj.huanxung.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bd.jianghongdianzi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yu.shtwfgs.cn

Ruby: def greet(name = "World") = name
来源：http://xs.newstarts.cn

C#:   string Greet(string name = "World") => name;
来源：http://cx.hahajie.cn

[C03] 可变参数
来源：http://nf.hnjuh.cn

Py:   def total(*args): return sum(args)
来源：http://vq.szsharing.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bb.asd995.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ct.shxzukj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sg.szxytkj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zx.szxytkj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kg.9csxet.cn

Ruby: def total(*nums); nums.sum; end
来源：http://kj.shxzukj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fh.yuntaijiaju.cn

[C04] 命名参数 / 关键字参数
来源：http://kv.jctech888.com.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bb.9csxet.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://uq.huixinmuqiang.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mx.newstarts.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rz.hahajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://qm.wgjwhj.cn

Go:   // 无：用配置结构体参数
来源：http://qc.huixiangedu.cn

Ruby: f(a: 1, b: 2)
来源：http://fk.szsharing.cn

C#:   f(a: 1, b: 2)
来源：http://bb.panjiajie.cn

[C05] 返回多个值
来源：http://jk.hnjuh.cn

Py:   return a, b
来源：http://dd.chemitech.net.cn

PHP:  return [$a, $b];
来源：http://pu.shxzskj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://tp.huanxung.cn

TS:   return { a, b };
来源：http://cz.nicolike.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mn.jianghongdianzi.cn

Go:   return a, b
来源：http://gw.yuexingan06.cn

Ruby: return a, b
来源：http://bh.jianghongdianzi.cn

C#:   return (a, b);              // ValueTuple
来源：http://uu.chemitech.net.cn

[C06] 匿名函数 / lambda
来源：http://lq.asd995.cn

Py:   square = lambda x: x * x
来源：http://wj.wgjwhj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://vy.521024.cn

JS:   const square = x => x * x;
来源：http://pb.muxihuayi.cn

TS:   const square = (x: number): number => x * x;
来源：http://mg.huanxung.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rr.huanxung.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ma.gzmigu.cn

Ruby: square = ->(x) { x * x }
来源：http://fn.521024.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ls.bjjhwx.cn

[C07] 把函数作为参数传入
来源：http://tp.hnjuh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ji.wgjwhj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://me.wgjwhj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hk.bjjhwx.cn

TS:   arr.map(String)
来源：http://an.nszjky.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ae.bookmarksfly.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qe.lnxyls.cn

Ruby: arr.map(&:upcase)
来源：http://ou.hnjuh.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://eu.shtwfgs.cn

[C08] 闭包
来源：http://ou.szxytkj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qh.hahajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fn.asd995.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pc.bjjhwx.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sz.hnjuh.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pj.bjjhwx.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vm.yuntaijiaju.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mk.9csxet.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qa.hahajie.cn

[C09] 递归
来源：http://xm.shxzskj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hm.nszjky.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://id.hnjuh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qq.asd995.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tp.colortex.cn


<!-- 参考信息 -->