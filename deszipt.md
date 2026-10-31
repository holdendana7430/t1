代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://xj.jianghongdianzi.cn

Py:   ord("A"); chr(65)
来源：http://cg.yuexingan06.cn

PHP:  ord("A"); chr(65)
来源：http://ke.chemitech.net.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xb.panjiajie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lq.yuexingan06.cn

Java: (int) 'A'; (char) 65
来源：http://wf.bjjhwx.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hk.huixinmuqiang.cn

Ruby: "A".ord; 65.chr
来源：http://oq.hnjuh.cn

C#:   (int)'A'; (char)65
来源：http://ld.521024.cn

[A19] 交换两个变量
来源：http://nv.shxzskj.cn

Py:   a, b = b, a
来源：http://zg.chemitech.net.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://lg.yuexingan06.cn

JS:   [a, b] = [b, a];
来源：http://ei.szxytkj.cn

TS:   [a, b] = [b, a];
来源：http://op.asd995.cn

Java: int t = a; a = b; b = t;
来源：http://fv.muxihuayi.cn

Go:   a, b = b, a
来源：http://vb.huixiangedu.cn

Ruby: a, b = b, a
来源：http://yw.haigaiapp.cn

C#:   (a, b) = (b, a);
来源：http://ab.szxytkj.cn

[A20] 读取标准输入
来源：http://ol.asd995.cn

Py:   name = input("请输入：")
来源：http://oe.shxzskj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://sq.lnxyls.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ns.jctech888.com.cn

TS:   // Node.js：readline 模块
来源：http://bw.asd995.cn

Java: new Scanner(System.in).nextLine()
来源：http://qt.lnxyls.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://yw.9csxet.cn

Ruby: gets.chomp
来源：http://wr.chemitech.net.cn

C#:   Console.ReadLine();
来源：http://ox.yuexingan06.cn

[A21] 保留指定小数位输出
来源：http://ua.lnxyls.cn

Py:   f"{3.14159:.2f}"
来源：http://yh.bookmarksfly.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mx.shxzukj.cn

JS:   (3.14159).toFixed(2)
来源：http://jp.huanxung.cn

TS:   (3.14159).toFixed(2)
来源：http://wj.jctech888.com.cn

Java: String.format("%.2f", 3.14159)
来源：http://jp.nicolike.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qc.shtwfgs.cn

Ruby: format("%.2f", 3.14159)
来源：http://ty.yuexingan06.cn

C#:   3.14159.ToString("F2")
来源：http://tq.huanxung.cn

[A22] 获取字符串长度
来源：http://vn.chemitech.net.cn

Py:   len(s)
来源：http://af.colortex.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yd.huanxung.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ii.panjiajie.cn

TS:   s.length
来源：http://oz.huixinmuqiang.cn

Java: s.length()
来源：http://tq.yuexingan06.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://oo.newstarts.cn

Ruby: s.length
来源：http://ow.9csxet.cn

C#:   s.Length
来源：http://ya.nicolike.cn

[A23] 大小写转换
来源：http://aw.haigaiapp.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ex.chemitech.net.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yj.szxytkj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rj.muxihuayi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ka.shxzskj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rd.521024.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ve.yuexingan06.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://sa.haigaiapp.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://hf.jianghongdianzi.cn

[A24] 去除首尾空白
来源：http://wd.yuexingan06.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lw.huanxung.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bv.huanxung.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vt.hnjuh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kg.shxzskj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://eg.yuexingan06.cn

Go:   strings.TrimSpace(s)
来源：http://uc.9csxet.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ap.521024.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jl.hnjuh.cn

[A25] 字符串比较
来源：http://jp.521024.cn

Py:   s1 == s2; s1 != s2
来源：http://te.asd995.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hn.haigaiapp.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://uw.szsharing.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qz.9csxet.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ea.jianghongdianzi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qh.hahajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://lh.nicolike.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xw.szxytkj.cn

[A26] 类型转换总览
来源：http://zk.wgjwhj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zb.colortex.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xw.szsharing.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wz.hahajie.cn

TS:   Number() String() Boolean() x as number
来源：http://na.asd995.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://uv.szsharing.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ck.haigaiapp.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rr.hahajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wn.jianghongdianzi.cn

================================================================================
来源：http://zd.colortex.cn

B. 流程控制
来源：http://ej.hahajie.cn

================================================================================
来源：http://xd.nszjky.cn

[B01] 条件判断 if / else
来源：http://ib.shtwfgs.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ez.bjjhwx.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://no.haigaiapp.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jg.shxzukj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qi.huanxung.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xz.newstarts.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pf.szsharing.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sb.muxihuayi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lb.huixinmuqiang.cn

[B02] 多分支 else if / elif
来源：http://rp.szxytkj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ln.colortex.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nh.chemitech.net.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ze.huanxung.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ql.wgjwhj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://am.jctech888.com.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zn.nicolike.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://px.huixiangedu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ft.9csxet.cn

