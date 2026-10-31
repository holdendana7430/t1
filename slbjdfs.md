代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ig.nszjky.cn

Java: (int) 'A'; (char) 65
来源：http://tp.hahajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ic.9csxet.cn

Ruby: "A".ord; 65.chr
来源：http://mr.jianghongdianzi.cn

C#:   (int)'A'; (char)65
来源：http://cl.hnjuh.cn

[A19] 交换两个变量
来源：http://qr.asd995.cn

Py:   a, b = b, a
来源：http://nr.hahajie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ky.gzmigu.cn

JS:   [a, b] = [b, a];
来源：http://ul.huixinmuqiang.cn

TS:   [a, b] = [b, a];
来源：http://vg.yuexingan06.cn

Java: int t = a; a = b; b = t;
来源：http://eq.hahajie.cn

Go:   a, b = b, a
来源：http://df.huixiangedu.cn

Ruby: a, b = b, a
来源：http://ro.wgjwhj.cn

C#:   (a, b) = (b, a);
来源：http://ya.nicolike.cn

[A20] 读取标准输入
来源：http://fq.jctech888.com.cn

Py:   name = input("请输入：")
来源：http://xa.szsharing.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://kg.yuexingan06.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hs.521024.cn

TS:   // Node.js：readline 模块
来源：http://wy.bjjhwx.cn

Java: new Scanner(System.in).nextLine()
来源：http://oa.shxzskj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ei.panjiajie.cn

Ruby: gets.chomp
来源：http://ac.bookmarksfly.cn

C#:   Console.ReadLine();
来源：http://ss.yuntaijiaju.cn

[A21] 保留指定小数位输出
来源：http://xf.huixiangedu.cn

Py:   f"{3.14159:.2f}"
来源：http://zx.haigaiapp.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://za.huixiangedu.cn

JS:   (3.14159).toFixed(2)
来源：http://uf.9csxet.cn

TS:   (3.14159).toFixed(2)
来源：http://od.shtwfgs.cn

Java: String.format("%.2f", 3.14159)
来源：http://bi.newstarts.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nq.huixinmuqiang.cn

Ruby: format("%.2f", 3.14159)
来源：http://ab.bjjhwx.cn

C#:   3.14159.ToString("F2")
来源：http://of.colortex.cn

[A22] 获取字符串长度
来源：http://ii.jianghongdianzi.cn

Py:   len(s)
来源：http://bs.nszjky.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ea.hahajie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ju.asd995.cn

TS:   s.length
来源：http://di.colortex.cn

Java: s.length()
来源：http://ng.szsharing.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gk.bookmarksfly.cn

Ruby: s.length
来源：http://al.wgjwhj.cn

C#:   s.Length
来源：http://bp.yuntaijiaju.cn

[A23] 大小写转换
来源：http://mn.hnjuh.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://cz.asd995.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ck.bookmarksfly.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mv.wgjwhj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://we.9csxet.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ba.shxzskj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gg.bookmarksfly.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ax.haigaiapp.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://yv.nszjky.cn

[A24] 去除首尾空白
来源：http://fh.szxytkj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://df.bjjhwx.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://im.asd995.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oh.huixiangedu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yx.bookmarksfly.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cv.hahajie.cn

Go:   strings.TrimSpace(s)
来源：http://bl.huanxung.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mx.yuntaijiaju.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ik.panjiajie.cn

[A25] 字符串比较
来源：http://iu.shtwfgs.cn

Py:   s1 == s2; s1 != s2
来源：http://kr.szsharing.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sm.lnxyls.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fy.hnjuh.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zb.yuntaijiaju.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bz.muxihuayi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xp.shtwfgs.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://gq.jctech888.com.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wk.shxzukj.cn

[A26] 类型转换总览
来源：http://mk.asd995.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vl.jianghongdianzi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uy.hahajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://iw.chemitech.net.cn

TS:   Number() String() Boolean() x as number
来源：http://xr.huixinmuqiang.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nm.yuexingan06.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rs.szxytkj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://uv.muxihuayi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qm.jctech888.com.cn

================================================================================
来源：http://au.huixinmuqiang.cn

B. 流程控制
来源：http://av.nszjky.cn

================================================================================
来源：http://rb.asd995.cn

[B01] 条件判断 if / else
来源：http://rf.colortex.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://fa.bookmarksfly.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hf.nicolike.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mf.bjjhwx.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rf.huixinmuqiang.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://lg.521024.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bk.huixiangedu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kc.bookmarksfly.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://uj.shxzukj.cn

[B02] 多分支 else if / elif
来源：http://bv.asd995.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nz.hnjuh.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gq.huixinmuqiang.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wn.shtwfgs.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zm.asd995.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vc.jctech888.com.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://te.chemitech.net.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zp.gzmigu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kd.wgjwhj.cn

