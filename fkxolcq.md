代发 wailian999

JS:   [a, b] = [b, a];
来源：http://er.newstarts.cn

TS:   [a, b] = [b, a];
来源：http://ev.bjjhwx.cn

Java: int t = a; a = b; b = t;
来源：http://fl.bookmarksfly.cn

Go:   a, b = b, a
来源：http://cu.521024.cn

Ruby: a, b = b, a
来源：http://vq.szxytkj.cn

C#:   (a, b) = (b, a);
来源：http://wm.jianghongdianzi.cn

[A20] 读取标准输入
来源：http://gp.jianghongdianzi.cn

Py:   name = input("请输入：")
来源：http://jp.asd995.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ix.huixinmuqiang.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dy.hnjuh.cn

TS:   // Node.js：readline 模块
来源：http://ug.newstarts.cn

Java: new Scanner(System.in).nextLine()
来源：http://ew.shtwfgs.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ft.hnjuh.cn

Ruby: gets.chomp
来源：http://xr.9csxet.cn

C#:   Console.ReadLine();
来源：http://gr.yuexingan06.cn

[A21] 保留指定小数位输出
来源：http://kf.shxzskj.cn

Py:   f"{3.14159:.2f}"
来源：http://fo.yuexingan06.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://iq.shxzukj.cn

JS:   (3.14159).toFixed(2)
来源：http://ww.huanxung.cn

TS:   (3.14159).toFixed(2)
来源：http://cn.bookmarksfly.cn

Java: String.format("%.2f", 3.14159)
来源：http://ts.lnxyls.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jv.nszjky.cn

Ruby: format("%.2f", 3.14159)
来源：http://gj.huanxung.cn

C#:   3.14159.ToString("F2")
来源：http://mm.newstarts.cn

[A22] 获取字符串长度
来源：http://se.yuntaijiaju.cn

Py:   len(s)
来源：http://ax.newstarts.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pg.shxzukj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tr.yuntaijiaju.cn

TS:   s.length
来源：http://an.bjjhwx.cn

Java: s.length()
来源：http://mr.newstarts.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://at.yuntaijiaju.cn

Ruby: s.length
来源：http://wp.hahajie.cn

C#:   s.Length
来源：http://bg.gzmigu.cn

[A23] 大小写转换
来源：http://yi.hahajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://kp.panjiajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jt.shxzukj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ky.lnxyls.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mk.hnjuh.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rc.huixinmuqiang.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vu.9csxet.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://na.yuexingan06.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://mb.bookmarksfly.cn

[A24] 去除首尾空白
来源：http://yt.yuexingan06.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://np.szxytkj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xv.chemitech.net.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://au.hahajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pm.colortex.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ph.jctech888.com.cn

Go:   strings.TrimSpace(s)
来源：http://so.newstarts.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vf.panjiajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lh.huixiangedu.cn

[A25] 字符串比较
来源：http://qg.nicolike.cn

Py:   s1 == s2; s1 != s2
来源：http://ji.szsharing.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vo.szsharing.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nw.shxzskj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yn.bjjhwx.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://na.521024.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://al.hahajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://jj.lnxyls.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bl.nszjky.cn

[A26] 类型转换总览
来源：http://he.muxihuayi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vo.yuntaijiaju.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cl.lnxyls.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jk.yuexingan06.cn

TS:   Number() String() Boolean() x as number
来源：http://xd.yuntaijiaju.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lu.szsharing.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ro.yuexingan06.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://tb.lnxyls.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cu.521024.cn

================================================================================
来源：http://nv.bookmarksfly.cn

B. 流程控制
来源：http://uu.521024.cn

================================================================================
来源：http://kz.bjjhwx.cn

[B01] 条件判断 if / else
来源：http://tc.wgjwhj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://fl.huixiangedu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zx.wgjwhj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://po.newstarts.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rr.nicolike.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://dw.bjjhwx.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zp.huanxung.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qv.521024.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wy.huixinmuqiang.cn

[B02] 多分支 else if / elif
来源：http://oj.huixinmuqiang.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://so.haigaiapp.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fm.huixinmuqiang.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bi.colortex.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hu.bookmarksfly.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oi.szxytkj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://re.jctech888.com.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://am.huixinmuqiang.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xs.yuexingan06.cn

[B03] switch / match / case
来源：http://xs.szsharing.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mp.shtwfgs.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zg.chemitech.net.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ri.newstarts.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gk.szxytkj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qq.wgjwhj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://sj.9csxet.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ou.gzmigu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wg.nszjky.cn

[B04] for 计数循环
来源：http://ux.wgjwhj.cn

Py:   for i in range(10): print(i)
来源：http://bo.bjjhwx.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://co.bookmarksfly.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dy.shtwfgs.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ic.chemitech.net.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jm.bjjhwx.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bs.muxihuayi.cn

