代发 wailian999

C#:   (int)'A'; (char)65
来源：http://jh.gzmigu.cn

[A19] 交换两个变量
来源：http://si.hnjuh.cn

Py:   a, b = b, a
来源：http://wk.panjiajie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://pq.gzmigu.cn

JS:   [a, b] = [b, a];
来源：http://xr.huanxung.cn

TS:   [a, b] = [b, a];
来源：http://mb.521024.cn

Java: int t = a; a = b; b = t;
来源：http://rb.huixinmuqiang.cn

Go:   a, b = b, a
来源：http://ww.panjiajie.cn

Ruby: a, b = b, a
来源：http://il.szxytkj.cn

C#:   (a, b) = (b, a);
来源：http://hm.jctech888.com.cn

[A20] 读取标准输入
来源：http://at.yuntaijiaju.cn

Py:   name = input("请输入：")
来源：http://hx.shtwfgs.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://eg.shxzukj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gl.hnjuh.cn

TS:   // Node.js：readline 模块
来源：http://ar.chemitech.net.cn

Java: new Scanner(System.in).nextLine()
来源：http://rb.haigaiapp.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qg.9csxet.cn

Ruby: gets.chomp
来源：http://fb.nicolike.cn

C#:   Console.ReadLine();
来源：http://to.hnjuh.cn

[A21] 保留指定小数位输出
来源：http://yz.shxzskj.cn

Py:   f"{3.14159:.2f}"
来源：http://zj.shtwfgs.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fj.hahajie.cn

JS:   (3.14159).toFixed(2)
来源：http://sl.szsharing.cn

TS:   (3.14159).toFixed(2)
来源：http://xv.bookmarksfly.cn

Java: String.format("%.2f", 3.14159)
来源：http://tg.hnjuh.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vf.521024.cn

Ruby: format("%.2f", 3.14159)
来源：http://fu.hahajie.cn

C#:   3.14159.ToString("F2")
来源：http://rk.huixinmuqiang.cn

[A22] 获取字符串长度
来源：http://zz.lnxyls.cn

Py:   len(s)
来源：http://nw.szxytkj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ew.wgjwhj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rr.hahajie.cn

TS:   s.length
来源：http://ak.huanxung.cn

Java: s.length()
来源：http://uu.hnjuh.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://oe.panjiajie.cn

Ruby: s.length
来源：http://gb.asd995.cn

C#:   s.Length
来源：http://qh.bookmarksfly.cn

[A23] 大小写转换
来源：http://lu.jctech888.com.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://hg.newstarts.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xl.huanxung.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bz.nicolike.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://me.bjjhwx.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ja.chemitech.net.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bn.shtwfgs.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qz.nszjky.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://gy.bjjhwx.cn

[A24] 去除首尾空白
来源：http://li.hnjuh.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fa.bookmarksfly.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ih.asd995.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wh.hnjuh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nq.hnjuh.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ej.9csxet.cn

Go:   strings.TrimSpace(s)
来源：http://un.lnxyls.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ip.lnxyls.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vg.newstarts.cn

[A25] 字符串比较
来源：http://ci.szxytkj.cn

Py:   s1 == s2; s1 != s2
来源：http://ir.lnxyls.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kw.newstarts.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lt.haigaiapp.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ln.newstarts.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://io.bjjhwx.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kx.jctech888.com.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://aj.hahajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wm.jianghongdianzi.cn

[A26] 类型转换总览
来源：http://xr.huixiangedu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vp.hnjuh.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://al.yuntaijiaju.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ee.jianghongdianzi.cn

TS:   Number() String() Boolean() x as number
来源：http://vm.521024.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ly.huixinmuqiang.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cf.colortex.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://il.521024.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jh.yuexingan06.cn

================================================================================
来源：http://vx.panjiajie.cn

B. 流程控制
来源：http://yc.yuntaijiaju.cn

================================================================================
来源：http://iy.muxihuayi.cn

[B01] 条件判断 if / else
来源：http://mu.nicolike.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ds.jctech888.com.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rg.asd995.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://iz.wgjwhj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rj.yuntaijiaju.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://cj.bjjhwx.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fw.shtwfgs.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dl.yuexingan06.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qc.huixiangedu.cn

[B02] 多分支 else if / elif
来源：http://wz.9csxet.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qj.bjjhwx.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://df.chemitech.net.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ns.wgjwhj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kp.nicolike.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ea.shtwfgs.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://sj.huixiangedu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ok.lnxyls.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mo.521024.cn

[B03] switch / match / case
来源：http://ct.newstarts.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://po.haigaiapp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cf.chemitech.net.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ny.lnxyls.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bt.chemitech.net.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ww.9csxet.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mi.hahajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ju.wgjwhj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ns.shxzskj.cn

[B04] for 计数循环
来源：http://zj.newstarts.cn

