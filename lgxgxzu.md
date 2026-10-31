代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sx.huanxung.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://sj.yuntaijiaju.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lg.jctech888.com.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dm.nicolike.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vy.newstarts.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fj.wgjwhj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qf.huanxung.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ez.haigaiapp.cn

[A18] 字符与 ASCII 码互转
来源：http://aa.shxzskj.cn

Py:   ord("A"); chr(65)
来源：http://og.521024.cn

PHP:  ord("A"); chr(65)
来源：http://gm.lnxyls.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fm.shtwfgs.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ix.szsharing.cn

Java: (int) 'A'; (char) 65
来源：http://ha.haigaiapp.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://oz.panjiajie.cn

Ruby: "A".ord; 65.chr
来源：http://ob.bookmarksfly.cn

C#:   (int)'A'; (char)65
来源：http://ne.bjjhwx.cn

[A19] 交换两个变量
来源：http://mx.chemitech.net.cn

Py:   a, b = b, a
来源：http://zb.newstarts.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ws.muxihuayi.cn

JS:   [a, b] = [b, a];
来源：http://yb.nicolike.cn

TS:   [a, b] = [b, a];
来源：http://kk.nszjky.cn

Java: int t = a; a = b; b = t;
来源：http://lx.nszjky.cn

Go:   a, b = b, a
来源：http://go.nicolike.cn

Ruby: a, b = b, a
来源：http://bt.colortex.cn

C#:   (a, b) = (b, a);
来源：http://iv.haigaiapp.cn

[A20] 读取标准输入
来源：http://cb.yuexingan06.cn

Py:   name = input("请输入：")
来源：http://lb.szsharing.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://lf.haigaiapp.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://im.asd995.cn

TS:   // Node.js：readline 模块
来源：http://fp.yuntaijiaju.cn

Java: new Scanner(System.in).nextLine()
来源：http://nn.shxzukj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dq.jctech888.com.cn

Ruby: gets.chomp
来源：http://vi.muxihuayi.cn

C#:   Console.ReadLine();
来源：http://qj.jianghongdianzi.cn

[A21] 保留指定小数位输出
来源：http://cj.szxytkj.cn

Py:   f"{3.14159:.2f}"
来源：http://ed.newstarts.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://df.shtwfgs.cn

JS:   (3.14159).toFixed(2)
来源：http://oa.huanxung.cn

TS:   (3.14159).toFixed(2)
来源：http://vg.szxytkj.cn

Java: String.format("%.2f", 3.14159)
来源：http://xg.haigaiapp.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zd.yuexingan06.cn

Ruby: format("%.2f", 3.14159)
来源：http://kh.bjjhwx.cn

C#:   3.14159.ToString("F2")
来源：http://go.gzmigu.cn

[A22] 获取字符串长度
来源：http://mc.muxihuayi.cn

Py:   len(s)
来源：http://bv.szsharing.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://aa.hnjuh.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cj.lnxyls.cn

TS:   s.length
来源：http://wi.colortex.cn

Java: s.length()
来源：http://yq.huanxung.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://od.huanxung.cn

Ruby: s.length
来源：http://pv.huixinmuqiang.cn

C#:   s.Length
来源：http://tq.shtwfgs.cn

[A23] 大小写转换
来源：http://sh.jianghongdianzi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://eo.huixinmuqiang.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://nj.9csxet.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://id.521024.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mm.shtwfgs.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wj.bookmarksfly.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://iw.shtwfgs.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wa.jianghongdianzi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ni.521024.cn

[A24] 去除首尾空白
来源：http://xk.hahajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ah.521024.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dm.panjiajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ns.gzmigu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rt.jctech888.com.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cg.wgjwhj.cn

Go:   strings.TrimSpace(s)
来源：http://my.huixinmuqiang.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xw.panjiajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cz.jianghongdianzi.cn

[A25] 字符串比较
来源：http://zh.colortex.cn

Py:   s1 == s2; s1 != s2
来源：http://fd.colortex.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vm.9csxet.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://sq.bjjhwx.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ez.szxytkj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fk.asd995.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fy.bookmarksfly.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://zn.szsharing.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lc.shtwfgs.cn

[A26] 类型转换总览
来源：http://di.hahajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fs.shxzskj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fu.9csxet.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tb.yuexingan06.cn

TS:   Number() String() Boolean() x as number
来源：http://at.huixiangedu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jf.9csxet.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cw.colortex.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://au.muxihuayi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vx.huixinmuqiang.cn

================================================================================
来源：http://im.huanxung.cn

B. 流程控制
来源：http://xv.haigaiapp.cn

================================================================================
来源：http://bl.nicolike.cn

[B01] 条件判断 if / else
来源：http://nb.hahajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://cs.yuexingan06.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kc.yuexingan06.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://on.wgjwhj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://de.yuexingan06.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://kq.hnjuh.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://uy.huanxung.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yl.wgjwhj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wf.shxzukj.cn

