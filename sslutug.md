代发 wailian999

JS:   [a, b] = [b, a];
来源：http://nk.szxytkj.cn

TS:   [a, b] = [b, a];
来源：http://nf.521024.cn

Java: int t = a; a = b; b = t;
来源：http://cy.lnxyls.cn

Go:   a, b = b, a
来源：http://zl.newstarts.cn

Ruby: a, b = b, a
来源：http://tl.gzmigu.cn

C#:   (a, b) = (b, a);
来源：http://wh.muxihuayi.cn

[A20] 读取标准输入
来源：http://ab.muxihuayi.cn

Py:   name = input("请输入：")
来源：http://db.newstarts.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://yp.lnxyls.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nb.shtwfgs.cn

TS:   // Node.js：readline 模块
来源：http://ba.newstarts.cn

Java: new Scanner(System.in).nextLine()
来源：http://yd.521024.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ni.shxzskj.cn

Ruby: gets.chomp
来源：http://kd.lnxyls.cn

C#:   Console.ReadLine();
来源：http://av.hahajie.cn

[A21] 保留指定小数位输出
来源：http://zf.shxzukj.cn

Py:   f"{3.14159:.2f}"
来源：http://ph.szsharing.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cc.haigaiapp.cn

JS:   (3.14159).toFixed(2)
来源：http://ru.hahajie.cn

TS:   (3.14159).toFixed(2)
来源：http://gj.shtwfgs.cn

Java: String.format("%.2f", 3.14159)
来源：http://vc.jianghongdianzi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ga.szsharing.cn

Ruby: format("%.2f", 3.14159)
来源：http://zg.bjjhwx.cn

C#:   3.14159.ToString("F2")
来源：http://zd.huixinmuqiang.cn

[A22] 获取字符串长度
来源：http://qi.nicolike.cn

Py:   len(s)
来源：http://jv.9csxet.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qb.huanxung.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://on.szxytkj.cn

TS:   s.length
来源：http://ji.haigaiapp.cn

Java: s.length()
来源：http://ey.gzmigu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ca.huanxung.cn

Ruby: s.length
来源：http://ut.huanxung.cn

C#:   s.Length
来源：http://gv.huixinmuqiang.cn

[A23] 大小写转换
来源：http://bg.9csxet.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://tb.wgjwhj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://id.colortex.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cg.panjiajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xd.huixiangedu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ol.szxytkj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sg.asd995.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mj.colortex.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://oc.nszjky.cn

[A24] 去除首尾空白
来源：http://ni.szxytkj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ys.huixinmuqiang.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tv.gzmigu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oe.huixinmuqiang.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jb.colortex.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tb.szsharing.cn

Go:   strings.TrimSpace(s)
来源：http://wj.jctech888.com.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ca.lnxyls.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fg.colortex.cn

[A25] 字符串比较
来源：http://jh.hahajie.cn

Py:   s1 == s2; s1 != s2
来源：http://zs.newstarts.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qw.jianghongdianzi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://by.wgjwhj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jt.panjiajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ot.nszjky.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xw.chemitech.net.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://do.asd995.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vz.colortex.cn

[A26] 类型转换总览
来源：http://zq.panjiajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://to.shxzukj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://oj.newstarts.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://eh.huixinmuqiang.cn

TS:   Number() String() Boolean() x as number
来源：http://vc.newstarts.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gz.haigaiapp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xg.bookmarksfly.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://cb.hahajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pr.asd995.cn

================================================================================
来源：http://wz.yuntaijiaju.cn

B. 流程控制
来源：http://qk.huixiangedu.cn

================================================================================
来源：http://eq.newstarts.cn

[B01] 条件判断 if / else
来源：http://ob.jctech888.com.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vw.yuexingan06.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lw.jianghongdianzi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zj.wgjwhj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fa.haigaiapp.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ld.hnjuh.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vj.huanxung.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ai.9csxet.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://do.lnxyls.cn

[B02] 多分支 else if / elif
来源：http://ui.9csxet.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ty.nszjky.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tf.panjiajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ye.shtwfgs.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://id.chemitech.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ai.shtwfgs.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kl.szxytkj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dz.asd995.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rt.jctech888.com.cn

[B03] switch / match / case
来源：http://ff.newstarts.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jr.shxzukj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fi.panjiajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jd.shxzukj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rn.jctech888.com.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tx.hahajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pz.colortex.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ya.jianghongdianzi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vy.muxihuayi.cn

[B04] for 计数循环
来源：http://xf.shxzukj.cn

Py:   for i in range(10): print(i)
来源：http://wh.shxzukj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://uk.9csxet.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dh.lnxyls.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ap.shxzukj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ls.shtwfgs.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dy.nszjky.cn

Ruby: 10.times { |i| puts i }
来源：http://dh.panjiajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qh.yuexingan06.cn

