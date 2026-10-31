代发 wailian999

C#:   (int)'A'; (char)65
来源：http://os.chemitech.net.cn

[A19] 交换两个变量
来源：http://wq.wgjwhj.cn

Py:   a, b = b, a
来源：http://gq.nszjky.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://er.szsharing.cn

JS:   [a, b] = [b, a];
来源：http://ng.huanxung.cn

TS:   [a, b] = [b, a];
来源：http://yi.yuntaijiaju.cn

Java: int t = a; a = b; b = t;
来源：http://gx.nicolike.cn

Go:   a, b = b, a
来源：http://pk.jctech888.com.cn

Ruby: a, b = b, a
来源：http://we.huanxung.cn

C#:   (a, b) = (b, a);
来源：http://ij.muxihuayi.cn

[A20] 读取标准输入
来源：http://be.wgjwhj.cn

Py:   name = input("请输入：")
来源：http://kh.asd995.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://nv.shtwfgs.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qv.shxzskj.cn

TS:   // Node.js：readline 模块
来源：http://cr.huixiangedu.cn

Java: new Scanner(System.in).nextLine()
来源：http://wh.bjjhwx.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://sd.panjiajie.cn

Ruby: gets.chomp
来源：http://wl.gzmigu.cn

C#:   Console.ReadLine();
来源：http://fi.hnjuh.cn

[A21] 保留指定小数位输出
来源：http://eo.wgjwhj.cn

Py:   f"{3.14159:.2f}"
来源：http://lf.newstarts.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xn.bookmarksfly.cn

JS:   (3.14159).toFixed(2)
来源：http://xc.hahajie.cn

TS:   (3.14159).toFixed(2)
来源：http://qx.colortex.cn

Java: String.format("%.2f", 3.14159)
来源：http://iy.nicolike.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nm.szxytkj.cn

Ruby: format("%.2f", 3.14159)
来源：http://fk.hnjuh.cn

C#:   3.14159.ToString("F2")
来源：http://mf.gzmigu.cn

[A22] 获取字符串长度
来源：http://kn.huanxung.cn

Py:   len(s)
来源：http://ja.huanxung.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fn.shxzskj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gz.shxzskj.cn

TS:   s.length
来源：http://oc.lnxyls.cn

Java: s.length()
来源：http://wr.521024.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ol.gzmigu.cn

Ruby: s.length
来源：http://sw.521024.cn

C#:   s.Length
来源：http://jo.9csxet.cn

[A23] 大小写转换
来源：http://qz.colortex.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://qb.nszjky.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yt.wgjwhj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fq.jianghongdianzi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qw.yuexingan06.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vy.szxytkj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fd.chemitech.net.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ej.colortex.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://cr.521024.cn

[A24] 去除首尾空白
来源：http://ch.hahajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zi.nszjky.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://na.szsharing.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zs.szsharing.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ay.yuexingan06.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xh.szxytkj.cn

Go:   strings.TrimSpace(s)
来源：http://cm.lnxyls.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tl.bookmarksfly.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pa.panjiajie.cn

[A25] 字符串比较
来源：http://tj.nicolike.cn

Py:   s1 == s2; s1 != s2
来源：http://dd.szsharing.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ej.panjiajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vo.gzmigu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jk.chemitech.net.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://el.chemitech.net.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vx.panjiajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://qo.newstarts.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dc.shxzskj.cn

[A26] 类型转换总览
来源：http://mm.bjjhwx.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gm.jctech888.com.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mg.szxytkj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ux.shxzukj.cn

TS:   Number() String() Boolean() x as number
来源：http://ae.nicolike.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://oo.gzmigu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cd.yuexingan06.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mg.lnxyls.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://du.jianghongdianzi.cn

================================================================================
来源：http://iy.gzmigu.cn

B. 流程控制
来源：http://xc.nicolike.cn

================================================================================
来源：http://oj.wgjwhj.cn

[B01] 条件判断 if / else
来源：http://tq.wgjwhj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xb.521024.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qy.jctech888.com.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vt.yuexingan06.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hc.bjjhwx.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ae.bookmarksfly.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xg.asd995.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gi.asd995.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://le.szxytkj.cn

[B02] 多分支 else if / elif
来源：http://qm.nszjky.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ly.szxytkj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://te.hnjuh.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pj.nicolike.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bt.asd995.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jc.bookmarksfly.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xp.hnjuh.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fe.wgjwhj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lh.9csxet.cn

[B03] switch / match / case
来源：http://av.haigaiapp.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mg.wgjwhj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nu.shxzskj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fg.newstarts.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ww.lnxyls.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zx.chemitech.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cu.wgjwhj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zt.hahajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pa.hnjuh.cn

[B04] for 计数循环
来源：http://az.jianghongdianzi.cn

