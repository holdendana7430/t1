代发 wailian999

Ruby: a, b = b, a
来源：http://ci.lnxyls.cn

C#:   (a, b) = (b, a);
来源：http://wi.shxzukj.cn

[A20] 读取标准输入
来源：http://kf.hnjuh.cn

Py:   name = input("请输入：")
来源：http://ij.chemitech.net.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://jn.szxytkj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yg.szsharing.cn

TS:   // Node.js：readline 模块
来源：http://pd.huixiangedu.cn

Java: new Scanner(System.in).nextLine()
来源：http://lr.jianghongdianzi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zg.huixiangedu.cn

Ruby: gets.chomp
来源：http://yy.panjiajie.cn

C#:   Console.ReadLine();
来源：http://yd.chemitech.net.cn

[A21] 保留指定小数位输出
来源：http://de.szxytkj.cn

Py:   f"{3.14159:.2f}"
来源：http://ru.lnxyls.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qt.muxihuayi.cn

JS:   (3.14159).toFixed(2)
来源：http://zd.shxzskj.cn

TS:   (3.14159).toFixed(2)
来源：http://ed.wgjwhj.cn

Java: String.format("%.2f", 3.14159)
来源：http://ut.newstarts.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ht.newstarts.cn

Ruby: format("%.2f", 3.14159)
来源：http://ew.huixinmuqiang.cn

C#:   3.14159.ToString("F2")
来源：http://iz.jctech888.com.cn

[A22] 获取字符串长度
来源：http://ag.haigaiapp.cn

Py:   len(s)
来源：http://oi.yuntaijiaju.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nv.9csxet.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fi.colortex.cn

TS:   s.length
来源：http://wk.nicolike.cn

Java: s.length()
来源：http://dz.shxzskj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://uk.wgjwhj.cn

Ruby: s.length
来源：http://ho.gzmigu.cn

C#:   s.Length
来源：http://jk.wgjwhj.cn

[A23] 大小写转换
来源：http://rc.bjjhwx.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://by.wgjwhj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://sw.gzmigu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rq.muxihuayi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ct.jianghongdianzi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bn.shxzskj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vv.asd995.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lt.bookmarksfly.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://fj.newstarts.cn

[A24] 去除首尾空白
来源：http://xo.jctech888.com.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qe.huixinmuqiang.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mw.hahajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oq.newstarts.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wn.yuexingan06.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kw.lnxyls.cn

Go:   strings.TrimSpace(s)
来源：http://sf.newstarts.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pl.newstarts.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lb.lnxyls.cn

[A25] 字符串比较
来源：http://yw.shtwfgs.cn

Py:   s1 == s2; s1 != s2
来源：http://uv.colortex.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nn.huixiangedu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ch.gzmigu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wz.asd995.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lm.521024.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nf.hahajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://zg.nicolike.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bb.yuntaijiaju.cn

[A26] 类型转换总览
来源：http://jy.jctech888.com.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bj.jctech888.com.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hu.huanxung.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://eu.haigaiapp.cn

TS:   Number() String() Boolean() x as number
来源：http://cr.newstarts.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ue.lnxyls.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://eq.shxzskj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zd.szxytkj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zf.shxzskj.cn

================================================================================
来源：http://in.muxihuayi.cn

B. 流程控制
来源：http://rp.chemitech.net.cn

================================================================================
来源：http://md.hahajie.cn

[B01] 条件判断 if / else
来源：http://iz.huixiangedu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xh.yuexingan06.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nk.newstarts.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ol.lnxyls.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xy.jctech888.com.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://wi.newstarts.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ik.bjjhwx.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ei.muxihuayi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kf.shxzukj.cn

[B02] 多分支 else if / elif
来源：http://rj.haigaiapp.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ih.panjiajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://io.9csxet.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zp.bjjhwx.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qz.shxzukj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kv.newstarts.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tu.nszjky.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wy.521024.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pf.hahajie.cn

[B03] switch / match / case
来源：http://di.haigaiapp.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://re.9csxet.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nt.asd995.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zc.colortex.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fc.shxzukj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ar.9csxet.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bz.colortex.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://oj.jctech888.com.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tu.nszjky.cn

[B04] for 计数循环
来源：http://tn.huanxung.cn

Py:   for i in range(10): print(i)
来源：http://pu.huixinmuqiang.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ox.huixiangedu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ow.hnjuh.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://as.9csxet.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ol.chemitech.net.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dw.shtwfgs.cn

Ruby: 10.times { |i| puts i }
来源：http://sr.bjjhwx.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vl.szxytkj.cn

[B05] 遍历数组 / 列表
来源：http://el.hnjuh.cn

Py:   for item in arr: print(item)
来源：http://io.huixiangedu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sd.wgjwhj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://uz.hnjuh.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://hr.9csxet.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sv.huixiangedu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cm.jianghongdianzi.cn

