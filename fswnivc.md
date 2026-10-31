代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cl.newstarts.cn

Java: (int) 'A'; (char) 65
来源：http://hz.gzmigu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://td.521024.cn

Ruby: "A".ord; 65.chr
来源：http://zl.haigaiapp.cn

C#:   (int)'A'; (char)65
来源：http://xy.hnjuh.cn

[A19] 交换两个变量
来源：http://yf.huixinmuqiang.cn

Py:   a, b = b, a
来源：http://zh.chemitech.net.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ye.bjjhwx.cn

JS:   [a, b] = [b, a];
来源：http://wx.yuexingan06.cn

TS:   [a, b] = [b, a];
来源：http://ji.yuexingan06.cn

Java: int t = a; a = b; b = t;
来源：http://wh.asd995.cn

Go:   a, b = b, a
来源：http://jl.yuntaijiaju.cn

Ruby: a, b = b, a
来源：http://rr.yuexingan06.cn

C#:   (a, b) = (b, a);
来源：http://on.asd995.cn

[A20] 读取标准输入
来源：http://zh.9csxet.cn

Py:   name = input("请输入：")
来源：http://fv.szsharing.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://vt.9csxet.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vf.nszjky.cn

TS:   // Node.js：readline 模块
来源：http://zf.huanxung.cn

Java: new Scanner(System.in).nextLine()
来源：http://kl.hahajie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ob.shtwfgs.cn

Ruby: gets.chomp
来源：http://xm.colortex.cn

C#:   Console.ReadLine();
来源：http://ra.521024.cn

[A21] 保留指定小数位输出
来源：http://vb.newstarts.cn

Py:   f"{3.14159:.2f}"
来源：http://ce.szsharing.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qx.nszjky.cn

JS:   (3.14159).toFixed(2)
来源：http://ru.jianghongdianzi.cn

TS:   (3.14159).toFixed(2)
来源：http://kw.muxihuayi.cn

Java: String.format("%.2f", 3.14159)
来源：http://js.jianghongdianzi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.nicolike.cn

Ruby: format("%.2f", 3.14159)
来源：http://vf.huixiangedu.cn

C#:   3.14159.ToString("F2")
来源：http://vt.wgjwhj.cn

[A22] 获取字符串长度
来源：http://nl.shtwfgs.cn

Py:   len(s)
来源：http://by.jianghongdianzi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cc.nszjky.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ld.asd995.cn

TS:   s.length
来源：http://hp.shtwfgs.cn

Java: s.length()
来源：http://ay.521024.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kc.bjjhwx.cn

Ruby: s.length
来源：http://ex.shtwfgs.cn

C#:   s.Length
来源：http://tt.jctech888.com.cn

[A23] 大小写转换
来源：http://ao.nszjky.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://xe.panjiajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gj.bookmarksfly.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://po.yuexingan06.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yg.yuntaijiaju.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ut.521024.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pm.jianghongdianzi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zp.newstarts.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://rq.huixinmuqiang.cn

[A24] 去除首尾空白
来源：http://zg.hahajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://az.bjjhwx.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dz.yuexingan06.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.newstarts.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bc.nszjky.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dd.huanxung.cn

Go:   strings.TrimSpace(s)
来源：http://tj.wgjwhj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vl.wgjwhj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ws.yuntaijiaju.cn

[A25] 字符串比较
来源：http://ck.hahajie.cn

Py:   s1 == s2; s1 != s2
来源：http://xu.shxzskj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://yz.521024.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vt.chemitech.net.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hg.haigaiapp.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://sd.chemitech.net.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mt.panjiajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://bz.yuntaijiaju.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qt.yuntaijiaju.cn

[A26] 类型转换总览
来源：http://tk.jctech888.com.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yo.huixinmuqiang.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vx.huixiangedu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ui.szxytkj.cn

TS:   Number() String() Boolean() x as number
来源：http://wb.muxihuayi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kz.lnxyls.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xd.yuntaijiaju.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lv.panjiajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ig.nicolike.cn

================================================================================
来源：http://nq.szsharing.cn

B. 流程控制
来源：http://wt.bjjhwx.cn

================================================================================
来源：http://jf.muxihuayi.cn

[B01] 条件判断 if / else
来源：http://ja.bookmarksfly.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://di.colortex.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bq.szsharing.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fp.yuexingan06.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pb.shxzskj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://it.lnxyls.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xo.szsharing.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vl.huixiangedu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://uy.szxytkj.cn

[B02] 多分支 else if / elif
来源：http://cl.yuntaijiaju.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sp.muxihuayi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mm.shxzskj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jm.szsharing.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dm.haigaiapp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jx.colortex.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fx.yuntaijiaju.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dz.shxzskj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://he.hahajie.cn

[B03] switch / match / case
来源：http://kt.muxihuayi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ni.shtwfgs.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tb.lnxyls.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bu.huixinmuqiang.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ta.shxzskj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sd.colortex.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hl.shtwfgs.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vi.nicolike.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fl.szsharing.cn

