代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qd.wgjwhj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mu.wgjwhj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ph.bjjhwx.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://da.shxzskj.cn

[A18] 字符与 ASCII 码互转
来源：http://ar.asd995.cn

Py:   ord("A"); chr(65)
来源：http://mz.wgjwhj.cn

PHP:  ord("A"); chr(65)
来源：http://lt.huanxung.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ai.jctech888.com.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yc.panjiajie.cn

Java: (int) 'A'; (char) 65
来源：http://cr.szsharing.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jh.yuntaijiaju.cn

Ruby: "A".ord; 65.chr
来源：http://cg.nicolike.cn

C#:   (int)'A'; (char)65
来源：http://vy.nicolike.cn

[A19] 交换两个变量
来源：http://cd.shxzskj.cn

Py:   a, b = b, a
来源：http://ln.9csxet.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://pi.szxytkj.cn

JS:   [a, b] = [b, a];
来源：http://oi.wgjwhj.cn

TS:   [a, b] = [b, a];
来源：http://bn.huanxung.cn

Java: int t = a; a = b; b = t;
来源：http://zr.panjiajie.cn

Go:   a, b = b, a
来源：http://ee.hahajie.cn

Ruby: a, b = b, a
来源：http://un.hahajie.cn

C#:   (a, b) = (b, a);
来源：http://bp.szxytkj.cn

[A20] 读取标准输入
来源：http://za.shxzskj.cn

Py:   name = input("请输入：")
来源：http://tw.gzmigu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://pu.muxihuayi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wd.bookmarksfly.cn

TS:   // Node.js：readline 模块
来源：http://ho.9csxet.cn

Java: new Scanner(System.in).nextLine()
来源：http://rh.colortex.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wg.nszjky.cn

Ruby: gets.chomp
来源：http://ei.bjjhwx.cn

C#:   Console.ReadLine();
来源：http://sa.hahajie.cn

[A21] 保留指定小数位输出
来源：http://ir.shxzskj.cn

Py:   f"{3.14159:.2f}"
来源：http://od.haigaiapp.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://nd.huixiangedu.cn

JS:   (3.14159).toFixed(2)
来源：http://yz.asd995.cn

TS:   (3.14159).toFixed(2)
来源：http://wv.huixiangedu.cn

Java: String.format("%.2f", 3.14159)
来源：http://sv.shxzskj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ew.szxytkj.cn

Ruby: format("%.2f", 3.14159)
来源：http://eu.hahajie.cn

C#:   3.14159.ToString("F2")
来源：http://sd.haigaiapp.cn

[A22] 获取字符串长度
来源：http://tn.hnjuh.cn

Py:   len(s)
来源：http://ol.gzmigu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hb.newstarts.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ak.jctech888.com.cn

TS:   s.length
来源：http://ro.yuexingan06.cn

Java: s.length()
来源：http://dj.yuexingan06.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qs.colortex.cn

Ruby: s.length
来源：http://eu.shxzskj.cn

C#:   s.Length
来源：http://im.huixinmuqiang.cn

[A23] 大小写转换
来源：http://lx.colortex.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://jm.huixinmuqiang.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ac.newstarts.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ow.nicolike.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rl.yuntaijiaju.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://it.haigaiapp.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kw.chemitech.net.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://eg.colortex.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://em.wgjwhj.cn

[A24] 去除首尾空白
来源：http://nm.nszjky.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jl.shtwfgs.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fw.shxzukj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yl.521024.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://li.bookmarksfly.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://px.hnjuh.cn

Go:   strings.TrimSpace(s)
来源：http://zi.panjiajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nw.jctech888.com.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kl.bjjhwx.cn

[A25] 字符串比较
来源：http://fy.lnxyls.cn

Py:   s1 == s2; s1 != s2
来源：http://dz.colortex.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fo.newstarts.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tj.shxzukj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rm.yuexingan06.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xu.9csxet.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ww.hahajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://uu.asd995.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sa.nszjky.cn

[A26] 类型转换总览
来源：http://yr.shxzukj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ht.hahajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zz.panjiajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dx.szsharing.cn

TS:   Number() String() Boolean() x as number
来源：http://au.yuntaijiaju.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ad.shxzskj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://py.bookmarksfly.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ie.panjiajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://iv.newstarts.cn

================================================================================
来源：http://lc.521024.cn

B. 流程控制
来源：http://lt.gzmigu.cn

================================================================================
来源：http://ky.shxzskj.cn

[B01] 条件判断 if / else
来源：http://lz.9csxet.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vg.newstarts.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gd.bookmarksfly.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gi.shtwfgs.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mj.huixinmuqiang.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://zr.szxytkj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://up.jctech888.com.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xa.chemitech.net.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kz.shxzskj.cn

[B02] 多分支 else if / elif
来源：http://rw.9csxet.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yg.jianghongdianzi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ui.nszjky.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pq.bookmarksfly.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ox.521024.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pe.jianghongdianzi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xy.panjiajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ku.chemitech.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fi.szxytkj.cn