Py:   for i in range(10): print(i)
来源：http://qb.bjjhwx.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xc.szsharing.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ec.huanxung.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tt.yuntaijiaju.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ni.muxihuayi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://sj.szxytkj.cn

Ruby: 10.times { |i| puts i }
来源：http://zb.muxihuayi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ji.chemitech.net.cn

[B05] 遍历数组 / 列表
来源：http://mz.gzmigu.cn

Py:   for item in arr: print(item)
来源：http://nd.yuexingan06.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fh.bookmarksfly.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yo.bjjhwx.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://he.jianghongdianzi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zc.nicolike.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ct.bjjhwx.cn

Ruby: arr.each { |item| puts item }
来源：http://fu.bjjhwx.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vg.nszjky.cn

[B06] 遍历字典 / 对象
来源：http://pq.panjiajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://yf.bookmarksfly.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://oh.yuexingan06.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pv.huixiangedu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bv.bookmarksfly.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ks.9csxet.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hc.nszjky.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tp.chemitech.net.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ag.gzmigu.cn

[B07] while 循环
来源：http://ho.jctech888.com.cn

Py:   while i < 10: i += 1
来源：http://rd.wgjwhj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ng.yuexingan06.cn

JS:   while (i < 10) { i++; }
来源：http://cs.hahajie.cn

TS:   while (i < 10) { i++; }
来源：http://pa.huixinmuqiang.cn

Java: while (i < 10) { i++; }
来源：http://lg.hnjuh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://de.huixinmuqiang.cn

Ruby: while i < 10; i += 1; end
来源：http://eq.szxytkj.cn

C#:   while (i < 10) { i++; }
来源：http://ac.9csxet.cn

[B08] do-while（至少执行一次）
来源：http://hk.jctech888.com.cn

Py:   # 无 do-while：用 while True + break
来源：http://cw.nszjky.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mz.haigaiapp.cn

JS:   do { i++; } while (i < 10);
来源：http://wc.szxytkj.cn

TS:   do { i++; } while (i < 10);
来源：http://vi.yuntaijiaju.cn

Java: do { i++; } while (i < 10);
来源：http://ru.bjjhwx.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://md.szxytkj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wz.jctech888.com.cn

C#:   do { i++; } while (i < 10);
来源：http://zw.lnxyls.cn

[B09] break 与 continue
来源：http://mv.szsharing.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://io.shxzukj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qz.hahajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://il.huixiangedu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rd.shxzukj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ht.jctech888.com.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tg.yuntaijiaju.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pg.shxzskj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kf.colortex.cn

[B10] 遍历同时拿索引
来源：http://ru.yuntaijiaju.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://oj.9csxet.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hs.newstarts.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fz.hahajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wz.shtwfgs.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lt.huixinmuqiang.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ox.asd995.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fx.hahajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wn.yuexingan06.cn

[B11] 生成数字序列 / 区间
来源：http://ey.gzmigu.cn

Py:   list(range(0, 10, 2))
来源：http://pi.jianghongdianzi.cn

PHP:  range(0, 10, 2);
来源：http://md.chemitech.net.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zn.jctech888.com.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jn.bjjhwx.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nm.huixiangedu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yn.nszjky.cn

Ruby: (0...10).step(2).to_a
来源：http://md.lnxyls.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nk.panjiajie.cn

[B12] 跳出多层循环
来源：http://dm.yuexingan06.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://lk.szxytkj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ex.haigaiapp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ju.haigaiapp.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://em.jianghongdianzi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://eg.jianghongdianzi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cb.chemitech.net.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yf.jianghongdianzi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jn.wgjwhj.cn

[B13] 判断是否为数字
来源：http://nn.yuexingan06.cn

Py:   isinstance(x, (int, float))
来源：http://nr.gzmigu.cn

PHP:  is_numeric($x)
来源：http://nv.chemitech.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://go.wgjwhj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tm.huanxung.cn

Java: x instanceof Number
来源：http://ej.chemitech.net.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yg.lnxyls.cn

Ruby: x.is_a?(Numeric)
来源：http://ih.shxzskj.cn

C#:   x is int or double or decimal
来源：http://gc.chemitech.net.cn

[B14] 判断值是否在集合内
来源：http://kh.wgjwhj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dw.nicolike.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zm.jctech888.com.cn

JS:   [1, 2, 3].includes(x)
来源：http://xb.szsharing.cn

TS:   [1, 2, 3].includes(x)
来源：http://uf.huanxung.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ms.hahajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wr.haigaiapp.cn

Ruby: [1, 2, 3].include?(x)
来源：http://nj.bjjhwx.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rw.shxzukj.cn

[B15] 布尔运算与取反
来源：http://gv.shtwfgs.cn

Py:   a and b or not c
来源：http://fz.muxihuayi.cn

PHP:  $a && $b || !$c
来源：http://ul.colortex.cn

JS:   a && b || !c
来源：http://zu.nszjky.cn

TS:   a && b || !c
来源：http://ck.nicolike.cn

