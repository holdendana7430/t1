代发 wailian999

Ruby: a, b = b, a
来源：http://eb.hahajie.cn

C#:   (a, b) = (b, a);
来源：http://xu.shtwfgs.cn

[A20] 读取标准输入
来源：http://wd.521024.cn

Py:   name = input("请输入：")
来源：http://ky.yuexingan06.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://yg.jctech888.com.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bd.jianghongdianzi.cn

TS:   // Node.js：readline 模块
来源：http://xm.szsharing.cn

Java: new Scanner(System.in).nextLine()
来源：http://ee.newstarts.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fl.hnjuh.cn

Ruby: gets.chomp
来源：http://gm.shtwfgs.cn

C#:   Console.ReadLine();
来源：http://yx.chemitech.net.cn

[A21] 保留指定小数位输出
来源：http://kb.jctech888.com.cn

Py:   f"{3.14159:.2f}"
来源：http://dd.huixiangedu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gc.yuexingan06.cn

JS:   (3.14159).toFixed(2)
来源：http://tq.shxzskj.cn

TS:   (3.14159).toFixed(2)
来源：http://dm.asd995.cn

Java: String.format("%.2f", 3.14159)
来源：http://wy.jctech888.com.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://az.shxzukj.cn

Ruby: format("%.2f", 3.14159)
来源：http://ct.hnjuh.cn

C#:   3.14159.ToString("F2")
来源：http://hg.huixinmuqiang.cn

[A22] 获取字符串长度
来源：http://cx.huixiangedu.cn

Py:   len(s)
来源：http://mc.haigaiapp.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ms.lnxyls.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ko.yuntaijiaju.cn

TS:   s.length
来源：http://wr.yuntaijiaju.cn

Java: s.length()
来源：http://hq.shxzukj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zd.shtwfgs.cn

Ruby: s.length
来源：http://mp.nszjky.cn

C#:   s.Length
来源：http://rp.huanxung.cn

[A23] 大小写转换
来源：http://ld.asd995.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://cz.nicolike.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wd.asd995.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://av.haigaiapp.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vl.shxzskj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rl.haigaiapp.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ue.yuntaijiaju.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bs.huixiangedu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://xh.haigaiapp.cn

[A24] 去除首尾空白
来源：http://ce.huanxung.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gx.hnjuh.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hx.nszjky.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vn.yuntaijiaju.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kv.szsharing.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zf.newstarts.cn

Go:   strings.TrimSpace(s)
来源：http://hq.bookmarksfly.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mf.521024.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tf.shxzukj.cn

[A25] 字符串比较
来源：http://xr.shtwfgs.cn

Py:   s1 == s2; s1 != s2
来源：http://bh.jctech888.com.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://lb.bookmarksfly.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vo.yuntaijiaju.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gi.szxytkj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://df.panjiajie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mf.nszjky.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://fx.haigaiapp.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mg.shxzskj.cn

[A26] 类型转换总览
来源：http://yo.gzmigu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ph.muxihuayi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lm.shxzukj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nv.yuntaijiaju.cn

TS:   Number() String() Boolean() x as number
来源：http://vq.gzmigu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gp.jctech888.com.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ea.hnjuh.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ac.szsharing.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fa.hnjuh.cn

================================================================================
来源：http://qu.9csxet.cn

B. 流程控制
来源：http://ni.hnjuh.cn

================================================================================
来源：http://nz.wgjwhj.cn

[B01] 条件判断 if / else
来源：http://ai.lnxyls.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://da.shxzukj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yn.colortex.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mm.wgjwhj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yg.shtwfgs.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ps.chemitech.net.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yt.szsharing.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://uo.shxzskj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mo.shxzskj.cn

[B02] 多分支 else if / elif
来源：http://jp.9csxet.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ok.shxzukj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sp.bjjhwx.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rf.yuexingan06.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nb.jianghongdianzi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ta.nicolike.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nw.huixiangedu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mj.bookmarksfly.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ao.huixinmuqiang.cn

[B03] switch / match / case
来源：http://vj.wgjwhj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yl.shxzukj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mc.asd995.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wr.shxzukj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://us.jctech888.com.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://po.huixinmuqiang.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nq.panjiajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jv.jianghongdianzi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ss.chemitech.net.cn

[B04] for 计数循环
来源：http://hk.panjiajie.cn

Py:   for i in range(10): print(i)
来源：http://wa.colortex.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yx.huixiangedu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jj.huixinmuqiang.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gg.jctech888.com.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ty.yuntaijiaju.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gf.521024.cn

Ruby: 10.times { |i| puts i }
来源：http://ge.521024.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jv.shxzskj.cn

[B05] 遍历数组 / 列表
来源：http://xi.huixiangedu.cn

