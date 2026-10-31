代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://te.nicolike.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://aa.521024.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kt.yuntaijiaju.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wq.nicolike.cn

[A18] 字符与 ASCII 码互转
来源：http://kb.lnxyls.cn

Py:   ord("A"); chr(65)
来源：http://md.szsharing.cn

PHP:  ord("A"); chr(65)
来源：http://zn.gzmigu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://td.hnjuh.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ki.9csxet.cn

Java: (int) 'A'; (char) 65
来源：http://dk.panjiajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ao.jctech888.com.cn

Ruby: "A".ord; 65.chr
来源：http://md.nicolike.cn

C#:   (int)'A'; (char)65
来源：http://oo.newstarts.cn

[A19] 交换两个变量
来源：http://wl.gzmigu.cn

Py:   a, b = b, a
来源：http://xb.huixinmuqiang.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ch.9csxet.cn

JS:   [a, b] = [b, a];
来源：http://kw.panjiajie.cn

TS:   [a, b] = [b, a];
来源：http://fz.huixinmuqiang.cn

Java: int t = a; a = b; b = t;
来源：http://lr.hnjuh.cn

Go:   a, b = b, a
来源：http://py.shxzukj.cn

Ruby: a, b = b, a
来源：http://gp.szsharing.cn

C#:   (a, b) = (b, a);
来源：http://jl.yuntaijiaju.cn

[A20] 读取标准输入
来源：http://tw.yuexingan06.cn

Py:   name = input("请输入：")
来源：http://iq.bjjhwx.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://yw.lnxyls.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fd.bjjhwx.cn

TS:   // Node.js：readline 模块
来源：http://mx.yuexingan06.cn

Java: new Scanner(System.in).nextLine()
来源：http://xo.hahajie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://sq.haigaiapp.cn

Ruby: gets.chomp
来源：http://px.jctech888.com.cn

C#:   Console.ReadLine();
来源：http://xn.bookmarksfly.cn

[A21] 保留指定小数位输出
来源：http://zc.colortex.cn

Py:   f"{3.14159:.2f}"
来源：http://xq.shxzukj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://oq.shtwfgs.cn

JS:   (3.14159).toFixed(2)
来源：http://oj.jctech888.com.cn

TS:   (3.14159).toFixed(2)
来源：http://wq.newstarts.cn

Java: String.format("%.2f", 3.14159)
来源：http://my.hnjuh.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ax.huixinmuqiang.cn

Ruby: format("%.2f", 3.14159)
来源：http://gg.huixinmuqiang.cn

C#:   3.14159.ToString("F2")
来源：http://dr.shtwfgs.cn

[A22] 获取字符串长度
来源：http://qq.huanxung.cn

Py:   len(s)
来源：http://bu.szxytkj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xi.colortex.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tn.521024.cn

TS:   s.length
来源：http://tq.bjjhwx.cn

Java: s.length()
来源：http://qe.yuntaijiaju.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kr.colortex.cn

Ruby: s.length
来源：http://ll.szsharing.cn

C#:   s.Length
来源：http://hg.panjiajie.cn

[A23] 大小写转换
来源：http://pm.9csxet.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://yi.yuntaijiaju.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vt.hnjuh.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://sq.yuexingan06.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lb.521024.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ts.szsharing.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xr.jianghongdianzi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ab.bjjhwx.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://of.huixiangedu.cn

[A24] 去除首尾空白
来源：http://ua.shxzukj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hj.szsharing.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://yw.shxzskj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://aa.bookmarksfly.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pg.muxihuayi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lf.huixinmuqiang.cn

Go:   strings.TrimSpace(s)
来源：http://rd.huanxung.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://we.panjiajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://me.szsharing.cn

[A25] 字符串比较
来源：http://ua.newstarts.cn

Py:   s1 == s2; s1 != s2
来源：http://at.muxihuayi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hl.chemitech.net.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pb.colortex.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bm.521024.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ig.muxihuayi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vx.panjiajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://eh.nszjky.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gu.huanxung.cn

[A26] 类型转换总览
来源：http://pt.hahajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://nr.nicolike.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://oq.szxytkj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://lb.yuexingan06.cn

TS:   Number() String() Boolean() x as number
来源：http://ob.jianghongdianzi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lb.chemitech.net.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ar.bjjhwx.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vj.nicolike.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nx.lnxyls.cn

================================================================================
来源：http://rf.chemitech.net.cn

B. 流程控制
来源：http://jz.nszjky.cn

================================================================================
来源：http://bo.hahajie.cn

[B01] 条件判断 if / else
来源：http://ic.lnxyls.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xz.9csxet.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hv.wgjwhj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xf.asd995.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://aq.haigaiapp.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://db.9csxet.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hm.panjiajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tn.haigaiapp.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ex.shtwfgs.cn

[B02] 多分支 else if / elif
来源：http://rg.yuntaijiaju.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pe.yuexingan06.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://te.newstarts.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://um.huanxung.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lo.asd995.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qg.chemitech.net.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://is.chemitech.net.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nw.shxzukj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mk.muxihuayi.cn

