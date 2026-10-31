代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kq.newstarts.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://pc.shtwfgs.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ds.521024.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ih.panjiajie.cn

[A18] 字符与 ASCII 码互转
来源：http://rn.bookmarksfly.cn

Py:   ord("A"); chr(65)
来源：http://wi.muxihuayi.cn

PHP:  ord("A"); chr(65)
来源：http://rh.nszjky.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://au.nszjky.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pi.shtwfgs.cn

Java: (int) 'A'; (char) 65
来源：http://ap.huixinmuqiang.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://nl.shxzukj.cn

Ruby: "A".ord; 65.chr
来源：http://mq.asd995.cn

C#:   (int)'A'; (char)65
来源：http://sk.huanxung.cn

[A19] 交换两个变量
来源：http://me.haigaiapp.cn

Py:   a, b = b, a
来源：http://ia.wgjwhj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://er.hnjuh.cn

JS:   [a, b] = [b, a];
来源：http://hv.521024.cn

TS:   [a, b] = [b, a];
来源：http://lw.huanxung.cn

Java: int t = a; a = b; b = t;
来源：http://xl.shxzukj.cn

Go:   a, b = b, a
来源：http://cw.panjiajie.cn

Ruby: a, b = b, a
来源：http://nc.nicolike.cn

C#:   (a, b) = (b, a);
来源：http://jk.panjiajie.cn

[A20] 读取标准输入
来源：http://of.colortex.cn

Py:   name = input("请输入：")
来源：http://ye.szsharing.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ne.jctech888.com.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bv.nicolike.cn

TS:   // Node.js：readline 模块
来源：http://jc.muxihuayi.cn

Java: new Scanner(System.in).nextLine()
来源：http://xl.yuntaijiaju.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fq.shtwfgs.cn

Ruby: gets.chomp
来源：http://un.jianghongdianzi.cn

C#:   Console.ReadLine();
来源：http://oe.9csxet.cn

[A21] 保留指定小数位输出
来源：http://ft.muxihuayi.cn

Py:   f"{3.14159:.2f}"
来源：http://ke.hahajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ta.gzmigu.cn

JS:   (3.14159).toFixed(2)
来源：http://uz.nicolike.cn

TS:   (3.14159).toFixed(2)
来源：http://mg.chemitech.net.cn

Java: String.format("%.2f", 3.14159)
来源：http://nr.newstarts.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wg.asd995.cn

Ruby: format("%.2f", 3.14159)
来源：http://ga.asd995.cn

C#:   3.14159.ToString("F2")
来源：http://qb.muxihuayi.cn

[A22] 获取字符串长度
来源：http://hr.yuexingan06.cn

Py:   len(s)
来源：http://xa.szsharing.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nr.bookmarksfly.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://no.huixiangedu.cn

TS:   s.length
来源：http://am.yuntaijiaju.cn

Java: s.length()
来源：http://on.chemitech.net.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://iw.shxzskj.cn

Ruby: s.length
来源：http://iq.9csxet.cn

C#:   s.Length
来源：http://cy.9csxet.cn

[A23] 大小写转换
来源：http://bi.9csxet.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://oz.hnjuh.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kw.lnxyls.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zh.bookmarksfly.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ik.jctech888.com.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kj.shtwfgs.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yc.muxihuayi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://aj.szsharing.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://tp.szsharing.cn

[A24] 去除首尾空白
来源：http://yr.colortex.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ap.asd995.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nw.bookmarksfly.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ck.szxytkj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ah.jianghongdianzi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gp.9csxet.cn

Go:   strings.TrimSpace(s)
来源：http://lb.nszjky.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://li.shxzskj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nb.yuntaijiaju.cn

[A25] 字符串比较
来源：http://jj.yuntaijiaju.cn

Py:   s1 == s2; s1 != s2
来源：http://sx.jctech888.com.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ki.muxihuayi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ii.yuntaijiaju.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mk.panjiajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tu.szsharing.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wc.521024.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hc.yuntaijiaju.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ib.shxzskj.cn

[A26] 类型转换总览
来源：http://pf.gzmigu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xc.huixinmuqiang.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qk.bjjhwx.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yx.shtwfgs.cn

TS:   Number() String() Boolean() x as number
来源：http://cx.nicolike.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mq.colortex.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ok.yuntaijiaju.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://qh.nszjky.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pt.9csxet.cn

================================================================================
来源：http://bl.colortex.cn

B. 流程控制
来源：http://yk.lnxyls.cn

================================================================================
来源：http://me.nicolike.cn

[B01] 条件判断 if / else
来源：http://zj.panjiajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xd.9csxet.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ss.9csxet.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://so.huixiangedu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wp.521024.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://lz.szsharing.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gt.shxzskj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ps.9csxet.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sm.asd995.cn

