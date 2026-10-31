代发 wailian999

C#:   (int)'A'; (char)65
来源：http://lr.hnjuh.cn

[A19] 交换两个变量
来源：http://yo.wgjwhj.cn

Py:   a, b = b, a
来源：http://mn.chemitech.net.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://io.bjjhwx.cn

JS:   [a, b] = [b, a];
来源：http://ow.shxzukj.cn

TS:   [a, b] = [b, a];
来源：http://aj.shxzskj.cn

Java: int t = a; a = b; b = t;
来源：http://ao.huixinmuqiang.cn

Go:   a, b = b, a
来源：http://ih.lnxyls.cn

Ruby: a, b = b, a
来源：http://uo.shxzskj.cn

C#:   (a, b) = (b, a);
来源：http://zu.yuntaijiaju.cn

[A20] 读取标准输入
来源：http://dm.panjiajie.cn

Py:   name = input("请输入：")
来源：http://vb.bookmarksfly.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ra.yuexingan06.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kc.yuexingan06.cn

TS:   // Node.js：readline 模块
来源：http://za.521024.cn

Java: new Scanner(System.in).nextLine()
来源：http://qu.yuexingan06.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://os.nicolike.cn

Ruby: gets.chomp
来源：http://of.hahajie.cn

C#:   Console.ReadLine();
来源：http://ig.asd995.cn

[A21] 保留指定小数位输出
来源：http://zw.colortex.cn

Py:   f"{3.14159:.2f}"
来源：http://os.haigaiapp.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fb.lnxyls.cn

JS:   (3.14159).toFixed(2)
来源：http://wj.nszjky.cn

TS:   (3.14159).toFixed(2)
来源：http://zz.szsharing.cn

Java: String.format("%.2f", 3.14159)
来源：http://nq.hnjuh.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://az.jianghongdianzi.cn

Ruby: format("%.2f", 3.14159)
来源：http://zj.shxzskj.cn

C#:   3.14159.ToString("F2")
来源：http://rb.shtwfgs.cn

[A22] 获取字符串长度
来源：http://xr.hnjuh.cn

Py:   len(s)
来源：http://pj.muxihuayi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dg.hahajie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ih.jctech888.com.cn

TS:   s.length
来源：http://xh.huixinmuqiang.cn

Java: s.length()
来源：http://xp.shxzukj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fk.muxihuayi.cn

Ruby: s.length
来源：http://hx.hnjuh.cn

C#:   s.Length
来源：http://kr.asd995.cn

[A23] 大小写转换
来源：http://sv.huixinmuqiang.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://qs.shxzskj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ej.shtwfgs.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cg.wgjwhj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://sl.jctech888.com.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xc.newstarts.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nz.nicolike.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://sk.yuexingan06.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://kf.521024.cn

[A24] 去除首尾空白
来源：http://hx.haigaiapp.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wv.newstarts.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nf.bjjhwx.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nz.szsharing.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yq.newstarts.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nn.huixinmuqiang.cn

Go:   strings.TrimSpace(s)
来源：http://vu.shtwfgs.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xp.shtwfgs.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lq.chemitech.net.cn

[A25] 字符串比较
来源：http://so.wgjwhj.cn

Py:   s1 == s2; s1 != s2
来源：http://he.colortex.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sw.jianghongdianzi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mf.yuntaijiaju.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hi.nicolike.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yq.gzmigu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hw.bjjhwx.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://uj.hnjuh.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jj.chemitech.net.cn

[A26] 类型转换总览
来源：http://uw.bookmarksfly.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qm.colortex.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://te.szsharing.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ch.hnjuh.cn

TS:   Number() String() Boolean() x as number
来源：http://go.hnjuh.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fo.gzmigu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kw.yuexingan06.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://qt.hahajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qk.bjjhwx.cn

================================================================================
来源：http://sh.jianghongdianzi.cn

B. 流程控制
来源：http://yc.shxzskj.cn

================================================================================
来源：http://cx.wgjwhj.cn

[B01] 条件判断 if / else
来源：http://jn.shtwfgs.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://tp.shxzskj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lf.shtwfgs.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mk.521024.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sd.521024.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://rv.colortex.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pp.panjiajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yd.shxzukj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kc.bookmarksfly.cn

[B02] 多分支 else if / elif
来源：http://ke.huixiangedu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zw.huanxung.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ao.shtwfgs.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ue.asd995.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ru.lnxyls.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ha.shxzskj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ri.jianghongdianzi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fn.chemitech.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ow.nszjky.cn

[B03] switch / match / case
来源：http://xr.jctech888.com.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://da.szxytkj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ut.shxzskj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ic.hahajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vb.yuexingan06.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jj.lnxyls.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ue.muxihuayi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gy.bjjhwx.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jh.nszjky.cn

[B04] for 计数循环
来源：http://rh.shxzukj.cn

