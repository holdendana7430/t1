代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://gf.hnjuh.cn

Py:   ord("A"); chr(65)
来源：http://qi.9csxet.cn

PHP:  ord("A"); chr(65)
来源：http://du.huixiangedu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pd.huanxung.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://db.9csxet.cn

Java: (int) 'A'; (char) 65
来源：http://ln.jctech888.com.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xk.bjjhwx.cn

Ruby: "A".ord; 65.chr
来源：http://ec.shxzskj.cn

C#:   (int)'A'; (char)65
来源：http://fi.huixiangedu.cn

[A19] 交换两个变量
来源：http://hw.shxzukj.cn

Py:   a, b = b, a
来源：http://ax.huanxung.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://df.chemitech.net.cn

JS:   [a, b] = [b, a];
来源：http://go.shxzskj.cn

TS:   [a, b] = [b, a];
来源：http://gt.nicolike.cn

Java: int t = a; a = b; b = t;
来源：http://kt.hahajie.cn

Go:   a, b = b, a
来源：http://id.nszjky.cn

Ruby: a, b = b, a
来源：http://uf.haigaiapp.cn

C#:   (a, b) = (b, a);
来源：http://ii.wgjwhj.cn

[A20] 读取标准输入
来源：http://ot.lnxyls.cn

Py:   name = input("请输入：")
来源：http://ci.colortex.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ep.huixiangedu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qr.szxytkj.cn

TS:   // Node.js：readline 模块
来源：http://jn.jctech888.com.cn

Java: new Scanner(System.in).nextLine()
来源：http://yu.nszjky.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qp.shtwfgs.cn

Ruby: gets.chomp
来源：http://az.muxihuayi.cn

C#:   Console.ReadLine();
来源：http://az.521024.cn

[A21] 保留指定小数位输出
来源：http://en.bookmarksfly.cn

Py:   f"{3.14159:.2f}"
来源：http://jj.bjjhwx.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rm.wgjwhj.cn

JS:   (3.14159).toFixed(2)
来源：http://al.nicolike.cn

TS:   (3.14159).toFixed(2)
来源：http://lv.jctech888.com.cn

Java: String.format("%.2f", 3.14159)
来源：http://yo.yuexingan06.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://im.asd995.cn

Ruby: format("%.2f", 3.14159)
来源：http://tj.shtwfgs.cn

C#:   3.14159.ToString("F2")
来源：http://xv.lnxyls.cn

[A22] 获取字符串长度
来源：http://jb.shxzskj.cn

Py:   len(s)
来源：http://rg.huixinmuqiang.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tq.jctech888.com.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pg.nicolike.cn

TS:   s.length
来源：http://ap.wgjwhj.cn

Java: s.length()
来源：http://qe.yuexingan06.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kb.bookmarksfly.cn

Ruby: s.length
来源：http://pu.shtwfgs.cn

C#:   s.Length
来源：http://mf.huixiangedu.cn

[A23] 大小写转换
来源：http://tj.9csxet.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://fo.chemitech.net.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bi.bjjhwx.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hf.szxytkj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ej.szsharing.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gb.yuntaijiaju.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cn.bookmarksfly.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qk.huanxung.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qq.hahajie.cn

[A24] 去除首尾空白
来源：http://il.bookmarksfly.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vv.bjjhwx.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kb.panjiajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nr.nicolike.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dx.jianghongdianzi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://px.hnjuh.cn

Go:   strings.TrimSpace(s)
来源：http://fj.nicolike.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qj.szsharing.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ln.shxzukj.cn

[A25] 字符串比较
来源：http://cs.asd995.cn

Py:   s1 == s2; s1 != s2
来源：http://db.lnxyls.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ww.gzmigu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://sz.shxzskj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://sb.haigaiapp.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ol.huanxung.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fr.shxzukj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ra.huixiangedu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ax.bjjhwx.cn

[A26] 类型转换总览
来源：http://gl.521024.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kr.huixinmuqiang.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sf.huixinmuqiang.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://lu.yuntaijiaju.cn

TS:   Number() String() Boolean() x as number
来源：http://ig.jianghongdianzi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cq.newstarts.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qq.yuexingan06.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://nk.huixiangedu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://on.huixinmuqiang.cn

================================================================================
来源：http://dv.lnxyls.cn

B. 流程控制
来源：http://jb.newstarts.cn

================================================================================
来源：http://jy.jianghongdianzi.cn

[B01] 条件判断 if / else
来源：http://wj.shtwfgs.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ld.521024.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mu.nicolike.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xb.bookmarksfly.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tq.hahajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://tk.shxzukj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zr.hahajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cv.huanxung.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jf.lnxyls.cn

[B02] 多分支 else if / elif
来源：http://ij.yuntaijiaju.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bk.bjjhwx.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hd.521024.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ol.huixiangedu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rl.521024.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xj.panjiajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mz.jctech888.com.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ac.huanxung.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bh.muxihuayi.cn