[B03] switch / match / case
来源：http://hn.newstarts.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yb.bookmarksfly.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ms.bjjhwx.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gn.521024.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ph.shtwfgs.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nx.huixinmuqiang.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rj.wgjwhj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nx.gzmigu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vz.panjiajie.cn

[B04] for 计数循环
来源：http://fz.bjjhwx.cn

Py:   for i in range(10): print(i)
来源：http://jy.9csxet.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yu.shxzukj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jm.huanxung.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ho.colortex.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gu.huixinmuqiang.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vk.yuntaijiaju.cn

Ruby: 10.times { |i| puts i }
来源：http://hf.panjiajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fi.jianghongdianzi.cn

[B05] 遍历数组 / 列表
来源：http://hp.shxzukj.cn

Py:   for item in arr: print(item)
来源：http://sw.jctech888.com.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bq.yuntaijiaju.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ay.9csxet.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://or.bookmarksfly.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lu.gzmigu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dp.9csxet.cn

Ruby: arr.each { |item| puts item }
来源：http://kg.shxzukj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yd.hahajie.cn

[B06] 遍历字典 / 对象
来源：http://rb.szsharing.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vz.yuexingan06.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mr.newstarts.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dy.bjjhwx.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://en.huanxung.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zm.bjjhwx.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fj.bookmarksfly.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ay.yuntaijiaju.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lp.bjjhwx.cn

[B07] while 循环
来源：http://qn.muxihuayi.cn

Py:   while i < 10: i += 1
来源：http://ll.newstarts.cn

PHP:  while ($i < 10) { $i++; }
来源：http://cn.huixinmuqiang.cn

JS:   while (i < 10) { i++; }
来源：http://vi.nszjky.cn

TS:   while (i < 10) { i++; }
来源：http://fn.huixiangedu.cn

Java: while (i < 10) { i++; }
来源：http://si.bookmarksfly.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cx.haigaiapp.cn

Ruby: while i < 10; i += 1; end
来源：http://sk.panjiajie.cn

C#:   while (i < 10) { i++; }
来源：http://xs.hahajie.cn

[B08] do-while（至少执行一次）
来源：http://wt.shxzskj.cn

Py:   # 无 do-while：用 while True + break
来源：http://gl.szxytkj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vu.huixinmuqiang.cn

JS:   do { i++; } while (i < 10);
来源：http://ci.newstarts.cn

TS:   do { i++; } while (i < 10);
来源：http://sg.hnjuh.cn

Java: do { i++; } while (i < 10);
来源：http://bw.nszjky.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bo.chemitech.net.cn

Ruby: begin; i += 1; end while i < 10
来源：http://gw.huixinmuqiang.cn

C#:   do { i++; } while (i < 10);
来源：http://kw.newstarts.cn

[B09] break 与 continue
来源：http://fa.jianghongdianzi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hs.bjjhwx.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dw.shxzskj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qi.bookmarksfly.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mm.jianghongdianzi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ul.521024.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vu.asd995.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bz.nszjky.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wu.panjiajie.cn

[B10] 遍历同时拿索引
来源：http://vy.panjiajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ng.szxytkj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mv.colortex.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bp.hahajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fd.bjjhwx.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://it.yuexingan06.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://za.shtwfgs.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fp.hahajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lb.shxzukj.cn

[B11] 生成数字序列 / 区间
来源：http://vu.muxihuayi.cn

Py:   list(range(0, 10, 2))
来源：http://zp.bookmarksfly.cn

PHP:  range(0, 10, 2);
来源：http://xr.muxihuayi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nn.shxzskj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vs.newstarts.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://iu.shxzukj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bh.asd995.cn

Ruby: (0...10).step(2).to_a
来源：http://qa.haigaiapp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yo.nicolike.cn

[B12] 跳出多层循环
来源：http://pw.huixiangedu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://kl.lnxyls.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ui.chemitech.net.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gj.9csxet.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hq.huixiangedu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://th.jianghongdianzi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pm.szsharing.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gi.nszjky.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://th.huixinmuqiang.cn

[B13] 判断是否为数字
来源：http://pn.jianghongdianzi.cn

Py:   isinstance(x, (int, float))
来源：http://dy.jctech888.com.cn

PHP:  is_numeric($x)
来源：http://xg.gzmigu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fq.wgjwhj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://un.jctech888.com.cn

Java: x instanceof Number
来源：http://it.asd995.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://to.gzmigu.cn

Ruby: x.is_a?(Numeric)
来源：http://jy.hnjuh.cn

C#:   x is int or double or decimal
来源：http://of.huixiangedu.cn

[B14] 判断值是否在集合内
来源：http://ae.521024.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://at.bookmarksfly.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://co.newstarts.cn

JS:   [1, 2, 3].includes(x)
来源：http://hr.jctech888.com.cn

TS:   [1, 2, 3].includes(x)
来源：http://mp.gzmigu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://mr.9csxet.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sp.shxzukj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rx.szxytkj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hd.hnjuh.cn

[B15] 布尔运算与取反
来源：http://vj.colortex.cn

