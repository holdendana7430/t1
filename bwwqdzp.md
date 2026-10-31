代发 wailian999

JS:   [a, b] = [b, a];
来源：http://vp.lnxyls.cn

TS:   [a, b] = [b, a];
来源：http://dq.hahajie.cn

Java: int t = a; a = b; b = t;
来源：http://gd.bjjhwx.cn

Go:   a, b = b, a
来源：http://zp.newstarts.cn

Ruby: a, b = b, a
来源：http://rp.huixinmuqiang.cn

C#:   (a, b) = (b, a);
来源：http://ko.huixiangedu.cn

[A20] 读取标准输入
来源：http://zt.lnxyls.cn

Py:   name = input("请输入：")
来源：http://ch.szsharing.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://sh.hnjuh.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jp.nszjky.cn

TS:   // Node.js：readline 模块
来源：http://fu.haigaiapp.cn

Java: new Scanner(System.in).nextLine()
来源：http://qg.muxihuayi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bz.szsharing.cn

Ruby: gets.chomp
来源：http://po.muxihuayi.cn

C#:   Console.ReadLine();
来源：http://qa.9csxet.cn

[A21] 保留指定小数位输出
来源：http://al.wgjwhj.cn

Py:   f"{3.14159:.2f}"
来源：http://qn.haigaiapp.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cs.bookmarksfly.cn

JS:   (3.14159).toFixed(2)
来源：http://td.haigaiapp.cn

TS:   (3.14159).toFixed(2)
来源：http://se.colortex.cn

Java: String.format("%.2f", 3.14159)
来源：http://rz.bookmarksfly.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://rz.wgjwhj.cn

Ruby: format("%.2f", 3.14159)
来源：http://sq.yuexingan06.cn

C#:   3.14159.ToString("F2")
来源：http://zi.nicolike.cn

[A22] 获取字符串长度
来源：http://fh.huixinmuqiang.cn

Py:   len(s)
来源：http://yh.wgjwhj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bk.huanxung.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zd.szsharing.cn

TS:   s.length
来源：http://aj.gzmigu.cn

Java: s.length()
来源：http://ez.panjiajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jq.yuexingan06.cn

Ruby: s.length
来源：http://lo.nszjky.cn

C#:   s.Length
来源：http://fw.colortex.cn

[A23] 大小写转换
来源：http://mz.nszjky.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zs.muxihuayi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mn.shxzukj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zb.jianghongdianzi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rt.hnjuh.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fy.huixinmuqiang.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sa.shtwfgs.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gi.lnxyls.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://vk.bookmarksfly.cn

[A24] 去除首尾空白
来源：http://cq.muxihuayi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://kz.gzmigu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://av.521024.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yq.gzmigu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gh.muxihuayi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tn.huanxung.cn

Go:   strings.TrimSpace(s)
来源：http://db.colortex.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zc.hnjuh.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kf.szsharing.cn

[A25] 字符串比较
来源：http://su.szxytkj.cn

Py:   s1 == s2; s1 != s2
来源：http://ym.yuntaijiaju.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zu.huixiangedu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fe.bjjhwx.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yu.9csxet.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qy.hnjuh.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pu.nicolike.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rq.jianghongdianzi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pq.huixinmuqiang.cn

[A26] 类型转换总览
来源：http://bj.shtwfgs.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ft.huanxung.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vk.hnjuh.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fi.muxihuayi.cn

TS:   Number() String() Boolean() x as number
来源：http://ok.yuexingan06.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zn.newstarts.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zu.nicolike.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ng.yuntaijiaju.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yh.hahajie.cn

================================================================================
来源：http://rq.shxzskj.cn

B. 流程控制
来源：http://ba.gzmigu.cn

================================================================================
来源：http://tv.yuexingan06.cn

[B01] 条件判断 if / else
来源：http://kg.jianghongdianzi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bn.colortex.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zt.gzmigu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yq.jianghongdianzi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qg.hahajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xi.shtwfgs.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mr.chemitech.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hy.szxytkj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fx.huanxung.cn

[B02] 多分支 else if / elif
来源：http://ot.521024.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vv.haigaiapp.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yh.huixinmuqiang.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dp.colortex.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://du.nicolike.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mo.jianghongdianzi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vu.shxzskj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bx.shxzskj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://td.nicolike.cn

[B03] switch / match / case
来源：http://xn.521024.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bm.chemitech.net.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ad.shxzskj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nd.lnxyls.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qr.szsharing.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gm.haigaiapp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://il.gzmigu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nf.nszjky.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tx.521024.cn

[B04] for 计数循环
来源：http://wi.shxzskj.cn

Py:   for i in range(10): print(i)
来源：http://hl.bookmarksfly.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ph.shtwfgs.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ha.panjiajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wi.bookmarksfly.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ha.asd995.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://aq.bjjhwx.cn

