代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kc.hahajie.cn

Java: (int) 'A'; (char) 65
来源：http://yv.hahajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vp.szsharing.cn

Ruby: "A".ord; 65.chr
来源：http://ve.9csxet.cn

C#:   (int)'A'; (char)65
来源：http://tl.yuexingan06.cn

[A19] 交换两个变量
来源：http://lb.nszjky.cn

Py:   a, b = b, a
来源：http://kl.szsharing.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://en.szxytkj.cn

JS:   [a, b] = [b, a];
来源：http://bn.asd995.cn

TS:   [a, b] = [b, a];
来源：http://jy.panjiajie.cn

Java: int t = a; a = b; b = t;
来源：http://nv.haigaiapp.cn

Go:   a, b = b, a
来源：http://sr.chemitech.net.cn

Ruby: a, b = b, a
来源：http://ht.huanxung.cn

C#:   (a, b) = (b, a);
来源：http://oz.521024.cn

[A20] 读取标准输入
来源：http://hz.szxytkj.cn

Py:   name = input("请输入：")
来源：http://ki.9csxet.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://kh.asd995.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rw.wgjwhj.cn

TS:   // Node.js：readline 模块
来源：http://xu.shxzskj.cn

Java: new Scanner(System.in).nextLine()
来源：http://jk.hahajie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bn.bookmarksfly.cn

Ruby: gets.chomp
来源：http://la.jctech888.com.cn

C#:   Console.ReadLine();
来源：http://sx.nszjky.cn

[A21] 保留指定小数位输出
来源：http://tl.shxzskj.cn

Py:   f"{3.14159:.2f}"
来源：http://ie.nszjky.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ue.shxzskj.cn

JS:   (3.14159).toFixed(2)
来源：http://xv.wgjwhj.cn

TS:   (3.14159).toFixed(2)
来源：http://iq.muxihuayi.cn

Java: String.format("%.2f", 3.14159)
来源：http://oe.bjjhwx.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lt.muxihuayi.cn

Ruby: format("%.2f", 3.14159)
来源：http://ba.szxytkj.cn

C#:   3.14159.ToString("F2")
来源：http://pa.lnxyls.cn

[A22] 获取字符串长度
来源：http://on.yuexingan06.cn

Py:   len(s)
来源：http://wj.yuntaijiaju.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fw.jianghongdianzi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ep.yuexingan06.cn

TS:   s.length
来源：http://nf.jianghongdianzi.cn

Java: s.length()
来源：http://hg.bjjhwx.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ci.nszjky.cn

Ruby: s.length
来源：http://bt.huanxung.cn

C#:   s.Length
来源：http://yn.yuexingan06.cn

[A23] 大小写转换
来源：http://mf.colortex.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://db.shtwfgs.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://df.haigaiapp.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ku.nszjky.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yr.szsharing.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://he.nszjky.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://oh.yuntaijiaju.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://av.huixiangedu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://gm.gzmigu.cn

[A24] 去除首尾空白
来源：http://do.muxihuayi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gp.hahajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sq.9csxet.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xq.colortex.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lh.hahajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wj.huixinmuqiang.cn

Go:   strings.TrimSpace(s)
来源：http://tq.shxzskj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bu.huanxung.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kz.szsharing.cn

[A25] 字符串比较
来源：http://mt.asd995.cn

Py:   s1 == s2; s1 != s2
来源：http://yo.huanxung.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kp.shtwfgs.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://av.colortex.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://il.huixinmuqiang.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jw.szsharing.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wm.hahajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://yt.colortex.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ny.hahajie.cn

[A26] 类型转换总览
来源：http://sp.gzmigu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bw.haigaiapp.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://px.asd995.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ow.szxytkj.cn

TS:   Number() String() Boolean() x as number
来源：http://lh.muxihuayi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xu.bookmarksfly.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ej.nicolike.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://he.huixinmuqiang.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://na.hahajie.cn

================================================================================
来源：http://iz.nicolike.cn

B. 流程控制
来源：http://bc.hnjuh.cn

================================================================================
来源：http://kl.huixiangedu.cn

[B01] 条件判断 if / else
来源：http://lc.shtwfgs.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://aw.muxihuayi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ff.hahajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jb.shxzskj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://an.chemitech.net.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ub.shxzskj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wb.hahajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ov.wgjwhj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mo.huixinmuqiang.cn

[B02] 多分支 else if / elif
来源：http://ko.yuexingan06.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cr.jianghongdianzi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qy.panjiajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ib.shxzukj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bk.bookmarksfly.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rb.jctech888.com.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vo.nszjky.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gx.muxihuayi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rz.wgjwhj.cn

[B03] switch / match / case
来源：http://jo.yuntaijiaju.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gw.asd995.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ta.huanxung.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wv.huixiangedu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zf.chemitech.net.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vj.9csxet.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://en.szxytkj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hn.shxzskj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jj.nszjky.cn

