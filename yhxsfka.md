代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://pj.wgjwhj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xp.hahajie.cn

TS:   // Node.js：readline 模块
来源：http://un.nszjky.cn

Java: new Scanner(System.in).nextLine()
来源：http://qi.hahajie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kf.haigaiapp.cn

Ruby: gets.chomp
来源：http://cf.gzmigu.cn

C#:   Console.ReadLine();
来源：http://tu.asd995.cn

[A21] 保留指定小数位输出
来源：http://io.jianghongdianzi.cn

Py:   f"{3.14159:.2f}"
来源：http://ai.huanxung.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://to.wgjwhj.cn

JS:   (3.14159).toFixed(2)
来源：http://za.jctech888.com.cn

TS:   (3.14159).toFixed(2)
来源：http://jk.bookmarksfly.cn

Java: String.format("%.2f", 3.14159)
来源：http://ro.newstarts.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tv.haigaiapp.cn

Ruby: format("%.2f", 3.14159)
来源：http://tu.huanxung.cn

C#:   3.14159.ToString("F2")
来源：http://lv.jianghongdianzi.cn

[A22] 获取字符串长度
来源：http://gp.jianghongdianzi.cn

Py:   len(s)
来源：http://hx.hahajie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://te.wgjwhj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ui.szxytkj.cn

TS:   s.length
来源：http://xh.9csxet.cn

Java: s.length()
来源：http://gc.huanxung.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ii.9csxet.cn

Ruby: s.length
来源：http://ks.newstarts.cn

C#:   s.Length
来源：http://ih.haigaiapp.cn

[A23] 大小写转换
来源：http://kw.jctech888.com.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://om.haigaiapp.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jx.bjjhwx.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bl.szxytkj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zr.huixiangedu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xw.gzmigu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jo.9csxet.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lf.panjiajie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://cb.shtwfgs.cn

[A24] 去除首尾空白
来源：http://pr.hahajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hg.jctech888.com.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ld.nicolike.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tb.szxytkj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wh.szsharing.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xv.bjjhwx.cn

Go:   strings.TrimSpace(s)
来源：http://ua.521024.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fl.nszjky.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dv.wgjwhj.cn

[A25] 字符串比较
来源：http://sy.hahajie.cn

Py:   s1 == s2; s1 != s2
来源：http://vq.nicolike.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xn.yuexingan06.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pc.hahajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zc.muxihuayi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mv.gzmigu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jy.hnjuh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://da.9csxet.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wa.gzmigu.cn

[A26] 类型转换总览
来源：http://tq.wgjwhj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ch.szxytkj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gw.chemitech.net.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fs.szsharing.cn

TS:   Number() String() Boolean() x as number
来源：http://bh.colortex.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ql.521024.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mv.hnjuh.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://jo.gzmigu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dj.9csxet.cn

================================================================================
来源：http://uv.shxzukj.cn

B. 流程控制
来源：http://cd.jctech888.com.cn

================================================================================
来源：http://vi.9csxet.cn

[B01] 条件判断 if / else
来源：http://wh.hnjuh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bs.wgjwhj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ru.newstarts.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://th.haigaiapp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tn.huanxung.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ri.shtwfgs.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gp.muxihuayi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cb.huixinmuqiang.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sm.colortex.cn

[B02] 多分支 else if / elif
来源：http://aj.newstarts.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ze.shxzskj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rh.gzmigu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pu.colortex.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yj.huixiangedu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ub.szsharing.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uz.gzmigu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mw.shtwfgs.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oz.yuntaijiaju.cn

[B03] switch / match / case
来源：http://lk.huixinmuqiang.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://co.panjiajie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mt.jianghongdianzi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qx.haigaiapp.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qr.bjjhwx.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dw.szsharing.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xr.szsharing.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mb.hahajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xp.nszjky.cn

[B04] for 计数循环
来源：http://ao.gzmigu.cn

Py:   for i in range(10): print(i)
来源：http://gu.newstarts.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qa.colortex.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kg.panjiajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vp.yuntaijiaju.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ly.szsharing.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://so.szxytkj.cn

Ruby: 10.times { |i| puts i }
来源：http://in.wgjwhj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tg.lnxyls.cn

[B05] 遍历数组 / 列表
来源：http://uf.szsharing.cn

Py:   for item in arr: print(item)
来源：http://xf.szsharing.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sl.yuexingan06.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gt.yuntaijiaju.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://dt.nicolike.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://cj.huixiangedu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lv.asd995.cn

Ruby: arr.each { |item| puts item }
来源：http://ei.muxihuayi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yh.huixinmuqiang.cn

