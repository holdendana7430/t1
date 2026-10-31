代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pn.shtwfgs.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://md.huixinmuqiang.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aa.hnjuh.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ei.panjiajie.cn

[A18] 字符与 ASCII 码互转
来源：http://xi.nicolike.cn

Py:   ord("A"); chr(65)
来源：http://ni.panjiajie.cn

PHP:  ord("A"); chr(65)
来源：http://ol.asd995.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lp.gzmigu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://we.shxzskj.cn

Java: (int) 'A'; (char) 65
来源：http://dn.shxzukj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ey.hahajie.cn

Ruby: "A".ord; 65.chr
来源：http://yi.jctech888.com.cn

C#:   (int)'A'; (char)65
来源：http://ly.panjiajie.cn

[A19] 交换两个变量
来源：http://ic.huixiangedu.cn

Py:   a, b = b, a
来源：http://tc.asd995.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://rj.nszjky.cn

JS:   [a, b] = [b, a];
来源：http://ib.huixinmuqiang.cn

TS:   [a, b] = [b, a];
来源：http://cq.bjjhwx.cn

Java: int t = a; a = b; b = t;
来源：http://lk.huanxung.cn

Go:   a, b = b, a
来源：http://qc.asd995.cn

Ruby: a, b = b, a
来源：http://cn.shxzukj.cn

C#:   (a, b) = (b, a);
来源：http://vj.yuntaijiaju.cn

[A20] 读取标准输入
来源：http://fj.huixinmuqiang.cn

Py:   name = input("请输入：")
来源：http://ex.9csxet.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ze.chemitech.net.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ta.bjjhwx.cn

TS:   // Node.js：readline 模块
来源：http://oc.huixiangedu.cn

Java: new Scanner(System.in).nextLine()
来源：http://qw.szxytkj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://rq.chemitech.net.cn

Ruby: gets.chomp
来源：http://sy.haigaiapp.cn

C#:   Console.ReadLine();
来源：http://yy.szxytkj.cn

[A21] 保留指定小数位输出
来源：http://od.chemitech.net.cn

Py:   f"{3.14159:.2f}"
来源：http://mj.wgjwhj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vg.shxzukj.cn

JS:   (3.14159).toFixed(2)
来源：http://vj.yuntaijiaju.cn

TS:   (3.14159).toFixed(2)
来源：http://mh.hahajie.cn

Java: String.format("%.2f", 3.14159)
来源：http://mf.hahajie.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://oy.bookmarksfly.cn

Ruby: format("%.2f", 3.14159)
来源：http://ln.jianghongdianzi.cn

C#:   3.14159.ToString("F2")
来源：http://od.521024.cn

[A22] 获取字符串长度
来源：http://ey.lnxyls.cn

Py:   len(s)
来源：http://rt.nicolike.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ef.panjiajie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://es.521024.cn

TS:   s.length
来源：http://is.muxihuayi.cn

Java: s.length()
来源：http://ok.shtwfgs.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bo.hnjuh.cn

Ruby: s.length
来源：http://eb.hnjuh.cn

C#:   s.Length
来源：http://rd.9csxet.cn

[A23] 大小写转换
来源：http://zs.panjiajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://jt.nszjky.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://be.gzmigu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://og.huixiangedu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xt.shtwfgs.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vy.wgjwhj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kp.panjiajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mz.9csxet.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://th.9csxet.cn

[A24] 去除首尾空白
来源：http://xq.hnjuh.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mf.shtwfgs.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gc.szsharing.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zz.huixinmuqiang.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lw.nszjky.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fz.colortex.cn

Go:   strings.TrimSpace(s)
来源：http://hq.bookmarksfly.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jj.szsharing.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://au.shxzukj.cn

[A25] 字符串比较
来源：http://di.yuexingan06.cn

Py:   s1 == s2; s1 != s2
来源：http://jb.yuexingan06.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ih.hnjuh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://so.hnjuh.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://iw.yuntaijiaju.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rz.shtwfgs.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gx.bjjhwx.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://po.bjjhwx.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bi.hnjuh.cn

[A26] 类型转换总览
来源：http://vn.hnjuh.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rz.yuntaijiaju.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uj.szsharing.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ru.jianghongdianzi.cn

TS:   Number() String() Boolean() x as number
来源：http://hu.shxzukj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qs.nicolike.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://aq.shxzskj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zd.muxihuayi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xy.wgjwhj.cn

================================================================================
来源：http://wz.jctech888.com.cn

B. 流程控制
来源：http://wv.shxzskj.cn

================================================================================
来源：http://ma.yuntaijiaju.cn

[B01] 条件判断 if / else
来源：http://pz.nicolike.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://lh.muxihuayi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rt.yuexingan06.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://us.bjjhwx.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hk.newstarts.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ts.wgjwhj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ng.huixiangedu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ln.colortex.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ws.colortex.cn