Ruby: 10.times { |i| puts i }
来源：http://vp.colortex.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sq.muxihuayi.cn

[B05] 遍历数组 / 列表
来源：http://rm.wgjwhj.cn

Py:   for item in arr: print(item)
来源：http://cw.szsharing.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://aa.huixiangedu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://em.gzmigu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bb.huixinmuqiang.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://uw.bjjhwx.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jo.9csxet.cn

Ruby: arr.each { |item| puts item }
来源：http://ju.yuexingan06.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lk.huixinmuqiang.cn

[B06] 遍历字典 / 对象
来源：http://fr.wgjwhj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://kf.wgjwhj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://va.shxzukj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bt.gzmigu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uf.lnxyls.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sf.newstarts.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ly.colortex.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nb.bookmarksfly.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://en.9csxet.cn

[B07] while 循环
来源：http://du.huanxung.cn

Py:   while i < 10: i += 1
来源：http://qu.gzmigu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://oa.newstarts.cn

JS:   while (i < 10) { i++; }
来源：http://gu.huixinmuqiang.cn

TS:   while (i < 10) { i++; }
来源：http://wd.hnjuh.cn

Java: while (i < 10) { i++; }
来源：http://vk.521024.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vv.huixiangedu.cn

Ruby: while i < 10; i += 1; end
来源：http://ou.hahajie.cn

C#:   while (i < 10) { i++; }
来源：http://or.newstarts.cn

[B08] do-while（至少执行一次）
来源：http://qb.nszjky.cn

Py:   # 无 do-while：用 while True + break
来源：http://rz.huixinmuqiang.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cb.521024.cn

JS:   do { i++; } while (i < 10);
来源：http://sn.panjiajie.cn

TS:   do { i++; } while (i < 10);
来源：http://na.521024.cn

Java: do { i++; } while (i < 10);
来源：http://bv.colortex.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vf.colortex.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qg.9csxet.cn

C#:   do { i++; } while (i < 10);
来源：http://ex.nszjky.cn

[B09] break 与 continue
来源：http://gi.9csxet.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hu.9csxet.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kb.nszjky.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hc.asd995.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bo.szxytkj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iz.bookmarksfly.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yt.yuntaijiaju.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hr.nszjky.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nc.shxzskj.cn

[B10] 遍历同时拿索引
来源：http://wk.muxihuayi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cd.nszjky.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zq.huixinmuqiang.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qg.yuntaijiaju.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rh.jctech888.com.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ga.gzmigu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rn.huixinmuqiang.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ce.gzmigu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pi.nszjky.cn

[B11] 生成数字序列 / 区间
来源：http://hp.wgjwhj.cn

Py:   list(range(0, 10, 2))
来源：http://nk.yuexingan06.cn

PHP:  range(0, 10, 2);
来源：http://so.yuntaijiaju.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uh.lnxyls.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ns.jctech888.com.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kf.haigaiapp.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sj.huixiangedu.cn

Ruby: (0...10).step(2).to_a
来源：http://zp.wgjwhj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ov.colortex.cn

[B12] 跳出多层循环
来源：http://me.nszjky.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://jc.bjjhwx.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zv.yuexingan06.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gq.jctech888.com.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xc.nicolike.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xm.shxzskj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wb.jianghongdianzi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vg.hahajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hu.bjjhwx.cn

[B13] 判断是否为数字
来源：http://qj.shtwfgs.cn

Py:   isinstance(x, (int, float))
来源：http://we.shxzskj.cn

PHP:  is_numeric($x)
来源：http://uu.hahajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dz.muxihuayi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mp.huanxung.cn

Java: x instanceof Number
来源：http://su.shxzskj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cd.lnxyls.cn

Ruby: x.is_a?(Numeric)
来源：http://xd.nicolike.cn

C#:   x is int or double or decimal
来源：http://ua.newstarts.cn

[B14] 判断值是否在集合内
来源：http://jk.panjiajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zl.haigaiapp.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xq.yuntaijiaju.cn

JS:   [1, 2, 3].includes(x)
来源：http://ay.yuexingan06.cn

TS:   [1, 2, 3].includes(x)
来源：http://bs.521024.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://fq.bookmarksfly.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vb.hnjuh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://go.huixiangedu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kc.jianghongdianzi.cn

[B15] 布尔运算与取反
来源：http://gm.newstarts.cn

Py:   a and b or not c
来源：http://fw.huixiangedu.cn

PHP:  $a && $b || !$c
来源：http://xf.gzmigu.cn

JS:   a && b || !c
来源：http://wq.hahajie.cn

TS:   a && b || !c
来源：http://ox.huanxung.cn

Java: a && b || !c
来源：http://th.newstarts.cn

Go:   a && b || !c
来源：http://xn.9csxet.cn

Ruby: a && b || !c
来源：http://hw.muxihuayi.cn

C#:   a && b || !c
来源：http://kn.yuexingan06.cn