[B03] switch / match / case
来源：http://tt.szsharing.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fo.wgjwhj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qr.bookmarksfly.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fw.haigaiapp.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tw.bookmarksfly.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zf.hahajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nd.asd995.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ik.jianghongdianzi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://id.jctech888.com.cn

[B04] for 计数循环
来源：http://po.521024.cn

Py:   for i in range(10): print(i)
来源：http://xl.bookmarksfly.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hu.huixinmuqiang.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://la.chemitech.net.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tj.colortex.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ug.wgjwhj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rg.bjjhwx.cn

Ruby: 10.times { |i| puts i }
来源：http://re.huixiangedu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ss.huanxung.cn

[B05] 遍历数组 / 列表
来源：http://to.muxihuayi.cn

Py:   for item in arr: print(item)
来源：http://oi.nicolike.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rv.gzmigu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://oc.hahajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://vp.jianghongdianzi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ra.nszjky.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mo.shxzukj.cn

Ruby: arr.each { |item| puts item }
来源：http://aq.jctech888.com.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vk.szxytkj.cn

[B06] 遍历字典 / 对象
来源：http://en.bjjhwx.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://yr.huanxung.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ik.yuexingan06.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fd.haigaiapp.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nv.nszjky.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qt.nicolike.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ie.newstarts.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lw.yuexingan06.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://uk.shxzukj.cn

[B07] while 循环
来源：http://rc.hahajie.cn

Py:   while i < 10: i += 1
来源：http://yo.colortex.cn

PHP:  while ($i < 10) { $i++; }
来源：http://aj.huixiangedu.cn

JS:   while (i < 10) { i++; }
来源：http://mf.colortex.cn

TS:   while (i < 10) { i++; }
来源：http://iz.yuntaijiaju.cn

Java: while (i < 10) { i++; }
来源：http://ab.jctech888.com.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qg.9csxet.cn

Ruby: while i < 10; i += 1; end
来源：http://sg.szxytkj.cn

C#:   while (i < 10) { i++; }
来源：http://hh.nicolike.cn

[B08] do-while（至少执行一次）
来源：http://oq.chemitech.net.cn

Py:   # 无 do-while：用 while True + break
来源：http://nb.huanxung.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zn.wgjwhj.cn

JS:   do { i++; } while (i < 10);
来源：http://hx.hnjuh.cn

TS:   do { i++; } while (i < 10);
来源：http://js.nszjky.cn

Java: do { i++; } while (i < 10);
来源：http://hb.hnjuh.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://rk.huixinmuqiang.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ly.hnjuh.cn

C#:   do { i++; } while (i < 10);
来源：http://bd.colortex.cn

[B09] break 与 continue
来源：http://in.muxihuayi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nj.huixiangedu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wo.panjiajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vi.shxzukj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gf.szxytkj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cd.shxzskj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sg.yuexingan06.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hl.9csxet.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tv.lnxyls.cn

[B10] 遍历同时拿索引
来源：http://ve.haigaiapp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zk.jianghongdianzi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://da.muxihuayi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ak.nszjky.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ip.bjjhwx.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nt.lnxyls.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ek.colortex.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ra.szsharing.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://af.panjiajie.cn

[B11] 生成数字序列 / 区间
来源：http://kw.wgjwhj.cn

Py:   list(range(0, 10, 2))
来源：http://tn.huanxung.cn

PHP:  range(0, 10, 2);
来源：http://fj.521024.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bw.szxytkj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bb.haigaiapp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mq.newstarts.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kc.nicolike.cn

Ruby: (0...10).step(2).to_a
来源：http://ip.huixinmuqiang.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://eb.bjjhwx.cn

[B12] 跳出多层循环
来源：http://pj.gzmigu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://va.muxihuayi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ug.9csxet.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kp.newstarts.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rm.lnxyls.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cj.colortex.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fd.chemitech.net.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zp.colortex.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nn.wgjwhj.cn

[B13] 判断是否为数字
来源：http://ma.chemitech.net.cn

Py:   isinstance(x, (int, float))
来源：http://dp.nicolike.cn

PHP:  is_numeric($x)
来源：http://kf.jianghongdianzi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ru.muxihuayi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yy.nicolike.cn

Java: x instanceof Number
来源：http://nh.hahajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://et.huanxung.cn

Ruby: x.is_a?(Numeric)
来源：http://qm.bjjhwx.cn

C#:   x is int or double or decimal
来源：http://rw.jctech888.com.cn

[B14] 判断值是否在集合内
来源：http://kl.9csxet.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gv.huixiangedu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cu.hahajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://zs.chemitech.net.cn

TS:   [1, 2, 3].includes(x)
来源：http://qx.yuntaijiaju.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hb.huanxung.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yg.shxzukj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://nl.muxihuayi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nl.wgjwhj.cn

[B15] 布尔运算与取反
来源：http://mp.hnjuh.cn

Py:   a and b or not c
来源：http://zt.asd995.cn

PHP:  $a && $b || !$c
来源：http://qw.bookmarksfly.cn