Ruby: arr.each { |item| puts item }
来源：http://do.huixiangedu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cx.wgjwhj.cn

[B06] 遍历字典 / 对象
来源：http://rh.521024.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://kb.panjiajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://om.newstarts.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qb.bookmarksfly.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ks.shtwfgs.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://it.lnxyls.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://om.hnjuh.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ep.yuntaijiaju.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mz.haigaiapp.cn

[B07] while 循环
来源：http://is.shtwfgs.cn

Py:   while i < 10: i += 1
来源：http://qt.szxytkj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ps.shxzskj.cn

JS:   while (i < 10) { i++; }
来源：http://cg.shxzskj.cn

TS:   while (i < 10) { i++; }
来源：http://fq.521024.cn

Java: while (i < 10) { i++; }
来源：http://wh.muxihuayi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xz.bjjhwx.cn

Ruby: while i < 10; i += 1; end
来源：http://cj.bookmarksfly.cn

C#:   while (i < 10) { i++; }
来源：http://br.lnxyls.cn

[B08] do-while（至少执行一次）
来源：http://pd.yuexingan06.cn

Py:   # 无 do-while：用 while True + break
来源：http://za.huanxung.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xa.hnjuh.cn

JS:   do { i++; } while (i < 10);
来源：http://yi.shtwfgs.cn

TS:   do { i++; } while (i < 10);
来源：http://zb.haigaiapp.cn

Java: do { i++; } while (i < 10);
来源：http://wh.panjiajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sw.nszjky.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vi.huanxung.cn

C#:   do { i++; } while (i < 10);
来源：http://xy.huanxung.cn

[B09] break 与 continue
来源：http://se.jctech888.com.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dp.yuexingan06.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://la.szxytkj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vd.jctech888.com.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ga.521024.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xy.shxzukj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://az.szxytkj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sh.nicolike.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hm.szxytkj.cn

[B10] 遍历同时拿索引
来源：http://ub.muxihuayi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qe.asd995.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bf.521024.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gt.bjjhwx.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dc.szsharing.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yk.huixiangedu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gm.gzmigu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qp.yuntaijiaju.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ax.panjiajie.cn

[B11] 生成数字序列 / 区间
来源：http://ke.hahajie.cn

Py:   list(range(0, 10, 2))
来源：http://dm.9csxet.cn

PHP:  range(0, 10, 2);
来源：http://cg.wgjwhj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lt.huixiangedu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://si.shxzskj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hw.muxihuayi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bu.gzmigu.cn

Ruby: (0...10).step(2).to_a
来源：http://qb.shxzskj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sg.bookmarksfly.cn

[B12] 跳出多层循环
来源：http://tl.shtwfgs.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://au.huixiangedu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zy.huixinmuqiang.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://af.jctech888.com.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bb.lnxyls.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sm.bookmarksfly.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gd.bookmarksfly.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://eu.asd995.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ir.hahajie.cn

[B13] 判断是否为数字
来源：http://nd.huixiangedu.cn

Py:   isinstance(x, (int, float))
来源：http://yf.gzmigu.cn

PHP:  is_numeric($x)
来源：http://rf.shtwfgs.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mf.muxihuayi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lw.huanxung.cn

Java: x instanceof Number
来源：http://sy.9csxet.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://em.jctech888.com.cn

Ruby: x.is_a?(Numeric)
来源：http://sd.jctech888.com.cn

C#:   x is int or double or decimal
来源：http://qu.nszjky.cn

[B14] 判断值是否在集合内
来源：http://ie.szsharing.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gf.shxzskj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gz.muxihuayi.cn

JS:   [1, 2, 3].includes(x)
来源：http://vk.shxzskj.cn

TS:   [1, 2, 3].includes(x)
来源：http://ud.lnxyls.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hk.asd995.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fs.lnxyls.cn

Ruby: [1, 2, 3].include?(x)
来源：http://lw.lnxyls.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ou.yuntaijiaju.cn

[B15] 布尔运算与取反
来源：http://zh.shxzskj.cn

Py:   a and b or not c
来源：http://un.hahajie.cn

PHP:  $a && $b || !$c
来源：http://nq.chemitech.net.cn

JS:   a && b || !c
来源：http://uy.bookmarksfly.cn

TS:   a && b || !c
来源：http://uh.shtwfgs.cn

Java: a && b || !c
来源：http://rn.bjjhwx.cn

Go:   a && b || !c
来源：http://dq.muxihuayi.cn

Ruby: a && b || !c
来源：http://vh.shxzskj.cn

C#:   a && b || !c
来源：http://xj.bookmarksfly.cn

[B16] 卫语句：不满足条件提前返回
来源：http://cx.nicolike.cn

