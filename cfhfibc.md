代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hk.huixiangedu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gk.9csxet.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ir.muxihuayi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qo.521024.cn

[A18] 字符与 ASCII 码互转
来源：http://yd.bookmarksfly.cn

Py:   ord("A"); chr(65)
来源：http://sg.szxytkj.cn

PHP:  ord("A"); chr(65)
来源：http://yh.jianghongdianzi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ns.hahajie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://id.bjjhwx.cn

Java: (int) 'A'; (char) 65
来源：http://qn.hahajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rm.521024.cn

Ruby: "A".ord; 65.chr
来源：http://vm.521024.cn

C#:   (int)'A'; (char)65
来源：http://yn.colortex.cn

[A19] 交换两个变量
来源：http://pf.9csxet.cn

Py:   a, b = b, a
来源：http://iw.9csxet.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://io.yuntaijiaju.cn

JS:   [a, b] = [b, a];
来源：http://xb.chemitech.net.cn

TS:   [a, b] = [b, a];
来源：http://yq.szxytkj.cn

Java: int t = a; a = b; b = t;
来源：http://bv.wgjwhj.cn

Go:   a, b = b, a
来源：http://sj.bjjhwx.cn

Ruby: a, b = b, a
来源：http://lz.gzmigu.cn

C#:   (a, b) = (b, a);
来源：http://ee.asd995.cn

[A20] 读取标准输入
来源：http://gp.shxzskj.cn

Py:   name = input("请输入：")
来源：http://dk.nicolike.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://gn.wgjwhj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lb.shxzskj.cn

TS:   // Node.js：readline 模块
来源：http://uq.newstarts.cn

Java: new Scanner(System.in).nextLine()
来源：http://je.chemitech.net.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vr.nszjky.cn

Ruby: gets.chomp
来源：http://ff.hnjuh.cn

C#:   Console.ReadLine();
来源：http://hf.jianghongdianzi.cn

[A21] 保留指定小数位输出
来源：http://lx.yuntaijiaju.cn

Py:   f"{3.14159:.2f}"
来源：http://no.hnjuh.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gb.gzmigu.cn

JS:   (3.14159).toFixed(2)
来源：http://pl.hahajie.cn

TS:   (3.14159).toFixed(2)
来源：http://ty.shxzukj.cn

Java: String.format("%.2f", 3.14159)
来源：http://cb.panjiajie.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sd.shxzukj.cn

Ruby: format("%.2f", 3.14159)
来源：http://gc.521024.cn

C#:   3.14159.ToString("F2")
来源：http://gh.521024.cn

[A22] 获取字符串长度
来源：http://nl.bookmarksfly.cn

Py:   len(s)
来源：http://jn.newstarts.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fi.wgjwhj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ug.jctech888.com.cn

TS:   s.length
来源：http://vl.szsharing.cn

Java: s.length()
来源：http://il.muxihuayi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vx.gzmigu.cn

Ruby: s.length
来源：http://us.colortex.cn

C#:   s.Length
来源：http://kn.panjiajie.cn

[A23] 大小写转换
来源：http://sr.hnjuh.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ky.bjjhwx.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://uj.shxzukj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qo.newstarts.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jp.jianghongdianzi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://iq.haigaiapp.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kw.szsharing.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://aw.bjjhwx.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zh.szsharing.cn

[A24] 去除首尾空白
来源：http://bf.panjiajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fp.panjiajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bt.panjiajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zh.hahajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ty.9csxet.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://yq.huixinmuqiang.cn

Go:   strings.TrimSpace(s)
来源：http://ae.shtwfgs.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ml.panjiajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gv.yuntaijiaju.cn

[A25] 字符串比较
来源：http://ds.panjiajie.cn

Py:   s1 == s2; s1 != s2
来源：http://iz.wgjwhj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wz.yuexingan06.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pn.huanxung.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ug.jianghongdianzi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vy.hahajie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rc.panjiajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ic.gzmigu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pp.szsharing.cn

[A26] 类型转换总览
来源：http://mn.huixinmuqiang.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ty.chemitech.net.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ir.huixinmuqiang.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://go.shxzskj.cn

TS:   Number() String() Boolean() x as number
来源：http://oy.bookmarksfly.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zy.jianghongdianzi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ve.jianghongdianzi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://on.panjiajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yu.shxzukj.cn

================================================================================
来源：http://qg.521024.cn

B. 流程控制
来源：http://vc.nszjky.cn

================================================================================
来源：http://ff.nszjky.cn

[B01] 条件判断 if / else
来源：http://ta.szxytkj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ds.newstarts.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ea.panjiajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wb.jctech888.com.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ej.muxihuayi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ls.yuexingan06.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://it.haigaiapp.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kt.szsharing.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kq.gzmigu.cn

[B02] 多分支 else if / elif
来源：http://cd.szxytkj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ay.wgjwhj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qg.huixinmuqiang.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rg.szsharing.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xv.gzmigu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qz.shxzskj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yp.nicolike.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gq.colortex.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rk.muxihuayi.cn