[B02] 多分支 else if / elif
来源：http://ky.bjjhwx.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://eo.yuexingan06.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://oq.bjjhwx.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pq.521024.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ol.hahajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fy.yuexingan06.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zq.yuntaijiaju.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mj.huixinmuqiang.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ls.muxihuayi.cn

[B03] switch / match / case
来源：http://bk.huanxung.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://oe.asd995.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yr.chemitech.net.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lq.nszjky.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gh.haigaiapp.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lw.9csxet.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ky.gzmigu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vv.colortex.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lr.shtwfgs.cn

[B04] for 计数循环
来源：http://af.colortex.cn

Py:   for i in range(10): print(i)
来源：http://fr.chemitech.net.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cz.lnxyls.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yw.jianghongdianzi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cm.shxzskj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yf.yuntaijiaju.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rv.newstarts.cn

Ruby: 10.times { |i| puts i }
来源：http://xb.jianghongdianzi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rg.521024.cn

[B05] 遍历数组 / 列表
来源：http://ak.yuexingan06.cn

Py:   for item in arr: print(item)
来源：http://iw.nicolike.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dh.jianghongdianzi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://vu.bjjhwx.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gt.shxzskj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fm.lnxyls.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wq.asd995.cn

Ruby: arr.each { |item| puts item }
来源：http://kq.nicolike.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dj.huixinmuqiang.cn

[B06] 遍历字典 / 对象
来源：http://ba.bookmarksfly.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://bb.asd995.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://oi.szsharing.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bb.bookmarksfly.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jt.shtwfgs.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uc.jianghongdianzi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gq.hahajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qr.yuntaijiaju.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ht.hahajie.cn

[B07] while 循环
来源：http://ab.huixinmuqiang.cn

Py:   while i < 10: i += 1
来源：http://nj.nszjky.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fi.hahajie.cn

JS:   while (i < 10) { i++; }
来源：http://de.asd995.cn

TS:   while (i < 10) { i++; }
来源：http://rz.nszjky.cn

Java: while (i < 10) { i++; }
来源：http://yj.huixiangedu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wh.lnxyls.cn

Ruby: while i < 10; i += 1; end
来源：http://ot.panjiajie.cn

C#:   while (i < 10) { i++; }
来源：http://is.wgjwhj.cn

[B08] do-while（至少执行一次）
来源：http://ut.chemitech.net.cn

Py:   # 无 do-while：用 while True + break
来源：http://cx.yuexingan06.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://gn.nszjky.cn

JS:   do { i++; } while (i < 10);
来源：http://bf.bjjhwx.cn

TS:   do { i++; } while (i < 10);
来源：http://wf.newstarts.cn

Java: do { i++; } while (i < 10);
来源：http://go.jctech888.com.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wc.hnjuh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ph.521024.cn

C#:   do { i++; } while (i < 10);
来源：http://fk.9csxet.cn

[B09] break 与 continue
来源：http://fe.wgjwhj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rk.jctech888.com.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cc.hnjuh.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gw.bookmarksfly.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mg.huixinmuqiang.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iv.newstarts.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bm.shxzukj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vb.bjjhwx.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gk.huixinmuqiang.cn

[B10] 遍历同时拿索引
来源：http://yk.asd995.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gq.yuexingan06.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wq.bookmarksfly.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dc.yuntaijiaju.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://np.lnxyls.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tn.chemitech.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lq.colortex.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xc.asd995.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bp.bjjhwx.cn

[B11] 生成数字序列 / 区间
来源：http://ry.huixinmuqiang.cn

Py:   list(range(0, 10, 2))
来源：http://of.nszjky.cn

PHP:  range(0, 10, 2);
来源：http://sb.muxihuayi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rn.huixinmuqiang.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ad.szsharing.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cf.huixinmuqiang.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://og.shxzukj.cn

Ruby: (0...10).step(2).to_a
来源：http://xw.colortex.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yy.shxzukj.cn

[B12] 跳出多层循环
来源：http://in.huixinmuqiang.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://gn.nszjky.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hq.huanxung.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qh.newstarts.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kz.haigaiapp.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jz.yuntaijiaju.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://oi.nicolike.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cl.hnjuh.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mo.szsharing.cn

[B13] 判断是否为数字
来源：http://eu.yuexingan06.cn

Py:   isinstance(x, (int, float))
来源：http://xw.521024.cn

PHP:  is_numeric($x)
来源：http://zx.wgjwhj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fg.yuntaijiaju.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wl.nszjky.cn

Java: x instanceof Number
来源：http://fi.hahajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tc.hnjuh.cn

Ruby: x.is_a?(Numeric)
来源：http://ha.nicolike.cn

C#:   x is int or double or decimal
来源：http://qi.szsharing.cn

[B14] 判断值是否在集合内
来源：http://ee.shxzskj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jm.colortex.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://an.jianghongdianzi.cn

JS:   [1, 2, 3].includes(x)
来源：http://dy.yuntaijiaju.cn

