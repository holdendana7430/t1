代发 wailian999

JS:   [a, b] = [b, a];
来源：http://xj.jctech888.com.cn

TS:   [a, b] = [b, a];
来源：http://ie.lnxyls.cn

Java: int t = a; a = b; b = t;
来源：http://pm.9csxet.cn

Go:   a, b = b, a
来源：http://xe.colortex.cn

Ruby: a, b = b, a
来源：http://uw.wgjwhj.cn

C#:   (a, b) = (b, a);
来源：http://wm.nicolike.cn

[A20] 读取标准输入
来源：http://ps.newstarts.cn

Py:   name = input("请输入：")
来源：http://cp.lnxyls.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://yx.yuntaijiaju.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ry.bjjhwx.cn

TS:   // Node.js：readline 模块
来源：http://bd.521024.cn

Java: new Scanner(System.in).nextLine()
来源：http://om.huanxung.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ns.hnjuh.cn

Ruby: gets.chomp
来源：http://rz.panjiajie.cn

C#:   Console.ReadLine();
来源：http://eb.chemitech.net.cn

[A21] 保留指定小数位输出
来源：http://ea.9csxet.cn

Py:   f"{3.14159:.2f}"
来源：http://ck.haigaiapp.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bd.bjjhwx.cn

JS:   (3.14159).toFixed(2)
来源：http://es.9csxet.cn

TS:   (3.14159).toFixed(2)
来源：http://sa.bookmarksfly.cn

Java: String.format("%.2f", 3.14159)
来源：http://le.newstarts.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xi.yuexingan06.cn

Ruby: format("%.2f", 3.14159)
来源：http://cs.lnxyls.cn

C#:   3.14159.ToString("F2")
来源：http://pv.wgjwhj.cn

[A22] 获取字符串长度
来源：http://fx.chemitech.net.cn

Py:   len(s)
来源：http://vp.jctech888.com.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yv.newstarts.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xo.gzmigu.cn

TS:   s.length
来源：http://zt.haigaiapp.cn

Java: s.length()
来源：http://dt.huixiangedu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://he.haigaiapp.cn

Ruby: s.length
来源：http://tb.yuexingan06.cn

C#:   s.Length
来源：http://hy.wgjwhj.cn

[A23] 大小写转换
来源：http://ik.huixinmuqiang.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wy.newstarts.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bi.yuexingan06.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qq.bjjhwx.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bs.nszjky.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mg.shtwfgs.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bm.panjiajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ho.newstarts.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://cm.huixinmuqiang.cn

[A24] 去除首尾空白
来源：http://pe.lnxyls.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pk.gzmigu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kz.yuexingan06.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://td.newstarts.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qa.newstarts.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cg.yuexingan06.cn

Go:   strings.TrimSpace(s)
来源：http://aa.jctech888.com.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rh.yuntaijiaju.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lq.jctech888.com.cn

[A25] 字符串比较
来源：http://uu.huixinmuqiang.cn

Py:   s1 == s2; s1 != s2
来源：http://ph.haigaiapp.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gz.huixinmuqiang.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kw.521024.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://sb.huixinmuqiang.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ss.newstarts.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xs.lnxyls.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://lh.jctech888.com.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vi.colortex.cn

[A26] 类型转换总览
来源：http://xn.jianghongdianzi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qf.nszjky.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ci.newstarts.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fn.muxihuayi.cn

TS:   Number() String() Boolean() x as number
来源：http://pg.muxihuayi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rf.huixiangedu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pl.521024.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zp.yuntaijiaju.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qb.hnjuh.cn

================================================================================
来源：http://ez.szsharing.cn

B. 流程控制
来源：http://gz.nszjky.cn

================================================================================
来源：http://jj.nszjky.cn

[B01] 条件判断 if / else
来源：http://pf.yuexingan06.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://un.asd995.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://iw.jianghongdianzi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lj.newstarts.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yo.9csxet.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://og.gzmigu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yt.haigaiapp.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nz.yuexingan06.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://at.nicolike.cn

[B02] 多分支 else if / elif
来源：http://cv.gzmigu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xp.hnjuh.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fx.gzmigu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dr.szxytkj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eu.jianghongdianzi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yo.shtwfgs.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kc.jianghongdianzi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gh.chemitech.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sh.asd995.cn

[B03] switch / match / case
来源：http://if.szsharing.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ak.szsharing.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zn.9csxet.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://te.hnjuh.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ib.9csxet.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xw.huanxung.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://py.gzmigu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://iq.haigaiapp.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://by.huixiangedu.cn

[B04] for 计数循环
来源：http://gu.huixinmuqiang.cn

Py:   for i in range(10): print(i)
来源：http://vc.shxzukj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fy.yuexingan06.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jz.jianghongdianzi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gj.huanxung.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://br.gzmigu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kj.shtwfgs.cn

