代发 wailian999

JS:   [a, b] = [b, a];
来源：http://pc.shxzukj.cn

TS:   [a, b] = [b, a];
来源：http://hf.chemitech.net.cn

Java: int t = a; a = b; b = t;
来源：http://py.shxzskj.cn

Go:   a, b = b, a
来源：http://ex.hnjuh.cn

Ruby: a, b = b, a
来源：http://xq.szxytkj.cn

C#:   (a, b) = (b, a);
来源：http://as.wgjwhj.cn

[A20] 读取标准输入
来源：http://si.asd995.cn

Py:   name = input("请输入：")
来源：http://qy.nicolike.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ma.huixiangedu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lq.bjjhwx.cn

TS:   // Node.js：readline 模块
来源：http://bx.colortex.cn

Java: new Scanner(System.in).nextLine()
来源：http://jw.hnjuh.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dn.haigaiapp.cn

Ruby: gets.chomp
来源：http://eg.hnjuh.cn

C#:   Console.ReadLine();
来源：http://wc.colortex.cn

[A21] 保留指定小数位输出
来源：http://tb.bjjhwx.cn

Py:   f"{3.14159:.2f}"
来源：http://ie.wgjwhj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dl.bjjhwx.cn

JS:   (3.14159).toFixed(2)
来源：http://xb.gzmigu.cn

TS:   (3.14159).toFixed(2)
来源：http://gw.huanxung.cn

Java: String.format("%.2f", 3.14159)
来源：http://mc.szxytkj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://dh.huixinmuqiang.cn

Ruby: format("%.2f", 3.14159)
来源：http://nb.bjjhwx.cn

C#:   3.14159.ToString("F2")
来源：http://da.nszjky.cn

[A22] 获取字符串长度
来源：http://le.jctech888.com.cn

Py:   len(s)
来源：http://nk.wgjwhj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bh.nszjky.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lg.9csxet.cn

TS:   s.length
来源：http://hr.chemitech.net.cn

Java: s.length()
来源：http://lt.9csxet.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vb.gzmigu.cn

Ruby: s.length
来源：http://hx.muxihuayi.cn

C#:   s.Length
来源：http://aw.nicolike.cn

[A23] 大小写转换
来源：http://gv.wgjwhj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://tr.hahajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vk.nszjky.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ah.asd995.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mg.jianghongdianzi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jd.jctech888.com.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wm.nszjky.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://un.asd995.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://do.huanxung.cn

[A24] 去除首尾空白
来源：http://xu.asd995.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fh.szxytkj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vs.nicolike.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mr.bjjhwx.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oq.nszjky.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ud.yuexingan06.cn

Go:   strings.TrimSpace(s)
来源：http://hg.yuntaijiaju.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qj.huixiangedu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gp.hahajie.cn

[A25] 字符串比较
来源：http://yl.521024.cn

Py:   s1 == s2; s1 != s2
来源：http://vx.haigaiapp.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ar.muxihuayi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jl.huixiangedu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://aq.jianghongdianzi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ty.nicolike.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jy.huixinmuqiang.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://cr.9csxet.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://op.521024.cn

[A26] 类型转换总览
来源：http://fw.nicolike.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://un.hnjuh.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ee.hnjuh.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zn.szsharing.cn

TS:   Number() String() Boolean() x as number
来源：http://vz.bookmarksfly.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vd.bookmarksfly.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://je.bookmarksfly.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ga.gzmigu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lc.shxzukj.cn

================================================================================
来源：http://fz.yuntaijiaju.cn

B. 流程控制
来源：http://xv.521024.cn

================================================================================
来源：http://ad.haigaiapp.cn

[B01] 条件判断 if / else
来源：http://tk.szsharing.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ec.muxihuayi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ha.wgjwhj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mb.shxzskj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dd.newstarts.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vg.hnjuh.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ba.shtwfgs.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wl.szsharing.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://io.nicolike.cn

[B02] 多分支 else if / elif
来源：http://tr.newstarts.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zo.yuexingan06.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wk.panjiajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wd.jianghongdianzi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://za.nszjky.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mq.huanxung.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ux.yuntaijiaju.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rg.gzmigu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ie.huixinmuqiang.cn

[B03] switch / match / case
来源：http://fw.huixiangedu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ga.jctech888.com.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dc.bookmarksfly.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ah.shxzukj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qh.hahajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vz.bookmarksfly.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ro.521024.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://op.yuntaijiaju.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mm.gzmigu.cn

[B04] for 计数循环
来源：http://oo.haigaiapp.cn

Py:   for i in range(10): print(i)
来源：http://zb.huanxung.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jp.shxzukj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://js.wgjwhj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ko.shxzskj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lf.jianghongdianzi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pr.yuntaijiaju.cn

Ruby: 10.times { |i| puts i }
来源：http://mm.nszjky.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ic.521024.cn