[B05] 遍历数组 / 列表
来源：http://gh.yuexingan06.cn

Py:   for item in arr: print(item)
来源：http://go.bookmarksfly.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://we.colortex.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://lp.lnxyls.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://zu.huanxung.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zp.asd995.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lk.hahajie.cn

Ruby: arr.each { |item| puts item }
来源：http://xw.shxzukj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://de.nszjky.cn

[B06] 遍历字典 / 对象
来源：http://tr.yuntaijiaju.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mm.jianghongdianzi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kx.9csxet.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hf.gzmigu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xz.gzmigu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ra.lnxyls.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nn.bookmarksfly.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ia.hahajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://si.huanxung.cn

[B07] while 循环
来源：http://kr.hnjuh.cn

Py:   while i < 10: i += 1
来源：http://fa.shxzukj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://yf.muxihuayi.cn

JS:   while (i < 10) { i++; }
来源：http://or.nicolike.cn

TS:   while (i < 10) { i++; }
来源：http://rr.9csxet.cn

Java: while (i < 10) { i++; }
来源：http://sr.nszjky.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ip.hnjuh.cn

Ruby: while i < 10; i += 1; end
来源：http://cm.bjjhwx.cn

C#:   while (i < 10) { i++; }
来源：http://mt.hahajie.cn

[B08] do-while（至少执行一次）
来源：http://le.hahajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://gq.hnjuh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mm.gzmigu.cn

JS:   do { i++; } while (i < 10);
来源：http://st.jianghongdianzi.cn

TS:   do { i++; } while (i < 10);
来源：http://yo.muxihuayi.cn

Java: do { i++; } while (i < 10);
来源：http://yz.huixiangedu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://az.huixiangedu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fp.huixiangedu.cn

C#:   do { i++; } while (i < 10);
来源：http://bh.bookmarksfly.cn

[B09] break 与 continue
来源：http://cl.szsharing.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dh.nszjky.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lu.huixiangedu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vl.szsharing.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aa.shxzskj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lq.huixiangedu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://og.yuexingan06.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qe.9csxet.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jt.jctech888.com.cn

[B10] 遍历同时拿索引
来源：http://zq.shxzukj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ly.521024.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nh.newstarts.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zy.asd995.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hp.szxytkj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xk.lnxyls.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kc.yuntaijiaju.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ws.wgjwhj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ip.huixinmuqiang.cn

[B11] 生成数字序列 / 区间
来源：http://he.nszjky.cn

Py:   list(range(0, 10, 2))
来源：http://wx.shxzskj.cn

PHP:  range(0, 10, 2);
来源：http://ls.haigaiapp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ob.yuexingan06.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lf.chemitech.net.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xy.gzmigu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yz.nszjky.cn

Ruby: (0...10).step(2).to_a
来源：http://mj.asd995.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://av.521024.cn

[B12] 跳出多层循环
来源：http://qc.gzmigu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://de.lnxyls.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fr.huixiangedu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hh.asd995.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://il.521024.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cw.shxzukj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://eb.shxzukj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ei.yuntaijiaju.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fm.panjiajie.cn

[B13] 判断是否为数字
来源：http://hc.panjiajie.cn

Py:   isinstance(x, (int, float))
来源：http://kv.bookmarksfly.cn

PHP:  is_numeric($x)
来源：http://in.huanxung.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bo.colortex.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.wgjwhj.cn

Java: x instanceof Number
来源：http://gh.gzmigu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ga.hahajie.cn

Ruby: x.is_a?(Numeric)
来源：http://ey.wgjwhj.cn

C#:   x is int or double or decimal
来源：http://oi.huanxung.cn

[B14] 判断值是否在集合内
来源：http://of.huixinmuqiang.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gu.lnxyls.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bq.bookmarksfly.cn

JS:   [1, 2, 3].includes(x)
来源：http://uh.shxzskj.cn

TS:   [1, 2, 3].includes(x)
来源：http://pg.chemitech.net.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xh.shtwfgs.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rd.newstarts.cn

Ruby: [1, 2, 3].include?(x)
来源：http://bs.huixinmuqiang.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hy.jctech888.com.cn

[B15] 布尔运算与取反
来源：http://qq.lnxyls.cn

Py:   a and b or not c
来源：http://kt.9csxet.cn

PHP:  $a && $b || !$c
来源：http://ci.bookmarksfly.cn

JS:   a && b || !c
来源：http://na.shtwfgs.cn

TS:   a && b || !c
来源：http://vg.colortex.cn

Java: a && b || !c
来源：http://jg.nszjky.cn

Go:   a && b || !c
来源：http://fn.hahajie.cn

Ruby: a && b || !c
来源：http://gs.bookmarksfly.cn

C#:   a && b || !c
来源：http://fh.9csxet.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vt.521024.cn

Py:   if not data: return
来源：http://nd.hahajie.cn