[B02] 多分支 else if / elif
来源：http://xm.jianghongdianzi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kv.haigaiapp.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ih.haigaiapp.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kh.panjiajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gz.shxzskj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rv.shxzskj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dn.wgjwhj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pn.yuexingan06.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yc.bookmarksfly.cn

[B03] switch / match / case
来源：http://fa.bjjhwx.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lh.yuexingan06.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fn.lnxyls.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bj.huixiangedu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://az.bjjhwx.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sy.haigaiapp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wp.huanxung.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fp.9csxet.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ge.521024.cn

[B04] for 计数循环
来源：http://qn.jianghongdianzi.cn

Py:   for i in range(10): print(i)
来源：http://er.lnxyls.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fv.lnxyls.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pk.wgjwhj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vm.nszjky.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ep.hnjuh.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kr.shxzskj.cn

Ruby: 10.times { |i| puts i }
来源：http://bx.nicolike.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cp.huanxung.cn

[B05] 遍历数组 / 列表
来源：http://mx.nszjky.cn

Py:   for item in arr: print(item)
来源：http://bo.yuntaijiaju.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://np.haigaiapp.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ta.bjjhwx.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tr.lnxyls.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fd.huixinmuqiang.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pt.colortex.cn

Ruby: arr.each { |item| puts item }
来源：http://um.521024.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ai.bookmarksfly.cn

[B06] 遍历字典 / 对象
来源：http://ur.hnjuh.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://rb.hahajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qe.nicolike.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jk.asd995.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sc.newstarts.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qy.hahajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xp.bjjhwx.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ki.muxihuayi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ik.yuntaijiaju.cn

[B07] while 循环
来源：http://ts.521024.cn

Py:   while i < 10: i += 1
来源：http://ma.wgjwhj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fl.yuntaijiaju.cn

JS:   while (i < 10) { i++; }
来源：http://pz.huanxung.cn

TS:   while (i < 10) { i++; }
来源：http://uo.nszjky.cn

Java: while (i < 10) { i++; }
来源：http://cy.muxihuayi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qb.asd995.cn

Ruby: while i < 10; i += 1; end
来源：http://ps.nicolike.cn

C#:   while (i < 10) { i++; }
来源：http://dx.jianghongdianzi.cn

[B08] do-while（至少执行一次）
来源：http://nm.szxytkj.cn

Py:   # 无 do-while：用 while True + break
来源：http://lq.chemitech.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://lx.colortex.cn

JS:   do { i++; } while (i < 10);
来源：http://ve.nicolike.cn

TS:   do { i++; } while (i < 10);
来源：http://dh.shtwfgs.cn

Java: do { i++; } while (i < 10);
来源：http://ck.bjjhwx.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://nn.jianghongdianzi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ae.bookmarksfly.cn

C#:   do { i++; } while (i < 10);
来源：http://bz.panjiajie.cn

[B09] break 与 continue
来源：http://fp.hahajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zw.9csxet.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ut.chemitech.net.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pf.wgjwhj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ea.szsharing.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pi.yuexingan06.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ig.bjjhwx.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mh.panjiajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yl.shxzskj.cn

[B10] 遍历同时拿索引
来源：http://ly.yuexingan06.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://oj.jianghongdianzi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ck.jianghongdianzi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sg.521024.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pa.muxihuayi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xz.nicolike.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jt.521024.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xp.shxzskj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pa.hahajie.cn

[B11] 生成数字序列 / 区间
来源：http://rv.panjiajie.cn

Py:   list(range(0, 10, 2))
来源：http://xp.9csxet.cn

PHP:  range(0, 10, 2);
来源：http://zm.haigaiapp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gp.panjiajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cb.bjjhwx.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ha.huixinmuqiang.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://iw.jianghongdianzi.cn

Ruby: (0...10).step(2).to_a
来源：http://ue.haigaiapp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dq.9csxet.cn

[B12] 跳出多层循环
来源：http://ph.9csxet.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://mh.nicolike.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://bz.nszjky.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sv.huixiangedu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bu.haigaiapp.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cr.bookmarksfly.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vx.9csxet.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tv.colortex.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ds.yuexingan06.cn

[B13] 判断是否为数字
来源：http://yn.nszjky.cn

Py:   isinstance(x, (int, float))
来源：http://mz.hnjuh.cn

PHP:  is_numeric($x)
来源：http://nn.chemitech.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://np.hahajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cm.wgjwhj.cn

Java: x instanceof Number
来源：http://qf.jianghongdianzi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bn.nicolike.cn

Ruby: x.is_a?(Numeric)
来源：http://fo.szxytkj.cn

C#:   x is int or double or decimal
来源：http://mt.huixiangedu.cn

[B14] 判断值是否在集合内
来源：http://gd.lnxyls.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zp.chemitech.net.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ej.szxytkj.cn

JS:   [1, 2, 3].includes(x)
来源：http://xx.szsharing.cn

TS:   [1, 2, 3].includes(x)
来源：http://nr.gzmigu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://aj.panjiajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jl.newstarts.cn

Ruby: [1, 2, 3].include?(x)
来源：http://nx.bjjhwx.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uz.panjiajie.cn

