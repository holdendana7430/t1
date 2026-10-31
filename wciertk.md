代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://nw.hnjuh.cn

Py:   ord("A"); chr(65)
来源：http://hs.szxytkj.cn

PHP:  ord("A"); chr(65)
来源：http://qg.yuntaijiaju.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gt.bjjhwx.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fs.szsharing.cn

Java: (int) 'A'; (char) 65
来源：http://kh.lnxyls.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ef.haigaiapp.cn

Ruby: "A".ord; 65.chr
来源：http://do.jianghongdianzi.cn

C#:   (int)'A'; (char)65
来源：http://pw.szsharing.cn

[A19] 交换两个变量
来源：http://bl.asd995.cn

Py:   a, b = b, a
来源：http://xe.haigaiapp.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://xb.szsharing.cn

JS:   [a, b] = [b, a];
来源：http://hj.szxytkj.cn

TS:   [a, b] = [b, a];
来源：http://jk.panjiajie.cn

Java: int t = a; a = b; b = t;
来源：http://ef.gzmigu.cn

Go:   a, b = b, a
来源：http://sw.hnjuh.cn

Ruby: a, b = b, a
来源：http://nk.jianghongdianzi.cn

C#:   (a, b) = (b, a);
来源：http://mb.jianghongdianzi.cn

[A20] 读取标准输入
来源：http://sc.yuntaijiaju.cn

Py:   name = input("请输入：")
来源：http://ht.chemitech.net.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ah.jctech888.com.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://sa.bookmarksfly.cn

TS:   // Node.js：readline 模块
来源：http://gp.jianghongdianzi.cn

Java: new Scanner(System.in).nextLine()
来源：http://bp.haigaiapp.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://tq.nicolike.cn

Ruby: gets.chomp
来源：http://vh.asd995.cn

C#:   Console.ReadLine();
来源：http://lc.521024.cn

[A21] 保留指定小数位输出
来源：http://xa.nicolike.cn

Py:   f"{3.14159:.2f}"
来源：http://xn.hnjuh.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gz.hnjuh.cn

JS:   (3.14159).toFixed(2)
来源：http://eg.wgjwhj.cn

TS:   (3.14159).toFixed(2)
来源：http://aq.shxzskj.cn

Java: String.format("%.2f", 3.14159)
来源：http://xa.shtwfgs.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ti.lnxyls.cn

Ruby: format("%.2f", 3.14159)
来源：http://bc.521024.cn

C#:   3.14159.ToString("F2")
来源：http://wb.nszjky.cn

[A22] 获取字符串长度
来源：http://qr.nszjky.cn

Py:   len(s)
来源：http://fj.szxytkj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://po.colortex.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fi.szsharing.cn

TS:   s.length
来源：http://zk.muxihuayi.cn

Java: s.length()
来源：http://nh.huixinmuqiang.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kx.521024.cn

Ruby: s.length
来源：http://ac.newstarts.cn

C#:   s.Length
来源：http://vg.muxihuayi.cn

[A23] 大小写转换
来源：http://mr.shxzskj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://xc.szxytkj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mf.huanxung.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zp.bookmarksfly.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ue.huanxung.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lh.yuntaijiaju.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tc.huanxung.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://he.shtwfgs.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ib.newstarts.cn

[A24] 去除首尾空白
来源：http://kz.nicolike.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sk.lnxyls.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vb.wgjwhj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ns.yuexingan06.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fq.9csxet.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ok.colortex.cn

Go:   strings.TrimSpace(s)
来源：http://jd.gzmigu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fi.521024.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://na.hahajie.cn

[A25] 字符串比较
来源：http://cr.asd995.cn

Py:   s1 == s2; s1 != s2
来源：http://gi.nicolike.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pk.shxzukj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mw.shxzskj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://az.huixiangedu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://px.panjiajie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hm.gzmigu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://eo.lnxyls.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nn.gzmigu.cn

[A26] 类型转换总览
来源：http://zm.huixiangedu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pu.newstarts.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bo.nicolike.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://eh.lnxyls.cn

TS:   Number() String() Boolean() x as number
来源：http://re.wgjwhj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://az.jctech888.com.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.bookmarksfly.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://se.bookmarksfly.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://co.jctech888.com.cn

================================================================================
来源：http://hq.szxytkj.cn

B. 流程控制
来源：http://qc.bjjhwx.cn

================================================================================
来源：http://zv.huixinmuqiang.cn

[B01] 条件判断 if / else
来源：http://bk.szxytkj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vy.hnjuh.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ej.szxytkj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fl.jianghongdianzi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jo.lnxyls.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://wv.yuexingan06.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jq.muxihuayi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nq.huixiangedu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bw.hahajie.cn

[B02] 多分支 else if / elif
来源：http://wx.panjiajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fu.nicolike.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fy.jianghongdianzi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zl.huixinmuqiang.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ta.hahajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://co.gzmigu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fs.panjiajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uk.asd995.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mh.szsharing.cn

