代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://os.hnjuh.cn

Java: (int) 'A'; (char) 65
来源：http://xp.wgjwhj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hw.yuntaijiaju.cn

Ruby: "A".ord; 65.chr
来源：http://px.nicolike.cn

C#:   (int)'A'; (char)65
来源：http://qs.bookmarksfly.cn

[A19] 交换两个变量
来源：http://od.lnxyls.cn

Py:   a, b = b, a
来源：http://xd.jctech888.com.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://tg.muxihuayi.cn

JS:   [a, b] = [b, a];
来源：http://lz.muxihuayi.cn

TS:   [a, b] = [b, a];
来源：http://lc.jctech888.com.cn

Java: int t = a; a = b; b = t;
来源：http://ps.nszjky.cn

Go:   a, b = b, a
来源：http://gf.nicolike.cn

Ruby: a, b = b, a
来源：http://dd.yuntaijiaju.cn

C#:   (a, b) = (b, a);
来源：http://fs.hnjuh.cn

[A20] 读取标准输入
来源：http://wu.shxzukj.cn

Py:   name = input("请输入：")
来源：http://wj.hnjuh.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://iu.wgjwhj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wq.bookmarksfly.cn

TS:   // Node.js：readline 模块
来源：http://sc.asd995.cn

Java: new Scanner(System.in).nextLine()
来源：http://hy.bjjhwx.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jn.bookmarksfly.cn

Ruby: gets.chomp
来源：http://ss.bjjhwx.cn

C#:   Console.ReadLine();
来源：http://fw.hnjuh.cn

[A21] 保留指定小数位输出
来源：http://mi.bjjhwx.cn

Py:   f"{3.14159:.2f}"
来源：http://xu.hnjuh.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xr.huixiangedu.cn

JS:   (3.14159).toFixed(2)
来源：http://om.shtwfgs.cn

TS:   (3.14159).toFixed(2)
来源：http://yr.panjiajie.cn

Java: String.format("%.2f", 3.14159)
来源：http://dk.chemitech.net.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://df.szxytkj.cn

Ruby: format("%.2f", 3.14159)
来源：http://zd.haigaiapp.cn

C#:   3.14159.ToString("F2")
来源：http://he.huanxung.cn

[A22] 获取字符串长度
来源：http://cd.wgjwhj.cn

Py:   len(s)
来源：http://po.nicolike.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dy.wgjwhj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://uo.nszjky.cn

TS:   s.length
来源：http://ej.asd995.cn

Java: s.length()
来源：http://sw.chemitech.net.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ot.szxytkj.cn

Ruby: s.length
来源：http://hc.shxzukj.cn

C#:   s.Length
来源：http://kn.521024.cn

[A23] 大小写转换
来源：http://pi.hnjuh.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://rw.colortex.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gd.bjjhwx.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hf.asd995.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zb.wgjwhj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pv.asd995.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yk.shxzskj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://po.huixiangedu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ce.szsharing.cn

[A24] 去除首尾空白
来源：http://ka.shxzukj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xe.asd995.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://oj.yuntaijiaju.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jx.chemitech.net.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fc.panjiajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ug.szsharing.cn

Go:   strings.TrimSpace(s)
来源：http://ir.9csxet.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ai.nszjky.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://my.9csxet.cn

[A25] 字符串比较
来源：http://ks.huixiangedu.cn

Py:   s1 == s2; s1 != s2
来源：http://pj.chemitech.net.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hl.hnjuh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://om.haigaiapp.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fm.bjjhwx.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ve.bjjhwx.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wy.yuexingan06.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rq.nszjky.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tt.szxytkj.cn

[A26] 类型转换总览
来源：http://fr.jianghongdianzi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fa.521024.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gq.huanxung.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://in.chemitech.net.cn

TS:   Number() String() Boolean() x as number
来源：http://my.jctech888.com.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dx.haigaiapp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dz.haigaiapp.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://fk.jctech888.com.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://to.shxzukj.cn

================================================================================
来源：http://rk.521024.cn

B. 流程控制
来源：http://rf.nszjky.cn

================================================================================
来源：http://hs.huixiangedu.cn

[B01] 条件判断 if / else
来源：http://fb.newstarts.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ih.szsharing.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zq.yuntaijiaju.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mh.nszjky.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://iw.newstarts.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://sm.nicolike.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vn.gzmigu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wn.chemitech.net.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qh.wgjwhj.cn

[B02] 多分支 else if / elif
来源：http://ux.szxytkj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xw.yuntaijiaju.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gs.szsharing.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://po.huixiangedu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zv.jctech888.com.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://op.nicolike.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fi.hahajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ru.huixinmuqiang.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qq.jianghongdianzi.cn

[B03] switch / match / case
来源：http://hm.asd995.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ej.jctech888.com.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hg.hahajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cd.9csxet.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ra.szxytkj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://js.jctech888.com.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fn.huixiangedu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://de.haigaiapp.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hv.muxihuayi.cn