[B05] 遍历数组 / 列表
来源：http://ay.jianghongdianzi.cn

Py:   for item in arr: print(item)
来源：http://zh.jianghongdianzi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zu.haigaiapp.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gl.shxzskj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://cu.shxzskj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://us.muxihuayi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fy.panjiajie.cn

Ruby: arr.each { |item| puts item }
来源：http://id.lnxyls.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fp.muxihuayi.cn

[B06] 遍历字典 / 对象
来源：http://xr.newstarts.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://jf.yuntaijiaju.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pp.nszjky.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ow.bjjhwx.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bc.shxzukj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qx.hnjuh.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qv.szsharing.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ok.nszjky.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yc.chemitech.net.cn

[B07] while 循环
来源：http://pr.521024.cn

Py:   while i < 10: i += 1
来源：http://uj.shtwfgs.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hq.jctech888.com.cn

JS:   while (i < 10) { i++; }
来源：http://pp.nszjky.cn

TS:   while (i < 10) { i++; }
来源：http://hc.bjjhwx.cn

Java: while (i < 10) { i++; }
来源：http://rz.jianghongdianzi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ah.chemitech.net.cn

Ruby: while i < 10; i += 1; end
来源：http://im.yuexingan06.cn

C#:   while (i < 10) { i++; }
来源：http://gz.hnjuh.cn

[B08] do-while（至少执行一次）
来源：http://lw.yuexingan06.cn

Py:   # 无 do-while：用 while True + break
来源：http://yo.asd995.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ct.haigaiapp.cn

JS:   do { i++; } while (i < 10);
来源：http://qw.huanxung.cn

TS:   do { i++; } while (i < 10);
来源：http://js.hahajie.cn

Java: do { i++; } while (i < 10);
来源：http://mo.yuexingan06.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://tg.yuntaijiaju.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vo.panjiajie.cn

C#:   do { i++; } while (i < 10);
来源：http://eb.huixinmuqiang.cn

[B09] break 与 continue
来源：http://vn.9csxet.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ub.yuntaijiaju.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://de.jianghongdianzi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ny.huanxung.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zl.lnxyls.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bw.yuntaijiaju.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lz.nicolike.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bh.9csxet.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cs.huixinmuqiang.cn

[B10] 遍历同时拿索引
来源：http://np.huixinmuqiang.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sd.szxytkj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xy.yuntaijiaju.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pq.szsharing.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ms.shxzskj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xj.nszjky.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mu.shxzukj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dl.shxzskj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jg.bjjhwx.cn

[B11] 生成数字序列 / 区间
来源：http://tf.hahajie.cn

Py:   list(range(0, 10, 2))
来源：http://rf.shtwfgs.cn

PHP:  range(0, 10, 2);
来源：http://uq.521024.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wt.hahajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cc.shxzukj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wa.bjjhwx.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vp.yuexingan06.cn

Ruby: (0...10).step(2).to_a
来源：http://ev.nicolike.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ic.shxzskj.cn

[B12] 跳出多层循环
来源：http://ti.nicolike.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yl.newstarts.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ob.huixiangedu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://en.haigaiapp.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://am.huixiangedu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kq.521024.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vq.lnxyls.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xv.huixinmuqiang.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://og.newstarts.cn

[B13] 判断是否为数字
来源：http://wd.colortex.cn

Py:   isinstance(x, (int, float))
来源：http://qm.haigaiapp.cn

PHP:  is_numeric($x)
来源：http://uz.yuexingan06.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://an.chemitech.net.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ud.haigaiapp.cn

Java: x instanceof Number
来源：http://gn.nicolike.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ty.jianghongdianzi.cn

Ruby: x.is_a?(Numeric)
来源：http://hk.521024.cn

C#:   x is int or double or decimal
来源：http://qj.gzmigu.cn

[B14] 判断值是否在集合内
来源：http://dc.panjiajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://am.wgjwhj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lm.muxihuayi.cn

JS:   [1, 2, 3].includes(x)
来源：http://uf.haigaiapp.cn

TS:   [1, 2, 3].includes(x)
来源：http://aq.lnxyls.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://wn.szxytkj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vn.huixinmuqiang.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xh.chemitech.net.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rd.521024.cn

[B15] 布尔运算与取反
来源：http://jg.jianghongdianzi.cn

Py:   a and b or not c
来源：http://fg.newstarts.cn

PHP:  $a && $b || !$c
来源：http://ei.nicolike.cn

JS:   a && b || !c
来源：http://ii.colortex.cn

TS:   a && b || !c
来源：http://vo.yuntaijiaju.cn

Java: a && b || !c
来源：http://zq.nicolike.cn

Go:   a && b || !c
来源：http://ez.bookmarksfly.cn

Ruby: a && b || !c
来源：http://wt.bookmarksfly.cn