[B03] switch / match / case
来源：http://zu.huixinmuqiang.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://uq.muxihuayi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rf.huixiangedu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ma.shtwfgs.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qp.hahajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kz.shxzskj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://at.muxihuayi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://no.shxzukj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kt.huixinmuqiang.cn

[B04] for 计数循环
来源：http://zm.newstarts.cn

Py:   for i in range(10): print(i)
来源：http://so.chemitech.net.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rq.huanxung.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uw.newstarts.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pz.bjjhwx.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.haigaiapp.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ve.yuexingan06.cn

Ruby: 10.times { |i| puts i }
来源：http://ig.muxihuayi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jb.hnjuh.cn

[B05] 遍历数组 / 列表
来源：http://wg.huanxung.cn

Py:   for item in arr: print(item)
来源：http://mv.asd995.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ti.huanxung.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yh.9csxet.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://pg.asd995.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ah.wgjwhj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://aa.yuntaijiaju.cn

Ruby: arr.each { |item| puts item }
来源：http://pr.asd995.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://oq.jctech888.com.cn

[B06] 遍历字典 / 对象
来源：http://bs.chemitech.net.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://dl.huanxung.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ne.bookmarksfly.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nv.huixinmuqiang.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bi.colortex.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dh.hnjuh.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ra.huixinmuqiang.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dh.bookmarksfly.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://px.shxzukj.cn

[B07] while 循环
来源：http://by.nszjky.cn

Py:   while i < 10: i += 1
来源：http://mf.panjiajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://yd.hahajie.cn

JS:   while (i < 10) { i++; }
来源：http://jd.nicolike.cn

TS:   while (i < 10) { i++; }
来源：http://bc.gzmigu.cn

Java: while (i < 10) { i++; }
来源：http://ao.huanxung.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wv.yuntaijiaju.cn

Ruby: while i < 10; i += 1; end
来源：http://jq.chemitech.net.cn

C#:   while (i < 10) { i++; }
来源：http://hk.muxihuayi.cn

[B08] do-while（至少执行一次）
来源：http://gc.huixinmuqiang.cn

Py:   # 无 do-while：用 while True + break
来源：http://gf.lnxyls.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://rl.nicolike.cn

JS:   do { i++; } while (i < 10);
来源：http://wu.shtwfgs.cn

TS:   do { i++; } while (i < 10);
来源：http://lb.szxytkj.cn

Java: do { i++; } while (i < 10);
来源：http://qy.wgjwhj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://dt.bjjhwx.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fs.wgjwhj.cn

C#:   do { i++; } while (i < 10);
来源：http://zg.newstarts.cn

[B09] break 与 continue
来源：http://hg.huixiangedu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lu.hahajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pd.wgjwhj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pk.huixiangedu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xn.huixinmuqiang.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qp.colortex.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://uj.muxihuayi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fi.521024.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jr.bookmarksfly.cn

[B10] 遍历同时拿索引
来源：http://fs.asd995.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://by.521024.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xp.nicolike.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vu.jctech888.com.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sn.huixinmuqiang.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xy.shxzukj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tw.hahajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cz.shxzukj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qv.haigaiapp.cn

[B11] 生成数字序列 / 区间
来源：http://ud.asd995.cn

Py:   list(range(0, 10, 2))
来源：http://oh.yuntaijiaju.cn

PHP:  range(0, 10, 2);
来源：http://sx.9csxet.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bf.yuexingan06.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rw.hahajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dc.bjjhwx.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xd.gzmigu.cn

Ruby: (0...10).step(2).to_a
来源：http://kz.9csxet.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bo.huixinmuqiang.cn

[B12] 跳出多层循环
来源：http://nh.jctech888.com.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://lv.colortex.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ud.szsharing.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dz.colortex.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hq.gzmigu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zd.huixinmuqiang.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bc.9csxet.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qm.panjiajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zm.nicolike.cn

[B13] 判断是否为数字
来源：http://rn.yuexingan06.cn

Py:   isinstance(x, (int, float))
来源：http://tz.szsharing.cn

PHP:  is_numeric($x)
来源：http://eq.yuntaijiaju.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sd.huixinmuqiang.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ub.szxytkj.cn

Java: x instanceof Number
来源：http://my.chemitech.net.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://md.shtwfgs.cn

Ruby: x.is_a?(Numeric)
来源：http://aw.yuexingan06.cn

C#:   x is int or double or decimal
来源：http://sp.wgjwhj.cn

[B14] 判断值是否在集合内
来源：http://iy.9csxet.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ro.lnxyls.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xx.nszjky.cn

JS:   [1, 2, 3].includes(x)
来源：http://yo.wgjwhj.cn

TS:   [1, 2, 3].includes(x)
来源：http://zw.huanxung.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://jq.521024.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bk.shtwfgs.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ft.lnxyls.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ib.huixiangedu.cn

[B15] 布尔运算与取反
来源：http://fo.9csxet.cn

