代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rl.bookmarksfly.cn

Java: (int) 'A'; (char) 65
来源：http://am.huixinmuqiang.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://tf.9csxet.cn

Ruby: "A".ord; 65.chr
来源：http://lj.shxzukj.cn

C#:   (int)'A'; (char)65
来源：http://yo.huixiangedu.cn

[A19] 交换两个变量
来源：http://ov.jianghongdianzi.cn

Py:   a, b = b, a
来源：http://se.huixinmuqiang.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://bt.panjiajie.cn

JS:   [a, b] = [b, a];
来源：http://ym.hnjuh.cn

TS:   [a, b] = [b, a];
来源：http://on.colortex.cn

Java: int t = a; a = b; b = t;
来源：http://me.nszjky.cn

Go:   a, b = b, a
来源：http://lb.bjjhwx.cn

Ruby: a, b = b, a
来源：http://zv.szxytkj.cn

C#:   (a, b) = (b, a);
来源：http://ir.hahajie.cn

[A20] 读取标准输入
来源：http://vv.szsharing.cn

Py:   name = input("请输入：")
来源：http://nq.huixinmuqiang.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://rk.panjiajie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yr.newstarts.cn

TS:   // Node.js：readline 模块
来源：http://kt.colortex.cn

Java: new Scanner(System.in).nextLine()
来源：http://ce.lnxyls.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gl.panjiajie.cn

Ruby: gets.chomp
来源：http://kc.lnxyls.cn

C#:   Console.ReadLine();
来源：http://cw.asd995.cn

[A21] 保留指定小数位输出
来源：http://dr.jianghongdianzi.cn

Py:   f"{3.14159:.2f}"
来源：http://uj.yuntaijiaju.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ub.asd995.cn

JS:   (3.14159).toFixed(2)
来源：http://op.panjiajie.cn

TS:   (3.14159).toFixed(2)
来源：http://bm.hahajie.cn

Java: String.format("%.2f", 3.14159)
来源：http://zx.gzmigu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tf.chemitech.net.cn

Ruby: format("%.2f", 3.14159)
来源：http://sj.yuexingan06.cn

C#:   3.14159.ToString("F2")
来源：http://ds.521024.cn

[A22] 获取字符串长度
来源：http://vw.huixinmuqiang.cn

Py:   len(s)
来源：http://cn.muxihuayi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hl.huanxung.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hk.panjiajie.cn

TS:   s.length
来源：http://sr.szxytkj.cn

Java: s.length()
来源：http://fl.shxzskj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wv.gzmigu.cn

Ruby: s.length
来源：http://xr.9csxet.cn

C#:   s.Length
来源：http://gu.szsharing.cn

[A23] 大小写转换
来源：http://ri.shxzskj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zv.colortex.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ei.newstarts.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qs.newstarts.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vw.huanxung.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jw.lnxyls.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vp.yuntaijiaju.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rd.szsharing.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://la.huixinmuqiang.cn

[A24] 去除首尾空白
来源：http://vq.hnjuh.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pd.szsharing.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rm.bookmarksfly.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jk.lnxyls.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://er.yuexingan06.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qg.hnjuh.cn

Go:   strings.TrimSpace(s)
来源：http://mt.521024.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mw.gzmigu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vo.bookmarksfly.cn

[A25] 字符串比较
来源：http://vc.panjiajie.cn

Py:   s1 == s2; s1 != s2
来源：http://tc.chemitech.net.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://uf.shxzukj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://eu.lnxyls.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vt.haigaiapp.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jz.9csxet.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ff.colortex.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://gz.jctech888.com.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://un.yuntaijiaju.cn

[A26] 类型转换总览
来源：http://nd.huixinmuqiang.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yb.jianghongdianzi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cn.shxzskj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://li.9csxet.cn

TS:   Number() String() Boolean() x as number
来源：http://la.hnjuh.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yz.haigaiapp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fr.521024.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ws.jianghongdianzi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yz.nicolike.cn

================================================================================
来源：http://hc.szxytkj.cn

B. 流程控制
来源：http://sr.muxihuayi.cn

================================================================================
来源：http://bf.gzmigu.cn

[B01] 条件判断 if / else
来源：http://oh.nicolike.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://af.jianghongdianzi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bp.chemitech.net.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.huixiangedu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hs.521024.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://sv.muxihuayi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fy.panjiajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ot.colortex.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ju.nszjky.cn

[B02] 多分支 else if / elif
来源：http://vz.shxzukj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tf.nszjky.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mc.jctech888.com.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wc.huixinmuqiang.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pa.szsharing.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hn.szsharing.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zk.shxzukj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lc.gzmigu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hb.wgjwhj.cn

[B03] switch / match / case
来源：http://hr.jctech888.com.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wr.shxzukj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qm.huixiangedu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bw.lnxyls.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ci.9csxet.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fj.yuexingan06.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pa.muxihuayi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ga.nszjky.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yc.huixinmuqiang.cn