Ruby: 10.times { |i| puts i }
来源：http://ll.huixinmuqiang.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vg.shtwfgs.cn

[B05] 遍历数组 / 列表
来源：http://mm.bookmarksfly.cn

Py:   for item in arr: print(item)
来源：http://yp.haigaiapp.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fo.asd995.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ei.huixinmuqiang.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://zr.yuexingan06.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://nl.521024.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ut.muxihuayi.cn

Ruby: arr.each { |item| puts item }
来源：http://ze.521024.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pg.yuntaijiaju.cn

[B06] 遍历字典 / 对象
来源：http://ba.nicolike.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xr.nicolike.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rf.jctech888.com.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hg.lnxyls.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wx.shtwfgs.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uh.szsharing.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nz.hnjuh.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ve.wgjwhj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vk.nicolike.cn

[B07] while 循环
来源：http://ja.shtwfgs.cn

Py:   while i < 10: i += 1
来源：http://rw.hahajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qq.yuntaijiaju.cn

JS:   while (i < 10) { i++; }
来源：http://em.szxytkj.cn

TS:   while (i < 10) { i++; }
来源：http://mv.newstarts.cn

Java: while (i < 10) { i++; }
来源：http://st.colortex.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tk.yuntaijiaju.cn

Ruby: while i < 10; i += 1; end
来源：http://lo.hahajie.cn

C#:   while (i < 10) { i++; }
来源：http://sz.asd995.cn

[B08] do-while（至少执行一次）
来源：http://xz.huixiangedu.cn

Py:   # 无 do-while：用 while True + break
来源：http://nm.shxzskj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ru.nszjky.cn

JS:   do { i++; } while (i < 10);
来源：http://xj.yuntaijiaju.cn

TS:   do { i++; } while (i < 10);
来源：http://hk.lnxyls.cn

Java: do { i++; } while (i < 10);
来源：http://fn.jctech888.com.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://pd.521024.cn

Ruby: begin; i += 1; end while i < 10
来源：http://if.panjiajie.cn

C#:   do { i++; } while (i < 10);
来源：http://ou.gzmigu.cn

[B09] break 与 continue
来源：http://vw.wgjwhj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://km.shxzukj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kz.wgjwhj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nm.nszjky.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hd.hnjuh.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kn.nszjky.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ux.huixinmuqiang.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vt.shxzskj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mg.wgjwhj.cn

[B10] 遍历同时拿索引
来源：http://wx.jianghongdianzi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://op.yuexingan06.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://iz.huanxung.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xr.521024.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://za.521024.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ob.wgjwhj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://or.yuexingan06.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hc.shxzukj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tw.asd995.cn

[B11] 生成数字序列 / 区间
来源：http://qb.muxihuayi.cn

Py:   list(range(0, 10, 2))
来源：http://zo.colortex.cn

PHP:  range(0, 10, 2);
来源：http://te.shtwfgs.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qh.haigaiapp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rz.newstarts.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://th.colortex.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://js.panjiajie.cn

Ruby: (0...10).step(2).to_a
来源：http://id.panjiajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zx.wgjwhj.cn

[B12] 跳出多层循环
来源：http://il.nszjky.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://np.bjjhwx.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zr.yuexingan06.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rn.lnxyls.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://eb.chemitech.net.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xt.szxytkj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://io.newstarts.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://do.gzmigu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qy.newstarts.cn

[B13] 判断是否为数字
来源：http://bj.yuexingan06.cn

Py:   isinstance(x, (int, float))
来源：http://pf.szxytkj.cn

PHP:  is_numeric($x)
来源：http://ea.521024.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pc.hnjuh.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ef.colortex.cn

Java: x instanceof Number
来源：http://wd.jctech888.com.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rf.9csxet.cn

Ruby: x.is_a?(Numeric)
来源：http://pa.yuexingan06.cn

C#:   x is int or double or decimal
来源：http://eo.521024.cn

[B14] 判断值是否在集合内
来源：http://pf.jctech888.com.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dl.szxytkj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ja.szsharing.cn

JS:   [1, 2, 3].includes(x)
来源：http://qq.shxzskj.cn

TS:   [1, 2, 3].includes(x)
来源：http://xf.huixinmuqiang.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://oh.yuntaijiaju.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fn.nszjky.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rj.521024.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mx.lnxyls.cn

[B15] 布尔运算与取反
来源：http://sx.hnjuh.cn

Py:   a and b or not c
来源：http://tj.jianghongdianzi.cn

PHP:  $a && $b || !$c
来源：http://tw.jctech888.com.cn

JS:   a && b || !c
来源：http://fo.shtwfgs.cn

TS:   a && b || !c
来源：http://tb.huixiangedu.cn

Java: a && b || !c
来源：http://nb.521024.cn

