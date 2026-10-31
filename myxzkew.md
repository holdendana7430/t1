代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rf.yuntaijiaju.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fz.haigaiapp.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pw.jctech888.com.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vi.szxytkj.cn

[A18] 字符与 ASCII 码互转
来源：http://iu.haigaiapp.cn

Py:   ord("A"); chr(65)
来源：http://du.huixiangedu.cn

PHP:  ord("A"); chr(65)
来源：http://gv.bjjhwx.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://to.huixinmuqiang.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mo.asd995.cn

Java: (int) 'A'; (char) 65
来源：http://lj.9csxet.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fm.szxytkj.cn

Ruby: "A".ord; 65.chr
来源：http://ql.colortex.cn

C#:   (int)'A'; (char)65
来源：http://gv.bjjhwx.cn

[A19] 交换两个变量
来源：http://ac.shxzukj.cn

Py:   a, b = b, a
来源：http://tm.521024.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://yx.bjjhwx.cn

JS:   [a, b] = [b, a];
来源：http://gw.newstarts.cn

TS:   [a, b] = [b, a];
来源：http://hz.hahajie.cn

Java: int t = a; a = b; b = t;
来源：http://hl.panjiajie.cn

Go:   a, b = b, a
来源：http://iy.jctech888.com.cn

Ruby: a, b = b, a
来源：http://cz.shxzukj.cn

C#:   (a, b) = (b, a);
来源：http://ki.newstarts.cn

[A20] 读取标准输入
来源：http://zi.szxytkj.cn

Py:   name = input("请输入：")
来源：http://eu.9csxet.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://qd.huixinmuqiang.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://np.bookmarksfly.cn

TS:   // Node.js：readline 模块
来源：http://kh.bjjhwx.cn

Java: new Scanner(System.in).nextLine()
来源：http://ja.shxzukj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dx.szxytkj.cn

Ruby: gets.chomp
来源：http://tn.nszjky.cn

C#:   Console.ReadLine();
来源：http://nk.szsharing.cn

[A21] 保留指定小数位输出
来源：http://jr.colortex.cn

Py:   f"{3.14159:.2f}"
来源：http://ek.haigaiapp.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cu.muxihuayi.cn

JS:   (3.14159).toFixed(2)
来源：http://ez.colortex.cn

TS:   (3.14159).toFixed(2)
来源：http://be.huixiangedu.cn

Java: String.format("%.2f", 3.14159)
来源：http://iz.bookmarksfly.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ri.nszjky.cn

Ruby: format("%.2f", 3.14159)
来源：http://ke.nszjky.cn

C#:   3.14159.ToString("F2")
来源：http://nd.shtwfgs.cn

[A22] 获取字符串长度
来源：http://cu.huixiangedu.cn

Py:   len(s)
来源：http://fh.panjiajie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://iq.521024.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://iy.9csxet.cn

TS:   s.length
来源：http://mj.huixinmuqiang.cn

Java: s.length()
来源：http://sa.gzmigu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pf.gzmigu.cn

Ruby: s.length
来源：http://hv.jianghongdianzi.cn

C#:   s.Length
来源：http://wl.yuntaijiaju.cn

[A23] 大小写转换
来源：http://sx.huixiangedu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zx.newstarts.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mq.szsharing.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hu.lnxyls.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xv.521024.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://km.jctech888.com.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vq.lnxyls.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hn.yuntaijiaju.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ba.bookmarksfly.cn

[A24] 去除首尾空白
来源：http://iv.bookmarksfly.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zv.bjjhwx.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vl.yuntaijiaju.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ap.9csxet.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wc.bookmarksfly.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qx.huixiangedu.cn

Go:   strings.TrimSpace(s)
来源：http://gf.lnxyls.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ov.521024.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rz.hnjuh.cn

[A25] 字符串比较
来源：http://sj.nicolike.cn

Py:   s1 == s2; s1 != s2
来源：http://ho.shxzskj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fr.bjjhwx.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lp.asd995.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ru.wgjwhj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tk.521024.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://oi.lnxyls.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ch.shxzskj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mc.hahajie.cn

[A26] 类型转换总览
来源：http://zg.gzmigu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ca.bjjhwx.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qi.lnxyls.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://aq.haigaiapp.cn

TS:   Number() String() Boolean() x as number
来源：http://zd.shxzskj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zs.asd995.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cy.muxihuayi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ly.shtwfgs.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ro.521024.cn

================================================================================
来源：http://sn.jctech888.com.cn

B. 流程控制
来源：http://qr.huanxung.cn

================================================================================
来源：http://jb.colortex.cn

[B01] 条件判断 if / else
来源：http://nq.muxihuayi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bv.nszjky.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fe.asd995.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ne.szsharing.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://uk.szxytkj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://go.yuntaijiaju.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vd.yuntaijiaju.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ja.szsharing.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ds.hahajie.cn

[B02] 多分支 else if / elif
来源：http://xi.yuntaijiaju.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sm.szxytkj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jb.szsharing.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aq.lnxyls.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bf.jctech888.com.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sm.bjjhwx.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://od.hahajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://af.nicolike.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xc.yuexingan06.cn