[B03] switch / match / case
来源：http://lg.newstarts.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ph.wgjwhj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gt.9csxet.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nq.newstarts.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rz.bookmarksfly.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://th.hnjuh.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yb.yuntaijiaju.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://aw.muxihuayi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kq.lnxyls.cn

[B04] for 计数循环
来源：http://yw.jianghongdianzi.cn

Py:   for i in range(10): print(i)
来源：http://hm.shxzskj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xz.huixiangedu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ab.panjiajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yf.chemitech.net.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bv.yuntaijiaju.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vr.nicolike.cn

Ruby: 10.times { |i| puts i }
来源：http://mw.chemitech.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lh.muxihuayi.cn

[B05] 遍历数组 / 列表
来源：http://zi.nszjky.cn

Py:   for item in arr: print(item)
来源：http://wd.hahajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hh.shxzskj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://xo.lnxyls.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://hb.gzmigu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://dx.shtwfgs.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mo.shtwfgs.cn

Ruby: arr.each { |item| puts item }
来源：http://cn.bjjhwx.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xh.muxihuayi.cn

[B06] 遍历字典 / 对象
来源：http://uv.huixiangedu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sl.panjiajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hb.yuexingan06.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cg.lnxyls.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gt.shxzskj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://un.yuexingan06.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pj.jianghongdianzi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rl.newstarts.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://di.muxihuayi.cn

[B07] while 循环
来源：http://lr.jianghongdianzi.cn

Py:   while i < 10: i += 1
来源：http://yp.haigaiapp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hg.shtwfgs.cn

JS:   while (i < 10) { i++; }
来源：http://mq.huixiangedu.cn

TS:   while (i < 10) { i++; }
来源：http://dd.hnjuh.cn

Java: while (i < 10) { i++; }
来源：http://ce.chemitech.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nw.9csxet.cn

Ruby: while i < 10; i += 1; end
来源：http://ww.shxzskj.cn

C#:   while (i < 10) { i++; }
来源：http://uk.muxihuayi.cn

[B08] do-while（至少执行一次）
来源：http://hm.521024.cn

Py:   # 无 do-while：用 while True + break
来源：http://yn.yuntaijiaju.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://fq.shtwfgs.cn

JS:   do { i++; } while (i < 10);
来源：http://cr.hnjuh.cn

TS:   do { i++; } while (i < 10);
来源：http://mz.gzmigu.cn

Java: do { i++; } while (i < 10);
来源：http://jx.bookmarksfly.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://my.muxihuayi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wl.bjjhwx.cn

C#:   do { i++; } while (i < 10);
来源：http://ea.panjiajie.cn

[B09] break 与 continue
来源：http://rl.gzmigu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xo.jianghongdianzi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cr.bookmarksfly.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yz.hahajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ii.lnxyls.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gm.colortex.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tn.shxzskj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jr.shxzskj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mz.shxzskj.cn

[B10] 遍历同时拿索引
来源：http://fj.muxihuayi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bl.huanxung.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://or.hnjuh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://af.huixinmuqiang.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uu.huanxung.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dd.bookmarksfly.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://si.yuexingan06.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dk.huixinmuqiang.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wb.wgjwhj.cn

[B11] 生成数字序列 / 区间
来源：http://qx.lnxyls.cn

Py:   list(range(0, 10, 2))
来源：http://iz.9csxet.cn

PHP:  range(0, 10, 2);
来源：http://dn.9csxet.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mp.yuexingan06.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fl.huixinmuqiang.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pu.colortex.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ed.asd995.cn

Ruby: (0...10).step(2).to_a
来源：http://gn.yuntaijiaju.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pq.shxzukj.cn

[B12] 跳出多层循环
来源：http://zp.huanxung.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://db.hahajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://sv.haigaiapp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ba.newstarts.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ec.szsharing.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qr.huixinmuqiang.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rf.gzmigu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pl.szsharing.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cz.shtwfgs.cn

[B13] 判断是否为数字
来源：http://cr.gzmigu.cn

Py:   isinstance(x, (int, float))
来源：http://nm.muxihuayi.cn

PHP:  is_numeric($x)
来源：http://mm.gzmigu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gv.shxzskj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://th.hnjuh.cn

Java: x instanceof Number
来源：http://or.shtwfgs.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wt.shxzukj.cn

Ruby: x.is_a?(Numeric)
来源：http://zg.nszjky.cn

C#:   x is int or double or decimal
来源：http://ou.521024.cn

[B14] 判断值是否在集合内
来源：http://dz.9csxet.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mf.huixinmuqiang.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ar.newstarts.cn

JS:   [1, 2, 3].includes(x)
来源：http://qz.huanxung.cn

TS:   [1, 2, 3].includes(x)
来源：http://ps.huixinmuqiang.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://if.hnjuh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://et.lnxyls.cn

Ruby: [1, 2, 3].include?(x)
来源：http://az.yuntaijiaju.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fj.szxytkj.cn

[B15] 布尔运算与取反
来源：http://vo.shxzskj.cn