Py:   for i in range(10): print(i)
来源：http://yk.asd995.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ro.yuexingan06.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eb.jctech888.com.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tz.nicolike.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://op.shxzskj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nd.521024.cn

Ruby: 10.times { |i| puts i }
来源：http://ho.asd995.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lt.szsharing.cn

[B05] 遍历数组 / 列表
来源：http://io.haigaiapp.cn

Py:   for item in arr: print(item)
来源：http://qw.yuntaijiaju.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jr.haigaiapp.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://nf.huixinmuqiang.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://uk.shxzukj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://kg.chemitech.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://td.haigaiapp.cn

Ruby: arr.each { |item| puts item }
来源：http://io.colortex.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ce.panjiajie.cn

[B06] 遍历字典 / 对象
来源：http://pr.yuntaijiaju.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ko.hnjuh.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jh.9csxet.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oj.yuntaijiaju.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://au.521024.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jz.muxihuayi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rx.lnxyls.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rf.gzmigu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rm.nszjky.cn

[B07] while 循环
来源：http://zh.wgjwhj.cn

Py:   while i < 10: i += 1
来源：http://gy.asd995.cn

PHP:  while ($i < 10) { $i++; }
来源：http://rj.9csxet.cn

JS:   while (i < 10) { i++; }
来源：http://yz.bjjhwx.cn

TS:   while (i < 10) { i++; }
来源：http://ru.lnxyls.cn

Java: while (i < 10) { i++; }
来源：http://xb.szxytkj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sq.panjiajie.cn

Ruby: while i < 10; i += 1; end
来源：http://uy.muxihuayi.cn

C#:   while (i < 10) { i++; }
来源：http://gg.haigaiapp.cn

[B08] do-while（至少执行一次）
来源：http://cm.colortex.cn

Py:   # 无 do-while：用 while True + break
来源：http://jr.nszjky.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://oi.yuntaijiaju.cn

JS:   do { i++; } while (i < 10);
来源：http://pa.hahajie.cn

TS:   do { i++; } while (i < 10);
来源：http://ba.huanxung.cn

Java: do { i++; } while (i < 10);
来源：http://go.bjjhwx.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://rj.chemitech.net.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wn.bjjhwx.cn

C#:   do { i++; } while (i < 10);
来源：http://vt.huixinmuqiang.cn

[B09] break 与 continue
来源：http://sw.huanxung.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qo.bookmarksfly.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ga.huixiangedu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nx.yuexingan06.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dy.nszjky.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ae.asd995.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ea.newstarts.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ct.panjiajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sd.shxzukj.cn

[B10] 遍历同时拿索引
来源：http://lt.9csxet.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ni.huixiangedu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ym.szsharing.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sb.huixinmuqiang.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rb.muxihuayi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://un.huixiangedu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://oq.9csxet.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mg.szxytkj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hj.chemitech.net.cn

[B11] 生成数字序列 / 区间
来源：http://ly.jianghongdianzi.cn

Py:   list(range(0, 10, 2))
来源：http://ei.huixinmuqiang.cn

PHP:  range(0, 10, 2);
来源：http://kc.hahajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://do.huixiangedu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ww.gzmigu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qv.panjiajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cb.colortex.cn

Ruby: (0...10).step(2).to_a
来源：http://ed.wgjwhj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xi.hnjuh.cn

[B12] 跳出多层循环
来源：http://hj.asd995.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yg.wgjwhj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mb.panjiajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qb.521024.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wr.hahajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://al.yuntaijiaju.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rk.yuexingan06.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kq.shxzskj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qk.yuntaijiaju.cn

[B13] 判断是否为数字
来源：http://to.huixinmuqiang.cn

Py:   isinstance(x, (int, float))
来源：http://pi.hahajie.cn

PHP:  is_numeric($x)
来源：http://ou.hahajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mo.nszjky.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xi.hahajie.cn

Java: x instanceof Number
来源：http://pu.huanxung.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://md.9csxet.cn

Ruby: x.is_a?(Numeric)
来源：http://it.nicolike.cn

C#:   x is int or double or decimal
来源：http://sz.asd995.cn

[B14] 判断值是否在集合内
来源：http://gi.bookmarksfly.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zx.huanxung.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jv.lnxyls.cn

JS:   [1, 2, 3].includes(x)
来源：http://gc.chemitech.net.cn

TS:   [1, 2, 3].includes(x)
来源：http://km.szxytkj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ch.asd995.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ex.lnxyls.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ec.hahajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vr.yuexingan06.cn

[B15] 布尔运算与取反
来源：http://nv.huixiangedu.cn

Py:   a and b or not c
来源：http://ps.hahajie.cn

PHP:  $a && $b || !$c
来源：http://wp.huixinmuqiang.cn

JS:   a && b || !c
来源：http://eu.9csxet.cn

TS:   a && b || !c
来源：http://hv.hahajie.cn

Java: a && b || !c
来源：http://so.szxytkj.cn