Py:   for i in range(10): print(i)
来源：http://jr.nicolike.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fp.9csxet.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ir.bookmarksfly.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ee.gzmigu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ek.colortex.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://om.jctech888.com.cn

Ruby: 10.times { |i| puts i }
来源：http://ax.wgjwhj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ca.jctech888.com.cn

[B05] 遍历数组 / 列表
来源：http://we.panjiajie.cn

Py:   for item in arr: print(item)
来源：http://cf.szxytkj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://oi.jctech888.com.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ok.huixinmuqiang.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://zy.gzmigu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zh.hnjuh.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ct.muxihuayi.cn

Ruby: arr.each { |item| puts item }
来源：http://tq.nszjky.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ts.shxzskj.cn

[B06] 遍历字典 / 对象
来源：http://oh.bookmarksfly.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://td.bookmarksfly.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ar.bjjhwx.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nn.newstarts.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vq.asd995.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ud.wgjwhj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gr.hnjuh.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dq.newstarts.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ss.shxzukj.cn

[B07] while 循环
来源：http://cn.szxytkj.cn

Py:   while i < 10: i += 1
来源：http://df.haigaiapp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fq.bjjhwx.cn

JS:   while (i < 10) { i++; }
来源：http://eq.bjjhwx.cn

TS:   while (i < 10) { i++; }
来源：http://gj.gzmigu.cn

Java: while (i < 10) { i++; }
来源：http://ex.asd995.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gp.lnxyls.cn

Ruby: while i < 10; i += 1; end
来源：http://ks.bjjhwx.cn

C#:   while (i < 10) { i++; }
来源：http://hh.lnxyls.cn

[B08] do-while（至少执行一次）
来源：http://uj.jianghongdianzi.cn

Py:   # 无 do-while：用 while True + break
来源：http://jd.szxytkj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://dg.asd995.cn

JS:   do { i++; } while (i < 10);
来源：http://pk.521024.cn

TS:   do { i++; } while (i < 10);
来源：http://hb.hnjuh.cn

Java: do { i++; } while (i < 10);
来源：http://cg.jianghongdianzi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mg.haigaiapp.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cu.haigaiapp.cn

C#:   do { i++; } while (i < 10);
来源：http://wm.colortex.cn

[B09] break 与 continue
来源：http://vk.yuntaijiaju.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ha.muxihuayi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dl.hahajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://va.yuntaijiaju.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ry.shxzukj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bi.huanxung.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ua.521024.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zs.jctech888.com.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qc.chemitech.net.cn

[B10] 遍历同时拿索引
来源：http://aa.shxzskj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yt.shxzskj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nf.9csxet.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sx.colortex.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vj.panjiajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mo.gzmigu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bk.shtwfgs.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vh.colortex.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yd.bjjhwx.cn

[B11] 生成数字序列 / 区间
来源：http://cn.haigaiapp.cn

Py:   list(range(0, 10, 2))
来源：http://wo.shxzukj.cn

PHP:  range(0, 10, 2);
来源：http://rf.lnxyls.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mo.colortex.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cb.yuntaijiaju.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nj.chemitech.net.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://it.wgjwhj.cn

Ruby: (0...10).step(2).to_a
来源：http://cf.haigaiapp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ad.muxihuayi.cn

[B12] 跳出多层循环
来源：http://hj.shtwfgs.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fo.bookmarksfly.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hd.nicolike.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lg.521024.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mq.chemitech.net.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jh.9csxet.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ao.jctech888.com.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gz.521024.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ct.szsharing.cn

[B13] 判断是否为数字
来源：http://ec.newstarts.cn

Py:   isinstance(x, (int, float))
来源：http://gz.bjjhwx.cn

PHP:  is_numeric($x)
来源：http://xs.jctech888.com.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xm.yuexingan06.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fa.chemitech.net.cn

Java: x instanceof Number
来源：http://pb.huixiangedu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jd.shtwfgs.cn

Ruby: x.is_a?(Numeric)
来源：http://vo.jianghongdianzi.cn

C#:   x is int or double or decimal
来源：http://cv.shxzukj.cn

[B14] 判断值是否在集合内
来源：http://he.nszjky.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ip.9csxet.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fb.nszjky.cn

JS:   [1, 2, 3].includes(x)
来源：http://ng.hahajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://jm.chemitech.net.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ll.nszjky.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ir.shxzskj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://sr.hnjuh.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fu.haigaiapp.cn

[B15] 布尔运算与取反
来源：http://kh.yuexingan06.cn

Py:   a and b or not c
来源：http://cs.szxytkj.cn

PHP:  $a && $b || !$c
来源：http://wd.hahajie.cn

JS:   a && b || !c
来源：http://gd.haigaiapp.cn

TS:   a && b || !c
来源：http://hq.huixinmuqiang.cn

