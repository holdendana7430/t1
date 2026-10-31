代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://jy.haigaiapp.cn

Py:   ord("A"); chr(65)
来源：http://ux.muxihuayi.cn

PHP:  ord("A"); chr(65)
来源：http://va.wgjwhj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mx.szxytkj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fp.wgjwhj.cn

Java: (int) 'A'; (char) 65
来源：http://dp.huanxung.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jh.shxzskj.cn

Ruby: "A".ord; 65.chr
来源：http://gr.shxzukj.cn

C#:   (int)'A'; (char)65
来源：http://kv.bjjhwx.cn

[A19] 交换两个变量
来源：http://dx.bookmarksfly.cn

Py:   a, b = b, a
来源：http://vq.bjjhwx.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://nz.shtwfgs.cn

JS:   [a, b] = [b, a];
来源：http://mx.shxzskj.cn

TS:   [a, b] = [b, a];
来源：http://nh.yuexingan06.cn

Java: int t = a; a = b; b = t;
来源：http://mn.shxzskj.cn

Go:   a, b = b, a
来源：http://oq.huixiangedu.cn

Ruby: a, b = b, a
来源：http://gb.lnxyls.cn

C#:   (a, b) = (b, a);
来源：http://uf.shtwfgs.cn

[A20] 读取标准输入
来源：http://bf.newstarts.cn

Py:   name = input("请输入：")
来源：http://lz.nszjky.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://dy.gzmigu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lo.gzmigu.cn

TS:   // Node.js：readline 模块
来源：http://gl.yuntaijiaju.cn

Java: new Scanner(System.in).nextLine()
来源：http://no.lnxyls.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mq.jctech888.com.cn

Ruby: gets.chomp
来源：http://cs.wgjwhj.cn

C#:   Console.ReadLine();
来源：http://dt.bookmarksfly.cn

[A21] 保留指定小数位输出
来源：http://bg.521024.cn

Py:   f"{3.14159:.2f}"
来源：http://am.panjiajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kg.szxytkj.cn

JS:   (3.14159).toFixed(2)
来源：http://tf.nicolike.cn

TS:   (3.14159).toFixed(2)
来源：http://vb.haigaiapp.cn

Java: String.format("%.2f", 3.14159)
来源：http://ac.szsharing.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gk.hahajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://wg.gzmigu.cn

C#:   3.14159.ToString("F2")
来源：http://km.wgjwhj.cn

[A22] 获取字符串长度
来源：http://nh.bjjhwx.cn

Py:   len(s)
来源：http://cg.colortex.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://iu.szsharing.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ze.wgjwhj.cn

TS:   s.length
来源：http://pc.gzmigu.cn

Java: s.length()
来源：http://zk.huanxung.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xg.muxihuayi.cn

Ruby: s.length
来源：http://rg.chemitech.net.cn

C#:   s.Length
来源：http://zn.wgjwhj.cn

[A23] 大小写转换
来源：http://lq.huixiangedu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://yc.gzmigu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yx.jianghongdianzi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://my.muxihuayi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fd.yuexingan06.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ft.nszjky.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://eo.muxihuayi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nc.huixinmuqiang.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ix.muxihuayi.cn

[A24] 去除首尾空白
来源：http://zc.shtwfgs.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ph.gzmigu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mw.colortex.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ox.haigaiapp.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ly.huixinmuqiang.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://we.bjjhwx.cn

Go:   strings.TrimSpace(s)
来源：http://ff.haigaiapp.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zm.panjiajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mf.huixiangedu.cn

[A25] 字符串比较
来源：http://vw.chemitech.net.cn

Py:   s1 == s2; s1 != s2
来源：http://jt.bookmarksfly.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://eo.newstarts.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://sa.wgjwhj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pj.chemitech.net.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://iy.nicolike.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ix.gzmigu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://eh.yuntaijiaju.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://os.colortex.cn

[A26] 类型转换总览
来源：http://pf.nszjky.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://oa.chemitech.net.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mi.yuntaijiaju.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://he.huixinmuqiang.cn

TS:   Number() String() Boolean() x as number
来源：http://jp.szxytkj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://eg.muxihuayi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rp.hnjuh.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://bb.huixiangedu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xi.huixinmuqiang.cn

================================================================================
来源：http://ee.lnxyls.cn

B. 流程控制
来源：http://lc.huanxung.cn

================================================================================
来源：http://ge.szxytkj.cn

[B01] 条件判断 if / else
来源：http://uz.newstarts.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xs.szxytkj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://el.yuexingan06.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bo.nszjky.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gd.haigaiapp.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ky.huixinmuqiang.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hj.newstarts.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zb.nicolike.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://oa.wgjwhj.cn

[B02] 多分支 else if / elif
来源：http://zo.nszjky.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pm.panjiajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://df.nicolike.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mt.asd995.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sp.shxzukj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eb.nicolike.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hq.szxytkj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ne.jianghongdianzi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tm.jianghongdianzi.cn