[B16] 卫语句：不满足条件提前返回
来源：http://wp.bookmarksfly.cn

Py:   if not data: return
来源：http://sv.muxihuayi.cn

PHP:  if (!$data) { return; }
来源：http://ae.chemitech.net.cn

JS:   if (!data) return;
来源：http://rp.szxytkj.cn

TS:   if (!data) return;
来源：http://ud.shtwfgs.cn

Java: if (data == null) return;
来源：http://xz.shxzskj.cn

Go:   if data == nil { return }
来源：http://kj.jctech888.com.cn

Ruby: return if data.nil?
来源：http://oh.521024.cn

C#:   if (data == null) return;
来源：http://ww.szsharing.cn

================================================================================
来源：http://ul.szxytkj.cn

C. 函数与作用域
来源：http://qm.chemitech.net.cn

================================================================================
来源：http://lv.hnjuh.cn

[C01] 定义函数
来源：http://zr.bjjhwx.cn

Py:   def add(a, b): return a + b
来源：http://pz.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xm.9csxet.cn

JS:   function add(a, b) { return a + b; }
来源：http://gd.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lr.panjiajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zj.nszjky.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ru.wgjwhj.cn

Ruby: def add(a, b); a + b; end
来源：http://yb.nszjky.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qi.haigaiapp.cn

[C02] 默认参数
来源：http://xr.bjjhwx.cn

Py:   def greet(name="World"): return name
来源：http://oe.hahajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://nq.szxytkj.cn

JS:   function greet(name = "World") { return name; }
来源：http://dt.huixiangedu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://pu.newstarts.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ub.colortex.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gu.shtwfgs.cn

Ruby: def greet(name = "World") = name
来源：http://ul.muxihuayi.cn

C#:   string Greet(string name = "World") => name;
来源：http://ca.gzmigu.cn

[C03] 可变参数
来源：http://xi.shxzukj.cn

Py:   def total(*args): return sum(args)
来源：http://le.asd995.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dj.huixinmuqiang.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dh.gzmigu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ac.lnxyls.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ey.chemitech.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fn.huanxung.cn

Ruby: def total(*nums); nums.sum; end
来源：http://in.muxihuayi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://op.huixiangedu.cn

[C04] 命名参数 / 关键字参数
来源：http://aw.hnjuh.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://iy.521024.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://aw.nszjky.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qi.521024.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yc.bookmarksfly.cn

Java: // 无：用 Builder 模式或 record
来源：http://oq.lnxyls.cn

Go:   // 无：用配置结构体参数
来源：http://hr.bookmarksfly.cn

Ruby: f(a: 1, b: 2)
来源：http://df.szxytkj.cn

C#:   f(a: 1, b: 2)
来源：http://fl.hnjuh.cn

[C05] 返回多个值
来源：http://ew.jctech888.com.cn

Py:   return a, b
来源：http://jr.huixiangedu.cn

PHP:  return [$a, $b];
来源：http://gw.huixinmuqiang.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ii.asd995.cn

TS:   return { a, b };
来源：http://yq.szxytkj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ry.shxzukj.cn

Go:   return a, b
来源：http://ep.colortex.cn

Ruby: return a, b
来源：http://ak.bjjhwx.cn

C#:   return (a, b);              // ValueTuple
来源：http://hm.huixinmuqiang.cn

[C06] 匿名函数 / lambda
来源：http://pp.yuexingan06.cn

Py:   square = lambda x: x * x
来源：http://jh.huixiangedu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://jt.chemitech.net.cn

JS:   const square = x => x * x;
来源：http://ap.bjjhwx.cn

TS:   const square = (x: number): number => x * x;
来源：http://ye.muxihuayi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ho.shtwfgs.cn

Go:   sq := func(x int) int { return x * x }
来源：http://tp.panjiajie.cn

Ruby: square = ->(x) { x * x }
来源：http://gj.chemitech.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ka.shtwfgs.cn

[C07] 把函数作为参数传入
来源：http://rs.muxihuayi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pc.shxzukj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://gf.jianghongdianzi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zv.bjjhwx.cn

TS:   arr.map(String)
来源：http://wi.nicolike.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mg.colortex.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://aw.9csxet.cn

Ruby: arr.map(&:upcase)
来源：http://rw.panjiajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://el.asd995.cn

[C08] 闭包
来源：http://gy.lnxyls.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bt.shtwfgs.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fj.huanxung.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cw.shtwfgs.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dl.bjjhwx.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ym.asd995.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ed.huixiangedu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vv.shtwfgs.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://es.hnjuh.cn

[C09] 递归
来源：http://ja.chemitech.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ad.gzmigu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mq.huixinmuqiang.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xk.shxzskj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dp.szsharing.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ly.asd995.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dl.wgjwhj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zg.nszjky.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mn.wgjwhj.cn


<!-- 参考信息 -->