代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://to.jianghongdianzi.cn

Py:   ord("A"); chr(65)
来源：http://jt.9csxet.cn

PHP:  ord("A"); chr(65)
来源：http://sr.chemitech.net.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qb.huixinmuqiang.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fo.huixinmuqiang.cn

Java: (int) 'A'; (char) 65
来源：http://ne.haigaiapp.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ur.jctech888.com.cn

Ruby: "A".ord; 65.chr
来源：http://mo.shxzukj.cn

C#:   (int)'A'; (char)65
来源：http://rg.huixinmuqiang.cn

[A19] 交换两个变量
来源：http://ki.9csxet.cn

Py:   a, b = b, a
来源：http://mv.colortex.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://nz.521024.cn

JS:   [a, b] = [b, a];
来源：http://vb.wgjwhj.cn

TS:   [a, b] = [b, a];
来源：http://cu.huixinmuqiang.cn

Java: int t = a; a = b; b = t;
来源：http://em.huixinmuqiang.cn

Go:   a, b = b, a
来源：http://gq.chemitech.net.cn

Ruby: a, b = b, a
来源：http://vd.szsharing.cn

C#:   (a, b) = (b, a);
来源：http://wf.huanxung.cn

[A20] 读取标准输入
来源：http://gz.jctech888.com.cn

Py:   name = input("请输入：")
来源：http://zc.colortex.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://au.szsharing.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://am.jianghongdianzi.cn

TS:   // Node.js：readline 模块
来源：http://ti.bjjhwx.cn

Java: new Scanner(System.in).nextLine()
来源：http://zg.521024.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gb.huixinmuqiang.cn

Ruby: gets.chomp
来源：http://vs.521024.cn

C#:   Console.ReadLine();
来源：http://vh.yuexingan06.cn

[A21] 保留指定小数位输出
来源：http://am.chemitech.net.cn

Py:   f"{3.14159:.2f}"
来源：http://cu.jianghongdianzi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wx.colortex.cn

JS:   (3.14159).toFixed(2)
来源：http://cs.bookmarksfly.cn

TS:   (3.14159).toFixed(2)
来源：http://as.szsharing.cn

Java: String.format("%.2f", 3.14159)
来源：http://co.nszjky.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fe.shxzskj.cn

Ruby: format("%.2f", 3.14159)
来源：http://xf.jianghongdianzi.cn

C#:   3.14159.ToString("F2")
来源：http://rg.wgjwhj.cn

[A22] 获取字符串长度
来源：http://fs.chemitech.net.cn

Py:   len(s)
来源：http://ou.newstarts.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ky.bjjhwx.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://yj.yuntaijiaju.cn

TS:   s.length
来源：http://wj.gzmigu.cn

Java: s.length()
来源：http://em.yuexingan06.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://yr.huanxung.cn

Ruby: s.length
来源：http://fd.hahajie.cn

C#:   s.Length
来源：http://jv.521024.cn

[A23] 大小写转换
来源：http://nc.muxihuayi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://rm.bookmarksfly.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zb.chemitech.net.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nc.nicolike.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tj.wgjwhj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wl.hnjuh.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://db.shxzukj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://we.panjiajie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://hg.hahajie.cn

[A24] 去除首尾空白
来源：http://qz.shxzukj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://my.nszjky.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rb.shxzukj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://px.chemitech.net.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ku.nszjky.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kj.huanxung.cn

Go:   strings.TrimSpace(s)
来源：http://kw.shxzskj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gp.bookmarksfly.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qs.hnjuh.cn

[A25] 字符串比较
来源：http://mf.gzmigu.cn

Py:   s1 == s2; s1 != s2
来源：http://dy.wgjwhj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://it.gzmigu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yv.nszjky.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ef.huanxung.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wq.9csxet.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qv.shxzskj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rp.huanxung.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hp.szxytkj.cn

[A26] 类型转换总览
来源：http://vf.asd995.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wf.yuexingan06.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gt.szsharing.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jf.bookmarksfly.cn

TS:   Number() String() Boolean() x as number
来源：http://fj.shxzukj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ms.shxzukj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lo.yuntaijiaju.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://kh.bjjhwx.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ao.hnjuh.cn

================================================================================
来源：http://rh.haigaiapp.cn

B. 流程控制
来源：http://tr.yuexingan06.cn

================================================================================
来源：http://kn.hnjuh.cn

[B01] 条件判断 if / else
来源：http://ir.hahajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xx.huixinmuqiang.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://to.yuexingan06.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qr.hnjuh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://re.newstarts.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://op.haigaiapp.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cv.huanxung.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ae.huanxung.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://aw.gzmigu.cn

[B02] 多分支 else if / elif
来源：http://ym.lnxyls.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jz.hnjuh.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cp.bjjhwx.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://de.shtwfgs.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oq.nszjky.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vv.jianghongdianzi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://np.bjjhwx.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ia.wgjwhj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rz.shxzukj.cn