[B03] switch / match / case
来源：http://xz.muxihuayi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qi.9csxet.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bc.shxzukj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://iz.shxzskj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sd.shxzukj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mi.jctech888.com.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pd.nszjky.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fi.shxzskj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gr.colortex.cn

[B04] for 计数循环
来源：http://lr.hnjuh.cn

Py:   for i in range(10): print(i)
来源：http://bi.haigaiapp.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fl.521024.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qs.521024.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://il.chemitech.net.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.jctech888.com.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ab.wgjwhj.cn

Ruby: 10.times { |i| puts i }
来源：http://zl.hnjuh.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lh.hahajie.cn

[B05] 遍历数组 / 列表
来源：http://iy.chemitech.net.cn

Py:   for item in arr: print(item)
来源：http://gd.9csxet.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gm.chemitech.net.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ej.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://jo.9csxet.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hx.haigaiapp.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://au.asd995.cn

Ruby: arr.each { |item| puts item }
来源：http://sg.colortex.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ok.huixinmuqiang.cn

[B06] 遍历字典 / 对象
来源：http://km.huixinmuqiang.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://py.muxihuayi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uc.shxzskj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ii.shtwfgs.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tt.wgjwhj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ul.shxzskj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cg.hahajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ic.jctech888.com.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wk.panjiajie.cn

[B07] while 循环
来源：http://nf.jctech888.com.cn

Py:   while i < 10: i += 1
来源：http://ul.nszjky.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xu.yuexingan06.cn

JS:   while (i < 10) { i++; }
来源：http://bl.gzmigu.cn

TS:   while (i < 10) { i++; }
来源：http://io.huixinmuqiang.cn

Java: while (i < 10) { i++; }
来源：http://my.nszjky.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xi.yuexingan06.cn

Ruby: while i < 10; i += 1; end
来源：http://yw.bookmarksfly.cn

C#:   while (i < 10) { i++; }
来源：http://fo.asd995.cn

[B08] do-while（至少执行一次）
来源：http://fo.jctech888.com.cn

Py:   # 无 do-while：用 while True + break
来源：http://em.yuexingan06.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://gm.bookmarksfly.cn

JS:   do { i++; } while (i < 10);
来源：http://pr.haigaiapp.cn

TS:   do { i++; } while (i < 10);
来源：http://lm.bjjhwx.cn

Java: do { i++; } while (i < 10);
来源：http://yu.panjiajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ra.nszjky.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wv.wgjwhj.cn

C#:   do { i++; } while (i < 10);
来源：http://nt.521024.cn

[B09] break 与 continue
来源：http://hd.huixiangedu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jr.shxzukj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ji.shxzskj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dx.nszjky.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vj.panjiajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wc.wgjwhj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ny.huanxung.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rk.shxzskj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ez.muxihuayi.cn

[B10] 遍历同时拿索引
来源：http://nz.yuntaijiaju.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cu.newstarts.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mi.haigaiapp.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pd.asd995.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tu.jctech888.com.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://am.panjiajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ec.shxzukj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://eo.shxzskj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sj.shxzukj.cn

[B11] 生成数字序列 / 区间
来源：http://sg.nszjky.cn

Py:   list(range(0, 10, 2))
来源：http://js.jianghongdianzi.cn

PHP:  range(0, 10, 2);
来源：http://gp.hnjuh.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ts.bookmarksfly.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://re.muxihuayi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rw.hnjuh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rw.bjjhwx.cn

Ruby: (0...10).step(2).to_a
来源：http://rc.hnjuh.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ba.colortex.cn

[B12] 跳出多层循环
来源：http://in.shtwfgs.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://qd.muxihuayi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://xr.wgjwhj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ni.bjjhwx.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ak.szsharing.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://al.jctech888.com.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fq.panjiajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tn.wgjwhj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pa.nicolike.cn

[B13] 判断是否为数字
来源：http://dy.521024.cn

Py:   isinstance(x, (int, float))
来源：http://ax.jianghongdianzi.cn

PHP:  is_numeric($x)
来源：http://jh.nszjky.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wt.muxihuayi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mf.bookmarksfly.cn

Java: x instanceof Number
来源：http://sv.yuexingan06.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://si.yuexingan06.cn

Ruby: x.is_a?(Numeric)
来源：http://xu.gzmigu.cn

C#:   x is int or double or decimal
来源：http://ar.muxihuayi.cn

[B14] 判断值是否在集合内
来源：http://gj.521024.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ov.wgjwhj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fv.shtwfgs.cn

JS:   [1, 2, 3].includes(x)
来源：http://oc.hahajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://pv.nicolike.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rd.jctech888.com.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ac.chemitech.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rm.yuexingan06.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vb.szxytkj.cn

[B15] 布尔运算与取反
来源：http://ee.9csxet.cn

Py:   a and b or not c
来源：http://hv.shxzskj.cn

