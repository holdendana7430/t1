代发 wailian999

Ruby: a, b = b, a
来源：http://od.jianghongdianzi.cn

C#:   (a, b) = (b, a);
来源：http://gg.shxzukj.cn

[A20] 读取标准输入
来源：http://ld.9csxet.cn

Py:   name = input("请输入：")
来源：http://xw.nszjky.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://yn.szsharing.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cm.gzmigu.cn

TS:   // Node.js：readline 模块
来源：http://fy.bookmarksfly.cn

Java: new Scanner(System.in).nextLine()
来源：http://hy.huanxung.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bv.newstarts.cn

Ruby: gets.chomp
来源：http://uw.bookmarksfly.cn

C#:   Console.ReadLine();
来源：http://iy.haigaiapp.cn

[A21] 保留指定小数位输出
来源：http://rn.yuexingan06.cn

Py:   f"{3.14159:.2f}"
来源：http://fd.shxzukj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bc.shxzskj.cn

JS:   (3.14159).toFixed(2)
来源：http://gi.szxytkj.cn

TS:   (3.14159).toFixed(2)
来源：http://gy.bjjhwx.cn

Java: String.format("%.2f", 3.14159)
来源：http://dg.shxzukj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://db.9csxet.cn

Ruby: format("%.2f", 3.14159)
来源：http://or.colortex.cn

C#:   3.14159.ToString("F2")
来源：http://pq.huanxung.cn

[A22] 获取字符串长度
来源：http://jb.haigaiapp.cn

Py:   len(s)
来源：http://ov.haigaiapp.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://da.jianghongdianzi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lc.huanxung.cn

TS:   s.length
来源：http://kh.panjiajie.cn

Java: s.length()
来源：http://qn.colortex.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ps.chemitech.net.cn

Ruby: s.length
来源：http://ql.huixinmuqiang.cn

C#:   s.Length
来源：http://uc.jctech888.com.cn

[A23] 大小写转换
来源：http://kw.521024.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wd.jianghongdianzi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yj.asd995.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xq.huixinmuqiang.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cr.yuntaijiaju.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xo.jianghongdianzi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mf.shtwfgs.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://kr.huixinmuqiang.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://an.szsharing.cn

[A24] 去除首尾空白
来源：http://vx.huixiangedu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xd.bookmarksfly.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ra.521024.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nq.nszjky.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kf.shxzskj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://oe.shxzukj.cn

Go:   strings.TrimSpace(s)
来源：http://no.huixiangedu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://py.panjiajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lv.colortex.cn

[A25] 字符串比较
来源：http://mw.yuntaijiaju.cn

Py:   s1 == s2; s1 != s2
来源：http://sj.bookmarksfly.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://uw.shtwfgs.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ml.yuntaijiaju.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ci.bjjhwx.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rd.yuntaijiaju.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mz.colortex.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://nb.huixinmuqiang.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mr.panjiajie.cn

[A26] 类型转换总览
来源：http://kh.yuntaijiaju.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ex.hahajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qx.hnjuh.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tw.panjiajie.cn

TS:   Number() String() Boolean() x as number
来源：http://vt.newstarts.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://go.yuexingan06.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bn.szxytkj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ia.gzmigu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qo.wgjwhj.cn

================================================================================
来源：http://hj.shxzskj.cn

B. 流程控制
来源：http://ma.hahajie.cn

================================================================================
来源：http://xc.shxzskj.cn

[B01] 条件判断 if / else
来源：http://tr.nicolike.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://sy.bjjhwx.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://eh.bjjhwx.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fq.jianghongdianzi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jy.jianghongdianzi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://pd.9csxet.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://da.shtwfgs.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pt.shxzskj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nx.chemitech.net.cn

[B02] 多分支 else if / elif
来源：http://ub.huixinmuqiang.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pj.yuexingan06.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gv.szsharing.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yd.bookmarksfly.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vw.hnjuh.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jw.bjjhwx.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kg.haigaiapp.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ps.newstarts.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ah.szxytkj.cn

[B03] switch / match / case
来源：http://ni.szxytkj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ww.jianghongdianzi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://at.szxytkj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yb.shtwfgs.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jc.hnjuh.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://al.haigaiapp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lr.huanxung.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yj.szsharing.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cx.szxytkj.cn

[B04] for 计数循环
来源：http://rs.shxzskj.cn

Py:   for i in range(10): print(i)
来源：http://pi.szsharing.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pj.colortex.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lx.shxzukj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dk.bjjhwx.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ae.colortex.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ya.521024.cn

Ruby: 10.times { |i| puts i }
来源：http://yi.gzmigu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xk.9csxet.cn

[B05] 遍历数组 / 列表
来源：http://xp.yuexingan06.cn