[B04] for 计数循环
来源：http://kb.huixinmuqiang.cn

Py:   for i in range(10): print(i)
来源：http://pj.szxytkj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zm.haigaiapp.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ip.haigaiapp.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sr.jianghongdianzi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://sz.newstarts.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://la.jctech888.com.cn

Ruby: 10.times { |i| puts i }
来源：http://bf.muxihuayi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ij.bookmarksfly.cn

[B05] 遍历数组 / 列表
来源：http://jf.nszjky.cn

Py:   for item in arr: print(item)
来源：http://qp.panjiajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ie.huixinmuqiang.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qs.shtwfgs.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gs.colortex.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://rb.huanxung.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hv.colortex.cn

Ruby: arr.each { |item| puts item }
来源：http://xq.huixinmuqiang.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fn.panjiajie.cn

[B06] 遍历字典 / 对象
来源：http://oq.hahajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vb.hnjuh.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://aj.huixinmuqiang.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sr.hnjuh.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xc.yuexingan06.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://oz.shtwfgs.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wo.bjjhwx.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dt.9csxet.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://at.wgjwhj.cn

[B07] while 循环
来源：http://mw.hnjuh.cn

Py:   while i < 10: i += 1
来源：http://mk.muxihuayi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://of.hahajie.cn

JS:   while (i < 10) { i++; }
来源：http://vm.521024.cn

TS:   while (i < 10) { i++; }
来源：http://ly.muxihuayi.cn

Java: while (i < 10) { i++; }
来源：http://tv.colortex.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ze.yuexingan06.cn

Ruby: while i < 10; i += 1; end
来源：http://nx.shxzukj.cn

C#:   while (i < 10) { i++; }
来源：http://to.colortex.cn

[B08] do-while（至少执行一次）
来源：http://sg.shxzukj.cn

Py:   # 无 do-while：用 while True + break
来源：http://dv.huanxung.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://bq.yuexingan06.cn

JS:   do { i++; } while (i < 10);
来源：http://dh.hahajie.cn

TS:   do { i++; } while (i < 10);
来源：http://if.szsharing.cn

Java: do { i++; } while (i < 10);
来源：http://rs.9csxet.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://kv.newstarts.cn

Ruby: begin; i += 1; end while i < 10
来源：http://yn.jctech888.com.cn

C#:   do { i++; } while (i < 10);
来源：http://me.hnjuh.cn

[B09] break 与 continue
来源：http://zg.jianghongdianzi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pc.shxzukj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://eb.szsharing.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hy.nicolike.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hx.asd995.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pe.bjjhwx.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://na.szsharing.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ih.panjiajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ft.bookmarksfly.cn

[B10] 遍历同时拿索引
来源：http://hg.bjjhwx.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vu.chemitech.net.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zt.shtwfgs.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://up.huanxung.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://id.nicolike.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vr.huanxung.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sl.colortex.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gm.huixiangedu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tq.nszjky.cn

[B11] 生成数字序列 / 区间
来源：http://vg.521024.cn

Py:   list(range(0, 10, 2))
来源：http://ex.9csxet.cn

PHP:  range(0, 10, 2);
来源：http://ou.asd995.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iw.huanxung.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hr.haigaiapp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qo.szxytkj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://as.wgjwhj.cn

Ruby: (0...10).step(2).to_a
来源：http://dh.9csxet.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zi.wgjwhj.cn

[B12] 跳出多层循环
来源：http://ed.haigaiapp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yn.521024.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://um.yuexingan06.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xj.huixiangedu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tr.jianghongdianzi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sw.panjiajie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bi.chemitech.net.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vf.jctech888.com.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zw.jianghongdianzi.cn

[B13] 判断是否为数字
来源：http://ux.huixinmuqiang.cn

Py:   isinstance(x, (int, float))
来源：http://jk.newstarts.cn

PHP:  is_numeric($x)
来源：http://mb.huanxung.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ij.szsharing.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sj.chemitech.net.cn

Java: x instanceof Number
来源：http://iz.huanxung.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fc.asd995.cn

Ruby: x.is_a?(Numeric)
来源：http://wx.521024.cn

C#:   x is int or double or decimal
来源：http://la.shtwfgs.cn

[B14] 判断值是否在集合内
来源：http://ap.9csxet.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ai.yuexingan06.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nw.521024.cn

JS:   [1, 2, 3].includes(x)
来源：http://hl.shxzukj.cn

TS:   [1, 2, 3].includes(x)
来源：http://en.jctech888.com.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://um.szsharing.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mw.huixinmuqiang.cn

Ruby: [1, 2, 3].include?(x)
来源：http://js.colortex.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sd.9csxet.cn

[B15] 布尔运算与取反
来源：http://jb.shxzukj.cn

Py:   a and b or not c
来源：http://fg.huixinmuqiang.cn