Py:   a and b or not c
来源：http://ea.szsharing.cn

PHP:  $a && $b || !$c
来源：http://gd.jianghongdianzi.cn

JS:   a && b || !c
来源：http://hx.shxzskj.cn

TS:   a && b || !c
来源：http://bk.shxzukj.cn

Java: a && b || !c
来源：http://me.huixinmuqiang.cn

Go:   a && b || !c
来源：http://ur.yuexingan06.cn

Ruby: a && b || !c
来源：http://fr.shxzskj.cn

C#:   a && b || !c
来源：http://nx.nszjky.cn

[B16] 卫语句：不满足条件提前返回
来源：http://rh.shxzukj.cn

Py:   if not data: return
来源：http://ds.haigaiapp.cn

PHP:  if (!$data) { return; }
来源：http://kz.gzmigu.cn

JS:   if (!data) return;
来源：http://un.shxzukj.cn

TS:   if (!data) return;
来源：http://aa.bookmarksfly.cn

Java: if (data == null) return;
来源：http://am.gzmigu.cn

Go:   if data == nil { return }
来源：http://jo.szsharing.cn

Ruby: return if data.nil?
来源：http://fc.hahajie.cn

C#:   if (data == null) return;
来源：http://ql.newstarts.cn

================================================================================
来源：http://vz.gzmigu.cn

C. 函数与作用域
来源：http://qq.gzmigu.cn

================================================================================
来源：http://ep.szsharing.cn

[C01] 定义函数
来源：http://un.huanxung.cn

Py:   def add(a, b): return a + b
来源：http://zp.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gc.yuntaijiaju.cn

JS:   function add(a, b) { return a + b; }
来源：http://xv.panjiajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dh.9csxet.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qc.haigaiapp.cn

Go:   func add(a, b int) int { return a + b }
来源：http://nw.nszjky.cn

Ruby: def add(a, b); a + b; end
来源：http://hs.asd995.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ov.newstarts.cn

[C02] 默认参数
来源：http://jx.shxzskj.cn

Py:   def greet(name="World"): return name
来源：http://bz.haigaiapp.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://my.yuntaijiaju.cn

JS:   function greet(name = "World") { return name; }
来源：http://xw.huixinmuqiang.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://kp.521024.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://sw.jianghongdianzi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rs.lnxyls.cn

Ruby: def greet(name = "World") = name
来源：http://pa.nicolike.cn

C#:   string Greet(string name = "World") => name;
来源：http://ki.hahajie.cn

[C03] 可变参数
来源：http://wu.panjiajie.cn

Py:   def total(*args): return sum(args)
来源：http://ej.lnxyls.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hs.huanxung.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gt.shxzskj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jm.nszjky.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ad.shtwfgs.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://iz.shxzukj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://an.muxihuayi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gk.wgjwhj.cn

[C04] 命名参数 / 关键字参数
来源：http://jg.shxzskj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kg.huixiangedu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://te.colortex.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rq.hnjuh.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dt.szxytkj.cn

Java: // 无：用 Builder 模式或 record
来源：http://ts.hnjuh.cn

Go:   // 无：用配置结构体参数
来源：http://yl.huanxung.cn

Ruby: f(a: 1, b: 2)
来源：http://dc.yuntaijiaju.cn

C#:   f(a: 1, b: 2)
来源：http://yt.nicolike.cn

[C05] 返回多个值
来源：http://mf.jctech888.com.cn

Py:   return a, b
来源：http://xi.huanxung.cn

PHP:  return [$a, $b];
来源：http://ry.hahajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ub.asd995.cn

TS:   return { a, b };
来源：http://vd.shxzukj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wn.shxzukj.cn

Go:   return a, b
来源：http://ji.jianghongdianzi.cn

Ruby: return a, b
来源：http://ba.nszjky.cn

C#:   return (a, b);              // ValueTuple
来源：http://pr.szxytkj.cn

[C06] 匿名函数 / lambda
来源：http://rj.shtwfgs.cn

Py:   square = lambda x: x * x
来源：http://yp.haigaiapp.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://et.hahajie.cn

JS:   const square = x => x * x;
来源：http://zl.panjiajie.cn

TS:   const square = (x: number): number => x * x;
来源：http://fr.szxytkj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tq.hnjuh.cn

Go:   sq := func(x int) int { return x * x }
来源：http://nj.bjjhwx.cn

Ruby: square = ->(x) { x * x }
来源：http://yg.szsharing.cn

C#:   Func<int, int> square = x => x * x;
来源：http://js.hahajie.cn

[C07] 把函数作为参数传入
来源：http://um.bookmarksfly.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ue.jianghongdianzi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vj.panjiajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rd.szxytkj.cn

TS:   arr.map(String)
来源：http://gw.shxzukj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ey.muxihuayi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ks.szxytkj.cn

Ruby: arr.map(&:upcase)
来源：http://rn.hahajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ny.muxihuayi.cn

[C08] 闭包
来源：http://ph.shxzukj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pm.521024.cn


<!-- 参考信息 -->