[B03] switch / match / case
来源：http://sp.szxytkj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wr.muxihuayi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ot.yuntaijiaju.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vp.bookmarksfly.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://im.muxihuayi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://am.521024.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bm.hahajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xx.shtwfgs.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zm.shxzukj.cn

[B04] for 计数循环
来源：http://xu.jianghongdianzi.cn

Py:   for i in range(10): print(i)
来源：http://cw.muxihuayi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://co.huixiangedu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sf.521024.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mo.bjjhwx.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cz.yuexingan06.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bh.asd995.cn

Ruby: 10.times { |i| puts i }
来源：http://rr.colortex.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ws.yuntaijiaju.cn

[B05] 遍历数组 / 列表
来源：http://lg.nszjky.cn

Py:   for item in arr: print(item)
来源：http://ey.colortex.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vj.bookmarksfly.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wj.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ao.szxytkj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yj.szxytkj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ng.hahajie.cn

Ruby: arr.each { |item| puts item }
来源：http://js.newstarts.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qg.yuexingan06.cn

[B06] 遍历字典 / 对象
来源：http://db.szxytkj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://dx.newstarts.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jb.nszjky.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lq.bjjhwx.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lp.chemitech.net.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gw.yuntaijiaju.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bo.newstarts.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rz.shtwfgs.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ay.bjjhwx.cn

[B07] while 循环
来源：http://am.lnxyls.cn

Py:   while i < 10: i += 1
来源：http://hc.hnjuh.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wo.hahajie.cn

JS:   while (i < 10) { i++; }
来源：http://yk.panjiajie.cn

TS:   while (i < 10) { i++; }
来源：http://ix.shxzskj.cn

Java: while (i < 10) { i++; }
来源：http://lx.huixiangedu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pn.shtwfgs.cn

Ruby: while i < 10; i += 1; end
来源：http://dd.wgjwhj.cn

C#:   while (i < 10) { i++; }
来源：http://ju.asd995.cn

[B08] do-while（至少执行一次）
来源：http://sa.shtwfgs.cn

Py:   # 无 do-while：用 while True + break
来源：http://fw.yuexingan06.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mo.lnxyls.cn

JS:   do { i++; } while (i < 10);
来源：http://mg.muxihuayi.cn

TS:   do { i++; } while (i < 10);
来源：http://ej.521024.cn

Java: do { i++; } while (i < 10);
来源：http://pb.nszjky.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://pn.bookmarksfly.cn

Ruby: begin; i += 1; end while i < 10
来源：http://sd.gzmigu.cn

C#:   do { i++; } while (i < 10);
来源：http://ec.shxzukj.cn

[B09] break 与 continue
来源：http://at.wgjwhj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tl.szsharing.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nn.shxzukj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ek.nszjky.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zr.lnxyls.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sl.haigaiapp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cm.lnxyls.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fx.huanxung.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lu.szxytkj.cn

[B10] 遍历同时拿索引
来源：http://yx.huanxung.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mv.9csxet.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gt.hnjuh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lx.colortex.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pm.shtwfgs.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zy.lnxyls.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dq.newstarts.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lq.nicolike.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sj.bjjhwx.cn

[B11] 生成数字序列 / 区间
来源：http://bz.shxzukj.cn

Py:   list(range(0, 10, 2))
来源：http://zz.shxzukj.cn

PHP:  range(0, 10, 2);
来源：http://km.asd995.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zl.nicolike.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pj.wgjwhj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://os.nicolike.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jd.huixinmuqiang.cn

Ruby: (0...10).step(2).to_a
来源：http://zd.gzmigu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jf.szxytkj.cn

[B12] 跳出多层循环
来源：http://at.szsharing.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://se.jianghongdianzi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://eg.hnjuh.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dm.yuexingan06.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dz.nicolike.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sw.9csxet.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mt.yuntaijiaju.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ls.bookmarksfly.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hu.gzmigu.cn

[B13] 判断是否为数字
来源：http://qm.shtwfgs.cn

Py:   isinstance(x, (int, float))
来源：http://om.nicolike.cn

PHP:  is_numeric($x)
来源：http://nb.9csxet.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fn.jianghongdianzi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bo.bjjhwx.cn

Java: x instanceof Number
来源：http://ck.hahajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://th.gzmigu.cn

Ruby: x.is_a?(Numeric)
来源：http://jr.huixiangedu.cn

C#:   x is int or double or decimal
来源：http://wx.nicolike.cn

[B14] 判断值是否在集合内
来源：http://sm.chemitech.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uh.asd995.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wi.haigaiapp.cn

JS:   [1, 2, 3].includes(x)
来源：http://fx.bjjhwx.cn

TS:   [1, 2, 3].includes(x)
来源：http://xk.colortex.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://up.chemitech.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xr.jianghongdianzi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ig.hahajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vg.wgjwhj.cn