Java: a && b || !c
来源：http://yo.gzmigu.cn

Go:   a && b || !c
来源：http://rn.gzmigu.cn

Ruby: a && b || !c
来源：http://jq.9csxet.cn

C#:   a && b || !c
来源：http://ku.szsharing.cn

[B16] 卫语句：不满足条件提前返回
来源：http://mb.colortex.cn

Py:   if not data: return
来源：http://qj.chemitech.net.cn

PHP:  if (!$data) { return; }
来源：http://st.yuexingan06.cn

JS:   if (!data) return;
来源：http://sb.hahajie.cn

TS:   if (!data) return;
来源：http://ap.huanxung.cn

Java: if (data == null) return;
来源：http://dj.521024.cn

Go:   if data == nil { return }
来源：http://cz.521024.cn

Ruby: return if data.nil?
来源：http://uh.nszjky.cn

C#:   if (data == null) return;
来源：http://pk.colortex.cn

================================================================================
来源：http://iv.haigaiapp.cn

C. 函数与作用域
来源：http://hb.huixiangedu.cn

================================================================================
来源：http://vb.newstarts.cn

[C01] 定义函数
来源：http://tr.jianghongdianzi.cn

Py:   def add(a, b): return a + b
来源：http://hv.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sx.hahajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://vd.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://co.szxytkj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bb.yuntaijiaju.cn

Go:   func add(a, b int) int { return a + b }
来源：http://af.szxytkj.cn

Ruby: def add(a, b); a + b; end
来源：http://kc.nicolike.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kp.muxihuayi.cn

[C02] 默认参数
来源：http://yr.bjjhwx.cn

Py:   def greet(name="World"): return name
来源：http://zl.asd995.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fn.hnjuh.cn

JS:   function greet(name = "World") { return name; }
来源：http://sx.szxytkj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ew.szxytkj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jn.huixiangedu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ra.nicolike.cn

Ruby: def greet(name = "World") = name
来源：http://zl.lnxyls.cn

C#:   string Greet(string name = "World") => name;
来源：http://sq.colortex.cn

[C03] 可变参数
来源：http://qt.wgjwhj.cn

Py:   def total(*args): return sum(args)
来源：http://de.bjjhwx.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fm.szsharing.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bj.hahajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qr.bookmarksfly.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mt.nszjky.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://aa.huanxung.cn

Ruby: def total(*nums); nums.sum; end
来源：http://be.bookmarksfly.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dy.shxzskj.cn

[C04] 命名参数 / 关键字参数
来源：http://vu.huanxung.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rx.shxzukj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ta.nszjky.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://eo.nszjky.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qj.bookmarksfly.cn

Java: // 无：用 Builder 模式或 record
来源：http://en.shtwfgs.cn

Go:   // 无：用配置结构体参数
来源：http://ue.gzmigu.cn

Ruby: f(a: 1, b: 2)
来源：http://dd.panjiajie.cn

C#:   f(a: 1, b: 2)
来源：http://gc.9csxet.cn

[C05] 返回多个值
来源：http://oo.colortex.cn

Py:   return a, b
来源：http://dg.panjiajie.cn

PHP:  return [$a, $b];
来源：http://lw.nszjky.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ya.bookmarksfly.cn

TS:   return { a, b };
来源：http://ad.jctech888.com.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://es.bjjhwx.cn

Go:   return a, b
来源：http://re.muxihuayi.cn

Ruby: return a, b
来源：http://dx.huixiangedu.cn

C#:   return (a, b);              // ValueTuple
来源：http://uv.shxzskj.cn

[C06] 匿名函数 / lambda
来源：http://ul.colortex.cn

Py:   square = lambda x: x * x
来源：http://uq.huixinmuqiang.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wp.colortex.cn

JS:   const square = x => x * x;
来源：http://td.panjiajie.cn

TS:   const square = (x: number): number => x * x;
来源：http://oq.lnxyls.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://oo.colortex.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ei.newstarts.cn

Ruby: square = ->(x) { x * x }
来源：http://tx.yuexingan06.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ly.chemitech.net.cn

[C07] 把函数作为参数传入
来源：http://ia.gzmigu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gs.nszjky.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xr.nszjky.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://as.newstarts.cn

TS:   arr.map(String)
来源：http://vt.newstarts.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xp.gzmigu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jo.jctech888.com.cn

Ruby: arr.map(&:upcase)
来源：http://lq.yuexingan06.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://vs.shxzskj.cn

[C08] 闭包
来源：http://ic.nszjky.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uy.szxytkj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qb.huixinmuqiang.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://oi.haigaiapp.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yl.panjiajie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zz.huixiangedu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ap.bookmarksfly.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ms.9csxet.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zt.hnjuh.cn

[C09] 递归
来源：http://em.szxytkj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xs.521024.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xl.shtwfgs.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ew.huixiangedu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ou.lnxyls.cn


<!-- 参考信息 -->