JS:   a && b || !c
来源：http://ms.bookmarksfly.cn

TS:   a && b || !c
来源：http://eo.hahajie.cn

Java: a && b || !c
来源：http://ti.521024.cn

Go:   a && b || !c
来源：http://fl.nszjky.cn

Ruby: a && b || !c
来源：http://nh.bookmarksfly.cn

C#:   a && b || !c
来源：http://xm.szxytkj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fd.lnxyls.cn

Py:   if not data: return
来源：http://th.wgjwhj.cn

PHP:  if (!$data) { return; }
来源：http://ld.jianghongdianzi.cn

JS:   if (!data) return;
来源：http://tf.colortex.cn

TS:   if (!data) return;
来源：http://mb.szsharing.cn

Java: if (data == null) return;
来源：http://ht.hahajie.cn

Go:   if data == nil { return }
来源：http://kx.bookmarksfly.cn

Ruby: return if data.nil?
来源：http://au.muxihuayi.cn

C#:   if (data == null) return;
来源：http://qy.jctech888.com.cn

================================================================================
来源：http://xz.panjiajie.cn

C. 函数与作用域
来源：http://vg.huixinmuqiang.cn

================================================================================
来源：http://od.521024.cn

[C01] 定义函数
来源：http://by.panjiajie.cn

Py:   def add(a, b): return a + b
来源：http://em.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lf.jianghongdianzi.cn

JS:   function add(a, b) { return a + b; }
来源：http://bp.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wo.shxzskj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ef.shtwfgs.cn

Go:   func add(a, b int) int { return a + b }
来源：http://tz.shxzskj.cn

Ruby: def add(a, b); a + b; end
来源：http://aw.nszjky.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xt.lnxyls.cn

[C02] 默认参数
来源：http://ao.panjiajie.cn

Py:   def greet(name="World"): return name
来源：http://ql.jctech888.com.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dx.gzmigu.cn

JS:   function greet(name = "World") { return name; }
来源：http://cj.nszjky.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://jq.bookmarksfly.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://pk.nicolike.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bq.panjiajie.cn

Ruby: def greet(name = "World") = name
来源：http://iw.jctech888.com.cn

C#:   string Greet(string name = "World") => name;
来源：http://ei.bookmarksfly.cn

[C03] 可变参数
来源：http://df.yuexingan06.cn

Py:   def total(*args): return sum(args)
来源：http://yb.shxzukj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ot.nszjky.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mq.huixiangedu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mj.haigaiapp.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qi.9csxet.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pn.szxytkj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pg.szxytkj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zy.hnjuh.cn

[C04] 命名参数 / 关键字参数
来源：http://qp.shtwfgs.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vg.huixinmuqiang.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://an.jctech888.com.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rq.lnxyls.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pd.bookmarksfly.cn

Java: // 无：用 Builder 模式或 record
来源：http://ai.9csxet.cn

Go:   // 无：用配置结构体参数
来源：http://tk.bjjhwx.cn

Ruby: f(a: 1, b: 2)
来源：http://xp.huanxung.cn

C#:   f(a: 1, b: 2)
来源：http://zz.huanxung.cn

[C05] 返回多个值
来源：http://nl.gzmigu.cn

Py:   return a, b
来源：http://wh.chemitech.net.cn

PHP:  return [$a, $b];
来源：http://co.haigaiapp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ux.shxzukj.cn

TS:   return { a, b };
来源：http://uh.gzmigu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bk.shxzskj.cn

Go:   return a, b
来源：http://at.yuexingan06.cn

Ruby: return a, b
来源：http://ir.9csxet.cn

C#:   return (a, b);              // ValueTuple
来源：http://fc.colortex.cn

[C06] 匿名函数 / lambda
来源：http://qf.yuntaijiaju.cn

Py:   square = lambda x: x * x
来源：http://kw.shtwfgs.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ri.jctech888.com.cn

JS:   const square = x => x * x;
来源：http://de.yuntaijiaju.cn

TS:   const square = (x: number): number => x * x;
来源：http://fa.shtwfgs.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ly.asd995.cn

Go:   sq := func(x int) int { return x * x }
来源：http://un.jianghongdianzi.cn

Ruby: square = ->(x) { x * x }
来源：http://mf.shxzskj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wc.panjiajie.cn

[C07] 把函数作为参数传入
来源：http://pq.shxzskj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tx.shtwfgs.cn

PHP:  array_map("strtoupper", $arr);
来源：http://tk.yuntaijiaju.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ma.muxihuayi.cn

TS:   arr.map(String)
来源：http://sh.nszjky.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rg.shtwfgs.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ie.gzmigu.cn

Ruby: arr.map(&:upcase)
来源：http://ow.wgjwhj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qs.gzmigu.cn

[C08] 闭包
来源：http://wa.hahajie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ki.wgjwhj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ic.szxytkj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://af.colortex.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://er.szxytkj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sm.huixiangedu.cn


<!-- 参考信息 -->