[B02] 多分支 else if / elif
来源：http://ke.yuntaijiaju.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zi.bookmarksfly.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ft.9csxet.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sy.huanxung.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mt.nicolike.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://je.jctech888.com.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pt.shtwfgs.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yr.9csxet.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ki.yuexingan06.cn

[B03] switch / match / case
来源：http://gw.huixinmuqiang.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dk.9csxet.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dj.shxzukj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mf.yuntaijiaju.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://by.yuntaijiaju.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hx.colortex.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zs.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xs.yuntaijiaju.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qu.gzmigu.cn

[B04] for 计数循环
来源：http://pr.huixiangedu.cn

Py:   for i in range(10): print(i)
来源：http://bt.chemitech.net.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ax.shtwfgs.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oo.panjiajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yc.newstarts.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yl.asd995.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dt.shxzskj.cn

Ruby: 10.times { |i| puts i }
来源：http://pe.bookmarksfly.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wt.shxzukj.cn

[B05] 遍历数组 / 列表
来源：http://zh.hahajie.cn

Py:   for item in arr: print(item)
来源：http://yv.9csxet.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ol.szxytkj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ht.9csxet.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ln.haigaiapp.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xp.bookmarksfly.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fs.jctech888.com.cn

Ruby: arr.each { |item| puts item }
来源：http://qq.shxzskj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dx.huixinmuqiang.cn

[B06] 遍历字典 / 对象
来源：http://kc.szsharing.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://kg.panjiajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mj.gzmigu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vf.nicolike.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mx.wgjwhj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tf.huixiangedu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xe.yuntaijiaju.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ru.panjiajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://co.szsharing.cn

[B07] while 循环
来源：http://gz.haigaiapp.cn

Py:   while i < 10: i += 1
来源：http://tb.colortex.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ts.colortex.cn

JS:   while (i < 10) { i++; }
来源：http://xt.yuexingan06.cn

TS:   while (i < 10) { i++; }
来源：http://db.nszjky.cn

Java: while (i < 10) { i++; }
来源：http://db.yuexingan06.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mx.yuntaijiaju.cn

Ruby: while i < 10; i += 1; end
来源：http://wb.huanxung.cn

C#:   while (i < 10) { i++; }
来源：http://vx.panjiajie.cn

[B08] do-while（至少执行一次）
来源：http://tk.9csxet.cn

Py:   # 无 do-while：用 while True + break
来源：http://ky.haigaiapp.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ub.haigaiapp.cn

JS:   do { i++; } while (i < 10);
来源：http://fg.szsharing.cn

TS:   do { i++; } while (i < 10);
来源：http://gb.9csxet.cn

Java: do { i++; } while (i < 10);
来源：http://rl.huixiangedu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://uk.hnjuh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://kd.haigaiapp.cn

C#:   do { i++; } while (i < 10);
来源：http://cz.bookmarksfly.cn

[B09] break 与 continue
来源：http://io.hnjuh.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hv.9csxet.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xi.521024.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rj.bookmarksfly.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ii.gzmigu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ne.bookmarksfly.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fk.nicolike.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xz.yuexingan06.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ao.wgjwhj.cn

[B10] 遍历同时拿索引
来源：http://sa.huanxung.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fz.wgjwhj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dy.hahajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gc.hnjuh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ev.huixinmuqiang.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xp.newstarts.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cz.yuntaijiaju.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kf.shxzukj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zn.colortex.cn

[B11] 生成数字序列 / 区间
来源：http://xj.chemitech.net.cn

Py:   list(range(0, 10, 2))
来源：http://hk.haigaiapp.cn

PHP:  range(0, 10, 2);
来源：http://bv.newstarts.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sf.huanxung.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ke.haigaiapp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gf.gzmigu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ri.asd995.cn

Ruby: (0...10).step(2).to_a
来源：http://kp.521024.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zu.huixinmuqiang.cn

[B12] 跳出多层循环
来源：http://gs.gzmigu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ui.hahajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ib.yuexingan06.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://is.huixinmuqiang.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lu.asd995.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cr.nszjky.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bq.gzmigu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yx.wgjwhj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://oy.szxytkj.cn

[B13] 判断是否为数字
来源：http://fp.muxihuayi.cn

Py:   isinstance(x, (int, float))
来源：http://uv.panjiajie.cn

PHP:  is_numeric($x)
来源：http://mt.huixiangedu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yi.muxihuayi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://du.lnxyls.cn

Java: x instanceof Number
来源：http://yk.jctech888.com.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://le.bjjhwx.cn

Ruby: x.is_a?(Numeric)
来源：http://gu.colortex.cn

C#:   x is int or double or decimal
来源：http://dj.hahajie.cn

[B14] 判断值是否在集合内
来源：http://mr.521024.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fx.colortex.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ob.panjiajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://va.yuexingan06.cn

TS:   [1, 2, 3].includes(x)
来源：http://uv.huanxung.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://yo.chemitech.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gf.9csxet.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vr.hahajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lo.jianghongdianzi.cn