Go:   a && b || !c
来源：http://sv.hnjuh.cn

Ruby: a && b || !c
来源：http://bq.asd995.cn

C#:   a && b || !c
来源：http://ro.lnxyls.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gu.haigaiapp.cn

Py:   if not data: return
来源：http://fo.wgjwhj.cn

PHP:  if (!$data) { return; }
来源：http://wq.521024.cn

JS:   if (!data) return;
来源：http://gu.521024.cn

TS:   if (!data) return;
来源：http://yt.hahajie.cn

Java: if (data == null) return;
来源：http://px.nszjky.cn

Go:   if data == nil { return }
来源：http://uv.hahajie.cn

Ruby: return if data.nil?
来源：http://ui.nicolike.cn

C#:   if (data == null) return;
来源：http://dp.lnxyls.cn

================================================================================
来源：http://mk.jctech888.com.cn

C. 函数与作用域
来源：http://we.shtwfgs.cn

================================================================================
来源：http://dn.muxihuayi.cn

[C01] 定义函数
来源：http://xg.wgjwhj.cn

Py:   def add(a, b): return a + b
来源：http://vf.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hi.muxihuayi.cn

JS:   function add(a, b) { return a + b; }
来源：http://xl.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vo.bookmarksfly.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://yu.hahajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qt.hnjuh.cn

Ruby: def add(a, b); a + b; end
来源：http://ni.wgjwhj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vd.gzmigu.cn

[C02] 默认参数
来源：http://xr.szsharing.cn

Py:   def greet(name="World"): return name
来源：http://nh.chemitech.net.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cv.chemitech.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://vd.yuexingan06.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://oo.bookmarksfly.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://iw.shxzukj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://st.9csxet.cn

Ruby: def greet(name = "World") = name
来源：http://yh.chemitech.net.cn

C#:   string Greet(string name = "World") => name;
来源：http://us.gzmigu.cn

[C03] 可变参数
来源：http://bq.jianghongdianzi.cn

Py:   def total(*args): return sum(args)
来源：http://qf.haigaiapp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ua.shxzskj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wx.bjjhwx.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://do.nicolike.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mv.chemitech.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dk.colortex.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pi.chemitech.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mz.shxzskj.cn

[C04] 命名参数 / 关键字参数
来源：http://sd.huanxung.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vr.hnjuh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dc.asd995.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yg.huixiangedu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dn.hnjuh.cn

Java: // 无：用 Builder 模式或 record
来源：http://fe.yuexingan06.cn

Go:   // 无：用配置结构体参数
来源：http://rv.colortex.cn

Ruby: f(a: 1, b: 2)
来源：http://jx.hahajie.cn

C#:   f(a: 1, b: 2)
来源：http://xo.521024.cn

[C05] 返回多个值
来源：http://xl.yuexingan06.cn

Py:   return a, b
来源：http://qy.chemitech.net.cn

PHP:  return [$a, $b];
来源：http://al.hnjuh.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jc.shtwfgs.cn

TS:   return { a, b };
来源：http://di.muxihuayi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gd.haigaiapp.cn

Go:   return a, b
来源：http://ud.521024.cn

Ruby: return a, b
来源：http://jj.9csxet.cn

C#:   return (a, b);              // ValueTuple
来源：http://hj.shxzskj.cn

[C06] 匿名函数 / lambda
来源：http://tq.nicolike.cn

Py:   square = lambda x: x * x
来源：http://tt.shtwfgs.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ka.yuexingan06.cn

JS:   const square = x => x * x;
来源：http://ch.shxzukj.cn

TS:   const square = (x: number): number => x * x;
来源：http://qn.gzmigu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jy.szxytkj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ed.newstarts.cn

Ruby: square = ->(x) { x * x }
来源：http://vx.wgjwhj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://pt.nicolike.cn

[C07] 把函数作为参数传入
来源：http://xc.bjjhwx.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ht.jctech888.com.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ee.muxihuayi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vo.hnjuh.cn

TS:   arr.map(String)
来源：http://fn.bookmarksfly.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tq.hnjuh.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://om.wgjwhj.cn

Ruby: arr.map(&:upcase)
来源：http://tc.haigaiapp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cj.newstarts.cn

[C08] 闭包
来源：http://gd.bookmarksfly.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qn.bookmarksfly.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hp.yuntaijiaju.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qx.panjiajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qe.asd995.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jo.huixiangedu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nr.haigaiapp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mw.huixiangedu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fc.bookmarksfly.cn

[C09] 递归
来源：http://hb.bjjhwx.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cu.lnxyls.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://js.nicolike.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://le.shxzskj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aq.nszjky.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ed.gzmigu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hc.bookmarksfly.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fh.szsharing.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pd.hahajie.cn


<!-- 参考信息 -->