[B04] for 计数循环
来源：http://ft.nszjky.cn

Py:   for i in range(10): print(i)
来源：http://ip.bjjhwx.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ir.9csxet.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rt.huixiangedu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uq.bjjhwx.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zi.szsharing.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mc.colortex.cn

Ruby: 10.times { |i| puts i }
来源：http://yh.bookmarksfly.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mj.lnxyls.cn

[B05] 遍历数组 / 列表
来源：http://zh.nszjky.cn

Py:   for item in arr: print(item)
来源：http://eu.gzmigu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fu.hahajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://oj.hahajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mr.panjiajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gz.chemitech.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fl.bjjhwx.cn

Ruby: arr.each { |item| puts item }
来源：http://gp.lnxyls.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xg.colortex.cn

[B06] 遍历字典 / 对象
来源：http://lm.lnxyls.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sh.shxzukj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dn.newstarts.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ht.szxytkj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zo.muxihuayi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bi.szsharing.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vr.521024.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gx.bookmarksfly.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vs.chemitech.net.cn

[B07] while 循环
来源：http://ji.huixinmuqiang.cn

Py:   while i < 10: i += 1
来源：http://vp.chemitech.net.cn

PHP:  while ($i < 10) { $i++; }
来源：http://kp.szxytkj.cn

JS:   while (i < 10) { i++; }
来源：http://iz.colortex.cn

TS:   while (i < 10) { i++; }
来源：http://km.521024.cn

Java: while (i < 10) { i++; }
来源：http://ow.shtwfgs.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ag.shtwfgs.cn

Ruby: while i < 10; i += 1; end
来源：http://zy.shxzukj.cn

C#:   while (i < 10) { i++; }
来源：http://sm.huixiangedu.cn

[B08] do-while（至少执行一次）
来源：http://oe.gzmigu.cn

Py:   # 无 do-while：用 while True + break
来源：http://ap.hnjuh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cu.asd995.cn

JS:   do { i++; } while (i < 10);
来源：http://zq.chemitech.net.cn

TS:   do { i++; } while (i < 10);
来源：http://yx.hahajie.cn

Java: do { i++; } while (i < 10);
来源：http://kb.haigaiapp.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ri.nicolike.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ky.colortex.cn

C#:   do { i++; } while (i < 10);
来源：http://ig.huixiangedu.cn

[B09] break 与 continue
来源：http://pw.colortex.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yi.muxihuayi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ay.huixinmuqiang.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nn.huanxung.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jk.jianghongdianzi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fc.wgjwhj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ea.gzmigu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vk.shtwfgs.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bm.yuntaijiaju.cn

[B10] 遍历同时拿索引
来源：http://ib.yuexingan06.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://om.nszjky.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ul.bjjhwx.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ee.lnxyls.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zf.huixinmuqiang.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bc.muxihuayi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lz.szsharing.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://an.huixinmuqiang.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://aw.yuexingan06.cn

[B11] 生成数字序列 / 区间
来源：http://mb.chemitech.net.cn

Py:   list(range(0, 10, 2))
来源：http://gf.bookmarksfly.cn

PHP:  range(0, 10, 2);
来源：http://la.asd995.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ry.521024.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qe.jctech888.com.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sm.newstarts.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://aa.lnxyls.cn

Ruby: (0...10).step(2).to_a
来源：http://uk.colortex.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jr.colortex.cn

[B12] 跳出多层循环
来源：http://mj.wgjwhj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bh.huixiangedu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://aa.szxytkj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zy.haigaiapp.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yy.521024.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cu.yuntaijiaju.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sk.nszjky.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wc.muxihuayi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://oo.bjjhwx.cn

[B13] 判断是否为数字
来源：http://gt.newstarts.cn

Py:   isinstance(x, (int, float))
来源：http://nc.nicolike.cn

PHP:  is_numeric($x)
来源：http://za.jianghongdianzi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ny.jianghongdianzi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kd.panjiajie.cn

Java: x instanceof Number
来源：http://fp.lnxyls.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mu.nicolike.cn

Ruby: x.is_a?(Numeric)
来源：http://ho.bookmarksfly.cn

C#:   x is int or double or decimal
来源：http://px.wgjwhj.cn

[B14] 判断值是否在集合内
来源：http://th.bookmarksfly.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nw.chemitech.net.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lo.huixiangedu.cn

JS:   [1, 2, 3].includes(x)
来源：http://cu.szsharing.cn

TS:   [1, 2, 3].includes(x)
来源：http://cf.haigaiapp.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://cm.9csxet.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vu.chemitech.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://yn.huixinmuqiang.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kf.shxzskj.cn

[B15] 布尔运算与取反
来源：http://mp.hnjuh.cn

Py:   a and b or not c
来源：http://fi.jctech888.com.cn