Py:   for item in arr: print(item)
来源：http://en.jctech888.com.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ca.asd995.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ev.panjiajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rb.9csxet.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ny.newstarts.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://un.nicolike.cn

Ruby: arr.each { |item| puts item }
来源：http://px.yuexingan06.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ud.bjjhwx.cn

[B06] 遍历字典 / 对象
来源：http://vj.521024.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tp.szsharing.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pl.hahajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qt.hahajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wt.panjiajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ii.panjiajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tv.panjiajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yf.9csxet.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ah.huixinmuqiang.cn

[B07] while 循环
来源：http://ef.wgjwhj.cn

Py:   while i < 10: i += 1
来源：http://uu.haigaiapp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gm.chemitech.net.cn

JS:   while (i < 10) { i++; }
来源：http://ne.yuntaijiaju.cn

TS:   while (i < 10) { i++; }
来源：http://mi.hahajie.cn

Java: while (i < 10) { i++; }
来源：http://jn.asd995.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hx.yuntaijiaju.cn

Ruby: while i < 10; i += 1; end
来源：http://cy.chemitech.net.cn

C#:   while (i < 10) { i++; }
来源：http://ws.haigaiapp.cn

[B08] do-while（至少执行一次）
来源：http://lj.chemitech.net.cn

Py:   # 无 do-while：用 while True + break
来源：http://oz.hahajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ez.szsharing.cn

JS:   do { i++; } while (i < 10);
来源：http://lj.lnxyls.cn

TS:   do { i++; } while (i < 10);
来源：http://eh.colortex.cn

Java: do { i++; } while (i < 10);
来源：http://re.nicolike.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sd.szxytkj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ro.shxzskj.cn

C#:   do { i++; } while (i < 10);
来源：http://af.huixinmuqiang.cn

[B09] break 与 continue
来源：http://rn.muxihuayi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fj.nszjky.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://oq.jianghongdianzi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bh.jianghongdianzi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ul.asd995.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uw.huixiangedu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vj.szsharing.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yg.jianghongdianzi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://be.shxzskj.cn

[B10] 遍历同时拿索引
来源：http://xh.chemitech.net.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nb.bjjhwx.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bj.huanxung.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vv.muxihuayi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://va.lnxyls.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ta.jctech888.com.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://us.9csxet.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kj.gzmigu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sk.bjjhwx.cn

[B11] 生成数字序列 / 区间
来源：http://sp.szxytkj.cn

Py:   list(range(0, 10, 2))
来源：http://uh.yuntaijiaju.cn

PHP:  range(0, 10, 2);
来源：http://mr.haigaiapp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dy.bookmarksfly.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wt.hahajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gv.haigaiapp.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qz.bjjhwx.cn

Ruby: (0...10).step(2).to_a
来源：http://hi.wgjwhj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://to.jctech888.com.cn

[B12] 跳出多层循环
来源：http://bu.huixinmuqiang.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yo.jianghongdianzi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://st.huanxung.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ol.shxzskj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dt.shtwfgs.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mp.szxytkj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.colortex.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://or.muxihuayi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yl.jianghongdianzi.cn

[B13] 判断是否为数字
来源：http://bg.muxihuayi.cn

Py:   isinstance(x, (int, float))
来源：http://qd.yuntaijiaju.cn

PHP:  is_numeric($x)
来源：http://vf.jianghongdianzi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uk.huixiangedu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ov.shxzskj.cn

Java: x instanceof Number
来源：http://uq.gzmigu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ax.bjjhwx.cn

Ruby: x.is_a?(Numeric)
来源：http://zo.szsharing.cn

C#:   x is int or double or decimal
来源：http://ez.haigaiapp.cn

[B14] 判断值是否在集合内
来源：http://nm.chemitech.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ti.shxzskj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pa.gzmigu.cn

JS:   [1, 2, 3].includes(x)
来源：http://db.shxzukj.cn

TS:   [1, 2, 3].includes(x)
来源：http://jf.szxytkj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://pl.shtwfgs.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vc.szxytkj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cb.jctech888.com.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ah.colortex.cn

[B15] 布尔运算与取反
来源：http://eo.nicolike.cn

Py:   a and b or not c
来源：http://cp.huixinmuqiang.cn

PHP:  $a && $b || !$c
来源：http://dk.colortex.cn

JS:   a && b || !c
来源：http://fc.wgjwhj.cn

TS:   a && b || !c
来源：http://ob.9csxet.cn

Java: a && b || !c
来源：http://eo.lnxyls.cn

Go:   a && b || !c
来源：http://iu.9csxet.cn

Ruby: a && b || !c
来源：http://cv.huixinmuqiang.cn

C#:   a && b || !c
来源：http://zd.yuexingan06.cn

[B16] 卫语句：不满足条件提前返回
来源：http://cg.szsharing.cn

Py:   if not data: return
来源：http://uw.hahajie.cn

