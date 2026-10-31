代发 wailian999

Ruby: a, b = b, a
来源：http://od.hahajie.cn

C#:   (a, b) = (b, a);
来源：http://dg.9csxet.cn

[A20] 读取标准输入
来源：http://lo.hnjuh.cn

Py:   name = input("请输入：")
来源：http://pf.huanxung.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.jianghongdianzi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://sd.huixinmuqiang.cn

TS:   // Node.js：readline 模块
来源：http://wa.shxzukj.cn

Java: new Scanner(System.in).nextLine()
来源：http://yg.muxihuayi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pb.szxytkj.cn

Ruby: gets.chomp
来源：http://sf.shtwfgs.cn

C#:   Console.ReadLine();
来源：http://ni.huanxung.cn

[A21] 保留指定小数位输出
来源：http://up.asd995.cn

Py:   f"{3.14159:.2f}"
来源：http://pf.huanxung.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rn.muxihuayi.cn

JS:   (3.14159).toFixed(2)
来源：http://cd.hnjuh.cn

TS:   (3.14159).toFixed(2)
来源：http://jq.newstarts.cn

Java: String.format("%.2f", 3.14159)
来源：http://mg.yuexingan06.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://dx.huanxung.cn

Ruby: format("%.2f", 3.14159)
来源：http://va.huixinmuqiang.cn

C#:   3.14159.ToString("F2")
来源：http://dy.jctech888.com.cn

[A22] 获取字符串长度
来源：http://ss.jctech888.com.cn

Py:   len(s)
来源：http://yb.wgjwhj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://li.asd995.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ih.huixiangedu.cn

TS:   s.length
来源：http://ph.colortex.cn

Java: s.length()
来源：http://kv.jianghongdianzi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mr.bjjhwx.cn

Ruby: s.length
来源：http://cr.lnxyls.cn

C#:   s.Length
来源：http://kd.521024.cn

[A23] 大小写转换
来源：http://wb.szxytkj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://fg.9csxet.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wk.yuntaijiaju.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://om.muxihuayi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://om.huanxung.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://uu.muxihuayi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xo.521024.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ll.huanxung.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://xq.shxzukj.cn

[A24] 去除首尾空白
来源：http://oq.szxytkj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qh.newstarts.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://by.haigaiapp.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bt.panjiajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qm.hnjuh.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wa.szsharing.cn

Go:   strings.TrimSpace(s)
来源：http://zv.nicolike.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hl.jianghongdianzi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fe.hahajie.cn

[A25] 字符串比较
来源：http://ra.huixinmuqiang.cn

Py:   s1 == s2; s1 != s2
来源：http://dr.shxzskj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qj.nicolike.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pw.hnjuh.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://sd.jianghongdianzi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lm.shxzukj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rr.hnjuh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://pz.newstarts.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nx.wgjwhj.cn

[A26] 类型转换总览
来源：http://uo.yuntaijiaju.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://po.jianghongdianzi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pd.nszjky.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://oh.huixinmuqiang.cn

TS:   Number() String() Boolean() x as number
来源：http://hc.lnxyls.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qr.shxzukj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://oe.yuexingan06.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zg.shtwfgs.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nr.bookmarksfly.cn

================================================================================
来源：http://vy.nicolike.cn

B. 流程控制
来源：http://ls.yuexingan06.cn

================================================================================
来源：http://ci.haigaiapp.cn

[B01] 条件判断 if / else
来源：http://ws.nicolike.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wh.shxzukj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tg.nicolike.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://au.huanxung.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vy.yuexingan06.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://uw.huanxung.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hd.shxzskj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ic.jctech888.com.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fk.shxzukj.cn

[B02] 多分支 else if / elif
来源：http://dz.nicolike.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hg.nszjky.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zu.521024.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lq.huixinmuqiang.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eu.chemitech.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uv.hahajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ls.szsharing.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ea.huanxung.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qu.haigaiapp.cn

[B03] switch / match / case
来源：http://gu.shtwfgs.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://up.hnjuh.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gj.bookmarksfly.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ju.nicolike.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ey.yuntaijiaju.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zd.huanxung.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zf.hnjuh.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ss.hnjuh.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hj.hahajie.cn

[B04] for 计数循环
来源：http://ku.asd995.cn

Py:   for i in range(10): print(i)
来源：http://vk.nicolike.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sp.jctech888.com.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://op.yuexingan06.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hi.9csxet.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wt.lnxyls.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://oe.huixiangedu.cn

Ruby: 10.times { |i| puts i }
来源：http://nw.nicolike.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dp.hahajie.cn

[B05] 遍历数组 / 列表
来源：http://kg.shxzskj.cn

Py:   for item in arr: print(item)
来源：http://dx.shxzukj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fj.bjjhwx.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ld.newstarts.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gk.521024.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qg.shxzskj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ol.chemitech.net.cn