Java: a && b || !c
来源：http://fy.asd995.cn

Go:   a && b || !c
来源：http://yw.szsharing.cn

Ruby: a && b || !c
来源：http://vr.chemitech.net.cn

C#:   a && b || !c
来源：http://xm.shtwfgs.cn

[B16] 卫语句：不满足条件提前返回
来源：http://df.wgjwhj.cn

Py:   if not data: return
来源：http://aw.newstarts.cn

PHP:  if (!$data) { return; }
来源：http://zq.szxytkj.cn

JS:   if (!data) return;
来源：http://bc.bookmarksfly.cn

TS:   if (!data) return;
来源：http://qz.gzmigu.cn

Java: if (data == null) return;
来源：http://bg.521024.cn

Go:   if data == nil { return }
来源：http://ky.huanxung.cn

Ruby: return if data.nil?
来源：http://wk.huanxung.cn

C#:   if (data == null) return;
来源：http://mr.panjiajie.cn

================================================================================
来源：http://nd.huanxung.cn

C. 函数与作用域
来源：http://ss.hahajie.cn

================================================================================
来源：http://qj.shtwfgs.cn

[C01] 定义函数
来源：http://gt.nicolike.cn

Py:   def add(a, b): return a + b
来源：http://hv.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tb.bjjhwx.cn

JS:   function add(a, b) { return a + b; }
来源：http://wn.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wd.yuexingan06.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://rn.jianghongdianzi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vz.chemitech.net.cn

Ruby: def add(a, b); a + b; end
来源：http://ig.haigaiapp.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://in.panjiajie.cn

[C02] 默认参数
来源：http://ld.nszjky.cn

Py:   def greet(name="World"): return name
来源：http://qf.panjiajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://nb.lnxyls.cn

JS:   function greet(name = "World") { return name; }
来源：http://vc.nszjky.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zy.asd995.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rd.chemitech.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wh.yuntaijiaju.cn

Ruby: def greet(name = "World") = name
来源：http://pl.chemitech.net.cn

C#:   string Greet(string name = "World") => name;
来源：http://ld.hahajie.cn

[C03] 可变参数
来源：http://rb.shxzskj.cn

Py:   def total(*args): return sum(args)
来源：http://ua.shxzskj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cf.szxytkj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zw.szsharing.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://du.panjiajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bw.newstarts.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ov.szsharing.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fp.shxzskj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ba.521024.cn

[C04] 命名参数 / 关键字参数
来源：http://xn.lnxyls.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://my.yuntaijiaju.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ef.szsharing.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hc.hnjuh.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sx.521024.cn

Java: // 无：用 Builder 模式或 record
来源：http://lk.shtwfgs.cn

Go:   // 无：用配置结构体参数
来源：http://ss.9csxet.cn

Ruby: f(a: 1, b: 2)
来源：http://ps.huanxung.cn

C#:   f(a: 1, b: 2)
来源：http://lu.huixiangedu.cn

[C05] 返回多个值
来源：http://oo.521024.cn

Py:   return a, b
来源：http://nk.huanxung.cn

PHP:  return [$a, $b];
来源：http://ye.colortex.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yp.yuntaijiaju.cn

TS:   return { a, b };
来源：http://qh.jctech888.com.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jf.newstarts.cn

Go:   return a, b
来源：http://bf.huixiangedu.cn

Ruby: return a, b
来源：http://zx.shxzskj.cn

C#:   return (a, b);              // ValueTuple
来源：http://cs.wgjwhj.cn

[C06] 匿名函数 / lambda
来源：http://jw.nszjky.cn

Py:   square = lambda x: x * x
来源：http://iw.colortex.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://na.gzmigu.cn

JS:   const square = x => x * x;
来源：http://kt.521024.cn

TS:   const square = (x: number): number => x * x;
来源：http://dk.wgjwhj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vr.chemitech.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://za.wgjwhj.cn

Ruby: square = ->(x) { x * x }
来源：http://ne.shxzskj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://us.bookmarksfly.cn

[C07] 把函数作为参数传入
来源：http://eu.szsharing.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mk.yuexingan06.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ep.shxzukj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xi.yuntaijiaju.cn

TS:   arr.map(String)
来源：http://as.nicolike.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hs.bookmarksfly.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ai.shxzskj.cn

Ruby: arr.map(&:upcase)
来源：http://dw.yuntaijiaju.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://sa.nicolike.cn

[C08] 闭包
来源：http://tr.asd995.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bo.yuntaijiaju.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qx.shxzukj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gi.shxzukj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://op.colortex.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tp.jctech888.com.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nv.hnjuh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gw.gzmigu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tl.521024.cn

[C09] 递归
来源：http://hj.jctech888.com.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gm.wgjwhj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kp.bjjhwx.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pf.hahajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wx.asd995.cn


<!-- 参考信息 -->