[B04] for 计数循环
来源：http://ja.521024.cn

Py:   for i in range(10): print(i)
来源：http://to.gzmigu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wj.nicolike.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sd.521024.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://os.521024.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pt.muxihuayi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ar.asd995.cn

Ruby: 10.times { |i| puts i }
来源：http://lp.huanxung.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bu.asd995.cn

[B05] 遍历数组 / 列表
来源：http://se.chemitech.net.cn

Py:   for item in arr: print(item)
来源：http://fa.muxihuayi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vs.haigaiapp.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://js.shxzukj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ni.9csxet.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yr.bookmarksfly.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ut.colortex.cn

Ruby: arr.each { |item| puts item }
来源：http://vu.shxzukj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hd.9csxet.cn

[B06] 遍历字典 / 对象
来源：http://py.gzmigu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ou.jctech888.com.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xv.yuntaijiaju.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ok.jianghongdianzi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://va.haigaiapp.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://is.huanxung.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yk.hahajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nr.chemitech.net.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qz.bookmarksfly.cn

[B07] while 循环
来源：http://rd.jctech888.com.cn

Py:   while i < 10: i += 1
来源：http://md.panjiajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fr.jctech888.com.cn

JS:   while (i < 10) { i++; }
来源：http://ga.wgjwhj.cn

TS:   while (i < 10) { i++; }
来源：http://hj.asd995.cn

Java: while (i < 10) { i++; }
来源：http://ro.nszjky.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hk.nszjky.cn

Ruby: while i < 10; i += 1; end
来源：http://yh.gzmigu.cn

C#:   while (i < 10) { i++; }
来源：http://wn.szsharing.cn

[B08] do-while（至少执行一次）
来源：http://sl.bookmarksfly.cn

Py:   # 无 do-while：用 while True + break
来源：http://tr.wgjwhj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vh.haigaiapp.cn

JS:   do { i++; } while (i < 10);
来源：http://je.hahajie.cn

TS:   do { i++; } while (i < 10);
来源：http://yw.yuntaijiaju.cn

Java: do { i++; } while (i < 10);
来源：http://nt.521024.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://as.shxzukj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://dx.yuntaijiaju.cn

C#:   do { i++; } while (i < 10);
来源：http://ni.wgjwhj.cn

[B09] break 与 continue
来源：http://xw.shxzukj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fk.yuntaijiaju.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gy.huixiangedu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ob.chemitech.net.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bc.hahajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ip.shxzukj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qd.shxzukj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sk.chemitech.net.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pt.chemitech.net.cn

[B10] 遍历同时拿索引
来源：http://hq.panjiajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://oi.haigaiapp.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://op.yuexingan06.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://id.521024.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wm.nicolike.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://oz.chemitech.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ry.jianghongdianzi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://oe.nszjky.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fc.nicolike.cn

[B11] 生成数字序列 / 区间
来源：http://vg.lnxyls.cn

Py:   list(range(0, 10, 2))
来源：http://sa.szxytkj.cn

PHP:  range(0, 10, 2);
来源：http://yn.asd995.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xt.asd995.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ip.huixinmuqiang.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ly.yuntaijiaju.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ve.shtwfgs.cn

Ruby: (0...10).step(2).to_a
来源：http://bc.shtwfgs.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fb.huixinmuqiang.cn

[B12] 跳出多层循环
来源：http://nj.newstarts.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://el.yuexingan06.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://rg.bookmarksfly.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cf.muxihuayi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qm.9csxet.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vc.bookmarksfly.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bz.nicolike.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tr.yuntaijiaju.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://iy.yuexingan06.cn

[B13] 判断是否为数字
来源：http://zb.hahajie.cn

Py:   isinstance(x, (int, float))
来源：http://kv.yuntaijiaju.cn

PHP:  is_numeric($x)
来源：http://dw.shtwfgs.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bu.9csxet.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fo.huanxung.cn

Java: x instanceof Number
来源：http://fc.shxzukj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://oc.jianghongdianzi.cn

Ruby: x.is_a?(Numeric)
来源：http://eb.gzmigu.cn

C#:   x is int or double or decimal
来源：http://qg.shxzskj.cn

[B14] 判断值是否在集合内
来源：http://vw.newstarts.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wq.asd995.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nx.huixiangedu.cn

JS:   [1, 2, 3].includes(x)
来源：http://mm.huanxung.cn

TS:   [1, 2, 3].includes(x)
来源：http://zy.colortex.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dr.jctech888.com.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jx.wgjwhj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fc.szsharing.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zv.bookmarksfly.cn

[B15] 布尔运算与取反
来源：http://tr.muxihuayi.cn

Py:   a and b or not c
来源：http://cx.szxytkj.cn

PHP:  $a && $b || !$c
来源：http://ix.wgjwhj.cn

JS:   a && b || !c
来源：http://sj.shxzskj.cn

TS:   a && b || !c
来源：http://sf.521024.cn