Py:   a and b or not c
来源：http://sc.huixiangedu.cn

PHP:  $a && $b || !$c
来源：http://dk.panjiajie.cn

JS:   a && b || !c
来源：http://lr.bookmarksfly.cn

TS:   a && b || !c
来源：http://zy.bookmarksfly.cn

Java: a && b || !c
来源：http://gx.gzmigu.cn

Go:   a && b || !c
来源：http://ol.9csxet.cn

Ruby: a && b || !c
来源：http://nw.jctech888.com.cn

C#:   a && b || !c
来源：http://if.9csxet.cn

[B16] 卫语句：不满足条件提前返回
来源：http://cn.shxzskj.cn

Py:   if not data: return
来源：http://gk.hahajie.cn

PHP:  if (!$data) { return; }
来源：http://qr.gzmigu.cn

JS:   if (!data) return;
来源：http://qy.chemitech.net.cn

TS:   if (!data) return;
来源：http://xp.newstarts.cn

Java: if (data == null) return;
来源：http://om.shxzukj.cn

Go:   if data == nil { return }
来源：http://he.newstarts.cn

Ruby: return if data.nil?
来源：http://gc.szxytkj.cn

C#:   if (data == null) return;
来源：http://sy.huixinmuqiang.cn

================================================================================
来源：http://sx.huixinmuqiang.cn

C. 函数与作用域
来源：http://jv.huixinmuqiang.cn

================================================================================
来源：http://oc.muxihuayi.cn

[C01] 定义函数
来源：http://mx.jctech888.com.cn

Py:   def add(a, b): return a + b
来源：http://wo.hahajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://un.newstarts.cn

JS:   function add(a, b) { return a + b; }
来源：http://kw.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fa.colortex.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://uj.jctech888.com.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zs.panjiajie.cn

Ruby: def add(a, b); a + b; end
来源：http://ti.asd995.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jb.shtwfgs.cn

[C02] 默认参数
来源：http://vh.chemitech.net.cn

Py:   def greet(name="World"): return name
来源：http://ln.521024.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tn.huanxung.cn

JS:   function greet(name = "World") { return name; }
来源：http://vf.bookmarksfly.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ds.colortex.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fw.huixiangedu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ju.chemitech.net.cn

Ruby: def greet(name = "World") = name
来源：http://fj.hnjuh.cn

C#:   string Greet(string name = "World") => name;
来源：http://iv.shtwfgs.cn

[C03] 可变参数
来源：http://cd.nszjky.cn

Py:   def total(*args): return sum(args)
来源：http://fr.bookmarksfly.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tv.shtwfgs.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jp.muxihuayi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gm.nszjky.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dz.asd995.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kt.asd995.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xh.panjiajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ai.muxihuayi.cn

[C04] 命名参数 / 关键字参数
来源：http://xc.bjjhwx.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yv.521024.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gy.9csxet.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hx.muxihuayi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jt.huixinmuqiang.cn

Java: // 无：用 Builder 模式或 record
来源：http://vk.hnjuh.cn

Go:   // 无：用配置结构体参数
来源：http://qg.muxihuayi.cn

Ruby: f(a: 1, b: 2)
来源：http://so.521024.cn

C#:   f(a: 1, b: 2)
来源：http://om.yuexingan06.cn

[C05] 返回多个值
来源：http://kz.yuexingan06.cn

Py:   return a, b
来源：http://gb.yuexingan06.cn

PHP:  return [$a, $b];
来源：http://pw.newstarts.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://lg.huixinmuqiang.cn

TS:   return { a, b };
来源：http://xu.panjiajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pt.muxihuayi.cn

Go:   return a, b
来源：http://jh.gzmigu.cn

Ruby: return a, b
来源：http://ez.jianghongdianzi.cn

C#:   return (a, b);              // ValueTuple
来源：http://um.shxzukj.cn

[C06] 匿名函数 / lambda
来源：http://jy.wgjwhj.cn

Py:   square = lambda x: x * x
来源：http://ra.chemitech.net.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://tu.shxzskj.cn

JS:   const square = x => x * x;
来源：http://hg.lnxyls.cn

TS:   const square = (x: number): number => x * x;
来源：http://or.nszjky.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ak.szxytkj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ki.nicolike.cn

Ruby: square = ->(x) { x * x }
来源：http://rw.bookmarksfly.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ad.panjiajie.cn

[C07] 把函数作为参数传入
来源：http://yw.chemitech.net.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ax.hahajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kw.yuexingan06.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mb.yuntaijiaju.cn

TS:   arr.map(String)
来源：http://og.jianghongdianzi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://eg.newstarts.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bd.lnxyls.cn

Ruby: arr.map(&:upcase)
来源：http://rv.9csxet.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fg.nszjky.cn

[C08] 闭包
来源：http://or.szxytkj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zh.shxzukj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vn.521024.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yc.wgjwhj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kn.nszjky.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dj.szxytkj.cn


<!-- 参考信息 -->