[B03] switch / match / case
来源：http://to.jctech888.com.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ex.huixiangedu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://iu.shxzskj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gs.jianghongdianzi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cd.gzmigu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jw.asd995.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uf.jianghongdianzi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dh.jctech888.com.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tl.muxihuayi.cn

[B04] for 计数循环
来源：http://yu.huixinmuqiang.cn

Py:   for i in range(10): print(i)
来源：http://fk.huixinmuqiang.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ls.bjjhwx.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dg.hahajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://or.yuexingan06.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vh.szxytkj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jb.shxzskj.cn

Ruby: 10.times { |i| puts i }
来源：http://mv.shxzukj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://as.huanxung.cn

[B05] 遍历数组 / 列表
来源：http://lk.huixinmuqiang.cn

Py:   for item in arr: print(item)
来源：http://ro.hnjuh.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lz.yuntaijiaju.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://lh.yuntaijiaju.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://oy.szxytkj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qs.lnxyls.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fx.shxzskj.cn

Ruby: arr.each { |item| puts item }
来源：http://mt.yuexingan06.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kz.huixiangedu.cn

[B06] 遍历字典 / 对象
来源：http://er.huixinmuqiang.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://gk.gzmigu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hv.newstarts.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wq.hahajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uh.wgjwhj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xq.bjjhwx.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xc.bjjhwx.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://iy.yuntaijiaju.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rj.hnjuh.cn

[B07] while 循环
来源：http://yi.shxzukj.cn

Py:   while i < 10: i += 1
来源：http://dj.bookmarksfly.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zd.panjiajie.cn

JS:   while (i < 10) { i++; }
来源：http://vi.colortex.cn

TS:   while (i < 10) { i++; }
来源：http://sb.bookmarksfly.cn

Java: while (i < 10) { i++; }
来源：http://mk.bjjhwx.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zi.bjjhwx.cn

Ruby: while i < 10; i += 1; end
来源：http://fn.yuntaijiaju.cn

C#:   while (i < 10) { i++; }
来源：http://iz.hahajie.cn

[B08] do-while（至少执行一次）
来源：http://gx.shxzskj.cn

Py:   # 无 do-while：用 while True + break
来源：http://xa.hnjuh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://yw.huixiangedu.cn

JS:   do { i++; } while (i < 10);
来源：http://kw.bookmarksfly.cn

TS:   do { i++; } while (i < 10);
来源：http://tw.newstarts.cn

Java: do { i++; } while (i < 10);
来源：http://oc.jctech888.com.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://km.huixiangedu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vd.gzmigu.cn

C#:   do { i++; } while (i < 10);
来源：http://yp.huanxung.cn

[B09] break 与 continue
来源：http://zy.shtwfgs.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jh.yuntaijiaju.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ep.haigaiapp.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vz.yuntaijiaju.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qy.wgjwhj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fl.wgjwhj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://py.jctech888.com.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gz.colortex.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wf.shxzskj.cn

[B10] 遍历同时拿索引
来源：http://lt.shxzukj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://eg.huixinmuqiang.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ar.szsharing.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fw.asd995.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qi.yuexingan06.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hg.huixiangedu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ps.szsharing.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gc.jianghongdianzi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://op.yuexingan06.cn

[B11] 生成数字序列 / 区间
来源：http://oo.shxzukj.cn

Py:   list(range(0, 10, 2))
来源：http://jt.haigaiapp.cn

PHP:  range(0, 10, 2);
来源：http://dp.colortex.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kr.wgjwhj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ea.bjjhwx.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ez.asd995.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cy.shxzskj.cn

Ruby: (0...10).step(2).to_a
来源：http://zi.nszjky.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://um.lnxyls.cn

[B12] 跳出多层循环
来源：http://ow.jctech888.com.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xe.wgjwhj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://xi.szsharing.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yg.huanxung.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ij.panjiajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mi.yuexingan06.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xn.gzmigu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ou.newstarts.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gj.nszjky.cn

[B13] 判断是否为数字
来源：http://rw.szxytkj.cn

Py:   isinstance(x, (int, float))
来源：http://ts.hnjuh.cn

PHP:  is_numeric($x)
来源：http://vw.wgjwhj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vl.gzmigu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uz.shxzskj.cn

Java: x instanceof Number
来源：http://gc.panjiajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xo.shxzukj.cn

Ruby: x.is_a?(Numeric)
来源：http://nw.newstarts.cn

C#:   x is int or double or decimal
来源：http://wm.bjjhwx.cn

[B14] 判断值是否在集合内
来源：http://wv.yuexingan06.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ay.bookmarksfly.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gn.panjiajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://ie.shxzskj.cn

TS:   [1, 2, 3].includes(x)
来源：http://lq.shtwfgs.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://mu.szxytkj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mo.bjjhwx.cn

Ruby: [1, 2, 3].include?(x)
来源：http://dv.hahajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qv.huixinmuqiang.cn