Py:   for item in arr: print(item)
来源：http://fi.gzmigu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jh.panjiajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dx.jctech888.com.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://lt.bjjhwx.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vv.muxihuayi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pq.9csxet.cn

Ruby: arr.each { |item| puts item }
来源：http://qi.nszjky.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ji.chemitech.net.cn

[B06] 遍历字典 / 对象
来源：http://so.9csxet.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://md.hnjuh.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ih.shxzskj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ai.shxzskj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qk.muxihuayi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ot.colortex.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vj.lnxyls.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ff.521024.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jb.colortex.cn

[B07] while 循环
来源：http://wn.nicolike.cn

Py:   while i < 10: i += 1
来源：http://oj.szxytkj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ag.newstarts.cn

JS:   while (i < 10) { i++; }
来源：http://ka.shxzskj.cn

TS:   while (i < 10) { i++; }
来源：http://jz.lnxyls.cn

Java: while (i < 10) { i++; }
来源：http://by.gzmigu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zb.colortex.cn

Ruby: while i < 10; i += 1; end
来源：http://xz.gzmigu.cn

C#:   while (i < 10) { i++; }
来源：http://gg.shxzskj.cn

[B08] do-while（至少执行一次）
来源：http://vz.nszjky.cn

Py:   # 无 do-while：用 while True + break
来源：http://an.nicolike.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xl.szxytkj.cn

JS:   do { i++; } while (i < 10);
来源：http://kb.bjjhwx.cn

TS:   do { i++; } while (i < 10);
来源：http://ax.jianghongdianzi.cn

Java: do { i++; } while (i < 10);
来源：http://oc.521024.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://lw.hahajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ix.huanxung.cn

C#:   do { i++; } while (i < 10);
来源：http://nm.yuexingan06.cn

[B09] break 与 continue
来源：http://ey.szxytkj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://el.shxzukj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://iq.asd995.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ps.szsharing.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xl.shxzskj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://al.nszjky.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hx.yuntaijiaju.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wy.muxihuayi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ub.bookmarksfly.cn

[B10] 遍历同时拿索引
来源：http://vg.bookmarksfly.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ih.haigaiapp.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cd.bookmarksfly.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mb.huanxung.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xo.wgjwhj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ia.yuntaijiaju.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dv.huixiangedu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fi.bjjhwx.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ek.521024.cn

[B11] 生成数字序列 / 区间
来源：http://yn.jctech888.com.cn

Py:   list(range(0, 10, 2))
来源：http://ic.lnxyls.cn

PHP:  range(0, 10, 2);
来源：http://np.nicolike.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pz.szsharing.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xp.jctech888.com.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mh.shxzskj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://td.hnjuh.cn

Ruby: (0...10).step(2).to_a
来源：http://ia.hahajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xb.asd995.cn

[B12] 跳出多层循环
来源：http://ed.bookmarksfly.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ql.szxytkj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ql.nszjky.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ym.haigaiapp.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ag.gzmigu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yw.asd995.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yx.jianghongdianzi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sj.nszjky.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nr.shxzskj.cn

[B13] 判断是否为数字
来源：http://km.szxytkj.cn

Py:   isinstance(x, (int, float))
来源：http://lh.bookmarksfly.cn

PHP:  is_numeric($x)
来源：http://oq.szxytkj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://he.szxytkj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gv.huixiangedu.cn

Java: x instanceof Number
来源：http://mc.haigaiapp.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jh.wgjwhj.cn

Ruby: x.is_a?(Numeric)
来源：http://oq.huanxung.cn

C#:   x is int or double or decimal
来源：http://ao.bookmarksfly.cn

[B14] 判断值是否在集合内
来源：http://ow.asd995.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://od.shtwfgs.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ah.huixiangedu.cn

JS:   [1, 2, 3].includes(x)
来源：http://qw.shxzskj.cn

TS:   [1, 2, 3].includes(x)
来源：http://vo.shxzskj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://yn.shxzukj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ld.newstarts.cn

Ruby: [1, 2, 3].include?(x)
来源：http://tz.hahajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://db.bjjhwx.cn

[B15] 布尔运算与取反
来源：http://io.9csxet.cn

Py:   a and b or not c
来源：http://mm.panjiajie.cn

PHP:  $a && $b || !$c
来源：http://wl.hahajie.cn

JS:   a && b || !c
来源：http://ki.wgjwhj.cn

TS:   a && b || !c
来源：http://pr.yuexingan06.cn

Java: a && b || !c
来源：http://py.wgjwhj.cn

Go:   a && b || !c
来源：http://xa.shtwfgs.cn

Ruby: a && b || !c
来源：http://zs.bookmarksfly.cn

C#:   a && b || !c
来源：http://dg.szxytkj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://dn.shxzskj.cn

Py:   if not data: return
来源：http://cd.huixinmuqiang.cn

PHP:  if (!$data) { return; }
来源：http://lh.9csxet.cn