[B04] for 计数循环
来源：http://yr.newstarts.cn

Py:   for i in range(10): print(i)
来源：http://pg.nszjky.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ew.hahajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lb.muxihuayi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://js.jctech888.com.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rs.hahajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gs.bjjhwx.cn

Ruby: 10.times { |i| puts i }
来源：http://xx.muxihuayi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xz.lnxyls.cn

[B05] 遍历数组 / 列表
来源：http://zz.huanxung.cn

Py:   for item in arr: print(item)
来源：http://nn.panjiajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lm.muxihuayi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gw.hahajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://nc.bjjhwx.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jj.bjjhwx.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ec.lnxyls.cn

Ruby: arr.each { |item| puts item }
来源：http://gu.yuexingan06.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gm.chemitech.net.cn

[B06] 遍历字典 / 对象
来源：http://rt.bjjhwx.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vq.yuntaijiaju.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bs.szsharing.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jv.shxzskj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://py.gzmigu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rk.9csxet.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tq.newstarts.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wi.hnjuh.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://af.lnxyls.cn

[B07] while 循环
来源：http://os.wgjwhj.cn

Py:   while i < 10: i += 1
来源：http://om.colortex.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qc.wgjwhj.cn

JS:   while (i < 10) { i++; }
来源：http://bh.chemitech.net.cn

TS:   while (i < 10) { i++; }
来源：http://uf.yuexingan06.cn

Java: while (i < 10) { i++; }
来源：http://kg.shxzukj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ce.muxihuayi.cn

Ruby: while i < 10; i += 1; end
来源：http://jm.yuexingan06.cn

C#:   while (i < 10) { i++; }
来源：http://ib.muxihuayi.cn

[B08] do-while（至少执行一次）
来源：http://rq.szsharing.cn

Py:   # 无 do-while：用 while True + break
来源：http://zb.panjiajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pj.nicolike.cn

JS:   do { i++; } while (i < 10);
来源：http://rm.chemitech.net.cn

TS:   do { i++; } while (i < 10);
来源：http://lu.chemitech.net.cn

Java: do { i++; } while (i < 10);
来源：http://go.huixiangedu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://db.huixinmuqiang.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mr.colortex.cn

C#:   do { i++; } while (i < 10);
来源：http://rf.yuexingan06.cn

[B09] break 与 continue
来源：http://em.hnjuh.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://av.haigaiapp.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ha.haigaiapp.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ve.9csxet.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gf.9csxet.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://df.gzmigu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ec.haigaiapp.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wj.hnjuh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nu.wgjwhj.cn

[B10] 遍历同时拿索引
来源：http://rs.nszjky.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mj.521024.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xf.asd995.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zw.jianghongdianzi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wg.9csxet.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jp.szsharing.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xc.jianghongdianzi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ka.wgjwhj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wg.hahajie.cn

[B11] 生成数字序列 / 区间
来源：http://ta.panjiajie.cn

Py:   list(range(0, 10, 2))
来源：http://ox.lnxyls.cn

PHP:  range(0, 10, 2);
来源：http://ws.nicolike.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hx.gzmigu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kw.shtwfgs.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ri.yuexingan06.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ne.szsharing.cn

Ruby: (0...10).step(2).to_a
来源：http://jx.nicolike.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hp.chemitech.net.cn

[B12] 跳出多层循环
来源：http://dv.shxzukj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pv.huanxung.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://xn.newstarts.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ch.shtwfgs.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dg.jctech888.com.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ll.asd995.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lm.huixiangedu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gx.colortex.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fm.jianghongdianzi.cn

[B13] 判断是否为数字
来源：http://ne.yuexingan06.cn

Py:   isinstance(x, (int, float))
来源：http://se.huixiangedu.cn

PHP:  is_numeric($x)
来源：http://dm.nicolike.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qs.shtwfgs.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ml.jianghongdianzi.cn

Java: x instanceof Number
来源：http://se.9csxet.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://eu.szxytkj.cn

Ruby: x.is_a?(Numeric)
来源：http://zy.huixiangedu.cn

C#:   x is int or double or decimal
来源：http://gq.yuexingan06.cn

[B14] 判断值是否在集合内
来源：http://un.newstarts.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qc.haigaiapp.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dg.newstarts.cn

JS:   [1, 2, 3].includes(x)
来源：http://jo.shxzskj.cn

TS:   [1, 2, 3].includes(x)
来源：http://ni.huixinmuqiang.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ds.jctech888.com.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://uq.haigaiapp.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fd.521024.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lc.muxihuayi.cn

[B15] 布尔运算与取反
来源：http://cd.hnjuh.cn

Py:   a and b or not c
来源：http://ea.yuexingan06.cn

PHP:  $a && $b || !$c
来源：http://xp.bjjhwx.cn