PHP:  if (!$data) { return; }
来源：http://qd.nicolike.cn

JS:   if (!data) return;
来源：http://ub.nszjky.cn

TS:   if (!data) return;
来源：http://rw.huixiangedu.cn

Java: if (data == null) return;
来源：http://bh.jianghongdianzi.cn

Go:   if data == nil { return }
来源：http://mg.jianghongdianzi.cn

Ruby: return if data.nil?
来源：http://lb.9csxet.cn

C#:   if (data == null) return;
来源：http://et.huixinmuqiang.cn

================================================================================
来源：http://cx.szxytkj.cn

C. 函数与作用域
来源：http://vd.szxytkj.cn

================================================================================
来源：http://gv.colortex.cn

[C01] 定义函数
来源：http://xj.haigaiapp.cn

Py:   def add(a, b): return a + b
来源：http://ml.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uv.newstarts.cn

JS:   function add(a, b) { return a + b; }
来源：http://ys.yuexingan06.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dv.huanxung.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dj.nicolike.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vh.shxzukj.cn

Ruby: def add(a, b); a + b; end
来源：http://xr.hnjuh.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tk.nicolike.cn

[C02] 默认参数
来源：http://wj.yuntaijiaju.cn

Py:   def greet(name="World"): return name
来源：http://wb.newstarts.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://nu.muxihuayi.cn

JS:   function greet(name = "World") { return name; }
来源：http://jh.yuntaijiaju.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fa.colortex.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vb.jianghongdianzi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://et.huanxung.cn

Ruby: def greet(name = "World") = name
来源：http://wo.hahajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://tr.yuntaijiaju.cn

[C03] 可变参数
来源：http://bg.jctech888.com.cn

Py:   def total(*args): return sum(args)
来源：http://on.huixinmuqiang.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zm.shtwfgs.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bi.bookmarksfly.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rt.9csxet.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tl.newstarts.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://aw.asd995.cn

Ruby: def total(*nums); nums.sum; end
来源：http://aw.nszjky.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ov.muxihuayi.cn

[C04] 命名参数 / 关键字参数
来源：http://nf.521024.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ef.panjiajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://te.newstarts.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bn.yuexingan06.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tj.hnjuh.cn

Java: // 无：用 Builder 模式或 record
来源：http://jv.colortex.cn

Go:   // 无：用配置结构体参数
来源：http://rd.muxihuayi.cn

Ruby: f(a: 1, b: 2)
来源：http://wi.newstarts.cn

C#:   f(a: 1, b: 2)
来源：http://yj.jianghongdianzi.cn

[C05] 返回多个值
来源：http://up.panjiajie.cn

Py:   return a, b
来源：http://vq.wgjwhj.cn

PHP:  return [$a, $b];
来源：http://ig.szsharing.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qb.nicolike.cn

TS:   return { a, b };
来源：http://tb.bookmarksfly.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dn.hahajie.cn

Go:   return a, b
来源：http://kq.panjiajie.cn

Ruby: return a, b
来源：http://lf.nszjky.cn

C#:   return (a, b);              // ValueTuple
来源：http://rv.nszjky.cn

[C06] 匿名函数 / lambda
来源：http://sn.chemitech.net.cn

Py:   square = lambda x: x * x
来源：http://rw.colortex.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://oi.chemitech.net.cn

JS:   const square = x => x * x;
来源：http://wm.shxzukj.cn

TS:   const square = (x: number): number => x * x;
来源：http://ac.szxytkj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tk.asd995.cn

Go:   sq := func(x int) int { return x * x }
来源：http://et.wgjwhj.cn

Ruby: square = ->(x) { x * x }
来源：http://pr.yuexingan06.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ga.haigaiapp.cn

[C07] 把函数作为参数传入
来源：http://jp.yuexingan06.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dy.szxytkj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kc.shxzskj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cy.huanxung.cn

TS:   arr.map(String)
来源：http://fa.shxzukj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ok.panjiajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tn.yuexingan06.cn

Ruby: arr.map(&:upcase)
来源：http://gk.huanxung.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://tu.nszjky.cn

[C08] 闭包
来源：http://ip.szsharing.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gt.muxihuayi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mi.panjiajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ab.shtwfgs.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bi.shxzukj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sd.colortex.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ng.huanxung.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nu.haigaiapp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bs.shxzskj.cn

[C09] 递归
来源：http://cq.yuntaijiaju.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.newstarts.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sr.hnjuh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uh.wgjwhj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xo.szsharing.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kq.yuntaijiaju.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://up.shxzskj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fc.szsharing.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bz.jianghongdianzi.cn

[C10] 变量作用域
来源：http://uk.haigaiapp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vr.gzmigu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jk.chemitech.net.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dv.lnxyls.cn


<!-- 参考信息 -->