[B03] switch / match / case
来源：http://sm.521024.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zl.521024.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tj.huixinmuqiang.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ix.shxzskj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rq.haigaiapp.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mg.nicolike.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wu.yuexingan06.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yq.panjiajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sg.huanxung.cn

[B04] for 计数循环
来源：http://yy.szxytkj.cn

Py:   for i in range(10): print(i)
来源：http://wl.nszjky.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vg.colortex.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ue.jianghongdianzi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qu.colortex.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yl.muxihuayi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ch.jctech888.com.cn

Ruby: 10.times { |i| puts i }
来源：http://zl.yuexingan06.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rs.9csxet.cn

[B05] 遍历数组 / 列表
来源：http://sc.newstarts.cn

Py:   for item in arr: print(item)
来源：http://ew.szsharing.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yn.szsharing.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://sw.shxzskj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://sn.jctech888.com.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://am.newstarts.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tz.hahajie.cn

Ruby: arr.each { |item| puts item }
来源：http://li.huixiangedu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ro.yuntaijiaju.cn

[B06] 遍历字典 / 对象
来源：http://yf.huixinmuqiang.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://cu.gzmigu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dl.bjjhwx.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ea.newstarts.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ao.muxihuayi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://go.panjiajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pq.jianghongdianzi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://li.colortex.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ul.huanxung.cn

[B07] while 循环
来源：http://gz.chemitech.net.cn

Py:   while i < 10: i += 1
来源：http://il.haigaiapp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wi.jianghongdianzi.cn

JS:   while (i < 10) { i++; }
来源：http://gm.hnjuh.cn

TS:   while (i < 10) { i++; }
来源：http://dy.shxzukj.cn

Java: while (i < 10) { i++; }
来源：http://hw.huixiangedu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gs.bookmarksfly.cn

Ruby: while i < 10; i += 1; end
来源：http://ir.shtwfgs.cn

C#:   while (i < 10) { i++; }
来源：http://ct.nicolike.cn

[B08] do-while（至少执行一次）
来源：http://ph.bookmarksfly.cn

Py:   # 无 do-while：用 while True + break
来源：http://ik.yuntaijiaju.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pg.panjiajie.cn

JS:   do { i++; } while (i < 10);
来源：http://ib.huixinmuqiang.cn

TS:   do { i++; } while (i < 10);
来源：http://sp.yuntaijiaju.cn

Java: do { i++; } while (i < 10);
来源：http://zj.huixinmuqiang.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ji.wgjwhj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fz.colortex.cn

C#:   do { i++; } while (i < 10);
来源：http://sm.szsharing.cn

[B09] break 与 continue
来源：http://mj.muxihuayi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jk.chemitech.net.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ro.gzmigu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yx.hahajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cf.521024.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://io.bjjhwx.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gm.colortex.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://os.huanxung.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rt.hnjuh.cn

[B10] 遍历同时拿索引
来源：http://rs.hnjuh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://to.huixinmuqiang.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fo.lnxyls.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vr.gzmigu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ov.9csxet.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pa.9csxet.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vl.huixiangedu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sa.hnjuh.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bo.shxzukj.cn

[B11] 生成数字序列 / 区间
来源：http://jg.521024.cn

Py:   list(range(0, 10, 2))
来源：http://xr.jianghongdianzi.cn

PHP:  range(0, 10, 2);
来源：http://he.chemitech.net.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jt.asd995.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cr.lnxyls.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rt.huixinmuqiang.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hg.bookmarksfly.cn

Ruby: (0...10).step(2).to_a
来源：http://om.nszjky.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zd.jianghongdianzi.cn

[B12] 跳出多层循环
来源：http://ut.shtwfgs.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wy.haigaiapp.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://pc.jianghongdianzi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xj.szsharing.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tk.bjjhwx.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fk.huixiangedu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bc.szxytkj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hb.wgjwhj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zz.yuntaijiaju.cn

[B13] 判断是否为数字
来源：http://mj.gzmigu.cn

Py:   isinstance(x, (int, float))
来源：http://io.huixinmuqiang.cn

PHP:  is_numeric($x)
来源：http://zi.huixinmuqiang.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hw.wgjwhj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gc.szxytkj.cn

Java: x instanceof Number
来源：http://pt.muxihuayi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hu.chemitech.net.cn

Ruby: x.is_a?(Numeric)
来源：http://hb.9csxet.cn

C#:   x is int or double or decimal
来源：http://yy.hahajie.cn

[B14] 判断值是否在集合内
来源：http://yx.muxihuayi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qo.bookmarksfly.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yc.szsharing.cn

JS:   [1, 2, 3].includes(x)
来源：http://pn.yuntaijiaju.cn

TS:   [1, 2, 3].includes(x)
来源：http://to.lnxyls.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://am.jctech888.com.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yc.szsharing.cn

Ruby: [1, 2, 3].include?(x)
来源：http://bf.shtwfgs.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uq.jctech888.com.cn