PHP:  $a && $b || !$c
来源：http://cs.szxytkj.cn

JS:   a && b || !c
来源：http://ax.bjjhwx.cn

TS:   a && b || !c
来源：http://pi.gzmigu.cn

Java: a && b || !c
来源：http://hl.bookmarksfly.cn

Go:   a && b || !c
来源：http://zr.lnxyls.cn

Ruby: a && b || !c
来源：http://vj.huanxung.cn

C#:   a && b || !c
来源：http://kg.521024.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hc.lnxyls.cn

Py:   if not data: return
来源：http://av.jctech888.com.cn

PHP:  if (!$data) { return; }
来源：http://md.newstarts.cn

JS:   if (!data) return;
来源：http://kk.nszjky.cn

TS:   if (!data) return;
来源：http://ct.521024.cn

Java: if (data == null) return;
来源：http://on.nszjky.cn

Go:   if data == nil { return }
来源：http://gx.hnjuh.cn

Ruby: return if data.nil?
来源：http://pn.szxytkj.cn

C#:   if (data == null) return;
来源：http://rr.szxytkj.cn

================================================================================
来源：http://sw.chemitech.net.cn

C. 函数与作用域
来源：http://wv.wgjwhj.cn

================================================================================
来源：http://su.huanxung.cn

[C01] 定义函数
来源：http://cl.nicolike.cn

Py:   def add(a, b): return a + b
来源：http://ut.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kw.lnxyls.cn

JS:   function add(a, b) { return a + b; }
来源：http://ix.huixinmuqiang.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kb.nszjky.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ub.lnxyls.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ch.yuntaijiaju.cn

Ruby: def add(a, b); a + b; end
来源：http://rz.nszjky.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fe.lnxyls.cn

[C02] 默认参数
来源：http://iy.jianghongdianzi.cn

Py:   def greet(name="World"): return name
来源：http://qr.colortex.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cc.nicolike.cn

JS:   function greet(name = "World") { return name; }
来源：http://zv.gzmigu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://mx.nszjky.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ey.muxihuayi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yj.shxzskj.cn

Ruby: def greet(name = "World") = name
来源：http://zt.muxihuayi.cn

C#:   string Greet(string name = "World") => name;
来源：http://er.nicolike.cn

[C03] 可变参数
来源：http://yc.asd995.cn

Py:   def total(*args): return sum(args)
来源：http://vx.nicolike.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://iu.jianghongdianzi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kl.nicolike.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ty.9csxet.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dv.shxzukj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jl.jianghongdianzi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://er.wgjwhj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qg.newstarts.cn

[C04] 命名参数 / 关键字参数
来源：http://uv.shxzskj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jj.nicolike.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://np.hahajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://iy.asd995.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gq.jctech888.com.cn

Java: // 无：用 Builder 模式或 record
来源：http://sc.shxzukj.cn

Go:   // 无：用配置结构体参数
来源：http://yt.yuntaijiaju.cn

Ruby: f(a: 1, b: 2)
来源：http://yv.szsharing.cn

C#:   f(a: 1, b: 2)
来源：http://kq.shxzskj.cn

[C05] 返回多个值
来源：http://hs.szxytkj.cn

Py:   return a, b
来源：http://gs.bookmarksfly.cn

PHP:  return [$a, $b];
来源：http://bc.wgjwhj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://rl.szsharing.cn

TS:   return { a, b };
来源：http://gi.jctech888.com.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gl.chemitech.net.cn

Go:   return a, b
来源：http://io.jctech888.com.cn

Ruby: return a, b
来源：http://pw.bookmarksfly.cn

C#:   return (a, b);              // ValueTuple
来源：http://yq.yuexingan06.cn

[C06] 匿名函数 / lambda
来源：http://ub.nicolike.cn

Py:   square = lambda x: x * x
来源：http://al.szsharing.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://to.wgjwhj.cn

JS:   const square = x => x * x;
来源：http://yp.wgjwhj.cn

TS:   const square = (x: number): number => x * x;
来源：http://ef.shtwfgs.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wq.colortex.cn

Go:   sq := func(x int) int { return x * x }
来源：http://sv.bjjhwx.cn

Ruby: square = ->(x) { x * x }
来源：http://gj.9csxet.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zu.jctech888.com.cn

[C07] 把函数作为参数传入
来源：http://wo.huixiangedu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kx.huixiangedu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://oj.yuexingan06.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yw.nszjky.cn

TS:   arr.map(String)
来源：http://fh.huixiangedu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wv.chemitech.net.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fm.szsharing.cn

Ruby: arr.map(&:upcase)
来源：http://oi.jctech888.com.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://md.colortex.cn

[C08] 闭包
来源：http://zy.haigaiapp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qm.nszjky.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://et.yuexingan06.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zb.haigaiapp.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qs.bookmarksfly.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cd.panjiajie.cn


<!-- 参考信息 -->