PHP:  $a && $b || !$c
来源：http://ko.asd995.cn

JS:   a && b || !c
来源：http://ae.haigaiapp.cn

TS:   a && b || !c
来源：http://ur.hnjuh.cn

Java: a && b || !c
来源：http://jj.szsharing.cn

Go:   a && b || !c
来源：http://bq.huixiangedu.cn

Ruby: a && b || !c
来源：http://ky.bjjhwx.cn

C#:   a && b || !c
来源：http://sd.muxihuayi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://yj.huanxung.cn

Py:   if not data: return
来源：http://ry.shxzskj.cn

PHP:  if (!$data) { return; }
来源：http://ns.nicolike.cn

JS:   if (!data) return;
来源：http://mo.yuntaijiaju.cn

TS:   if (!data) return;
来源：http://zx.wgjwhj.cn

Java: if (data == null) return;
来源：http://zu.bookmarksfly.cn

Go:   if data == nil { return }
来源：http://bs.hahajie.cn

Ruby: return if data.nil?
来源：http://vw.hnjuh.cn

C#:   if (data == null) return;
来源：http://rz.szsharing.cn

================================================================================
来源：http://dj.colortex.cn

C. 函数与作用域
来源：http://mu.nszjky.cn

================================================================================
来源：http://ua.huixinmuqiang.cn

[C01] 定义函数
来源：http://aj.lnxyls.cn

Py:   def add(a, b): return a + b
来源：http://fn.shxzskj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kp.hnjuh.cn

JS:   function add(a, b) { return a + b; }
来源：http://ru.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xw.wgjwhj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://yw.yuexingan06.cn

Go:   func add(a, b int) int { return a + b }
来源：http://iy.chemitech.net.cn

Ruby: def add(a, b); a + b; end
来源：http://ah.shxzskj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zy.huanxung.cn

[C02] 默认参数
来源：http://ov.newstarts.cn

Py:   def greet(name="World"): return name
来源：http://ra.521024.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xm.hahajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://uq.colortex.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zg.panjiajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://en.huanxung.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tj.muxihuayi.cn

Ruby: def greet(name = "World") = name
来源：http://ym.panjiajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://eg.szxytkj.cn

[C03] 可变参数
来源：http://pd.bjjhwx.cn

Py:   def total(*args): return sum(args)
来源：http://vh.lnxyls.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mh.panjiajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xk.yuexingan06.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xm.jianghongdianzi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vq.521024.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kv.jianghongdianzi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ns.9csxet.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hk.521024.cn

[C04] 命名参数 / 关键字参数
来源：http://jb.shtwfgs.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fa.bjjhwx.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hc.shxzukj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://df.gzmigu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://py.muxihuayi.cn

Java: // 无：用 Builder 模式或 record
来源：http://sm.szsharing.cn

Go:   // 无：用配置结构体参数
来源：http://wo.gzmigu.cn

Ruby: f(a: 1, b: 2)
来源：http://ut.gzmigu.cn

C#:   f(a: 1, b: 2)
来源：http://kq.newstarts.cn

[C05] 返回多个值
来源：http://jc.jctech888.com.cn

Py:   return a, b
来源：http://tl.szxytkj.cn

PHP:  return [$a, $b];
来源：http://vd.szxytkj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://mf.yuexingan06.cn

TS:   return { a, b };
来源：http://da.asd995.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fo.nszjky.cn

Go:   return a, b
来源：http://km.muxihuayi.cn

Ruby: return a, b
来源：http://iq.yuexingan06.cn

C#:   return (a, b);              // ValueTuple
来源：http://yg.hnjuh.cn

[C06] 匿名函数 / lambda
来源：http://hq.lnxyls.cn

Py:   square = lambda x: x * x
来源：http://iy.hahajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://en.shtwfgs.cn

JS:   const square = x => x * x;
来源：http://hc.bookmarksfly.cn

TS:   const square = (x: number): number => x * x;
来源：http://sp.gzmigu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rt.nicolike.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fr.bookmarksfly.cn

Ruby: square = ->(x) { x * x }
来源：http://qw.szxytkj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://vk.szxytkj.cn

[C07] 把函数作为参数传入
来源：http://gf.huanxung.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xi.panjiajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kb.jianghongdianzi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qm.bookmarksfly.cn

TS:   arr.map(String)
来源：http://wv.yuexingan06.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://te.jianghongdianzi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qo.shtwfgs.cn

Ruby: arr.map(&:upcase)
来源：http://al.huixiangedu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://rg.shxzskj.cn

[C08] 闭包
来源：http://wq.yuexingan06.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nj.9csxet.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hv.bookmarksfly.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dd.yuexingan06.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://iz.bookmarksfly.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fb.haigaiapp.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ie.hnjuh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pb.shxzskj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ko.colortex.cn

[C09] 递归
来源：http://oc.newstarts.cn


<!-- 参考信息 -->