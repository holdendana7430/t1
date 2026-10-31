代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://iv.muxihuayi.cn

Java: (int) 'A'; (char) 65
来源：http://em.huixinmuqiang.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://uj.521024.cn

Ruby: "A".ord; 65.chr
来源：http://xw.lnxyls.cn

C#:   (int)'A'; (char)65
来源：http://xt.newstarts.cn

[A19] 交换两个变量
来源：http://sv.nicolike.cn

Py:   a, b = b, a
来源：http://jx.bookmarksfly.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://mc.muxihuayi.cn

JS:   [a, b] = [b, a];
来源：http://xx.9csxet.cn

TS:   [a, b] = [b, a];
来源：http://la.bookmarksfly.cn

Java: int t = a; a = b; b = t;
来源：http://wo.gzmigu.cn

Go:   a, b = b, a
来源：http://no.colortex.cn

Ruby: a, b = b, a
来源：http://rh.shxzskj.cn

C#:   (a, b) = (b, a);
来源：http://wd.hahajie.cn

[A20] 读取标准输入
来源：http://gv.nszjky.cn

Py:   name = input("请输入：")
来源：http://qr.gzmigu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://qd.bjjhwx.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wz.haigaiapp.cn

TS:   // Node.js：readline 模块
来源：http://xy.asd995.cn

Java: new Scanner(System.in).nextLine()
来源：http://pq.huixiangedu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hw.bjjhwx.cn

Ruby: gets.chomp
来源：http://xy.chemitech.net.cn

C#:   Console.ReadLine();
来源：http://nc.yuexingan06.cn

[A21] 保留指定小数位输出
来源：http://gb.jianghongdianzi.cn

Py:   f"{3.14159:.2f}"
来源：http://pl.shxzukj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://un.shxzukj.cn

JS:   (3.14159).toFixed(2)
来源：http://vb.huixiangedu.cn

TS:   (3.14159).toFixed(2)
来源：http://ij.panjiajie.cn

Java: String.format("%.2f", 3.14159)
来源：http://im.szsharing.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pi.nszjky.cn

Ruby: format("%.2f", 3.14159)
来源：http://ts.huanxung.cn

C#:   3.14159.ToString("F2")
来源：http://fw.bookmarksfly.cn

[A22] 获取字符串长度
来源：http://dg.gzmigu.cn

Py:   len(s)
来源：http://br.gzmigu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tn.shtwfgs.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ra.wgjwhj.cn

TS:   s.length
来源：http://pw.asd995.cn

Java: s.length()
来源：http://hi.yuexingan06.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fi.newstarts.cn

Ruby: s.length
来源：http://cp.wgjwhj.cn

C#:   s.Length
来源：http://yo.wgjwhj.cn

[A23] 大小写转换
来源：http://hr.shxzukj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://kk.yuntaijiaju.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mx.muxihuayi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://sv.wgjwhj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jh.521024.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fu.colortex.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rg.lnxyls.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ye.asd995.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://tx.panjiajie.cn

[A24] 去除首尾空白
来源：http://nv.szsharing.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vp.9csxet.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rm.nicolike.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xy.shxzskj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gs.huixinmuqiang.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cy.panjiajie.cn

Go:   strings.TrimSpace(s)
来源：http://go.haigaiapp.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://io.nszjky.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hf.colortex.cn

[A25] 字符串比较
来源：http://on.haigaiapp.cn

Py:   s1 == s2; s1 != s2
来源：http://oq.yuexingan06.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sd.szsharing.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://as.colortex.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lb.haigaiapp.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jw.yuexingan06.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jc.yuexingan06.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://fv.newstarts.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fh.huanxung.cn

[A26] 类型转换总览
来源：http://ag.lnxyls.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gv.yuntaijiaju.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kl.colortex.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qd.szsharing.cn

TS:   Number() String() Boolean() x as number
来源：http://hx.wgjwhj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ej.shtwfgs.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qc.gzmigu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://sg.szsharing.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ki.chemitech.net.cn

================================================================================
来源：http://fi.bjjhwx.cn

B. 流程控制
来源：http://da.bookmarksfly.cn

================================================================================
来源：http://by.shxzskj.cn

[B01] 条件判断 if / else
来源：http://he.jianghongdianzi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://mw.haigaiapp.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qu.bookmarksfly.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kn.yuexingan06.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pd.shxzskj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://wr.bookmarksfly.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jr.yuexingan06.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dg.nicolike.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ro.asd995.cn

[B02] 多分支 else if / elif
来源：http://hw.shxzukj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xt.nszjky.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rc.huixinmuqiang.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pb.jianghongdianzi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cx.nicolike.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yx.panjiajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://sz.shxzskj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://na.huanxung.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vz.haigaiapp.cn

[B03] switch / match / case
来源：http://nb.wgjwhj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xj.9csxet.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rb.jctech888.com.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ui.szxytkj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://az.nicolike.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pv.jianghongdianzi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://on.jianghongdianzi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jp.hahajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vp.muxihuayi.cn