[B15] 布尔运算与取反
来源：http://gg.521024.cn

Py:   a and b or not c
来源：http://jw.bookmarksfly.cn

PHP:  $a && $b || !$c
来源：http://ob.szxytkj.cn

JS:   a && b || !c
来源：http://rg.nicolike.cn

TS:   a && b || !c
来源：http://mj.hnjuh.cn

Java: a && b || !c
来源：http://ru.wgjwhj.cn

Go:   a && b || !c
来源：http://xn.shxzukj.cn

Ruby: a && b || !c
来源：http://np.nicolike.cn

C#:   a && b || !c
来源：http://nv.panjiajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ry.bookmarksfly.cn

Py:   if not data: return
来源：http://cn.hahajie.cn

PHP:  if (!$data) { return; }
来源：http://io.newstarts.cn

JS:   if (!data) return;
来源：http://lp.yuntaijiaju.cn

TS:   if (!data) return;
来源：http://dm.chemitech.net.cn

Java: if (data == null) return;
来源：http://xi.jctech888.com.cn

Go:   if data == nil { return }
来源：http://gj.lnxyls.cn

Ruby: return if data.nil?
来源：http://yo.wgjwhj.cn

C#:   if (data == null) return;
来源：http://jy.newstarts.cn

================================================================================
来源：http://hz.hnjuh.cn

C. 函数与作用域
来源：http://aw.shxzskj.cn

================================================================================
来源：http://fp.asd995.cn

[C01] 定义函数
来源：http://bd.9csxet.cn

Py:   def add(a, b): return a + b
来源：http://kj.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cw.jianghongdianzi.cn

JS:   function add(a, b) { return a + b; }
来源：http://xk.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wg.shxzukj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mf.lnxyls.cn

Go:   func add(a, b int) int { return a + b }
来源：http://gl.jianghongdianzi.cn

Ruby: def add(a, b); a + b; end
来源：http://uq.jctech888.com.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rs.asd995.cn

[C02] 默认参数
来源：http://xa.wgjwhj.cn

Py:   def greet(name="World"): return name
来源：http://is.wgjwhj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://rh.yuntaijiaju.cn

JS:   function greet(name = "World") { return name; }
来源：http://vm.bookmarksfly.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rx.szxytkj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://iz.jianghongdianzi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ej.wgjwhj.cn

Ruby: def greet(name = "World") = name
来源：http://iq.521024.cn

C#:   string Greet(string name = "World") => name;
来源：http://ej.9csxet.cn

[C03] 可变参数
来源：http://ru.haigaiapp.cn

Py:   def total(*args): return sum(args)
来源：http://vu.bjjhwx.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://eq.bookmarksfly.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lt.bookmarksfly.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://az.asd995.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pc.jctech888.com.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://eo.shxzskj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yb.huanxung.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xz.huanxung.cn

[C04] 命名参数 / 关键字参数
来源：http://yv.asd995.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dx.szxytkj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kk.bookmarksfly.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xw.yuntaijiaju.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wt.yuexingan06.cn

Java: // 无：用 Builder 模式或 record
来源：http://ir.chemitech.net.cn

Go:   // 无：用配置结构体参数
来源：http://ze.hahajie.cn

Ruby: f(a: 1, b: 2)
来源：http://uj.jianghongdianzi.cn

C#:   f(a: 1, b: 2)
来源：http://ug.huixiangedu.cn

[C05] 返回多个值
来源：http://ye.huixiangedu.cn

Py:   return a, b
来源：http://kj.wgjwhj.cn

PHP:  return [$a, $b];
来源：http://nh.panjiajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ig.lnxyls.cn

TS:   return { a, b };
来源：http://ei.521024.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://py.9csxet.cn

Go:   return a, b
来源：http://qc.nicolike.cn

Ruby: return a, b
来源：http://kx.szxytkj.cn

C#:   return (a, b);              // ValueTuple
来源：http://dj.szxytkj.cn

[C06] 匿名函数 / lambda
来源：http://dn.9csxet.cn

Py:   square = lambda x: x * x
来源：http://fk.hnjuh.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ik.haigaiapp.cn

JS:   const square = x => x * x;
来源：http://rz.huanxung.cn

TS:   const square = (x: number): number => x * x;
来源：http://zl.lnxyls.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lm.huixinmuqiang.cn

Go:   sq := func(x int) int { return x * x }
来源：http://cp.panjiajie.cn

Ruby: square = ->(x) { x * x }
来源：http://wy.bjjhwx.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fs.yuexingan06.cn

[C07] 把函数作为参数传入
来源：http://fe.wgjwhj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jf.jctech888.com.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bo.521024.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://es.asd995.cn

TS:   arr.map(String)
来源：http://sk.521024.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ih.shtwfgs.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ma.hahajie.cn

Ruby: arr.map(&:upcase)
来源：http://hs.muxihuayi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://dm.nszjky.cn

[C08] 闭包
来源：http://ap.wgjwhj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kd.asd995.cn


<!-- 参考信息 -->