[B03] switch / match / case
来源：http://jt.asd995.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cq.lnxyls.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yl.jianghongdianzi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dk.shtwfgs.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ow.hnjuh.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://iq.newstarts.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ob.lnxyls.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xp.huanxung.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mi.panjiajie.cn

[B04] for 计数循环
来源：http://bw.szxytkj.cn

Py:   for i in range(10): print(i)
来源：http://za.yuexingan06.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://um.haigaiapp.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ky.yuexingan06.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xf.huixinmuqiang.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ls.yuntaijiaju.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wg.gzmigu.cn

Ruby: 10.times { |i| puts i }
来源：http://kk.asd995.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sf.nszjky.cn

[B05] 遍历数组 / 列表
来源：http://fg.chemitech.net.cn

Py:   for item in arr: print(item)
来源：http://on.shtwfgs.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dy.bookmarksfly.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dd.shxzukj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ln.asd995.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pw.lnxyls.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://oh.hnjuh.cn

Ruby: arr.each { |item| puts item }
来源：http://te.nszjky.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zm.hnjuh.cn

[B06] 遍历字典 / 对象
来源：http://li.wgjwhj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://iq.hahajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vv.shtwfgs.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pr.bjjhwx.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ij.nszjky.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rj.bjjhwx.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hb.521024.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://va.bjjhwx.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ag.nszjky.cn

[B07] while 循环
来源：http://fu.jianghongdianzi.cn

Py:   while i < 10: i += 1
来源：http://fa.huixinmuqiang.cn

PHP:  while ($i < 10) { $i++; }
来源：http://da.9csxet.cn

JS:   while (i < 10) { i++; }
来源：http://zt.gzmigu.cn

TS:   while (i < 10) { i++; }
来源：http://az.newstarts.cn

Java: while (i < 10) { i++; }
来源：http://tz.nszjky.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ac.szxytkj.cn

Ruby: while i < 10; i += 1; end
来源：http://le.huixinmuqiang.cn

C#:   while (i < 10) { i++; }
来源：http://uj.bjjhwx.cn

[B08] do-while（至少执行一次）
来源：http://sq.521024.cn

Py:   # 无 do-while：用 while True + break
来源：http://pq.hnjuh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://dl.newstarts.cn

JS:   do { i++; } while (i < 10);
来源：http://lg.muxihuayi.cn

TS:   do { i++; } while (i < 10);
来源：http://hk.chemitech.net.cn

Java: do { i++; } while (i < 10);
来源：http://fw.bjjhwx.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fl.gzmigu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://uy.muxihuayi.cn

C#:   do { i++; } while (i < 10);
来源：http://pg.muxihuayi.cn

[B09] break 与 continue
来源：http://ji.nszjky.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jw.huixiangedu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ju.hahajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wj.colortex.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cp.9csxet.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xn.nszjky.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pi.huanxung.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ki.bookmarksfly.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://td.hahajie.cn

[B10] 遍历同时拿索引
来源：http://mi.yuexingan06.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nh.bjjhwx.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jw.shtwfgs.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vy.chemitech.net.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fn.colortex.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vk.bookmarksfly.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yz.yuexingan06.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yy.jianghongdianzi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zs.huixinmuqiang.cn

[B11] 生成数字序列 / 区间
来源：http://xk.nszjky.cn

Py:   list(range(0, 10, 2))
来源：http://zo.9csxet.cn

PHP:  range(0, 10, 2);
来源：http://tz.huixinmuqiang.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ln.huixiangedu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pq.yuexingan06.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zx.lnxyls.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://um.huixiangedu.cn

Ruby: (0...10).step(2).to_a
来源：http://nw.yuntaijiaju.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dz.lnxyls.cn

[B12] 跳出多层循环
来源：http://jo.chemitech.net.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://vf.jctech888.com.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://sl.shxzskj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zk.shtwfgs.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ze.panjiajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hh.shxzukj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kb.521024.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ex.shxzukj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ld.huixinmuqiang.cn

[B13] 判断是否为数字
来源：http://ar.bjjhwx.cn

Py:   isinstance(x, (int, float))
来源：http://ve.521024.cn

PHP:  is_numeric($x)
来源：http://yk.bookmarksfly.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pt.bjjhwx.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vl.bjjhwx.cn

Java: x instanceof Number
来源：http://ah.huixinmuqiang.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ai.szsharing.cn

Ruby: x.is_a?(Numeric)
来源：http://md.colortex.cn

C#:   x is int or double or decimal
来源：http://dd.shxzskj.cn

[B14] 判断值是否在集合内
来源：http://jn.shxzukj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ta.jianghongdianzi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cm.jctech888.com.cn

JS:   [1, 2, 3].includes(x)
来源：http://qu.szxytkj.cn

TS:   [1, 2, 3].includes(x)
来源：http://dw.hahajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xd.yuexingan06.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hc.jctech888.com.cn

Ruby: [1, 2, 3].include?(x)
来源：http://bx.haigaiapp.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ik.jianghongdianzi.cn