[B15] 布尔运算与取反
来源：http://dk.chemitech.net.cn

Py:   a and b or not c
来源：http://kp.yuexingan06.cn

PHP:  $a && $b || !$c
来源：http://wu.chemitech.net.cn

JS:   a && b || !c
来源：http://da.521024.cn

TS:   a && b || !c
来源：http://gr.hahajie.cn

Java: a && b || !c
来源：http://fn.9csxet.cn

Go:   a && b || !c
来源：http://vj.yuexingan06.cn

Ruby: a && b || !c
来源：http://dx.panjiajie.cn

C#:   a && b || !c
来源：http://lw.panjiajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vc.muxihuayi.cn

Py:   if not data: return
来源：http://yq.yuntaijiaju.cn

PHP:  if (!$data) { return; }
来源：http://nv.huixinmuqiang.cn

JS:   if (!data) return;
来源：http://xq.shxzskj.cn

TS:   if (!data) return;
来源：http://ia.huixiangedu.cn

Java: if (data == null) return;
来源：http://fc.9csxet.cn

Go:   if data == nil { return }
来源：http://zc.gzmigu.cn

Ruby: return if data.nil?
来源：http://ue.wgjwhj.cn

C#:   if (data == null) return;
来源：http://tc.huixinmuqiang.cn

================================================================================
来源：http://lo.gzmigu.cn

C. 函数与作用域
来源：http://kh.lnxyls.cn

================================================================================
来源：http://de.colortex.cn

[C01] 定义函数
来源：http://vt.muxihuayi.cn

Py:   def add(a, b): return a + b
来源：http://pz.haigaiapp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kt.shtwfgs.cn

JS:   function add(a, b) { return a + b; }
来源：http://nx.hahajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cp.colortex.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qx.bookmarksfly.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vl.shtwfgs.cn

Ruby: def add(a, b); a + b; end
来源：http://vr.jctech888.com.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ko.szsharing.cn

[C02] 默认参数
来源：http://kf.chemitech.net.cn

Py:   def greet(name="World"): return name
来源：http://hd.shtwfgs.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://in.huixinmuqiang.cn

JS:   function greet(name = "World") { return name; }
来源：http://sc.shtwfgs.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cr.huanxung.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ro.hahajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dv.jctech888.com.cn

Ruby: def greet(name = "World") = name
来源：http://sy.yuntaijiaju.cn

C#:   string Greet(string name = "World") => name;
来源：http://vc.szxytkj.cn

[C03] 可变参数
来源：http://op.szsharing.cn

Py:   def total(*args): return sum(args)
来源：http://uv.shxzskj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ft.muxihuayi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ss.szsharing.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cb.9csxet.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wg.huixinmuqiang.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xl.huanxung.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hg.panjiajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fn.521024.cn

[C04] 命名参数 / 关键字参数
来源：http://ju.hahajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qc.huixiangedu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zi.chemitech.net.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mm.szxytkj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kq.hnjuh.cn

Java: // 无：用 Builder 模式或 record
来源：http://kq.shxzukj.cn

Go:   // 无：用配置结构体参数
来源：http://co.nicolike.cn

Ruby: f(a: 1, b: 2)
来源：http://ib.nicolike.cn

C#:   f(a: 1, b: 2)
来源：http://md.panjiajie.cn

[C05] 返回多个值
来源：http://sr.muxihuayi.cn

Py:   return a, b
来源：http://mb.jctech888.com.cn

PHP:  return [$a, $b];
来源：http://fi.521024.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://hp.szxytkj.cn

TS:   return { a, b };
来源：http://lg.colortex.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ei.colortex.cn

Go:   return a, b
来源：http://xs.hahajie.cn

Ruby: return a, b
来源：http://tl.nicolike.cn

C#:   return (a, b);              // ValueTuple
来源：http://uw.bjjhwx.cn

[C06] 匿名函数 / lambda
来源：http://ct.bookmarksfly.cn

Py:   square = lambda x: x * x
来源：http://wu.9csxet.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qe.nszjky.cn

JS:   const square = x => x * x;
来源：http://go.shxzskj.cn

TS:   const square = (x: number): number => x * x;
来源：http://lt.szxytkj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sv.huixinmuqiang.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fv.nszjky.cn

Ruby: square = ->(x) { x * x }
来源：http://fh.lnxyls.cn

C#:   Func<int, int> square = x => x * x;
来源：http://oy.jctech888.com.cn

[C07] 把函数作为参数传入
来源：http://ui.yuntaijiaju.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hi.hnjuh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://pe.haigaiapp.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zj.newstarts.cn

TS:   arr.map(String)
来源：http://ks.jianghongdianzi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mv.hahajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://va.wgjwhj.cn

Ruby: arr.map(&:upcase)
来源：http://ec.yuntaijiaju.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://tn.jctech888.com.cn

[C08] 闭包
来源：http://nm.jctech888.com.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yl.chemitech.net.cn


<!-- 参考信息 -->