[B15] 布尔运算与取反
来源：http://yv.wgjwhj.cn

Py:   a and b or not c
来源：http://oh.muxihuayi.cn

PHP:  $a && $b || !$c
来源：http://lh.huanxung.cn

JS:   a && b || !c
来源：http://ag.wgjwhj.cn

TS:   a && b || !c
来源：http://ov.asd995.cn

Java: a && b || !c
来源：http://sd.asd995.cn

Go:   a && b || !c
来源：http://zy.szxytkj.cn

Ruby: a && b || !c
来源：http://ft.yuntaijiaju.cn

C#:   a && b || !c
来源：http://dk.shxzukj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://pp.hahajie.cn

Py:   if not data: return
来源：http://qo.asd995.cn

PHP:  if (!$data) { return; }
来源：http://tu.shtwfgs.cn

JS:   if (!data) return;
来源：http://ln.jctech888.com.cn

TS:   if (!data) return;
来源：http://kv.jianghongdianzi.cn

Java: if (data == null) return;
来源：http://jy.jianghongdianzi.cn

Go:   if data == nil { return }
来源：http://ey.jctech888.com.cn

Ruby: return if data.nil?
来源：http://vz.jianghongdianzi.cn

C#:   if (data == null) return;
来源：http://xp.asd995.cn

================================================================================
来源：http://qo.szxytkj.cn

C. 函数与作用域
来源：http://jr.9csxet.cn

================================================================================
来源：http://tx.521024.cn

[C01] 定义函数
来源：http://mg.newstarts.cn

Py:   def add(a, b): return a + b
来源：http://rp.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xl.huixinmuqiang.cn

JS:   function add(a, b) { return a + b; }
来源：http://yt.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mx.szsharing.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gn.bookmarksfly.cn

Go:   func add(a, b int) int { return a + b }
来源：http://kp.newstarts.cn

Ruby: def add(a, b); a + b; end
来源：http://co.szsharing.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ki.9csxet.cn

[C02] 默认参数
来源：http://ag.huixinmuqiang.cn

Py:   def greet(name="World"): return name
来源：http://gr.szxytkj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ur.chemitech.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://fn.gzmigu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://dt.gzmigu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wi.bjjhwx.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ih.jctech888.com.cn

Ruby: def greet(name = "World") = name
来源：http://un.huixinmuqiang.cn

C#:   string Greet(string name = "World") => name;
来源：http://vi.szsharing.cn

[C03] 可变参数
来源：http://eq.shtwfgs.cn

Py:   def total(*args): return sum(args)
来源：http://jy.shxzskj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dc.521024.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://um.521024.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ct.muxihuayi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://my.shxzskj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mk.panjiajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qk.hahajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ix.wgjwhj.cn

[C04] 命名参数 / 关键字参数
来源：http://ba.shtwfgs.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cv.szxytkj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tr.9csxet.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ue.hahajie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sh.newstarts.cn

Java: // 无：用 Builder 模式或 record
来源：http://ke.gzmigu.cn

Go:   // 无：用配置结构体参数
来源：http://we.9csxet.cn

Ruby: f(a: 1, b: 2)
来源：http://aq.521024.cn

C#:   f(a: 1, b: 2)
来源：http://oz.gzmigu.cn

[C05] 返回多个值
来源：http://ml.nszjky.cn

Py:   return a, b
来源：http://on.szsharing.cn

PHP:  return [$a, $b];
来源：http://zm.panjiajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://cr.9csxet.cn

TS:   return { a, b };
来源：http://dh.wgjwhj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yr.colortex.cn

Go:   return a, b
来源：http://bf.lnxyls.cn

Ruby: return a, b
来源：http://lu.yuexingan06.cn

C#:   return (a, b);              // ValueTuple
来源：http://vm.chemitech.net.cn

[C06] 匿名函数 / lambda
来源：http://tf.szsharing.cn

Py:   square = lambda x: x * x
来源：http://os.shxzskj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://up.hahajie.cn

JS:   const square = x => x * x;
来源：http://do.huanxung.cn

TS:   const square = (x: number): number => x * x;
来源：http://jb.chemitech.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kz.haigaiapp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ke.shxzukj.cn

Ruby: square = ->(x) { x * x }
来源：http://te.haigaiapp.cn

C#:   Func<int, int> square = x => x * x;
来源：http://db.newstarts.cn

[C07] 把函数作为参数传入
来源：http://oh.haigaiapp.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yn.nicolike.cn

PHP:  array_map("strtoupper", $arr);
来源：http://fs.yuntaijiaju.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jj.shxzskj.cn

TS:   arr.map(String)
来源：http://oz.hnjuh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pn.colortex.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rb.szxytkj.cn

Ruby: arr.map(&:upcase)
来源：http://wu.jianghongdianzi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mh.shtwfgs.cn

[C08] 闭包
来源：http://pt.hnjuh.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ak.muxihuayi.cn


<!-- 参考信息 -->