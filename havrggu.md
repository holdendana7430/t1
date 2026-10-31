代发 wailian999

Ruby: a, b = b, a
来源：http://fg.szxytkj.cn

C#:   (a, b) = (b, a);
来源：http://bl.szsharing.cn

[A20] 读取标准输入
来源：http://aj.shxzukj.cn

Py:   name = input("请输入：")
来源：http://df.chemitech.net.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://dz.gzmigu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qa.yuexingan06.cn

TS:   // Node.js：readline 模块
来源：http://tk.huanxung.cn

Java: new Scanner(System.in).nextLine()
来源：http://nl.huanxung.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ib.asd995.cn

Ruby: gets.chomp
来源：http://hm.yuntaijiaju.cn

C#:   Console.ReadLine();
来源：http://co.hahajie.cn

[A21] 保留指定小数位输出
来源：http://jg.shxzskj.cn

Py:   f"{3.14159:.2f}"
来源：http://qu.hnjuh.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hr.521024.cn

JS:   (3.14159).toFixed(2)
来源：http://yl.hahajie.cn

TS:   (3.14159).toFixed(2)
来源：http://nr.9csxet.cn

Java: String.format("%.2f", 3.14159)
来源：http://qh.jianghongdianzi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ml.gzmigu.cn

Ruby: format("%.2f", 3.14159)
来源：http://fd.shtwfgs.cn

C#:   3.14159.ToString("F2")
来源：http://zu.hahajie.cn

[A22] 获取字符串长度
来源：http://nf.huanxung.cn

Py:   len(s)
来源：http://fq.lnxyls.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jh.muxihuayi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jt.9csxet.cn

TS:   s.length
来源：http://tm.muxihuayi.cn

Java: s.length()
来源：http://rw.muxihuayi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ng.shxzukj.cn

Ruby: s.length
来源：http://kg.huanxung.cn

C#:   s.Length
来源：http://nv.yuexingan06.cn

[A23] 大小写转换
来源：http://tk.wgjwhj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ht.wgjwhj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bt.szsharing.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fi.shtwfgs.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yh.yuexingan06.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hr.bjjhwx.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pa.shxzskj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pm.shtwfgs.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ft.szxytkj.cn

[A24] 去除首尾空白
来源：http://bd.chemitech.net.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ir.bookmarksfly.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lv.wgjwhj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ua.jctech888.com.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bn.hahajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://de.lnxyls.cn

Go:   strings.TrimSpace(s)
来源：http://oz.colortex.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hv.nszjky.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jz.shxzukj.cn

[A25] 字符串比较
来源：http://pc.wgjwhj.cn

Py:   s1 == s2; s1 != s2
来源：http://eh.hahajie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cr.9csxet.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://sm.huixiangedu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ww.shtwfgs.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://oo.9csxet.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pm.huixiangedu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://kn.bjjhwx.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dz.haigaiapp.cn

[A26] 类型转换总览
来源：http://pj.panjiajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zo.jianghongdianzi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ph.muxihuayi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ym.shtwfgs.cn

TS:   Number() String() Boolean() x as number
来源：http://yd.chemitech.net.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hn.huixinmuqiang.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sa.shxzskj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://do.asd995.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ft.jianghongdianzi.cn

================================================================================
来源：http://bs.shxzukj.cn

B. 流程控制
来源：http://oi.haigaiapp.cn

================================================================================
来源：http://hr.wgjwhj.cn

[B01] 条件判断 if / else
来源：http://qh.asd995.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ym.asd995.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ew.huanxung.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pv.gzmigu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gp.szsharing.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ri.9csxet.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kz.hnjuh.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xn.yuexingan06.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jg.muxihuayi.cn

[B02] 多分支 else if / elif
来源：http://go.huanxung.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tt.yuntaijiaju.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bd.haigaiapp.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yw.yuntaijiaju.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mn.hnjuh.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iu.szxytkj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xg.yuntaijiaju.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tl.asd995.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://od.hahajie.cn

[B03] switch / match / case
来源：http://pn.521024.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ac.shxzukj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rx.yuexingan06.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xu.newstarts.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uj.lnxyls.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ts.huixinmuqiang.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dq.huanxung.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ab.szxytkj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qx.szxytkj.cn

[B04] for 计数循环
来源：http://in.lnxyls.cn

Py:   for i in range(10): print(i)
来源：http://jm.bjjhwx.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cj.haigaiapp.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mz.chemitech.net.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nu.hahajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jk.9csxet.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cc.yuexingan06.cn

Ruby: 10.times { |i| puts i }
来源：http://el.bjjhwx.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bz.panjiajie.cn

[B05] 遍历数组 / 列表
来源：http://ex.huixinmuqiang.cn