[B06] 遍历字典 / 对象
来源：http://sj.521024.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://rt.huixiangedu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nm.huixiangedu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://in.szxytkj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://av.colortex.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tr.shxzukj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://si.huanxung.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kl.wgjwhj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://af.muxihuayi.cn

[B07] while 循环
来源：http://mr.jianghongdianzi.cn

Py:   while i < 10: i += 1
来源：http://zz.huanxung.cn

PHP:  while ($i < 10) { $i++; }
来源：http://cw.szxytkj.cn

JS:   while (i < 10) { i++; }
来源：http://lo.hahajie.cn

TS:   while (i < 10) { i++; }
来源：http://hn.newstarts.cn

Java: while (i < 10) { i++; }
来源：http://xj.yuntaijiaju.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ow.newstarts.cn

Ruby: while i < 10; i += 1; end
来源：http://id.haigaiapp.cn

C#:   while (i < 10) { i++; }
来源：http://qc.jianghongdianzi.cn

[B08] do-while（至少执行一次）
来源：http://sn.bjjhwx.cn

Py:   # 无 do-while：用 while True + break
来源：http://rp.nicolike.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jx.nszjky.cn

JS:   do { i++; } while (i < 10);
来源：http://bj.bookmarksfly.cn

TS:   do { i++; } while (i < 10);
来源：http://km.gzmigu.cn

Java: do { i++; } while (i < 10);
来源：http://yp.shxzskj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ja.521024.cn

Ruby: begin; i += 1; end while i < 10
来源：http://iv.shxzskj.cn

C#:   do { i++; } while (i < 10);
来源：http://md.chemitech.net.cn

[B09] break 与 continue
来源：http://bf.huixinmuqiang.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://im.bookmarksfly.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lp.haigaiapp.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://td.wgjwhj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fj.panjiajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wz.panjiajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fm.muxihuayi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jj.yuntaijiaju.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mo.huixinmuqiang.cn

[B10] 遍历同时拿索引
来源：http://ui.shxzukj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ea.muxihuayi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ju.szsharing.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://in.huixinmuqiang.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cj.panjiajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nr.gzmigu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hu.gzmigu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qu.haigaiapp.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sh.chemitech.net.cn

[B11] 生成数字序列 / 区间
来源：http://bc.shxzskj.cn

Py:   list(range(0, 10, 2))
来源：http://bv.yuntaijiaju.cn

PHP:  range(0, 10, 2);
来源：http://du.jianghongdianzi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cz.panjiajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://il.nicolike.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bb.nszjky.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bc.wgjwhj.cn

Ruby: (0...10).step(2).to_a
来源：http://qo.bookmarksfly.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://di.wgjwhj.cn

[B12] 跳出多层循环
来源：http://mn.panjiajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zj.huixinmuqiang.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wv.wgjwhj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hk.shxzukj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pl.huixinmuqiang.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zo.shxzskj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bf.szxytkj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ug.shxzskj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yd.chemitech.net.cn

[B13] 判断是否为数字
来源：http://hv.shxzskj.cn

Py:   isinstance(x, (int, float))
来源：http://sj.chemitech.net.cn

PHP:  is_numeric($x)
来源：http://ba.bjjhwx.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ag.huixiangedu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wv.szxytkj.cn

Java: x instanceof Number
来源：http://ce.nszjky.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rd.gzmigu.cn

Ruby: x.is_a?(Numeric)
来源：http://yb.521024.cn

C#:   x is int or double or decimal
来源：http://pk.bjjhwx.cn

[B14] 判断值是否在集合内
来源：http://jj.shxzskj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ay.9csxet.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ut.hahajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://zq.wgjwhj.cn

TS:   [1, 2, 3].includes(x)
来源：http://je.yuntaijiaju.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://nd.shxzskj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lr.hnjuh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://wr.muxihuayi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ak.hahajie.cn

[B15] 布尔运算与取反
来源：http://jx.szxytkj.cn

Py:   a and b or not c
来源：http://mv.chemitech.net.cn

PHP:  $a && $b || !$c
来源：http://qw.newstarts.cn

JS:   a && b || !c
来源：http://eq.szsharing.cn

TS:   a && b || !c
来源：http://fk.nszjky.cn

Java: a && b || !c
来源：http://bj.yuexingan06.cn

Go:   a && b || !c
来源：http://fs.huanxung.cn

Ruby: a && b || !c
来源：http://zt.szxytkj.cn

C#:   a && b || !c
来源：http://hl.shxzskj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://iq.bookmarksfly.cn

Py:   if not data: return
来源：http://hq.szsharing.cn

PHP:  if (!$data) { return; }
来源：http://el.yuexingan06.cn

JS:   if (!data) return;
来源：http://cs.shxzskj.cn

TS:   if (!data) return;
来源：http://lj.hnjuh.cn