[B04] for 计数循环
来源：http://wp.szxytkj.cn

Py:   for i in range(10): print(i)
来源：http://nb.chemitech.net.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ub.huanxung.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mq.jianghongdianzi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jk.jianghongdianzi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mn.bookmarksfly.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://sk.shxzukj.cn

Ruby: 10.times { |i| puts i }
来源：http://nt.yuexingan06.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zb.newstarts.cn

[B05] 遍历数组 / 列表
来源：http://lw.huixiangedu.cn

Py:   for item in arr: print(item)
来源：http://yz.shxzukj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yt.shxzskj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://vh.hnjuh.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tz.wgjwhj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://md.shxzskj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fp.asd995.cn

Ruby: arr.each { |item| puts item }
来源：http://ib.nicolike.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hj.szsharing.cn

[B06] 遍历字典 / 对象
来源：http://ly.muxihuayi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zk.haigaiapp.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hw.shxzukj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sn.newstarts.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sj.bookmarksfly.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pl.colortex.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nz.hnjuh.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ch.shxzukj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sp.bjjhwx.cn

[B07] while 循环
来源：http://mp.wgjwhj.cn

Py:   while i < 10: i += 1
来源：http://ha.nicolike.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qp.szxytkj.cn

JS:   while (i < 10) { i++; }
来源：http://hj.jianghongdianzi.cn

TS:   while (i < 10) { i++; }
来源：http://es.szsharing.cn

Java: while (i < 10) { i++; }
来源：http://ts.huanxung.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bf.bjjhwx.cn

Ruby: while i < 10; i += 1; end
来源：http://ri.nszjky.cn

C#:   while (i < 10) { i++; }
来源：http://uq.shxzukj.cn

[B08] do-while（至少执行一次）
来源：http://rj.panjiajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://uz.jctech888.com.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://um.huixiangedu.cn

JS:   do { i++; } while (i < 10);
来源：http://he.wgjwhj.cn

TS:   do { i++; } while (i < 10);
来源：http://yj.lnxyls.cn

Java: do { i++; } while (i < 10);
来源：http://uy.haigaiapp.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ip.shxzukj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fr.yuexingan06.cn

C#:   do { i++; } while (i < 10);
来源：http://sv.asd995.cn

[B09] break 与 continue
来源：http://jz.muxihuayi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jj.gzmigu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mm.yuntaijiaju.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sv.newstarts.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.nszjky.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vi.panjiajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qc.szxytkj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ip.newstarts.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://up.hnjuh.cn

[B10] 遍历同时拿索引
来源：http://kx.shxzskj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zz.nicolike.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://so.bjjhwx.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gn.9csxet.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://in.hahajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wt.521024.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xo.521024.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fi.chemitech.net.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jr.chemitech.net.cn

[B11] 生成数字序列 / 区间
来源：http://ww.hahajie.cn

Py:   list(range(0, 10, 2))
来源：http://bv.szxytkj.cn

PHP:  range(0, 10, 2);
来源：http://tx.szsharing.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zh.9csxet.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vq.muxihuayi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sz.hnjuh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yr.nszjky.cn

Ruby: (0...10).step(2).to_a
来源：http://dl.haigaiapp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sw.huanxung.cn

[B12] 跳出多层循环
来源：http://ng.shxzukj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://sk.jianghongdianzi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://le.shtwfgs.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yb.jianghongdianzi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pl.huixiangedu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cx.huixinmuqiang.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tq.hnjuh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pb.9csxet.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fk.szxytkj.cn

[B13] 判断是否为数字
来源：http://mc.huixinmuqiang.cn

Py:   isinstance(x, (int, float))
来源：http://da.huixinmuqiang.cn

PHP:  is_numeric($x)
来源：http://xw.nicolike.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ql.wgjwhj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://me.huixiangedu.cn

Java: x instanceof Number
来源：http://gx.shxzskj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://in.bjjhwx.cn

Ruby: x.is_a?(Numeric)
来源：http://bw.bjjhwx.cn

C#:   x is int or double or decimal
来源：http://bx.hahajie.cn

[B14] 判断值是否在集合内
来源：http://oi.colortex.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kp.huixiangedu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://re.nicolike.cn

JS:   [1, 2, 3].includes(x)
来源：http://on.shxzskj.cn

TS:   [1, 2, 3].includes(x)
来源：http://ct.huixiangedu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://yd.lnxyls.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gc.yuexingan06.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jh.panjiajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ly.bjjhwx.cn

[B15] 布尔运算与取反
来源：http://dw.haigaiapp.cn

Py:   a and b or not c
来源：http://zi.newstarts.cn

PHP:  $a && $b || !$c
来源：http://pp.colortex.cn

JS:   a && b || !c
来源：http://ca.jianghongdianzi.cn

TS:   a && b || !c
来源：http://hw.szsharing.cn

