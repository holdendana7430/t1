代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pq.haigaiapp.cn

Java: (int) 'A'; (char) 65
来源：http://sj.shtwfgs.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gd.huixinmuqiang.cn

Ruby: "A".ord; 65.chr
来源：http://iu.bjjhwx.cn

C#:   (int)'A'; (char)65
来源：http://cm.lnxyls.cn

[A19] 交换两个变量
来源：http://an.nszjky.cn

Py:   a, b = b, a
来源：http://cv.panjiajie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://vk.gzmigu.cn

JS:   [a, b] = [b, a];
来源：http://al.bjjhwx.cn

TS:   [a, b] = [b, a];
来源：http://se.szxytkj.cn

Java: int t = a; a = b; b = t;
来源：http://dr.huixinmuqiang.cn

Go:   a, b = b, a
来源：http://tb.bjjhwx.cn

Ruby: a, b = b, a
来源：http://jh.gzmigu.cn

C#:   (a, b) = (b, a);
来源：http://vs.colortex.cn

[A20] 读取标准输入
来源：http://so.shxzskj.cn

Py:   name = input("请输入：")
来源：http://zl.muxihuayi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ad.jianghongdianzi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ka.nicolike.cn

TS:   // Node.js：readline 模块
来源：http://wp.huixiangedu.cn

Java: new Scanner(System.in).nextLine()
来源：http://hc.shxzukj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lx.asd995.cn

Ruby: gets.chomp
来源：http://ta.newstarts.cn

C#:   Console.ReadLine();
来源：http://wf.panjiajie.cn

[A21] 保留指定小数位输出
来源：http://da.chemitech.net.cn

Py:   f"{3.14159:.2f}"
来源：http://ac.9csxet.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wx.szsharing.cn

JS:   (3.14159).toFixed(2)
来源：http://th.muxihuayi.cn

TS:   (3.14159).toFixed(2)
来源：http://wp.9csxet.cn

Java: String.format("%.2f", 3.14159)
来源：http://mx.lnxyls.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://iw.nicolike.cn

Ruby: format("%.2f", 3.14159)
来源：http://ic.huixiangedu.cn

C#:   3.14159.ToString("F2")
来源：http://jl.9csxet.cn

[A22] 获取字符串长度
来源：http://sl.lnxyls.cn

Py:   len(s)
来源：http://tk.bookmarksfly.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ak.szsharing.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ed.huanxung.cn

TS:   s.length
来源：http://pk.chemitech.net.cn

Java: s.length()
来源：http://cc.nszjky.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://of.9csxet.cn

Ruby: s.length
来源：http://jk.nicolike.cn

C#:   s.Length
来源：http://mq.shtwfgs.cn

[A23] 大小写转换
来源：http://qn.szsharing.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://bj.wgjwhj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ht.bookmarksfly.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zr.yuexingan06.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cg.shtwfgs.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lp.9csxet.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ha.lnxyls.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://od.haigaiapp.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://vt.9csxet.cn

[A24] 去除首尾空白
来源：http://um.nszjky.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ad.chemitech.net.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gw.newstarts.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fr.bjjhwx.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hr.shxzskj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qc.hahajie.cn

Go:   strings.TrimSpace(s)
来源：http://qn.newstarts.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lj.colortex.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sb.shtwfgs.cn

[A25] 字符串比较
来源：http://vi.muxihuayi.cn

Py:   s1 == s2; s1 != s2
来源：http://gi.asd995.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://db.panjiajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jz.huixinmuqiang.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ty.chemitech.net.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yv.szxytkj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cu.szsharing.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://pq.szxytkj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xc.shxzukj.cn

[A26] 类型转换总览
来源：http://kq.bjjhwx.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://nb.nszjky.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ks.yuexingan06.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dw.9csxet.cn

TS:   Number() String() Boolean() x as number
来源：http://vl.521024.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rc.9csxet.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ar.lnxyls.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://wt.bjjhwx.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vt.huanxung.cn

================================================================================
来源：http://hr.huixiangedu.cn

B. 流程控制
来源：http://gn.panjiajie.cn

================================================================================
来源：http://sj.muxihuayi.cn

[B01] 条件判断 if / else
来源：http://jc.newstarts.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://cy.haigaiapp.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zq.asd995.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rf.newstarts.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mi.shxzukj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bn.huixinmuqiang.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ff.shxzskj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fo.yuntaijiaju.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jk.nszjky.cn

[B02] 多分支 else if / elif
来源：http://fs.521024.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://or.muxihuayi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ye.bookmarksfly.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ht.szsharing.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ym.colortex.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://om.muxihuayi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://sa.9csxet.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://sn.shxzukj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qp.521024.cn

[B03] switch / match / case
来源：http://uz.newstarts.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rv.yuexingan06.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://is.nszjky.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ry.muxihuayi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zi.hnjuh.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://eb.gzmigu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nj.panjiajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lz.yuntaijiaju.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zu.szsharing.cn