[B15] 布尔运算与取反
来源：http://bf.9csxet.cn

Py:   a and b or not c
来源：http://bx.yuntaijiaju.cn

PHP:  $a && $b || !$c
来源：http://gw.panjiajie.cn

JS:   a && b || !c
来源：http://us.nicolike.cn

TS:   a && b || !c
来源：http://om.huanxung.cn

Java: a && b || !c
来源：http://ad.szsharing.cn

Go:   a && b || !c
来源：http://vd.chemitech.net.cn

Ruby: a && b || !c
来源：http://og.asd995.cn

C#:   a && b || !c
来源：http://kh.gzmigu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://tq.huixiangedu.cn

Py:   if not data: return
来源：http://mk.wgjwhj.cn

PHP:  if (!$data) { return; }
来源：http://sj.hahajie.cn

JS:   if (!data) return;
来源：http://df.yuexingan06.cn

TS:   if (!data) return;
来源：http://tw.bookmarksfly.cn

Java: if (data == null) return;
来源：http://uv.gzmigu.cn

Go:   if data == nil { return }
来源：http://my.jianghongdianzi.cn

Ruby: return if data.nil?
来源：http://gi.yuexingan06.cn

C#:   if (data == null) return;
来源：http://ho.szxytkj.cn

================================================================================
来源：http://aw.colortex.cn

C. 函数与作用域
来源：http://he.wgjwhj.cn

================================================================================
来源：http://kx.gzmigu.cn

[C01] 定义函数
来源：http://bj.colortex.cn

Py:   def add(a, b): return a + b
来源：http://nc.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ns.521024.cn

JS:   function add(a, b) { return a + b; }
来源：http://jc.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yd.shxzukj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://uz.jctech888.com.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vr.huanxung.cn

Ruby: def add(a, b); a + b; end
来源：http://sh.nszjky.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jw.panjiajie.cn

[C02] 默认参数
来源：http://oi.jctech888.com.cn

Py:   def greet(name="World"): return name
来源：http://xk.szsharing.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ag.chemitech.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://em.shxzskj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://et.panjiajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://se.huixiangedu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hl.szxytkj.cn

Ruby: def greet(name = "World") = name
来源：http://ai.gzmigu.cn

C#:   string Greet(string name = "World") => name;
来源：http://eg.hahajie.cn

[C03] 可变参数
来源：http://tv.bjjhwx.cn

Py:   def total(*args): return sum(args)
来源：http://uq.9csxet.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://af.nicolike.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qf.shtwfgs.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://le.521024.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xo.shxzskj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ny.hnjuh.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rv.huixiangedu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wk.chemitech.net.cn

[C04] 命名参数 / 关键字参数
来源：http://rd.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ts.szsharing.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ye.yuntaijiaju.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ss.521024.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fb.haigaiapp.cn

Java: // 无：用 Builder 模式或 record
来源：http://qt.szxytkj.cn

Go:   // 无：用配置结构体参数
来源：http://ml.gzmigu.cn

Ruby: f(a: 1, b: 2)
来源：http://zi.jctech888.com.cn

C#:   f(a: 1, b: 2)
来源：http://ny.bjjhwx.cn

[C05] 返回多个值
来源：http://ct.nszjky.cn

Py:   return a, b
来源：http://hp.huanxung.cn

PHP:  return [$a, $b];
来源：http://jl.szsharing.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fi.yuntaijiaju.cn

TS:   return { a, b };
来源：http://sp.huanxung.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ws.bjjhwx.cn

Go:   return a, b
来源：http://nh.521024.cn

Ruby: return a, b
来源：http://xo.huixinmuqiang.cn

C#:   return (a, b);              // ValueTuple
来源：http://ox.huixiangedu.cn

[C06] 匿名函数 / lambda
来源：http://lj.shxzukj.cn

Py:   square = lambda x: x * x
来源：http://io.gzmigu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://jw.9csxet.cn

JS:   const square = x => x * x;
来源：http://rl.bjjhwx.cn

TS:   const square = (x: number): number => x * x;
来源：http://fm.hahajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qp.chemitech.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://je.yuexingan06.cn

Ruby: square = ->(x) { x * x }
来源：http://ip.9csxet.cn

C#:   Func<int, int> square = x => x * x;
来源：http://vj.nicolike.cn

[C07] 把函数作为参数传入
来源：http://jn.gzmigu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ji.szxytkj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://mf.shtwfgs.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mm.shxzukj.cn

TS:   arr.map(String)
来源：http://vq.shtwfgs.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://is.szxytkj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xs.yuntaijiaju.cn

Ruby: arr.map(&:upcase)
来源：http://gj.jctech888.com.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cn.shtwfgs.cn

[C08] 闭包
来源：http://tp.shxzskj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zd.yuexingan06.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pk.jianghongdianzi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qq.shxzskj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ha.shtwfgs.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cb.9csxet.cn


<!-- 参考信息 -->