Go:   a && b || !c
来源：http://qn.szxytkj.cn

Ruby: a && b || !c
来源：http://qs.shxzskj.cn

C#:   a && b || !c
来源：http://xv.chemitech.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ty.nicolike.cn

Py:   if not data: return
来源：http://nq.chemitech.net.cn

PHP:  if (!$data) { return; }
来源：http://nl.shxzskj.cn

JS:   if (!data) return;
来源：http://dk.shxzukj.cn

TS:   if (!data) return;
来源：http://os.asd995.cn

Java: if (data == null) return;
来源：http://us.muxihuayi.cn

Go:   if data == nil { return }
来源：http://sp.wgjwhj.cn

Ruby: return if data.nil?
来源：http://yf.szxytkj.cn

C#:   if (data == null) return;
来源：http://qr.521024.cn

================================================================================
来源：http://ds.wgjwhj.cn

C. 函数与作用域
来源：http://eo.bjjhwx.cn

================================================================================
来源：http://op.gzmigu.cn

[C01] 定义函数
来源：http://ts.yuntaijiaju.cn

Py:   def add(a, b): return a + b
来源：http://dw.shxzskj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sg.asd995.cn

JS:   function add(a, b) { return a + b; }
来源：http://uk.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mw.muxihuayi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://at.panjiajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://nn.lnxyls.cn

Ruby: def add(a, b); a + b; end
来源：http://pv.huixinmuqiang.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vf.yuexingan06.cn

[C02] 默认参数
来源：http://zo.jctech888.com.cn

Py:   def greet(name="World"): return name
来源：http://rh.shtwfgs.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://rp.huanxung.cn

JS:   function greet(name = "World") { return name; }
来源：http://xv.huixiangedu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://kb.huixiangedu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://yj.szsharing.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zh.bjjhwx.cn

Ruby: def greet(name = "World") = name
来源：http://zr.bookmarksfly.cn

C#:   string Greet(string name = "World") => name;
来源：http://dn.haigaiapp.cn

[C03] 可变参数
来源：http://qc.nszjky.cn

Py:   def total(*args): return sum(args)
来源：http://tt.asd995.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lr.jianghongdianzi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wu.521024.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://iw.jianghongdianzi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gl.newstarts.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vp.panjiajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yl.chemitech.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tc.haigaiapp.cn

[C04] 命名参数 / 关键字参数
来源：http://um.huanxung.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vy.yuexingan06.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qs.colortex.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cv.wgjwhj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qw.hahajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://hc.nicolike.cn

Go:   // 无：用配置结构体参数
来源：http://ug.yuntaijiaju.cn

Ruby: f(a: 1, b: 2)
来源：http://tf.nicolike.cn

C#:   f(a: 1, b: 2)
来源：http://ns.shxzskj.cn

[C05] 返回多个值
来源：http://ga.huanxung.cn

Py:   return a, b
来源：http://zf.colortex.cn

PHP:  return [$a, $b];
来源：http://xr.asd995.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ea.huixiangedu.cn

TS:   return { a, b };
来源：http://xd.wgjwhj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vx.yuexingan06.cn

Go:   return a, b
来源：http://oe.muxihuayi.cn

Ruby: return a, b
来源：http://vj.9csxet.cn

C#:   return (a, b);              // ValueTuple
来源：http://cz.jianghongdianzi.cn

[C06] 匿名函数 / lambda
来源：http://hk.asd995.cn

Py:   square = lambda x: x * x
来源：http://aa.jianghongdianzi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ew.newstarts.cn

JS:   const square = x => x * x;
来源：http://ec.nicolike.cn

TS:   const square = (x: number): number => x * x;
来源：http://gi.9csxet.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sj.chemitech.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://pv.panjiajie.cn

Ruby: square = ->(x) { x * x }
来源：http://il.521024.cn

C#:   Func<int, int> square = x => x * x;
来源：http://kd.panjiajie.cn

[C07] 把函数作为参数传入
来源：http://bq.chemitech.net.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://uk.nicolike.cn

PHP:  array_map("strtoupper", $arr);
来源：http://id.nicolike.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://oj.nszjky.cn

TS:   arr.map(String)
来源：http://tm.shtwfgs.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dr.shtwfgs.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ap.haigaiapp.cn

Ruby: arr.map(&:upcase)
来源：http://nt.haigaiapp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xp.hahajie.cn

[C08] 闭包
来源：http://lv.muxihuayi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vb.yuntaijiaju.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ul.hnjuh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lc.gzmigu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://la.bookmarksfly.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ud.lnxyls.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zc.haigaiapp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://en.lnxyls.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pr.newstarts.cn

[C09] 递归
来源：http://mt.panjiajie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pz.gzmigu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gs.chemitech.net.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zk.hnjuh.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vk.wgjwhj.cn


<!-- 参考信息 -->