Ruby: 10.times { |i| puts i }
来源：http://vz.chemitech.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cg.jctech888.com.cn

[B05] 遍历数组 / 列表
来源：http://ct.bookmarksfly.cn

Py:   for item in arr: print(item)
来源：http://pm.shxzukj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ot.bjjhwx.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://lx.szsharing.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://vx.huixinmuqiang.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ju.colortex.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://av.shtwfgs.cn

Ruby: arr.each { |item| puts item }
来源：http://ht.panjiajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nd.shxzskj.cn

[B06] 遍历字典 / 对象
来源：http://iq.szxytkj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ye.jctech888.com.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gd.newstarts.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://um.shxzukj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hp.jctech888.com.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://us.nszjky.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xw.nszjky.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sm.yuexingan06.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ap.yuexingan06.cn

[B07] while 循环
来源：http://tq.yuntaijiaju.cn

Py:   while i < 10: i += 1
来源：http://tf.nicolike.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gg.szsharing.cn

JS:   while (i < 10) { i++; }
来源：http://ew.huanxung.cn

TS:   while (i < 10) { i++; }
来源：http://gr.nszjky.cn

Java: while (i < 10) { i++; }
来源：http://kp.chemitech.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ud.nicolike.cn

Ruby: while i < 10; i += 1; end
来源：http://zo.wgjwhj.cn

C#:   while (i < 10) { i++; }
来源：http://si.chemitech.net.cn

[B08] do-while（至少执行一次）
来源：http://xf.colortex.cn

Py:   # 无 do-while：用 while True + break
来源：http://ti.9csxet.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zi.jianghongdianzi.cn

JS:   do { i++; } while (i < 10);
来源：http://os.nszjky.cn

TS:   do { i++; } while (i < 10);
来源：http://sp.asd995.cn

Java: do { i++; } while (i < 10);
来源：http://sq.nicolike.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://zn.haigaiapp.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ml.asd995.cn

C#:   do { i++; } while (i < 10);
来源：http://yz.panjiajie.cn

[B09] break 与 continue
来源：http://pa.wgjwhj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ga.jianghongdianzi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qg.newstarts.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cx.muxihuayi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ce.chemitech.net.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uy.muxihuayi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vt.panjiajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jb.bjjhwx.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zq.shxzskj.cn

[B10] 遍历同时拿索引
来源：http://by.yuexingan06.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nd.newstarts.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ve.huixiangedu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cd.jianghongdianzi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://as.szxytkj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wn.jianghongdianzi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wr.jianghongdianzi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kq.colortex.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ms.jctech888.com.cn

[B11] 生成数字序列 / 区间
来源：http://qn.bookmarksfly.cn

Py:   list(range(0, 10, 2))
来源：http://in.chemitech.net.cn

PHP:  range(0, 10, 2);
来源：http://tb.jctech888.com.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ol.szxytkj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ec.szxytkj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://on.wgjwhj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://to.colortex.cn

Ruby: (0...10).step(2).to_a
来源：http://kq.szxytkj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qo.asd995.cn

[B12] 跳出多层循环
来源：http://kp.chemitech.net.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bl.bjjhwx.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://lb.panjiajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yg.hnjuh.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ur.szsharing.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nd.newstarts.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ct.yuexingan06.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://na.hahajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qm.shtwfgs.cn

[B13] 判断是否为数字
来源：http://ii.asd995.cn

Py:   isinstance(x, (int, float))
来源：http://rn.hnjuh.cn

PHP:  is_numeric($x)
来源：http://pr.bjjhwx.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fm.9csxet.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hs.huanxung.cn

Java: x instanceof Number
来源：http://hw.wgjwhj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kx.521024.cn

Ruby: x.is_a?(Numeric)
来源：http://jc.jianghongdianzi.cn

C#:   x is int or double or decimal
来源：http://gc.panjiajie.cn

[B14] 判断值是否在集合内
来源：http://lx.huanxung.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://is.szsharing.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nh.yuntaijiaju.cn

JS:   [1, 2, 3].includes(x)
来源：http://cn.nicolike.cn

TS:   [1, 2, 3].includes(x)
来源：http://jt.huixinmuqiang.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ej.hnjuh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ja.panjiajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rb.szxytkj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yf.gzmigu.cn

[B15] 布尔运算与取反
来源：http://tn.shxzskj.cn

Py:   a and b or not c
来源：http://pp.huanxung.cn

PHP:  $a && $b || !$c
来源：http://qa.huixinmuqiang.cn

JS:   a && b || !c
来源：http://ur.szsharing.cn

TS:   a && b || !c
来源：http://nj.jianghongdianzi.cn

Java: a && b || !c
来源：http://lm.chemitech.net.cn

Go:   a && b || !c
来源：http://mz.lnxyls.cn