Ruby: arr.each { |item| puts item }
来源：http://cj.huixiangedu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xa.shxzukj.cn

[B06] 遍历字典 / 对象
来源：http://af.shxzukj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hh.shxzukj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://on.jianghongdianzi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ki.chemitech.net.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mz.shxzskj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tn.colortex.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lx.bjjhwx.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ur.hahajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://am.521024.cn

[B07] while 循环
来源：http://su.shxzskj.cn

Py:   while i < 10: i += 1
来源：http://lr.shtwfgs.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wj.shxzskj.cn

JS:   while (i < 10) { i++; }
来源：http://zc.bjjhwx.cn

TS:   while (i < 10) { i++; }
来源：http://kw.szxytkj.cn

Java: while (i < 10) { i++; }
来源：http://zz.bjjhwx.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ci.szsharing.cn

Ruby: while i < 10; i += 1; end
来源：http://is.shxzskj.cn

C#:   while (i < 10) { i++; }
来源：http://wr.yuexingan06.cn

[B08] do-while（至少执行一次）
来源：http://dr.jianghongdianzi.cn

Py:   # 无 do-while：用 while True + break
来源：http://lu.haigaiapp.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vb.muxihuayi.cn

JS:   do { i++; } while (i < 10);
来源：http://cr.jianghongdianzi.cn

TS:   do { i++; } while (i < 10);
来源：http://ku.colortex.cn

Java: do { i++; } while (i < 10);
来源：http://pj.shtwfgs.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wu.szxytkj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://yi.huanxung.cn

C#:   do { i++; } while (i < 10);
来源：http://wd.nicolike.cn

[B09] break 与 continue
来源：http://ry.shxzskj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rh.colortex.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pp.wgjwhj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pw.shtwfgs.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fr.colortex.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://na.lnxyls.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://oj.shtwfgs.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ai.yuntaijiaju.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bv.muxihuayi.cn

[B10] 遍历同时拿索引
来源：http://ua.chemitech.net.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ku.shtwfgs.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ah.9csxet.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fv.521024.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pn.hahajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dw.huixinmuqiang.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vj.haigaiapp.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ta.hahajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://uq.bookmarksfly.cn

[B11] 生成数字序列 / 区间
来源：http://fj.bjjhwx.cn

Py:   list(range(0, 10, 2))
来源：http://ze.huixinmuqiang.cn

PHP:  range(0, 10, 2);
来源：http://sw.hnjuh.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hm.yuexingan06.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fj.shxzukj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sl.huixinmuqiang.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wp.521024.cn

Ruby: (0...10).step(2).to_a
来源：http://de.yuntaijiaju.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vp.huixiangedu.cn

[B12] 跳出多层循环
来源：http://nw.bookmarksfly.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ly.colortex.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://dv.nicolike.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://oa.huanxung.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hs.huixiangedu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zw.nicolike.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ur.nicolike.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xk.gzmigu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pp.bookmarksfly.cn

[B13] 判断是否为数字
来源：http://dl.huanxung.cn

Py:   isinstance(x, (int, float))
来源：http://rx.bookmarksfly.cn

PHP:  is_numeric($x)
来源：http://pz.yuexingan06.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yt.jianghongdianzi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tg.bjjhwx.cn

Java: x instanceof Number
来源：http://js.lnxyls.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nz.wgjwhj.cn

Ruby: x.is_a?(Numeric)
来源：http://qq.huixinmuqiang.cn

C#:   x is int or double or decimal
来源：http://ot.shtwfgs.cn

[B14] 判断值是否在集合内
来源：http://oc.jianghongdianzi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zw.hahajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gj.shxzukj.cn

JS:   [1, 2, 3].includes(x)
来源：http://pm.jctech888.com.cn

TS:   [1, 2, 3].includes(x)
来源：http://ro.gzmigu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://go.colortex.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://aq.nicolike.cn

Ruby: [1, 2, 3].include?(x)
来源：http://sz.huanxung.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://eu.9csxet.cn

[B15] 布尔运算与取反
来源：http://bd.muxihuayi.cn

Py:   a and b or not c
来源：http://ef.shxzukj.cn

PHP:  $a && $b || !$c
来源：http://hb.jctech888.com.cn

JS:   a && b || !c
来源：http://qo.nszjky.cn

TS:   a && b || !c
来源：http://ed.shxzskj.cn

Java: a && b || !c
来源：http://wi.bookmarksfly.cn

Go:   a && b || !c
来源：http://zo.newstarts.cn

Ruby: a && b || !c
来源：http://kk.shxzukj.cn

C#:   a && b || !c
来源：http://gc.nszjky.cn

[B16] 卫语句：不满足条件提前返回
来源：http://wg.colortex.cn