PHP:  $a && $b || !$c
来源：http://ts.yuexingan06.cn

JS:   a && b || !c
来源：http://iy.huixinmuqiang.cn

TS:   a && b || !c
来源：http://uf.wgjwhj.cn

Java: a && b || !c
来源：http://wa.huixinmuqiang.cn

Go:   a && b || !c
来源：http://og.gzmigu.cn

Ruby: a && b || !c
来源：http://ew.chemitech.net.cn

C#:   a && b || !c
来源：http://ta.shxzskj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://he.szsharing.cn

Py:   if not data: return
来源：http://wv.huanxung.cn

PHP:  if (!$data) { return; }
来源：http://pl.panjiajie.cn

JS:   if (!data) return;
来源：http://jv.szsharing.cn

TS:   if (!data) return;
来源：http://fm.jctech888.com.cn

Java: if (data == null) return;
来源：http://vu.9csxet.cn

Go:   if data == nil { return }
来源：http://tw.jianghongdianzi.cn

Ruby: return if data.nil?
来源：http://wx.chemitech.net.cn

C#:   if (data == null) return;
来源：http://od.newstarts.cn

================================================================================
来源：http://pf.shxzukj.cn

C. 函数与作用域
来源：http://om.jianghongdianzi.cn

================================================================================
来源：http://vf.chemitech.net.cn

[C01] 定义函数
来源：http://lh.jctech888.com.cn

Py:   def add(a, b): return a + b
来源：http://ba.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ym.nicolike.cn

JS:   function add(a, b) { return a + b; }
来源：http://zx.yuexingan06.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zl.shxzskj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://jw.jianghongdianzi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://uo.9csxet.cn

Ruby: def add(a, b); a + b; end
来源：http://ou.nicolike.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gt.shxzukj.cn

[C02] 默认参数
来源：http://ms.haigaiapp.cn

Py:   def greet(name="World"): return name
来源：http://op.huixiangedu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ij.hnjuh.cn

JS:   function greet(name = "World") { return name; }
来源：http://lx.521024.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yj.szxytkj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wn.yuntaijiaju.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pa.wgjwhj.cn

Ruby: def greet(name = "World") = name
来源：http://qr.bookmarksfly.cn

C#:   string Greet(string name = "World") => name;
来源：http://xi.chemitech.net.cn

[C03] 可变参数
来源：http://mb.hnjuh.cn

Py:   def total(*args): return sum(args)
来源：http://ha.nszjky.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ug.hahajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fc.bjjhwx.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sz.jctech888.com.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lb.szsharing.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yr.colortex.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xe.jianghongdianzi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qu.521024.cn

[C04] 命名参数 / 关键字参数
来源：http://vj.lnxyls.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fh.hnjuh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://iu.gzmigu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rd.gzmigu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cu.shxzskj.cn

Java: // 无：用 Builder 模式或 record
来源：http://ga.jctech888.com.cn

Go:   // 无：用配置结构体参数
来源：http://fu.panjiajie.cn

Ruby: f(a: 1, b: 2)
来源：http://cl.muxihuayi.cn

C#:   f(a: 1, b: 2)
来源：http://cq.hnjuh.cn

[C05] 返回多个值
来源：http://ja.huanxung.cn

Py:   return a, b
来源：http://cd.gzmigu.cn

PHP:  return [$a, $b];
来源：http://cv.shtwfgs.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qc.asd995.cn

TS:   return { a, b };
来源：http://ip.szsharing.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ku.lnxyls.cn

Go:   return a, b
来源：http://nh.521024.cn

Ruby: return a, b
来源：http://pv.shxzukj.cn

C#:   return (a, b);              // ValueTuple
来源：http://be.jianghongdianzi.cn

[C06] 匿名函数 / lambda
来源：http://gl.haigaiapp.cn

Py:   square = lambda x: x * x
来源：http://te.bjjhwx.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qv.jctech888.com.cn

JS:   const square = x => x * x;
来源：http://fy.haigaiapp.cn

TS:   const square = (x: number): number => x * x;
来源：http://hj.gzmigu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zg.nicolike.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ur.lnxyls.cn

Ruby: square = ->(x) { x * x }
来源：http://tr.colortex.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hv.nszjky.cn

[C07] 把函数作为参数传入
来源：http://bz.muxihuayi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ya.gzmigu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jl.asd995.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wz.asd995.cn

TS:   arr.map(String)
来源：http://jj.hahajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://og.yuntaijiaju.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hc.szxytkj.cn

Ruby: arr.map(&:upcase)
来源：http://ue.huixiangedu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ny.hnjuh.cn

[C08] 闭包
来源：http://pt.jctech888.com.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://us.bookmarksfly.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lx.shtwfgs.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yl.shxzskj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dp.haigaiapp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fk.chemitech.net.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vz.bookmarksfly.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nk.9csxet.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fo.hnjuh.cn

[C09] 递归
来源：http://wt.shxzskj.cn


<!-- 参考信息 -->