[B03] switch / match / case
来源：http://tu.yuexingan06.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qt.haigaiapp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cr.hahajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vl.szxytkj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uf.yuntaijiaju.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://is.nicolike.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uz.panjiajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lh.shxzukj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ux.jctech888.com.cn

[B04] for 计数循环
来源：http://mv.521024.cn

Py:   for i in range(10): print(i)
来源：http://hv.colortex.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mo.szxytkj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vj.newstarts.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ad.bookmarksfly.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jm.wgjwhj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fp.gzmigu.cn

Ruby: 10.times { |i| puts i }
来源：http://ce.shxzukj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jq.haigaiapp.cn

[B05] 遍历数组 / 列表
来源：http://cu.chemitech.net.cn

Py:   for item in arr: print(item)
来源：http://zi.muxihuayi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://uw.521024.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ks.jctech888.com.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tu.bookmarksfly.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ff.lnxyls.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://by.hahajie.cn

Ruby: arr.each { |item| puts item }
来源：http://zb.chemitech.net.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xr.haigaiapp.cn

[B06] 遍历字典 / 对象
来源：http://ah.chemitech.net.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://us.lnxyls.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dc.jianghongdianzi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://od.huixinmuqiang.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ij.jctech888.com.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hc.haigaiapp.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jl.szxytkj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sm.szxytkj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://id.wgjwhj.cn

[B07] while 循环
来源：http://gr.huixiangedu.cn

Py:   while i < 10: i += 1
来源：http://ct.lnxyls.cn

PHP:  while ($i < 10) { $i++; }
来源：http://rc.wgjwhj.cn

JS:   while (i < 10) { i++; }
来源：http://dm.521024.cn

TS:   while (i < 10) { i++; }
来源：http://cn.panjiajie.cn

Java: while (i < 10) { i++; }
来源：http://za.lnxyls.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dc.hahajie.cn

Ruby: while i < 10; i += 1; end
来源：http://jk.shtwfgs.cn

C#:   while (i < 10) { i++; }
来源：http://dz.hnjuh.cn

[B08] do-while（至少执行一次）
来源：http://fo.hahajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://gy.yuexingan06.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://av.bjjhwx.cn

JS:   do { i++; } while (i < 10);
来源：http://xc.szxytkj.cn

TS:   do { i++; } while (i < 10);
来源：http://sm.colortex.cn

Java: do { i++; } while (i < 10);
来源：http://fo.yuntaijiaju.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fr.hahajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pq.szxytkj.cn

C#:   do { i++; } while (i < 10);
来源：http://bt.huixiangedu.cn

[B09] break 与 continue
来源：http://zl.shtwfgs.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ic.huixiangedu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dw.yuntaijiaju.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sb.521024.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ud.wgjwhj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fm.huanxung.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://aq.nicolike.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://oc.shtwfgs.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ug.newstarts.cn

[B10] 遍历同时拿索引
来源：http://hw.jctech888.com.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mh.bookmarksfly.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xl.szxytkj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qx.colortex.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pv.bjjhwx.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://us.hahajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dj.szxytkj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tv.asd995.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ke.lnxyls.cn

[B11] 生成数字序列 / 区间
来源：http://lc.nszjky.cn

Py:   list(range(0, 10, 2))
来源：http://ys.chemitech.net.cn

PHP:  range(0, 10, 2);
来源：http://pf.szxytkj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sf.shtwfgs.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ox.panjiajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sm.haigaiapp.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mr.panjiajie.cn

Ruby: (0...10).step(2).to_a
来源：http://pj.lnxyls.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ab.szxytkj.cn

[B12] 跳出多层循环
来源：http://wt.bjjhwx.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ja.shxzukj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://da.jctech888.com.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hm.hnjuh.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://iy.shtwfgs.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qu.gzmigu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zx.shtwfgs.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dj.shxzskj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fc.hahajie.cn

[B13] 判断是否为数字
来源：http://ej.huixinmuqiang.cn

Py:   isinstance(x, (int, float))
来源：http://tk.yuexingan06.cn

PHP:  is_numeric($x)
来源：http://zl.shxzukj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ka.yuexingan06.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rh.newstarts.cn

Java: x instanceof Number
来源：http://yw.chemitech.net.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ja.yuntaijiaju.cn

Ruby: x.is_a?(Numeric)
来源：http://uu.bjjhwx.cn

C#:   x is int or double or decimal
来源：http://nj.wgjwhj.cn

[B14] 判断值是否在集合内
来源：http://pw.shtwfgs.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yd.nicolike.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://om.nicolike.cn

JS:   [1, 2, 3].includes(x)
来源：http://tc.szsharing.cn

TS:   [1, 2, 3].includes(x)
来源：http://jh.panjiajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ce.shxzskj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xc.9csxet.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xz.szxytkj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fl.shxzskj.cn

[B15] 布尔运算与取反
来源：http://zp.jctech888.com.cn

Py:   a and b or not c
来源：http://ie.yuexingan06.cn