Py:   if not data: return
来源：http://fc.muxihuayi.cn

PHP:  if (!$data) { return; }
来源：http://iw.huixinmuqiang.cn

JS:   if (!data) return;
来源：http://kl.huixiangedu.cn

TS:   if (!data) return;
来源：http://qt.yuexingan06.cn

Java: if (data == null) return;
来源：http://wl.521024.cn

Go:   if data == nil { return }
来源：http://yb.huixiangedu.cn

Ruby: return if data.nil?
来源：http://ms.yuntaijiaju.cn

C#:   if (data == null) return;
来源：http://bj.9csxet.cn

================================================================================
来源：http://fn.gzmigu.cn

C. 函数与作用域
来源：http://xg.bjjhwx.cn

================================================================================
来源：http://pd.shxzukj.cn

[C01] 定义函数
来源：http://ah.huanxung.cn

Py:   def add(a, b): return a + b
来源：http://by.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://am.9csxet.cn

JS:   function add(a, b) { return a + b; }
来源：http://am.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vd.haigaiapp.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://yg.gzmigu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vo.huixiangedu.cn

Ruby: def add(a, b); a + b; end
来源：http://gp.muxihuayi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qe.lnxyls.cn

[C02] 默认参数
来源：http://xj.nszjky.cn

Py:   def greet(name="World"): return name
来源：http://fi.szxytkj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://kp.asd995.cn

JS:   function greet(name = "World") { return name; }
来源：http://or.shxzskj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://eh.hnjuh.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://mb.lnxyls.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ue.huixinmuqiang.cn

Ruby: def greet(name = "World") = name
来源：http://jg.panjiajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://rg.nicolike.cn

[C03] 可变参数
来源：http://ix.bjjhwx.cn

Py:   def total(*args): return sum(args)
来源：http://ol.yuntaijiaju.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vh.szsharing.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ya.huanxung.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ux.jctech888.com.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zh.hnjuh.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://os.nicolike.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xr.lnxyls.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hs.szsharing.cn

[C04] 命名参数 / 关键字参数
来源：http://cm.nicolike.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qy.lnxyls.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nf.newstarts.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bm.9csxet.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fx.bjjhwx.cn

Java: // 无：用 Builder 模式或 record
来源：http://ca.yuntaijiaju.cn

Go:   // 无：用配置结构体参数
来源：http://ee.nicolike.cn

Ruby: f(a: 1, b: 2)
来源：http://yi.gzmigu.cn

C#:   f(a: 1, b: 2)
来源：http://dh.shxzukj.cn

[C05] 返回多个值
来源：http://hf.lnxyls.cn

Py:   return a, b
来源：http://pf.bjjhwx.cn

PHP:  return [$a, $b];
来源：http://ez.nszjky.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pe.shtwfgs.cn

TS:   return { a, b };
来源：http://bz.jianghongdianzi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hi.lnxyls.cn

Go:   return a, b
来源：http://er.nszjky.cn

Ruby: return a, b
来源：http://yg.yuntaijiaju.cn

C#:   return (a, b);              // ValueTuple
来源：http://jf.yuntaijiaju.cn

[C06] 匿名函数 / lambda
来源：http://ty.wgjwhj.cn

Py:   square = lambda x: x * x
来源：http://tl.shxzukj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://gt.nszjky.cn

JS:   const square = x => x * x;
来源：http://rx.9csxet.cn

TS:   const square = (x: number): number => x * x;
来源：http://ih.haigaiapp.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tc.gzmigu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wo.huixinmuqiang.cn

Ruby: square = ->(x) { x * x }
来源：http://fh.jianghongdianzi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dt.newstarts.cn

[C07] 把函数作为参数传入
来源：http://se.hnjuh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ap.szsharing.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jh.chemitech.net.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nd.szsharing.cn

TS:   arr.map(String)
来源：http://ss.szxytkj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jo.colortex.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ys.jianghongdianzi.cn

Ruby: arr.map(&:upcase)
来源：http://op.bjjhwx.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://eg.nicolike.cn

[C08] 闭包
来源：http://sf.haigaiapp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gb.hnjuh.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kv.muxihuayi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cw.szsharing.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ul.chemitech.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jk.bjjhwx.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yg.nszjky.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://je.yuntaijiaju.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://eb.colortex.cn

[C09] 递归
来源：http://td.huixinmuqiang.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gr.haigaiapp.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gf.nicolike.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://np.panjiajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bc.jianghongdianzi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hp.yuexingan06.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sj.bookmarksfly.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hl.chemitech.net.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fm.bookmarksfly.cn

[C10] 变量作用域
来源：http://ce.shxzskj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sb.nicolike.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://px.asd995.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qn.yuexingan06.cn


<!-- 参考信息 -->