[B04] for 计数循环
来源：http://st.huanxung.cn

Py:   for i in range(10): print(i)
来源：http://iv.hnjuh.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pq.panjiajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pr.jianghongdianzi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pt.shxzukj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://un.hnjuh.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ec.jianghongdianzi.cn

Ruby: 10.times { |i| puts i }
来源：http://rz.lnxyls.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://va.szxytkj.cn

[B05] 遍历数组 / 列表
来源：http://ev.huanxung.cn

Py:   for item in arr: print(item)
来源：http://op.colortex.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rc.521024.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ne.nicolike.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ej.hahajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jw.gzmigu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ii.shtwfgs.cn

Ruby: arr.each { |item| puts item }
来源：http://ga.nicolike.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://aa.9csxet.cn

[B06] 遍历字典 / 对象
来源：http://ei.szsharing.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fw.newstarts.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qz.newstarts.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cu.yuexingan06.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xa.szsharing.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cb.panjiajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fv.asd995.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kw.newstarts.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ne.shxzskj.cn

[B07] while 循环
来源：http://rs.hahajie.cn

Py:   while i < 10: i += 1
来源：http://es.bookmarksfly.cn

PHP:  while ($i < 10) { $i++; }
来源：http://la.hnjuh.cn

JS:   while (i < 10) { i++; }
来源：http://xg.haigaiapp.cn

TS:   while (i < 10) { i++; }
来源：http://xz.hahajie.cn

Java: while (i < 10) { i++; }
来源：http://tl.yuntaijiaju.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ku.huixinmuqiang.cn

Ruby: while i < 10; i += 1; end
来源：http://ha.9csxet.cn

C#:   while (i < 10) { i++; }
来源：http://ow.asd995.cn

[B08] do-while（至少执行一次）
来源：http://mh.lnxyls.cn

Py:   # 无 do-while：用 while True + break
来源：http://gt.huixiangedu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://us.bjjhwx.cn

JS:   do { i++; } while (i < 10);
来源：http://dl.haigaiapp.cn

TS:   do { i++; } while (i < 10);
来源：http://nb.jianghongdianzi.cn

Java: do { i++; } while (i < 10);
来源：http://lo.colortex.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://cg.bjjhwx.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xd.jianghongdianzi.cn

C#:   do { i++; } while (i < 10);
来源：http://ij.huixinmuqiang.cn

[B09] break 与 continue
来源：http://oy.huixinmuqiang.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://oj.huixinmuqiang.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tt.newstarts.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sm.bookmarksfly.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://se.yuexingan06.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sy.colortex.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ei.yuntaijiaju.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pv.hnjuh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oz.shxzukj.cn

[B10] 遍历同时拿索引
来源：http://tn.yuntaijiaju.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ut.nszjky.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xe.gzmigu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zg.muxihuayi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zt.nszjky.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://si.huixinmuqiang.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yf.huanxung.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mm.nszjky.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sc.hnjuh.cn

[B11] 生成数字序列 / 区间
来源：http://nw.shxzukj.cn

Py:   list(range(0, 10, 2))
来源：http://eb.lnxyls.cn

PHP:  range(0, 10, 2);
来源：http://gf.asd995.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://np.yuntaijiaju.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xs.panjiajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rb.szxytkj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hj.shxzukj.cn

Ruby: (0...10).step(2).to_a
来源：http://ta.yuntaijiaju.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ww.lnxyls.cn

[B12] 跳出多层循环
来源：http://xr.szxytkj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://eb.newstarts.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mf.huixiangedu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uh.muxihuayi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cx.yuexingan06.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xi.nicolike.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uw.asd995.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rv.hnjuh.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fd.huixiangedu.cn

[B13] 判断是否为数字
来源：http://cr.bjjhwx.cn

Py:   isinstance(x, (int, float))
来源：http://wp.shxzskj.cn

PHP:  is_numeric($x)
来源：http://gm.huixiangedu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vz.szsharing.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ms.yuntaijiaju.cn

Java: x instanceof Number
来源：http://pc.haigaiapp.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ho.szxytkj.cn

Ruby: x.is_a?(Numeric)
来源：http://pc.hnjuh.cn

C#:   x is int or double or decimal
来源：http://ch.jctech888.com.cn

[B14] 判断值是否在集合内
来源：http://wg.haigaiapp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hf.nszjky.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wa.nszjky.cn

JS:   [1, 2, 3].includes(x)
来源：http://mm.9csxet.cn

TS:   [1, 2, 3].includes(x)
来源：http://ww.newstarts.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hr.szxytkj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ws.jianghongdianzi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xp.521024.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rm.newstarts.cn

[B15] 布尔运算与取反
来源：http://zh.jctech888.com.cn

Py:   a and b or not c
来源：http://ns.shxzskj.cn

PHP:  $a && $b || !$c
来源：http://it.muxihuayi.cn

JS:   a && b || !c
来源：http://yp.shxzukj.cn

TS:   a && b || !c
来源：http://rg.szxytkj.cn