Ruby: a && b || !c
来源：http://bm.hahajie.cn

C#:   a && b || !c
来源：http://gh.muxihuayi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://rg.panjiajie.cn

Py:   if not data: return
来源：http://cz.521024.cn

PHP:  if (!$data) { return; }
来源：http://be.yuexingan06.cn

JS:   if (!data) return;
来源：http://kt.shxzukj.cn

TS:   if (!data) return;
来源：http://il.nszjky.cn

Java: if (data == null) return;
来源：http://gv.panjiajie.cn

Go:   if data == nil { return }
来源：http://gb.shtwfgs.cn

Ruby: return if data.nil?
来源：http://si.shtwfgs.cn

C#:   if (data == null) return;
来源：http://ee.huixiangedu.cn

================================================================================
来源：http://in.jianghongdianzi.cn

C. 函数与作用域
来源：http://cv.9csxet.cn

================================================================================
来源：http://cg.asd995.cn

[C01] 定义函数
来源：http://op.yuexingan06.cn

Py:   def add(a, b): return a + b
来源：http://tz.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lp.gzmigu.cn

JS:   function add(a, b) { return a + b; }
来源：http://fz.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jm.shtwfgs.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dn.huanxung.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ar.asd995.cn

Ruby: def add(a, b); a + b; end
来源：http://dx.shxzskj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gc.szxytkj.cn

[C02] 默认参数
来源：http://bp.szxytkj.cn

Py:   def greet(name="World"): return name
来源：http://ej.hahajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ci.jianghongdianzi.cn

JS:   function greet(name = "World") { return name; }
来源：http://ni.jctech888.com.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lu.panjiajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://uv.bjjhwx.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ip.chemitech.net.cn

Ruby: def greet(name = "World") = name
来源：http://xv.yuntaijiaju.cn

C#:   string Greet(string name = "World") => name;
来源：http://ip.bookmarksfly.cn

[C03] 可变参数
来源：http://ak.wgjwhj.cn

Py:   def total(*args): return sum(args)
来源：http://tc.szsharing.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ef.hnjuh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xu.muxihuayi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://iz.panjiajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wj.chemitech.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sx.jctech888.com.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hb.gzmigu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hk.shxzskj.cn

[C04] 命名参数 / 关键字参数
来源：http://ba.szsharing.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://eo.shxzskj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fh.lnxyls.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wq.huixiangedu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://my.jctech888.com.cn

Java: // 无：用 Builder 模式或 record
来源：http://jf.521024.cn

Go:   // 无：用配置结构体参数
来源：http://qa.newstarts.cn

Ruby: f(a: 1, b: 2)
来源：http://jd.bjjhwx.cn

C#:   f(a: 1, b: 2)
来源：http://ex.shtwfgs.cn

[C05] 返回多个值
来源：http://ba.9csxet.cn

Py:   return a, b
来源：http://uf.szsharing.cn

PHP:  return [$a, $b];
来源：http://rq.huanxung.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://el.521024.cn

TS:   return { a, b };
来源：http://jy.szsharing.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ar.9csxet.cn

Go:   return a, b
来源：http://eh.colortex.cn

Ruby: return a, b
来源：http://ty.asd995.cn

C#:   return (a, b);              // ValueTuple
来源：http://ub.chemitech.net.cn

[C06] 匿名函数 / lambda
来源：http://to.bjjhwx.cn

Py:   square = lambda x: x * x
来源：http://ld.muxihuayi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://tx.gzmigu.cn

JS:   const square = x => x * x;
来源：http://ha.shtwfgs.cn

TS:   const square = (x: number): number => x * x;
来源：http://ik.szsharing.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kj.jctech888.com.cn

Go:   sq := func(x int) int { return x * x }
来源：http://cm.nicolike.cn

Ruby: square = ->(x) { x * x }
来源：http://st.shxzukj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hk.521024.cn

[C07] 把函数作为参数传入
来源：http://jv.huixiangedu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://an.bjjhwx.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xr.gzmigu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pc.colortex.cn

TS:   arr.map(String)
来源：http://ob.shxzukj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xl.jianghongdianzi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://em.gzmigu.cn

Ruby: arr.map(&:upcase)
来源：http://nb.yuntaijiaju.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://yv.yuexingan06.cn

[C08] 闭包
来源：http://qf.nicolike.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kb.jctech888.com.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lp.huixiangedu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xc.chemitech.net.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uc.jianghongdianzi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wg.yuntaijiaju.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xc.lnxyls.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://oq.lnxyls.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://la.hahajie.cn

[C09] 递归
来源：http://bj.huixiangedu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uw.bookmarksfly.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nk.hnjuh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mw.newstarts.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ia.colortex.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fo.panjiajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://id.yuexingan06.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kd.huixinmuqiang.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://as.yuexingan06.cn


<!-- 参考信息 -->