Py:   a and b or not c
来源：http://qu.haigaiapp.cn

PHP:  $a && $b || !$c
来源：http://zm.panjiajie.cn

JS:   a && b || !c
来源：http://rj.jianghongdianzi.cn

TS:   a && b || !c
来源：http://wy.szsharing.cn

Java: a && b || !c
来源：http://hk.9csxet.cn

Go:   a && b || !c
来源：http://az.521024.cn

Ruby: a && b || !c
来源：http://kq.gzmigu.cn

C#:   a && b || !c
来源：http://qt.newstarts.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xf.huanxung.cn

Py:   if not data: return
来源：http://kk.newstarts.cn

PHP:  if (!$data) { return; }
来源：http://ls.jctech888.com.cn

JS:   if (!data) return;
来源：http://hw.nicolike.cn

TS:   if (!data) return;
来源：http://vh.szsharing.cn

Java: if (data == null) return;
来源：http://vq.newstarts.cn

Go:   if data == nil { return }
来源：http://zj.9csxet.cn

Ruby: return if data.nil?
来源：http://py.chemitech.net.cn

C#:   if (data == null) return;
来源：http://lf.shxzukj.cn

================================================================================
来源：http://eh.asd995.cn

C. 函数与作用域
来源：http://qj.shxzukj.cn

================================================================================
来源：http://bs.jianghongdianzi.cn

[C01] 定义函数
来源：http://kq.nszjky.cn

Py:   def add(a, b): return a + b
来源：http://wa.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fb.nszjky.cn

JS:   function add(a, b) { return a + b; }
来源：http://jw.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fw.panjiajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://sb.shxzukj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ub.haigaiapp.cn

Ruby: def add(a, b); a + b; end
来源：http://co.nszjky.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uh.jctech888.com.cn

[C02] 默认参数
来源：http://yp.jianghongdianzi.cn

Py:   def greet(name="World"): return name
来源：http://tz.shxzskj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ig.hahajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://hl.yuexingan06.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ki.panjiajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wc.chemitech.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kh.bjjhwx.cn

Ruby: def greet(name = "World") = name
来源：http://ts.asd995.cn

C#:   string Greet(string name = "World") => name;
来源：http://kr.wgjwhj.cn

[C03] 可变参数
来源：http://us.521024.cn

Py:   def total(*args): return sum(args)
来源：http://nv.nszjky.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zf.szxytkj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fa.szsharing.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bm.szxytkj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wd.haigaiapp.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lz.nicolike.cn

Ruby: def total(*nums); nums.sum; end
来源：http://av.9csxet.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ld.jctech888.com.cn

[C04] 命名参数 / 关键字参数
来源：http://aq.521024.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nc.bookmarksfly.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ca.521024.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kg.nicolike.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wr.wgjwhj.cn

Java: // 无：用 Builder 模式或 record
来源：http://op.bjjhwx.cn

Go:   // 无：用配置结构体参数
来源：http://ww.9csxet.cn

Ruby: f(a: 1, b: 2)
来源：http://uh.muxihuayi.cn

C#:   f(a: 1, b: 2)
来源：http://ax.shxzskj.cn

[C05] 返回多个值
来源：http://kg.yuexingan06.cn

Py:   return a, b
来源：http://cs.asd995.cn

PHP:  return [$a, $b];
来源：http://ue.asd995.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://cl.colortex.cn

TS:   return { a, b };
来源：http://rl.yuexingan06.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ji.haigaiapp.cn

Go:   return a, b
来源：http://yk.szsharing.cn

Ruby: return a, b
来源：http://az.nicolike.cn

C#:   return (a, b);              // ValueTuple
来源：http://zi.haigaiapp.cn

[C06] 匿名函数 / lambda
来源：http://by.nicolike.cn

Py:   square = lambda x: x * x
来源：http://lo.hahajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://mk.huanxung.cn

JS:   const square = x => x * x;
来源：http://tj.yuntaijiaju.cn

TS:   const square = (x: number): number => x * x;
来源：http://rc.szxytkj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ss.huixinmuqiang.cn

Go:   sq := func(x int) int { return x * x }
来源：http://tb.wgjwhj.cn

Ruby: square = ->(x) { x * x }
来源：http://sl.colortex.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zz.9csxet.cn

[C07] 把函数作为参数传入
来源：http://wh.shtwfgs.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sf.newstarts.cn

PHP:  array_map("strtoupper", $arr);
来源：http://fc.9csxet.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://iv.9csxet.cn

TS:   arr.map(String)
来源：http://kx.lnxyls.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cd.nszjky.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kq.newstarts.cn

Ruby: arr.map(&:upcase)
来源：http://wz.bookmarksfly.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://zl.szsharing.cn

[C08] 闭包
来源：http://ij.szsharing.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lg.huanxung.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://el.newstarts.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fg.chemitech.net.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://le.jianghongdianzi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://li.gzmigu.cn


<!-- 参考信息 -->