PHP:  $a && $b || !$c
来源：http://vn.huixinmuqiang.cn

JS:   a && b || !c
来源：http://ht.lnxyls.cn

TS:   a && b || !c
来源：http://fh.huixiangedu.cn

Java: a && b || !c
来源：http://vr.huixiangedu.cn

Go:   a && b || !c
来源：http://jd.wgjwhj.cn

Ruby: a && b || !c
来源：http://cb.shtwfgs.cn

C#:   a && b || !c
来源：http://li.huixinmuqiang.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lv.muxihuayi.cn

Py:   if not data: return
来源：http://mc.shxzukj.cn

PHP:  if (!$data) { return; }
来源：http://ph.szsharing.cn

JS:   if (!data) return;
来源：http://zk.colortex.cn

TS:   if (!data) return;
来源：http://iu.gzmigu.cn

Java: if (data == null) return;
来源：http://xc.shxzukj.cn

Go:   if data == nil { return }
来源：http://og.newstarts.cn

Ruby: return if data.nil?
来源：http://za.bjjhwx.cn

C#:   if (data == null) return;
来源：http://ox.muxihuayi.cn

================================================================================
来源：http://ft.lnxyls.cn

C. 函数与作用域
来源：http://jo.nszjky.cn

================================================================================
来源：http://jj.yuntaijiaju.cn

[C01] 定义函数
来源：http://px.yuntaijiaju.cn

Py:   def add(a, b): return a + b
来源：http://gn.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tm.gzmigu.cn

JS:   function add(a, b) { return a + b; }
来源：http://vc.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://my.szxytkj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://uq.asd995.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ce.yuexingan06.cn

Ruby: def add(a, b); a + b; end
来源：http://dm.521024.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kp.jctech888.com.cn

[C02] 默认参数
来源：http://sy.lnxyls.cn

Py:   def greet(name="World"): return name
来源：http://dm.hahajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://sy.panjiajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://rt.hnjuh.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bz.huixiangedu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ye.jianghongdianzi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lv.yuexingan06.cn

Ruby: def greet(name = "World") = name
来源：http://sw.521024.cn

C#:   string Greet(string name = "World") => name;
来源：http://lw.shxzskj.cn

[C03] 可变参数
来源：http://lx.colortex.cn

Py:   def total(*args): return sum(args)
来源：http://ry.colortex.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xi.shxzukj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bz.chemitech.net.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gr.szxytkj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gb.asd995.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cy.asd995.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yj.hnjuh.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pi.wgjwhj.cn

[C04] 命名参数 / 关键字参数
来源：http://zq.9csxet.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ez.chemitech.net.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fj.huixinmuqiang.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zc.gzmigu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ml.szsharing.cn

Java: // 无：用 Builder 模式或 record
来源：http://rv.wgjwhj.cn

Go:   // 无：用配置结构体参数
来源：http://rj.nicolike.cn

Ruby: f(a: 1, b: 2)
来源：http://kr.huixinmuqiang.cn

C#:   f(a: 1, b: 2)
来源：http://df.chemitech.net.cn

[C05] 返回多个值
来源：http://pc.521024.cn

Py:   return a, b
来源：http://sy.521024.cn

PHP:  return [$a, $b];
来源：http://pu.panjiajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://tf.huixiangedu.cn

TS:   return { a, b };
来源：http://ig.jctech888.com.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zf.hahajie.cn

Go:   return a, b
来源：http://rl.shxzskj.cn

Ruby: return a, b
来源：http://rr.wgjwhj.cn

C#:   return (a, b);              // ValueTuple
来源：http://ah.9csxet.cn

[C06] 匿名函数 / lambda
来源：http://uy.nszjky.cn

Py:   square = lambda x: x * x
来源：http://de.bjjhwx.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ah.bookmarksfly.cn

JS:   const square = x => x * x;
来源：http://lb.colortex.cn

TS:   const square = (x: number): number => x * x;
来源：http://yo.jctech888.com.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wn.jctech888.com.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gx.chemitech.net.cn

Ruby: square = ->(x) { x * x }
来源：http://nf.huixinmuqiang.cn

C#:   Func<int, int> square = x => x * x;
来源：http://os.jianghongdianzi.cn

[C07] 把函数作为参数传入
来源：http://zd.hnjuh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qk.newstarts.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ij.9csxet.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jf.521024.cn

TS:   arr.map(String)
来源：http://jb.szsharing.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hf.hnjuh.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qz.szxytkj.cn

Ruby: arr.map(&:upcase)
来源：http://vb.shtwfgs.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://to.huixinmuqiang.cn

[C08] 闭包
来源：http://zi.huanxung.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ux.gzmigu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jz.hahajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wy.hnjuh.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tv.gzmigu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pw.huixinmuqiang.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nz.szxytkj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pp.szxytkj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://aw.shxzukj.cn

[C09] 递归
来源：http://uo.bookmarksfly.cn


<!-- 参考信息 -->