Java: a && b || !c
来源：http://mh.521024.cn

Go:   a && b || !c
来源：http://xm.yuntaijiaju.cn

Ruby: a && b || !c
来源：http://yq.asd995.cn

C#:   a && b || !c
来源：http://zi.huixiangedu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://mk.gzmigu.cn

Py:   if not data: return
来源：http://wj.yuntaijiaju.cn

PHP:  if (!$data) { return; }
来源：http://uz.9csxet.cn

JS:   if (!data) return;
来源：http://vc.bjjhwx.cn

TS:   if (!data) return;
来源：http://ny.szxytkj.cn

Java: if (data == null) return;
来源：http://xh.yuexingan06.cn

Go:   if data == nil { return }
来源：http://va.huixiangedu.cn

Ruby: return if data.nil?
来源：http://ie.szxytkj.cn

C#:   if (data == null) return;
来源：http://ik.huanxung.cn

================================================================================
来源：http://ax.shtwfgs.cn

C. 函数与作用域
来源：http://ya.bookmarksfly.cn

================================================================================
来源：http://ba.wgjwhj.cn

[C01] 定义函数
来源：http://pp.hahajie.cn

Py:   def add(a, b): return a + b
来源：http://do.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fi.colortex.cn

JS:   function add(a, b) { return a + b; }
来源：http://xx.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tn.gzmigu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lc.panjiajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://uy.shxzukj.cn

Ruby: def add(a, b); a + b; end
来源：http://vg.hahajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://il.yuntaijiaju.cn

[C02] 默认参数
来源：http://ip.shxzukj.cn

Py:   def greet(name="World"): return name
来源：http://iw.lnxyls.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ht.jianghongdianzi.cn

JS:   function greet(name = "World") { return name; }
来源：http://hf.muxihuayi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://av.szxytkj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://gq.huixiangedu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lq.bjjhwx.cn

Ruby: def greet(name = "World") = name
来源：http://ht.shxzukj.cn

C#:   string Greet(string name = "World") => name;
来源：http://mt.shtwfgs.cn

[C03] 可变参数
来源：http://yo.colortex.cn

Py:   def total(*args): return sum(args)
来源：http://bq.shxzskj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://aa.bjjhwx.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gb.chemitech.net.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ni.colortex.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bq.521024.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ss.muxihuayi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hh.bookmarksfly.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://is.yuntaijiaju.cn

[C04] 命名参数 / 关键字参数
来源：http://xj.yuexingan06.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nl.jianghongdianzi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kt.muxihuayi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mc.hnjuh.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hr.huixiangedu.cn

Java: // 无：用 Builder 模式或 record
来源：http://ap.shxzukj.cn

Go:   // 无：用配置结构体参数
来源：http://ji.yuntaijiaju.cn

Ruby: f(a: 1, b: 2)
来源：http://ov.yuexingan06.cn

C#:   f(a: 1, b: 2)
来源：http://bu.chemitech.net.cn

[C05] 返回多个值
来源：http://bd.jctech888.com.cn

Py:   return a, b
来源：http://jq.9csxet.cn

PHP:  return [$a, $b];
来源：http://kw.9csxet.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dy.shxzskj.cn

TS:   return { a, b };
来源：http://ic.huixiangedu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cq.huixiangedu.cn

Go:   return a, b
来源：http://yb.huixiangedu.cn

Ruby: return a, b
来源：http://ki.newstarts.cn

C#:   return (a, b);              // ValueTuple
来源：http://hi.huixinmuqiang.cn

[C06] 匿名函数 / lambda
来源：http://gj.colortex.cn

Py:   square = lambda x: x * x
来源：http://aj.huixinmuqiang.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://lk.jctech888.com.cn

JS:   const square = x => x * x;
来源：http://ca.hahajie.cn

TS:   const square = (x: number): number => x * x;
来源：http://ng.yuntaijiaju.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ry.nszjky.cn

Go:   sq := func(x int) int { return x * x }
来源：http://tj.panjiajie.cn

Ruby: square = ->(x) { x * x }
来源：http://fj.jctech888.com.cn

C#:   Func<int, int> square = x => x * x;
来源：http://iw.huanxung.cn

[C07] 把函数作为参数传入
来源：http://co.chemitech.net.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://do.jctech888.com.cn

PHP:  array_map("strtoupper", $arr);
来源：http://al.panjiajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qa.chemitech.net.cn

TS:   arr.map(String)
来源：http://as.haigaiapp.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mx.nicolike.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nk.newstarts.cn

Ruby: arr.map(&:upcase)
来源：http://wb.szsharing.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gs.jctech888.com.cn

[C08] 闭包
来源：http://cq.szxytkj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dt.colortex.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fb.shxzukj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://we.bookmarksfly.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nf.gzmigu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tb.wgjwhj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ma.huixinmuqiang.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mb.shxzskj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://aq.lnxyls.cn

[C09] 递归
来源：http://uq.chemitech.net.cn


<!-- 参考信息 -->