[B15] 布尔运算与取反
来源：http://bk.shtwfgs.cn

Py:   a and b or not c
来源：http://xx.hnjuh.cn

PHP:  $a && $b || !$c
来源：http://oe.chemitech.net.cn

JS:   a && b || !c
来源：http://mu.jctech888.com.cn

TS:   a && b || !c
来源：http://hu.yuexingan06.cn

Java: a && b || !c
来源：http://sj.szsharing.cn

Go:   a && b || !c
来源：http://nf.asd995.cn

Ruby: a && b || !c
来源：http://gd.shxzukj.cn

C#:   a && b || !c
来源：http://bz.hahajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gr.jctech888.com.cn

Py:   if not data: return
来源：http://qp.haigaiapp.cn

PHP:  if (!$data) { return; }
来源：http://lf.yuexingan06.cn

JS:   if (!data) return;
来源：http://mn.gzmigu.cn

TS:   if (!data) return;
来源：http://zs.newstarts.cn

Java: if (data == null) return;
来源：http://fm.hnjuh.cn

Go:   if data == nil { return }
来源：http://qp.hahajie.cn

Ruby: return if data.nil?
来源：http://hw.jctech888.com.cn

C#:   if (data == null) return;
来源：http://hr.bjjhwx.cn

================================================================================
来源：http://ya.huixinmuqiang.cn

C. 函数与作用域
来源：http://bx.huixiangedu.cn

================================================================================
来源：http://ir.huanxung.cn

[C01] 定义函数
来源：http://to.521024.cn

Py:   def add(a, b): return a + b
来源：http://cg.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cu.hnjuh.cn

JS:   function add(a, b) { return a + b; }
来源：http://ch.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ot.wgjwhj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lc.huixiangedu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ac.shtwfgs.cn

Ruby: def add(a, b); a + b; end
来源：http://qa.gzmigu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ql.shtwfgs.cn

[C02] 默认参数
来源：http://iq.yuexingan06.cn

Py:   def greet(name="World"): return name
来源：http://lr.yuexingan06.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://js.bjjhwx.cn

JS:   function greet(name = "World") { return name; }
来源：http://ip.chemitech.net.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://de.lnxyls.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ho.lnxyls.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nn.nszjky.cn

Ruby: def greet(name = "World") = name
来源：http://yk.newstarts.cn

C#:   string Greet(string name = "World") => name;
来源：http://ah.shxzukj.cn

[C03] 可变参数
来源：http://gq.szxytkj.cn

Py:   def total(*args): return sum(args)
来源：http://jn.panjiajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ux.shxzskj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dd.chemitech.net.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pu.nszjky.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ar.muxihuayi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ru.bookmarksfly.cn

Ruby: def total(*nums); nums.sum; end
来源：http://kd.shtwfgs.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://om.jctech888.com.cn

[C04] 命名参数 / 关键字参数
来源：http://lz.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sb.gzmigu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yc.newstarts.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tv.szxytkj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fu.muxihuayi.cn

Java: // 无：用 Builder 模式或 record
来源：http://ek.hnjuh.cn

Go:   // 无：用配置结构体参数
来源：http://yx.nicolike.cn

Ruby: f(a: 1, b: 2)
来源：http://xr.gzmigu.cn

C#:   f(a: 1, b: 2)
来源：http://tr.lnxyls.cn

[C05] 返回多个值
来源：http://yb.muxihuayi.cn

Py:   return a, b
来源：http://io.newstarts.cn

PHP:  return [$a, $b];
来源：http://je.bjjhwx.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://sb.shxzskj.cn

TS:   return { a, b };
来源：http://gy.shxzskj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cy.huanxung.cn

Go:   return a, b
来源：http://dq.muxihuayi.cn

Ruby: return a, b
来源：http://dq.panjiajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://rs.wgjwhj.cn

[C06] 匿名函数 / lambda
来源：http://tk.yuexingan06.cn

Py:   square = lambda x: x * x
来源：http://ei.huixiangedu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://yh.panjiajie.cn

JS:   const square = x => x * x;
来源：http://kg.shxzukj.cn

TS:   const square = (x: number): number => x * x;
来源：http://by.hahajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hw.lnxyls.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zn.gzmigu.cn

Ruby: square = ->(x) { x * x }
来源：http://yc.shtwfgs.cn

C#:   Func<int, int> square = x => x * x;
来源：http://eu.jianghongdianzi.cn

[C07] 把函数作为参数传入
来源：http://uq.shxzukj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sg.szsharing.cn

PHP:  array_map("strtoupper", $arr);
来源：http://uq.lnxyls.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fo.szxytkj.cn

TS:   arr.map(String)
来源：http://bc.521024.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vd.hnjuh.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sq.wgjwhj.cn

Ruby: arr.map(&:upcase)
来源：http://xb.hahajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://kg.haigaiapp.cn

[C08] 闭包
来源：http://zc.521024.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kp.gzmigu.cn


<!-- 参考信息 -->