Py:   for item in arr: print(item)
来源：http://bm.9csxet.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://iu.colortex.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yg.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gn.nicolike.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jg.panjiajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nl.huanxung.cn

Ruby: arr.each { |item| puts item }
来源：http://we.chemitech.net.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zh.hnjuh.cn

[B06] 遍历字典 / 对象
来源：http://bm.hahajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ax.gzmigu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tk.chemitech.net.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dc.bookmarksfly.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uk.521024.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://me.asd995.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dv.newstarts.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wb.muxihuayi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ce.newstarts.cn

[B07] while 循环
来源：http://xu.panjiajie.cn

Py:   while i < 10: i += 1
来源：http://gn.muxihuayi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fi.jianghongdianzi.cn

JS:   while (i < 10) { i++; }
来源：http://pf.newstarts.cn

TS:   while (i < 10) { i++; }
来源：http://sf.9csxet.cn

Java: while (i < 10) { i++; }
来源：http://qe.9csxet.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sv.shtwfgs.cn

Ruby: while i < 10; i += 1; end
来源：http://aa.szsharing.cn

C#:   while (i < 10) { i++; }
来源：http://gj.wgjwhj.cn

[B08] do-while（至少执行一次）
来源：http://rd.9csxet.cn

Py:   # 无 do-while：用 while True + break
来源：http://uj.jianghongdianzi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://si.shxzskj.cn

JS:   do { i++; } while (i < 10);
来源：http://ac.nszjky.cn

TS:   do { i++; } while (i < 10);
来源：http://yg.yuntaijiaju.cn

Java: do { i++; } while (i < 10);
来源：http://ur.nicolike.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sw.bookmarksfly.cn

Ruby: begin; i += 1; end while i < 10
来源：http://oi.shxzskj.cn

C#:   do { i++; } while (i < 10);
来源：http://mf.shxzukj.cn

[B09] break 与 continue
来源：http://ye.colortex.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ll.hahajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ym.jianghongdianzi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iz.szxytkj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rb.shxzskj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uf.szsharing.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zk.shtwfgs.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://es.newstarts.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gz.shxzskj.cn

[B10] 遍历同时拿索引
来源：http://jy.asd995.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wt.shtwfgs.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ot.newstarts.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ao.panjiajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gs.wgjwhj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nw.muxihuayi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bp.gzmigu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nj.shxzukj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ll.hnjuh.cn

[B11] 生成数字序列 / 区间
来源：http://cw.lnxyls.cn

Py:   list(range(0, 10, 2))
来源：http://ha.colortex.cn

PHP:  range(0, 10, 2);
来源：http://cl.huanxung.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vw.lnxyls.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jc.hnjuh.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yy.huanxung.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qh.colortex.cn

Ruby: (0...10).step(2).to_a
来源：http://ql.panjiajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qt.yuntaijiaju.cn

[B12] 跳出多层循环
来源：http://jp.colortex.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wl.huixiangedu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ub.shtwfgs.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bt.wgjwhj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zq.huanxung.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qo.jctech888.com.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nq.521024.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lr.szsharing.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ht.wgjwhj.cn

[B13] 判断是否为数字
来源：http://ac.9csxet.cn

Py:   isinstance(x, (int, float))
来源：http://om.huixinmuqiang.cn

PHP:  is_numeric($x)
来源：http://nx.lnxyls.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lg.haigaiapp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ql.szxytkj.cn

Java: x instanceof Number
来源：http://xm.newstarts.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://np.shxzukj.cn

Ruby: x.is_a?(Numeric)
来源：http://te.huanxung.cn

C#:   x is int or double or decimal
来源：http://le.521024.cn

[B14] 判断值是否在集合内
来源：http://sy.jctech888.com.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cj.wgjwhj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vk.colortex.cn

JS:   [1, 2, 3].includes(x)
来源：http://xh.jctech888.com.cn

TS:   [1, 2, 3].includes(x)
来源：http://eq.colortex.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vb.hahajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xh.newstarts.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mt.nicolike.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ow.huixiangedu.cn

[B15] 布尔运算与取反
来源：http://mc.huixinmuqiang.cn

Py:   a and b or not c
来源：http://gt.huixinmuqiang.cn

PHP:  $a && $b || !$c
来源：http://kw.jianghongdianzi.cn

JS:   a && b || !c
来源：http://ih.huixinmuqiang.cn

TS:   a && b || !c
来源：http://al.wgjwhj.cn

Java: a && b || !c
来源：http://mp.gzmigu.cn

Go:   a && b || !c
来源：http://eq.panjiajie.cn

Ruby: a && b || !c
来源：http://nj.9csxet.cn

C#:   a && b || !c
来源：http://zo.bjjhwx.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jq.nszjky.cn

Py:   if not data: return
来源：http://gx.shxzskj.cn