C#:   a && b || !c
来源：http://bj.hahajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://yf.bookmarksfly.cn

Py:   if not data: return
来源：http://ax.newstarts.cn

PHP:  if (!$data) { return; }
来源：http://wr.szxytkj.cn

JS:   if (!data) return;
来源：http://lv.asd995.cn

TS:   if (!data) return;
来源：http://ry.bookmarksfly.cn

Java: if (data == null) return;
来源：http://pu.bookmarksfly.cn

Go:   if data == nil { return }
来源：http://wp.huanxung.cn

Ruby: return if data.nil?
来源：http://nf.jctech888.com.cn

C#:   if (data == null) return;
来源：http://tb.wgjwhj.cn

================================================================================
来源：http://og.colortex.cn

C. 函数与作用域
来源：http://pf.jctech888.com.cn

================================================================================
来源：http://lq.wgjwhj.cn

[C01] 定义函数
来源：http://eb.521024.cn

Py:   def add(a, b): return a + b
来源：http://py.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iw.panjiajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://fe.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ym.bookmarksfly.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://px.yuntaijiaju.cn

Go:   func add(a, b int) int { return a + b }
来源：http://sz.szsharing.cn

Ruby: def add(a, b); a + b; end
来源：http://nk.gzmigu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rx.huixinmuqiang.cn

[C02] 默认参数
来源：http://bn.wgjwhj.cn

Py:   def greet(name="World"): return name
来源：http://ik.bookmarksfly.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ab.bookmarksfly.cn

JS:   function greet(name = "World") { return name; }
来源：http://ex.chemitech.net.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ot.chemitech.net.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://om.haigaiapp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://uy.yuntaijiaju.cn

Ruby: def greet(name = "World") = name
来源：http://pg.jianghongdianzi.cn

C#:   string Greet(string name = "World") => name;
来源：http://df.shtwfgs.cn

[C03] 可变参数
来源：http://me.bookmarksfly.cn

Py:   def total(*args): return sum(args)
来源：http://qx.hnjuh.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pk.szxytkj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rw.colortex.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pt.muxihuayi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cu.haigaiapp.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cd.szxytkj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yx.wgjwhj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mi.bookmarksfly.cn

[C04] 命名参数 / 关键字参数
来源：http://eb.521024.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dx.hnjuh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://np.huanxung.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gd.bookmarksfly.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zx.szsharing.cn

Java: // 无：用 Builder 模式或 record
来源：http://bn.jianghongdianzi.cn

Go:   // 无：用配置结构体参数
来源：http://jr.szsharing.cn

Ruby: f(a: 1, b: 2)
来源：http://zp.yuexingan06.cn

C#:   f(a: 1, b: 2)
来源：http://oy.nicolike.cn

[C05] 返回多个值
来源：http://ui.hnjuh.cn

Py:   return a, b
来源：http://bp.shtwfgs.cn

PHP:  return [$a, $b];
来源：http://kc.shxzukj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dj.panjiajie.cn

TS:   return { a, b };
来源：http://mr.521024.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://br.szsharing.cn

Go:   return a, b
来源：http://vr.shxzskj.cn

Ruby: return a, b
来源：http://ua.bjjhwx.cn

C#:   return (a, b);              // ValueTuple
来源：http://mq.panjiajie.cn

[C06] 匿名函数 / lambda
来源：http://ot.jianghongdianzi.cn

Py:   square = lambda x: x * x
来源：http://uv.huanxung.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://us.jctech888.com.cn

JS:   const square = x => x * x;
来源：http://ml.szsharing.cn

TS:   const square = (x: number): number => x * x;
来源：http://nv.panjiajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://oh.szxytkj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rc.colortex.cn

Ruby: square = ->(x) { x * x }
来源：http://kk.huanxung.cn

C#:   Func<int, int> square = x => x * x;
来源：http://yg.newstarts.cn

[C07] 把函数作为参数传入
来源：http://ig.521024.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dw.yuntaijiaju.cn

PHP:  array_map("strtoupper", $arr);
来源：http://rw.asd995.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dg.gzmigu.cn

TS:   arr.map(String)
来源：http://yz.yuexingan06.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fx.muxihuayi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://om.panjiajie.cn

Ruby: arr.map(&:upcase)
来源：http://at.huanxung.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://lm.huixinmuqiang.cn

[C08] 闭包
来源：http://ec.9csxet.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qz.huanxung.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hu.shxzskj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kf.bookmarksfly.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pk.shtwfgs.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vs.szsharing.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zi.jctech888.com.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vm.shxzukj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kk.521024.cn

[C09] 递归
来源：http://kn.newstarts.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://iv.wgjwhj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ff.yuntaijiaju.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jb.asd995.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kq.jianghongdianzi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pd.yuntaijiaju.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qv.lnxyls.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ji.jctech888.com.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ma.huixinmuqiang.cn


<!-- 参考信息 -->