Java: if (data == null) return;
来源：http://og.nicolike.cn

Go:   if data == nil { return }
来源：http://xd.szxytkj.cn

Ruby: return if data.nil?
来源：http://zp.yuexingan06.cn

C#:   if (data == null) return;
来源：http://pn.lnxyls.cn

================================================================================
来源：http://ho.shxzukj.cn

C. 函数与作用域
来源：http://gp.bookmarksfly.cn

================================================================================
来源：http://fv.muxihuayi.cn

[C01] 定义函数
来源：http://si.bjjhwx.cn

Py:   def add(a, b): return a + b
来源：http://rw.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tq.yuntaijiaju.cn

JS:   function add(a, b) { return a + b; }
来源：http://po.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yf.huixinmuqiang.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xf.shxzskj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jt.bjjhwx.cn

Ruby: def add(a, b); a + b; end
来源：http://kk.huixiangedu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mk.nszjky.cn

[C02] 默认参数
来源：http://rl.yuexingan06.cn

Py:   def greet(name="World"): return name
来源：http://ah.muxihuayi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://rn.9csxet.cn

JS:   function greet(name = "World") { return name; }
来源：http://ir.huixinmuqiang.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cz.shtwfgs.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ay.huixinmuqiang.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hc.lnxyls.cn

Ruby: def greet(name = "World") = name
来源：http://hu.hahajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://hv.huixiangedu.cn

[C03] 可变参数
来源：http://va.hnjuh.cn

Py:   def total(*args): return sum(args)
来源：http://gt.shxzukj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pe.shxzskj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zr.bookmarksfly.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://eq.hnjuh.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ld.bjjhwx.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cu.szxytkj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vz.huixiangedu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gz.szxytkj.cn

[C04] 命名参数 / 关键字参数
来源：http://dw.huanxung.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nx.huanxung.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lr.nicolike.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vi.bjjhwx.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ve.shxzukj.cn

Java: // 无：用 Builder 模式或 record
来源：http://ip.shtwfgs.cn

Go:   // 无：用配置结构体参数
来源：http://vt.muxihuayi.cn

Ruby: f(a: 1, b: 2)
来源：http://jm.huanxung.cn

C#:   f(a: 1, b: 2)
来源：http://xy.colortex.cn

[C05] 返回多个值
来源：http://nw.shxzskj.cn

Py:   return a, b
来源：http://ww.shtwfgs.cn

PHP:  return [$a, $b];
来源：http://nd.haigaiapp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ln.hnjuh.cn

TS:   return { a, b };
来源：http://ic.gzmigu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://su.panjiajie.cn

Go:   return a, b
来源：http://uo.gzmigu.cn

Ruby: return a, b
来源：http://bs.jianghongdianzi.cn

C#:   return (a, b);              // ValueTuple
来源：http://km.muxihuayi.cn

[C06] 匿名函数 / lambda
来源：http://yl.szsharing.cn

Py:   square = lambda x: x * x
来源：http://mf.huixinmuqiang.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zh.lnxyls.cn

JS:   const square = x => x * x;
来源：http://ug.9csxet.cn

TS:   const square = (x: number): number => x * x;
来源：http://ld.colortex.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mq.jianghongdianzi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qt.haigaiapp.cn

Ruby: square = ->(x) { x * x }
来源：http://id.shtwfgs.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ol.huixiangedu.cn

[C07] 把函数作为参数传入
来源：http://cx.jctech888.com.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pw.szsharing.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wf.nicolike.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vu.shxzskj.cn

TS:   arr.map(String)
来源：http://xj.haigaiapp.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ja.shtwfgs.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://he.huixiangedu.cn

Ruby: arr.map(&:upcase)
来源：http://ec.shxzukj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wg.wgjwhj.cn

[C08] 闭包
来源：http://vj.nicolike.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://am.nicolike.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wy.hnjuh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vp.chemitech.net.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kh.gzmigu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://eo.wgjwhj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ny.bookmarksfly.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bo.lnxyls.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fv.wgjwhj.cn

[C09] 递归
来源：http://wd.asd995.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nv.nicolike.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xc.yuexingan06.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bl.muxihuayi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wu.huanxung.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fq.wgjwhj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sg.szsharing.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jf.gzmigu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vv.yuntaijiaju.cn

[C10] 变量作用域
来源：http://gp.yuexingan06.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://da.gzmigu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zt.huixiangedu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hm.panjiajie.cn

TS:   同 JS
来源：http://yp.szxytkj.cn

Java: 方法内为块级作用域
来源：http://ia.huixiangedu.cn

Go:   花括号块级作用域
来源：http://kl.yuntaijiaju.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pj.hnjuh.cn


<!-- 参考信息 -->