TS:   [1, 2, 3].includes(x)
来源：http://jl.bookmarksfly.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://pk.hnjuh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://uk.colortex.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fp.haigaiapp.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qc.hnjuh.cn

[B15] 布尔运算与取反
来源：http://io.huixinmuqiang.cn

Py:   a and b or not c
来源：http://mv.shtwfgs.cn

PHP:  $a && $b || !$c
来源：http://pf.shxzukj.cn

JS:   a && b || !c
来源：http://fi.huixinmuqiang.cn

TS:   a && b || !c
来源：http://oo.9csxet.cn

Java: a && b || !c
来源：http://wg.nicolike.cn

Go:   a && b || !c
来源：http://rn.asd995.cn

Ruby: a && b || !c
来源：http://rk.hahajie.cn

C#:   a && b || !c
来源：http://ep.jianghongdianzi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xi.szsharing.cn

Py:   if not data: return
来源：http://zw.hahajie.cn

PHP:  if (!$data) { return; }
来源：http://cq.shtwfgs.cn

JS:   if (!data) return;
来源：http://kt.yuntaijiaju.cn

TS:   if (!data) return;
来源：http://yq.nicolike.cn

Java: if (data == null) return;
来源：http://kh.lnxyls.cn

Go:   if data == nil { return }
来源：http://yf.shxzukj.cn

Ruby: return if data.nil?
来源：http://hd.panjiajie.cn

C#:   if (data == null) return;
来源：http://il.shxzukj.cn

================================================================================
来源：http://oc.szxytkj.cn

C. 函数与作用域
来源：http://dk.hnjuh.cn

================================================================================
来源：http://ag.chemitech.net.cn

[C01] 定义函数
来源：http://hp.nicolike.cn

Py:   def add(a, b): return a + b
来源：http://gx.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jp.huixinmuqiang.cn

JS:   function add(a, b) { return a + b; }
来源：http://vf.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ja.chemitech.net.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lx.jianghongdianzi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ut.wgjwhj.cn

Ruby: def add(a, b); a + b; end
来源：http://ig.hnjuh.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ro.nicolike.cn

[C02] 默认参数
来源：http://in.shxzukj.cn

Py:   def greet(name="World"): return name
来源：http://ry.521024.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lq.szxytkj.cn

JS:   function greet(name = "World") { return name; }
来源：http://it.szxytkj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://jj.nszjky.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://gp.9csxet.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ug.hnjuh.cn

Ruby: def greet(name = "World") = name
来源：http://qn.szxytkj.cn

C#:   string Greet(string name = "World") => name;
来源：http://yz.szsharing.cn

[C03] 可变参数
来源：http://rs.shxzukj.cn

Py:   def total(*args): return sum(args)
来源：http://su.szsharing.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mh.huixiangedu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://by.huanxung.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tp.bookmarksfly.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://th.shtwfgs.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ip.gzmigu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fg.shxzukj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ec.hahajie.cn

[C04] 命名参数 / 关键字参数
来源：http://rt.hahajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qs.bjjhwx.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ha.haigaiapp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zg.haigaiapp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ce.bookmarksfly.cn

Java: // 无：用 Builder 模式或 record
来源：http://io.jianghongdianzi.cn

Go:   // 无：用配置结构体参数
来源：http://ik.lnxyls.cn

Ruby: f(a: 1, b: 2)
来源：http://pe.hnjuh.cn

C#:   f(a: 1, b: 2)
来源：http://mf.panjiajie.cn

[C05] 返回多个值
来源：http://aj.chemitech.net.cn

Py:   return a, b
来源：http://qp.gzmigu.cn

PHP:  return [$a, $b];
来源：http://gn.hnjuh.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://np.9csxet.cn

TS:   return { a, b };
来源：http://li.colortex.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gl.bookmarksfly.cn

Go:   return a, b
来源：http://gb.hnjuh.cn

Ruby: return a, b
来源：http://xo.szsharing.cn

C#:   return (a, b);              // ValueTuple
来源：http://bb.huixiangedu.cn

[C06] 匿名函数 / lambda
来源：http://ay.szxytkj.cn

Py:   square = lambda x: x * x
来源：http://iz.asd995.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xr.hnjuh.cn

JS:   const square = x => x * x;
来源：http://wj.jctech888.com.cn

TS:   const square = (x: number): number => x * x;
来源：http://ts.hnjuh.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ol.haigaiapp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://lt.shxzskj.cn

Ruby: square = ->(x) { x * x }
来源：http://ny.bjjhwx.cn

C#:   Func<int, int> square = x => x * x;
来源：http://cv.lnxyls.cn

[C07] 把函数作为参数传入
来源：http://vp.newstarts.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zv.9csxet.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ys.jctech888.com.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zc.huanxung.cn

TS:   arr.map(String)
来源：http://gv.nicolike.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ck.hahajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fm.asd995.cn


<!-- 参考信息 -->