PHP:  if (!$data) { return; }
来源：http://ai.jctech888.com.cn

JS:   if (!data) return;
来源：http://vw.9csxet.cn

TS:   if (!data) return;
来源：http://rz.szxytkj.cn

Java: if (data == null) return;
来源：http://ps.panjiajie.cn

Go:   if data == nil { return }
来源：http://lr.521024.cn

Ruby: return if data.nil?
来源：http://rz.9csxet.cn

C#:   if (data == null) return;
来源：http://im.huixiangedu.cn

================================================================================
来源：http://he.huixinmuqiang.cn

C. 函数与作用域
来源：http://qo.huanxung.cn

================================================================================
来源：http://ea.szxytkj.cn

[C01] 定义函数
来源：http://tu.muxihuayi.cn

Py:   def add(a, b): return a + b
来源：http://ck.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rm.521024.cn

JS:   function add(a, b) { return a + b; }
来源：http://ln.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lf.521024.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://jx.shxzukj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://td.jctech888.com.cn

Ruby: def add(a, b); a + b; end
来源：http://mr.newstarts.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xy.huixinmuqiang.cn

[C02] 默认参数
来源：http://rm.haigaiapp.cn

Py:   def greet(name="World"): return name
来源：http://ip.hahajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vr.huixinmuqiang.cn

JS:   function greet(name = "World") { return name; }
来源：http://pw.muxihuayi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://va.jianghongdianzi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://my.jianghongdianzi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kc.szxytkj.cn

Ruby: def greet(name = "World") = name
来源：http://qo.bjjhwx.cn

C#:   string Greet(string name = "World") => name;
来源：http://lf.bookmarksfly.cn

[C03] 可变参数
来源：http://cm.newstarts.cn

Py:   def total(*args): return sum(args)
来源：http://kf.jianghongdianzi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vr.newstarts.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xy.huanxung.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wa.shtwfgs.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bp.asd995.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sd.huixinmuqiang.cn

Ruby: def total(*nums); nums.sum; end
来源：http://nm.huixiangedu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dh.huixiangedu.cn

[C04] 命名参数 / 关键字参数
来源：http://ll.shxzukj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zi.yuexingan06.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ss.colortex.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ci.asd995.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wi.9csxet.cn

Java: // 无：用 Builder 模式或 record
来源：http://cj.gzmigu.cn

Go:   // 无：用配置结构体参数
来源：http://jf.wgjwhj.cn

Ruby: f(a: 1, b: 2)
来源：http://gl.bjjhwx.cn

C#:   f(a: 1, b: 2)
来源：http://qg.yuntaijiaju.cn

[C05] 返回多个值
来源：http://pv.szxytkj.cn

Py:   return a, b
来源：http://sd.shtwfgs.cn

PHP:  return [$a, $b];
来源：http://fl.hahajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://br.bookmarksfly.cn

TS:   return { a, b };
来源：http://xt.shxzukj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rd.gzmigu.cn

Go:   return a, b
来源：http://mg.huanxung.cn

Ruby: return a, b
来源：http://ag.nszjky.cn

C#:   return (a, b);              // ValueTuple
来源：http://fw.colortex.cn

[C06] 匿名函数 / lambda
来源：http://ed.szsharing.cn

Py:   square = lambda x: x * x
来源：http://qx.panjiajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://lc.9csxet.cn

JS:   const square = x => x * x;
来源：http://tn.yuntaijiaju.cn

TS:   const square = (x: number): number => x * x;
来源：http://ci.yuexingan06.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vy.huanxung.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xg.yuexingan06.cn

Ruby: square = ->(x) { x * x }
来源：http://pi.colortex.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bs.wgjwhj.cn

[C07] 把函数作为参数传入
来源：http://ux.colortex.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qj.shxzukj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://mi.yuexingan06.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ml.haigaiapp.cn

TS:   arr.map(String)
来源：http://uo.chemitech.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sh.panjiajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yf.shxzukj.cn

Ruby: arr.map(&:upcase)
来源：http://gc.jctech888.com.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://bi.nszjky.cn

[C08] 闭包
来源：http://vm.muxihuayi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://sl.haigaiapp.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ju.huanxung.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://of.lnxyls.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yr.yuexingan06.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qs.huanxung.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://se.yuntaijiaju.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ba.gzmigu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mq.lnxyls.cn

[C09] 递归
来源：http://hs.newstarts.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://eh.asd995.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dh.hnjuh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ix.wgjwhj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oj.nicolike.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kj.jianghongdianzi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ok.nicolike.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vz.huixiangedu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sy.wgjwhj.cn

[C10] 变量作用域
来源：http://af.muxihuayi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yg.panjiajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ds.nicolike.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fx.haigaiapp.cn


<!-- 参考信息 -->