Java: a && b || !c
来源：http://ra.szxytkj.cn

Go:   a && b || !c
来源：http://wh.nszjky.cn

Ruby: a && b || !c
来源：http://uo.jctech888.com.cn

C#:   a && b || !c
来源：http://nb.szsharing.cn

[B16] 卫语句：不满足条件提前返回
来源：http://kf.yuexingan06.cn

Py:   if not data: return
来源：http://hg.nicolike.cn

PHP:  if (!$data) { return; }
来源：http://vd.nicolike.cn

JS:   if (!data) return;
来源：http://rr.hahajie.cn

TS:   if (!data) return;
来源：http://di.gzmigu.cn

Java: if (data == null) return;
来源：http://za.521024.cn

Go:   if data == nil { return }
来源：http://fq.muxihuayi.cn

Ruby: return if data.nil?
来源：http://lt.yuexingan06.cn

C#:   if (data == null) return;
来源：http://ib.szxytkj.cn

================================================================================
来源：http://vp.yuntaijiaju.cn

C. 函数与作用域
来源：http://qp.9csxet.cn

================================================================================
来源：http://zm.wgjwhj.cn

[C01] 定义函数
来源：http://ml.bjjhwx.cn

Py:   def add(a, b): return a + b
来源：http://cv.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yc.hnjuh.cn

JS:   function add(a, b) { return a + b; }
来源：http://mx.panjiajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ni.nszjky.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ty.chemitech.net.cn

Go:   func add(a, b int) int { return a + b }
来源：http://gz.newstarts.cn

Ruby: def add(a, b); a + b; end
来源：http://sa.shxzskj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wl.shtwfgs.cn

[C02] 默认参数
来源：http://xt.lnxyls.cn

Py:   def greet(name="World"): return name
来源：http://mt.jianghongdianzi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://gj.asd995.cn

JS:   function greet(name = "World") { return name; }
来源：http://vw.szxytkj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qc.colortex.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://gd.huanxung.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sw.szxytkj.cn

Ruby: def greet(name = "World") = name
来源：http://pv.szxytkj.cn

C#:   string Greet(string name = "World") => name;
来源：http://wj.gzmigu.cn

[C03] 可变参数
来源：http://sc.shtwfgs.cn

Py:   def total(*args): return sum(args)
来源：http://vk.nszjky.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lf.nicolike.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mu.nicolike.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cc.shxzskj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ru.newstarts.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bj.colortex.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ks.521024.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gd.lnxyls.cn

[C04] 命名参数 / 关键字参数
来源：http://rc.shxzukj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://at.nicolike.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://td.haigaiapp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lu.jianghongdianzi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dt.hnjuh.cn

Java: // 无：用 Builder 模式或 record
来源：http://sq.colortex.cn

Go:   // 无：用配置结构体参数
来源：http://wa.asd995.cn

Ruby: f(a: 1, b: 2)
来源：http://js.nicolike.cn

C#:   f(a: 1, b: 2)
来源：http://ae.9csxet.cn

[C05] 返回多个值
来源：http://zn.9csxet.cn

Py:   return a, b
来源：http://zq.muxihuayi.cn

PHP:  return [$a, $b];
来源：http://xg.9csxet.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yd.hnjuh.cn

TS:   return { a, b };
来源：http://ql.jctech888.com.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://re.521024.cn

Go:   return a, b
来源：http://zo.colortex.cn

Ruby: return a, b
来源：http://fb.muxihuayi.cn

C#:   return (a, b);              // ValueTuple
来源：http://ue.szxytkj.cn

[C06] 匿名函数 / lambda
来源：http://vk.wgjwhj.cn

Py:   square = lambda x: x * x
来源：http://km.chemitech.net.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fw.huixinmuqiang.cn

JS:   const square = x => x * x;
来源：http://ff.gzmigu.cn

TS:   const square = (x: number): number => x * x;
来源：http://jb.szsharing.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yx.haigaiapp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ni.huixinmuqiang.cn

Ruby: square = ->(x) { x * x }
来源：http://oe.lnxyls.cn

C#:   Func<int, int> square = x => x * x;
来源：http://mb.colortex.cn

[C07] 把函数作为参数传入
来源：http://xu.hnjuh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bs.shxzskj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ai.panjiajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dc.nicolike.cn

TS:   arr.map(String)
来源：http://aj.yuexingan06.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zx.szxytkj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gg.jianghongdianzi.cn

Ruby: arr.map(&:upcase)
来源：http://fc.521024.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://vs.szsharing.cn

[C08] 闭包
来源：http://gh.jianghongdianzi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://sm.haigaiapp.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ky.huanxung.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xa.szsharing.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ym.shxzukj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ul.haigaiapp.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lk.gzmigu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gt.jianghongdianzi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.chemitech.net.cn

[C09] 递归
来源：http://yw.gzmigu.cn


<!-- 参考信息 -->