Java: a && b || !c
来源：http://vo.nicolike.cn

Go:   a && b || !c
来源：http://sw.haigaiapp.cn

Ruby: a && b || !c
来源：http://oa.hnjuh.cn

C#:   a && b || !c
来源：http://fk.huixinmuqiang.cn

[B16] 卫语句：不满足条件提前返回
来源：http://nv.muxihuayi.cn

Py:   if not data: return
来源：http://pf.yuexingan06.cn

PHP:  if (!$data) { return; }
来源：http://gg.huixiangedu.cn

JS:   if (!data) return;
来源：http://lg.shxzukj.cn

TS:   if (!data) return;
来源：http://gg.szxytkj.cn

Java: if (data == null) return;
来源：http://nc.9csxet.cn

Go:   if data == nil { return }
来源：http://te.bookmarksfly.cn

Ruby: return if data.nil?
来源：http://dr.jctech888.com.cn

C#:   if (data == null) return;
来源：http://pq.yuexingan06.cn

================================================================================
来源：http://ng.shxzukj.cn

C. 函数与作用域
来源：http://nq.jctech888.com.cn

================================================================================
来源：http://ay.bookmarksfly.cn

[C01] 定义函数
来源：http://mb.bookmarksfly.cn

Py:   def add(a, b): return a + b
来源：http://ha.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://im.szxytkj.cn

JS:   function add(a, b) { return a + b; }
来源：http://sj.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yk.huixinmuqiang.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hj.huanxung.cn

Go:   func add(a, b int) int { return a + b }
来源：http://he.haigaiapp.cn

Ruby: def add(a, b); a + b; end
来源：http://vy.bjjhwx.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sa.newstarts.cn

[C02] 默认参数
来源：http://wj.shxzskj.cn

Py:   def greet(name="World"): return name
来源：http://gs.lnxyls.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xw.haigaiapp.cn

JS:   function greet(name = "World") { return name; }
来源：http://nr.jianghongdianzi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ds.huixinmuqiang.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hw.gzmigu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fo.lnxyls.cn

Ruby: def greet(name = "World") = name
来源：http://mm.nicolike.cn

C#:   string Greet(string name = "World") => name;
来源：http://op.shxzukj.cn

[C03] 可变参数
来源：http://el.haigaiapp.cn

Py:   def total(*args): return sum(args)
来源：http://as.9csxet.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xt.yuexingan06.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xd.wgjwhj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zk.9csxet.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://da.colortex.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dz.asd995.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ga.colortex.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://af.newstarts.cn

[C04] 命名参数 / 关键字参数
来源：http://kl.shxzskj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cm.wgjwhj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tg.nszjky.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tt.hnjuh.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://oe.newstarts.cn

Java: // 无：用 Builder 模式或 record
来源：http://sa.gzmigu.cn

Go:   // 无：用配置结构体参数
来源：http://oy.yuexingan06.cn

Ruby: f(a: 1, b: 2)
来源：http://jh.nicolike.cn

C#:   f(a: 1, b: 2)
来源：http://ei.shxzskj.cn

[C05] 返回多个值
来源：http://od.bjjhwx.cn

Py:   return a, b
来源：http://mq.szsharing.cn

PHP:  return [$a, $b];
来源：http://kk.szsharing.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xx.hnjuh.cn

TS:   return { a, b };
来源：http://xa.chemitech.net.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kq.wgjwhj.cn

Go:   return a, b
来源：http://xk.newstarts.cn

Ruby: return a, b
来源：http://nm.gzmigu.cn

C#:   return (a, b);              // ValueTuple
来源：http://xn.chemitech.net.cn

[C06] 匿名函数 / lambda
来源：http://kl.nicolike.cn

Py:   square = lambda x: x * x
来源：http://kk.yuntaijiaju.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://id.wgjwhj.cn

JS:   const square = x => x * x;
来源：http://me.asd995.cn

TS:   const square = (x: number): number => x * x;
来源：http://nx.colortex.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ps.bjjhwx.cn

Go:   sq := func(x int) int { return x * x }
来源：http://du.huixinmuqiang.cn

Ruby: square = ->(x) { x * x }
来源：http://rz.hnjuh.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ag.chemitech.net.cn

[C07] 把函数作为参数传入
来源：http://ha.newstarts.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ld.haigaiapp.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ax.bookmarksfly.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qv.asd995.cn

TS:   arr.map(String)
来源：http://mb.nicolike.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zn.lnxyls.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://me.nszjky.cn

Ruby: arr.map(&:upcase)
来源：http://qi.panjiajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://td.521024.cn

[C08] 闭包
来源：http://uz.lnxyls.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mq.jctech888.com.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://et.yuexingan06.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qb.szsharing.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tr.bookmarksfly.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ww.wgjwhj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ro.colortex.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hm.panjiajie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://un.szxytkj.cn

[C09] 递归
来源：http://wm.jianghongdianzi.cn


<!-- 参考信息 -->