JS:   if (!data) return;
来源：http://fp.haigaiapp.cn

TS:   if (!data) return;
来源：http://vx.nicolike.cn

Java: if (data == null) return;
来源：http://rd.yuexingan06.cn

Go:   if data == nil { return }
来源：http://dv.huixinmuqiang.cn

Ruby: return if data.nil?
来源：http://jb.jianghongdianzi.cn

C#:   if (data == null) return;
来源：http://io.521024.cn

================================================================================
来源：http://rf.wgjwhj.cn

C. 函数与作用域
来源：http://rl.muxihuayi.cn

================================================================================
来源：http://lv.yuntaijiaju.cn

[C01] 定义函数
来源：http://bx.wgjwhj.cn

Py:   def add(a, b): return a + b
来源：http://ca.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fn.huixinmuqiang.cn

JS:   function add(a, b) { return a + b; }
来源：http://bh.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tj.nszjky.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dh.jctech888.com.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xm.yuntaijiaju.cn

Ruby: def add(a, b); a + b; end
来源：http://gn.jianghongdianzi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bw.yuexingan06.cn

[C02] 默认参数
来源：http://zq.huixiangedu.cn

Py:   def greet(name="World"): return name
来源：http://oo.521024.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://jw.huixiangedu.cn

JS:   function greet(name = "World") { return name; }
来源：http://ef.hahajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lx.newstarts.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ku.yuexingan06.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fu.jianghongdianzi.cn

Ruby: def greet(name = "World") = name
来源：http://kq.shtwfgs.cn

C#:   string Greet(string name = "World") => name;
来源：http://ya.lnxyls.cn

[C03] 可变参数
来源：http://fi.huixiangedu.cn

Py:   def total(*args): return sum(args)
来源：http://ex.muxihuayi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://te.szxytkj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vc.jianghongdianzi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pe.asd995.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rg.hnjuh.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://iw.chemitech.net.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pa.gzmigu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tz.chemitech.net.cn

[C04] 命名参数 / 关键字参数
来源：http://ir.haigaiapp.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://as.huixinmuqiang.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ua.huanxung.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fx.haigaiapp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zh.haigaiapp.cn

Java: // 无：用 Builder 模式或 record
来源：http://ng.huixinmuqiang.cn

Go:   // 无：用配置结构体参数
来源：http://ip.huanxung.cn

Ruby: f(a: 1, b: 2)
来源：http://fn.szsharing.cn

C#:   f(a: 1, b: 2)
来源：http://ct.haigaiapp.cn

[C05] 返回多个值
来源：http://qq.panjiajie.cn

Py:   return a, b
来源：http://mr.hahajie.cn

PHP:  return [$a, $b];
来源：http://cz.panjiajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://cg.chemitech.net.cn

TS:   return { a, b };
来源：http://on.haigaiapp.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vw.shtwfgs.cn

Go:   return a, b
来源：http://rk.jctech888.com.cn

Ruby: return a, b
来源：http://wl.szsharing.cn

C#:   return (a, b);              // ValueTuple
来源：http://ti.lnxyls.cn

[C06] 匿名函数 / lambda
来源：http://sm.huixinmuqiang.cn

Py:   square = lambda x: x * x
来源：http://sa.asd995.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pp.panjiajie.cn

JS:   const square = x => x * x;
来源：http://pu.szxytkj.cn

TS:   const square = (x: number): number => x * x;
来源：http://me.panjiajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yq.shtwfgs.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zn.gzmigu.cn

Ruby: square = ->(x) { x * x }
来源：http://do.huixinmuqiang.cn

C#:   Func<int, int> square = x => x * x;
来源：http://jm.szsharing.cn

[C07] 把函数作为参数传入
来源：http://cg.yuntaijiaju.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pv.gzmigu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://og.shtwfgs.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vb.hnjuh.cn

TS:   arr.map(String)
来源：http://mb.nicolike.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tx.shxzskj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gx.huanxung.cn

Ruby: arr.map(&:upcase)
来源：http://ky.yuntaijiaju.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ne.bjjhwx.cn

[C08] 闭包
来源：http://dn.muxihuayi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ex.521024.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sp.huixinmuqiang.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rk.panjiajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xp.bjjhwx.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yf.huixinmuqiang.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://il.bjjhwx.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jz.jctech888.com.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zd.bjjhwx.cn

[C09] 递归
来源：http://fr.hnjuh.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bg.jctech888.com.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wm.huixinmuqiang.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lb.hnjuh.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ke.jianghongdianzi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://km.shxzskj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fc.lnxyls.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dc.huixinmuqiang.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ty.colortex.cn

[C10] 变量作用域
来源：http://eg.huixinmuqiang.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ne.szsharing.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://he.shxzukj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cv.shxzukj.cn


<!-- 参考信息 -->