PHP:  if (!$data) { return; }
来源：http://bo.huanxung.cn

JS:   if (!data) return;
来源：http://tf.wgjwhj.cn

TS:   if (!data) return;
来源：http://hu.asd995.cn

Java: if (data == null) return;
来源：http://si.shxzukj.cn

Go:   if data == nil { return }
来源：http://jv.nicolike.cn

Ruby: return if data.nil?
来源：http://ju.huanxung.cn

C#:   if (data == null) return;
来源：http://oz.yuntaijiaju.cn

================================================================================
来源：http://wq.jianghongdianzi.cn

C. 函数与作用域
来源：http://ed.nicolike.cn

================================================================================
来源：http://lr.wgjwhj.cn

[C01] 定义函数
来源：http://gr.muxihuayi.cn

Py:   def add(a, b): return a + b
来源：http://ic.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pt.521024.cn

JS:   function add(a, b) { return a + b; }
来源：http://wa.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lb.hnjuh.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ww.hahajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://pn.chemitech.net.cn

Ruby: def add(a, b); a + b; end
来源：http://ud.bjjhwx.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mt.huixiangedu.cn

[C02] 默认参数
来源：http://eh.yuntaijiaju.cn

Py:   def greet(name="World"): return name
来源：http://qu.szsharing.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://sx.huixiangedu.cn

JS:   function greet(name = "World") { return name; }
来源：http://ie.bookmarksfly.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zz.huixiangedu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://lj.jctech888.com.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ag.yuntaijiaju.cn

Ruby: def greet(name = "World") = name
来源：http://gw.521024.cn

C#:   string Greet(string name = "World") => name;
来源：http://nq.bjjhwx.cn

[C03] 可变参数
来源：http://ku.muxihuayi.cn

Py:   def total(*args): return sum(args)
来源：http://lg.shtwfgs.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ld.bookmarksfly.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zp.bjjhwx.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://at.shxzukj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ct.jianghongdianzi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://as.nicolike.cn

Ruby: def total(*nums); nums.sum; end
来源：http://cv.shxzskj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gd.asd995.cn

[C04] 命名参数 / 关键字参数
来源：http://lw.shtwfgs.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pg.yuntaijiaju.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nb.jianghongdianzi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://td.wgjwhj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xu.huanxung.cn

Java: // 无：用 Builder 模式或 record
来源：http://xz.lnxyls.cn

Go:   // 无：用配置结构体参数
来源：http://jm.lnxyls.cn

Ruby: f(a: 1, b: 2)
来源：http://au.jctech888.com.cn

C#:   f(a: 1, b: 2)
来源：http://ys.shtwfgs.cn

[C05] 返回多个值
来源：http://jt.haigaiapp.cn

Py:   return a, b
来源：http://nf.yuexingan06.cn

PHP:  return [$a, $b];
来源：http://fg.huanxung.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jd.nicolike.cn

TS:   return { a, b };
来源：http://ko.yuexingan06.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sx.jianghongdianzi.cn

Go:   return a, b
来源：http://dz.shtwfgs.cn

Ruby: return a, b
来源：http://iz.bookmarksfly.cn

C#:   return (a, b);              // ValueTuple
来源：http://gz.wgjwhj.cn

[C06] 匿名函数 / lambda
来源：http://vq.hnjuh.cn

Py:   square = lambda x: x * x
来源：http://sd.haigaiapp.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qu.yuexingan06.cn

JS:   const square = x => x * x;
来源：http://rx.panjiajie.cn

TS:   const square = (x: number): number => x * x;
来源：http://di.huixiangedu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://my.lnxyls.cn

Go:   sq := func(x int) int { return x * x }
来源：http://cz.muxihuayi.cn

Ruby: square = ->(x) { x * x }
来源：http://eo.szxytkj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://no.panjiajie.cn

[C07] 把函数作为参数传入
来源：http://gn.huixinmuqiang.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ln.chemitech.net.cn

PHP:  array_map("strtoupper", $arr);
来源：http://lw.asd995.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bi.jctech888.com.cn

TS:   arr.map(String)
来源：http://rx.jianghongdianzi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xi.nszjky.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xg.haigaiapp.cn

Ruby: arr.map(&:upcase)
来源：http://yg.bjjhwx.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ed.huixinmuqiang.cn

[C08] 闭包
来源：http://ns.panjiajie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://an.colortex.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nx.shxzskj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ep.chemitech.net.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fz.yuntaijiaju.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mr.9csxet.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ca.521024.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fh.muxihuayi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zc.szxytkj.cn

[C09] 递归
来源：http://xt.panjiajie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gq.haigaiapp.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://he.9csxet.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kk.shxzukj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dn.hnjuh.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ou.521024.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qs.521024.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hu.nicolike.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uw.shtwfgs.cn


<!-- 参考信息 -->