[B15] 布尔运算与取反
来源：http://jp.huixiangedu.cn

Py:   a and b or not c
来源：http://su.bjjhwx.cn

PHP:  $a && $b || !$c
来源：http://sl.asd995.cn

JS:   a && b || !c
来源：http://ws.jianghongdianzi.cn

TS:   a && b || !c
来源：http://cb.newstarts.cn

Java: a && b || !c
来源：http://cg.hahajie.cn

Go:   a && b || !c
来源：http://dh.521024.cn

Ruby: a && b || !c
来源：http://ee.shtwfgs.cn

C#:   a && b || !c
来源：http://hv.huixiangedu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://mf.9csxet.cn

Py:   if not data: return
来源：http://xf.nszjky.cn

PHP:  if (!$data) { return; }
来源：http://ed.gzmigu.cn

JS:   if (!data) return;
来源：http://pi.shtwfgs.cn

TS:   if (!data) return;
来源：http://qo.lnxyls.cn

Java: if (data == null) return;
来源：http://sq.szsharing.cn

Go:   if data == nil { return }
来源：http://cb.bjjhwx.cn

Ruby: return if data.nil?
来源：http://tu.muxihuayi.cn

C#:   if (data == null) return;
来源：http://cx.nicolike.cn

================================================================================
来源：http://tz.shxzukj.cn

C. 函数与作用域
来源：http://ye.yuntaijiaju.cn

================================================================================
来源：http://ps.asd995.cn

[C01] 定义函数
来源：http://rd.hnjuh.cn

Py:   def add(a, b): return a + b
来源：http://lo.haigaiapp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nj.shxzukj.cn

JS:   function add(a, b) { return a + b; }
来源：http://ss.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://if.hahajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qs.lnxyls.cn

Go:   func add(a, b int) int { return a + b }
来源：http://nx.bjjhwx.cn

Ruby: def add(a, b); a + b; end
来源：http://de.huixiangedu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sy.521024.cn

[C02] 默认参数
来源：http://el.9csxet.cn

Py:   def greet(name="World"): return name
来源：http://ad.nicolike.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://pb.hnjuh.cn

JS:   function greet(name = "World") { return name; }
来源：http://sd.shxzskj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gb.newstarts.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ze.jianghongdianzi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rl.gzmigu.cn

Ruby: def greet(name = "World") = name
来源：http://pj.panjiajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://if.nicolike.cn

[C03] 可变参数
来源：http://zz.huixinmuqiang.cn

Py:   def total(*args): return sum(args)
来源：http://eu.shtwfgs.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dk.shxzskj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://se.lnxyls.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pt.szsharing.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bn.szxytkj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ra.chemitech.net.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qg.bjjhwx.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gl.bookmarksfly.cn

[C04] 命名参数 / 关键字参数
来源：http://mt.panjiajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sa.jctech888.com.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ip.jctech888.com.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ib.bookmarksfly.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ik.yuexingan06.cn

Java: // 无：用 Builder 模式或 record
来源：http://wm.chemitech.net.cn

Go:   // 无：用配置结构体参数
来源：http://og.szsharing.cn

Ruby: f(a: 1, b: 2)
来源：http://xm.wgjwhj.cn

C#:   f(a: 1, b: 2)
来源：http://tm.haigaiapp.cn

[C05] 返回多个值
来源：http://bh.muxihuayi.cn

Py:   return a, b
来源：http://sz.shxzukj.cn

PHP:  return [$a, $b];
来源：http://vt.lnxyls.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jc.colortex.cn

TS:   return { a, b };
来源：http://zx.shxzukj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ms.chemitech.net.cn

Go:   return a, b
来源：http://ut.lnxyls.cn

Ruby: return a, b
来源：http://ux.lnxyls.cn

C#:   return (a, b);              // ValueTuple
来源：http://lt.newstarts.cn

[C06] 匿名函数 / lambda
来源：http://jq.asd995.cn

Py:   square = lambda x: x * x
来源：http://xl.jctech888.com.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pf.panjiajie.cn

JS:   const square = x => x * x;
来源：http://bb.asd995.cn

TS:   const square = (x: number): number => x * x;
来源：http://bp.szxytkj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ph.asd995.cn

Go:   sq := func(x int) int { return x * x }
来源：http://uz.521024.cn

Ruby: square = ->(x) { x * x }
来源：http://pk.bjjhwx.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ul.yuntaijiaju.cn

[C07] 把函数作为参数传入
来源：http://fg.shxzukj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jg.huixinmuqiang.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ns.lnxyls.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ji.shxzskj.cn

TS:   arr.map(String)
来源：http://an.huixiangedu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lu.gzmigu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ue.jianghongdianzi.cn

Ruby: arr.map(&:upcase)
来源：http://uf.9csxet.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jf.chemitech.net.cn

[C08] 闭包
来源：http://tj.9csxet.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dm.nszjky.cn


<!-- 参考信息 -->