Py:   if not data: return
来源：http://lo.gzmigu.cn

PHP:  if (!$data) { return; }
来源：http://ti.asd995.cn

JS:   if (!data) return;
来源：http://xc.szsharing.cn

TS:   if (!data) return;
来源：http://kk.shxzskj.cn

Java: if (data == null) return;
来源：http://ya.haigaiapp.cn

Go:   if data == nil { return }
来源：http://vh.nszjky.cn

Ruby: return if data.nil?
来源：http://fn.nszjky.cn

C#:   if (data == null) return;
来源：http://am.wgjwhj.cn

================================================================================
来源：http://mm.bjjhwx.cn

C. 函数与作用域
来源：http://mh.yuexingan06.cn

================================================================================
来源：http://am.gzmigu.cn

[C01] 定义函数
来源：http://mr.colortex.cn

Py:   def add(a, b): return a + b
来源：http://sm.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yy.szsharing.cn

JS:   function add(a, b) { return a + b; }
来源：http://sl.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oy.jianghongdianzi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://jc.shxzukj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ho.wgjwhj.cn

Ruby: def add(a, b); a + b; end
来源：http://jw.asd995.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cr.chemitech.net.cn

[C02] 默认参数
来源：http://cp.shtwfgs.cn

Py:   def greet(name="World"): return name
来源：http://ui.bookmarksfly.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yw.bjjhwx.cn

JS:   function greet(name = "World") { return name; }
来源：http://yc.hnjuh.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://uj.nicolike.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vc.hnjuh.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dm.yuexingan06.cn

Ruby: def greet(name = "World") = name
来源：http://aa.shxzskj.cn

C#:   string Greet(string name = "World") => name;
来源：http://cu.shxzskj.cn

[C03] 可变参数
来源：http://xw.shxzskj.cn

Py:   def total(*args): return sum(args)
来源：http://kv.9csxet.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wj.9csxet.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mg.huixinmuqiang.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zq.panjiajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ca.jianghongdianzi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qx.muxihuayi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hf.bookmarksfly.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wm.wgjwhj.cn

[C04] 命名参数 / 关键字参数
来源：http://dj.panjiajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cr.shtwfgs.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zt.jianghongdianzi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zh.hahajie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dp.colortex.cn

Java: // 无：用 Builder 模式或 record
来源：http://jm.huixiangedu.cn

Go:   // 无：用配置结构体参数
来源：http://qd.jianghongdianzi.cn

Ruby: f(a: 1, b: 2)
来源：http://jf.9csxet.cn

C#:   f(a: 1, b: 2)
来源：http://gz.panjiajie.cn

[C05] 返回多个值
来源：http://dl.9csxet.cn

Py:   return a, b
来源：http://wa.shtwfgs.cn

PHP:  return [$a, $b];
来源：http://ha.huanxung.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ij.szsharing.cn

TS:   return { a, b };
来源：http://ov.jctech888.com.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ce.hnjuh.cn

Go:   return a, b
来源：http://yd.szsharing.cn

Ruby: return a, b
来源：http://sj.521024.cn

C#:   return (a, b);              // ValueTuple
来源：http://gs.haigaiapp.cn

[C06] 匿名函数 / lambda
来源：http://sf.haigaiapp.cn

Py:   square = lambda x: x * x
来源：http://vq.bookmarksfly.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ye.szxytkj.cn

JS:   const square = x => x * x;
来源：http://kl.szxytkj.cn

TS:   const square = (x: number): number => x * x;
来源：http://kj.huixiangedu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fy.newstarts.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ig.9csxet.cn

Ruby: square = ->(x) { x * x }
来源：http://wg.haigaiapp.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qd.shtwfgs.cn

[C07] 把函数作为参数传入
来源：http://tu.huixinmuqiang.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zu.lnxyls.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jn.hnjuh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uc.chemitech.net.cn

TS:   arr.map(String)
来源：http://ha.shtwfgs.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tw.521024.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hr.jianghongdianzi.cn

Ruby: arr.map(&:upcase)
来源：http://za.panjiajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://id.shxzukj.cn

[C08] 闭包
来源：http://hl.bookmarksfly.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://sc.newstarts.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://so.shxzukj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wx.hnjuh.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ey.shxzskj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ab.jianghongdianzi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ec.jctech888.com.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ek.huanxung.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lx.lnxyls.cn

[C09] 递归
来源：http://hs.yuexingan06.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mm.hnjuh.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lq.muxihuayi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tt.yuntaijiaju.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ro.huanxung.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hahajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mq.yuexingan06.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tz.panjiajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bb.lnxyls.cn

[C10] 变量作用域
来源：http://rr.bookmarksfly.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://do.shxzskj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wr.szxytkj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tj.jianghongdianzi.cn


<!-- 参考信息 -->