JS:   a && b || !c
来源：http://tt.9csxet.cn

TS:   a && b || !c
来源：http://ht.muxihuayi.cn

Java: a && b || !c
来源：http://ib.bookmarksfly.cn

Go:   a && b || !c
来源：http://wd.jianghongdianzi.cn

Ruby: a && b || !c
来源：http://uj.yuexingan06.cn

C#:   a && b || !c
来源：http://nn.szxytkj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ov.panjiajie.cn

Py:   if not data: return
来源：http://nj.shxzskj.cn

PHP:  if (!$data) { return; }
来源：http://ho.colortex.cn

JS:   if (!data) return;
来源：http://hz.wgjwhj.cn

TS:   if (!data) return;
来源：http://sg.asd995.cn

Java: if (data == null) return;
来源：http://uc.szsharing.cn

Go:   if data == nil { return }
来源：http://dz.shxzukj.cn

Ruby: return if data.nil?
来源：http://ih.huanxung.cn

C#:   if (data == null) return;
来源：http://hl.chemitech.net.cn

================================================================================
来源：http://mf.asd995.cn

C. 函数与作用域
来源：http://te.hnjuh.cn

================================================================================
来源：http://ej.hnjuh.cn

[C01] 定义函数
来源：http://gb.yuexingan06.cn

Py:   def add(a, b): return a + b
来源：http://cu.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ky.panjiajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://du.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ks.newstarts.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://df.szxytkj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://sd.szsharing.cn

Ruby: def add(a, b); a + b; end
来源：http://ub.asd995.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ar.gzmigu.cn

[C02] 默认参数
来源：http://zk.panjiajie.cn

Py:   def greet(name="World"): return name
来源：http://nk.hahajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://rh.yuntaijiaju.cn

JS:   function greet(name = "World") { return name; }
来源：http://dm.yuntaijiaju.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lc.newstarts.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dv.jianghongdianzi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vj.haigaiapp.cn

Ruby: def greet(name = "World") = name
来源：http://ch.muxihuayi.cn

C#:   string Greet(string name = "World") => name;
来源：http://mn.nicolike.cn

[C03] 可变参数
来源：http://qu.colortex.cn

Py:   def total(*args): return sum(args)
来源：http://se.haigaiapp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sz.nicolike.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tt.shxzukj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vr.muxihuayi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wm.bookmarksfly.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dh.huanxung.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tt.hahajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gz.521024.cn

[C04] 命名参数 / 关键字参数
来源：http://zn.wgjwhj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yv.muxihuayi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qu.muxihuayi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pf.lnxyls.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gb.jianghongdianzi.cn

Java: // 无：用 Builder 模式或 record
来源：http://kn.haigaiapp.cn

Go:   // 无：用配置结构体参数
来源：http://rq.szxytkj.cn

Ruby: f(a: 1, b: 2)
来源：http://dh.haigaiapp.cn

C#:   f(a: 1, b: 2)
来源：http://eu.muxihuayi.cn

[C05] 返回多个值
来源：http://ck.chemitech.net.cn

Py:   return a, b
来源：http://gg.chemitech.net.cn

PHP:  return [$a, $b];
来源：http://kw.gzmigu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yq.muxihuayi.cn

TS:   return { a, b };
来源：http://ka.hnjuh.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sp.bjjhwx.cn

Go:   return a, b
来源：http://hg.hahajie.cn

Ruby: return a, b
来源：http://ul.hnjuh.cn

C#:   return (a, b);              // ValueTuple
来源：http://dr.newstarts.cn

[C06] 匿名函数 / lambda
来源：http://pl.521024.cn

Py:   square = lambda x: x * x
来源：http://tk.asd995.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://jj.lnxyls.cn

JS:   const square = x => x * x;
来源：http://rn.colortex.cn

TS:   const square = (x: number): number => x * x;
来源：http://gp.gzmigu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bh.hahajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gb.lnxyls.cn

Ruby: square = ->(x) { x * x }
来源：http://dx.gzmigu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ue.huixiangedu.cn

[C07] 把函数作为参数传入
来源：http://ck.nszjky.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zm.bjjhwx.cn

PHP:  array_map("strtoupper", $arr);
来源：http://cq.hnjuh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hg.huanxung.cn

TS:   arr.map(String)
来源：http://nv.shxzukj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yo.shxzskj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://au.shxzukj.cn

Ruby: arr.map(&:upcase)
来源：http://zs.hnjuh.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://yz.yuexingan06.cn

[C08] 闭包
来源：http://ix.newstarts.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://he.muxihuayi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ml.lnxyls.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://em.chemitech.net.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://en.wgjwhj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pw.shxzukj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ox.wgjwhj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xq.jctech888.com.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yi.jctech888.com.cn

[C09] 递归
来源：http://ij.bjjhwx.cn


<!-- 参考信息 -->