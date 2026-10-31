代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pb.asd995.cn

Ruby: gets.chomp
来源：http://oe.lnxyls.cn

C#:   Console.ReadLine();
来源：http://sn.szxytkj.cn

[A21] 保留指定小数位输出
来源：http://zh.jianghongdianzi.cn

Py:   f"{3.14159:.2f}"
来源：http://br.bookmarksfly.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mm.nszjky.cn

JS:   (3.14159).toFixed(2)
来源：http://or.yuexingan06.cn

TS:   (3.14159).toFixed(2)
来源：http://jy.asd995.cn

Java: String.format("%.2f", 3.14159)
来源：http://ho.nszjky.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://av.chemitech.net.cn

Ruby: format("%.2f", 3.14159)
来源：http://tw.hahajie.cn

C#:   3.14159.ToString("F2")
来源：http://sl.bookmarksfly.cn

[A22] 获取字符串长度
来源：http://sc.muxihuayi.cn

Py:   len(s)
来源：http://xz.chemitech.net.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://al.521024.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qa.shxzukj.cn

TS:   s.length
来源：http://ci.huanxung.cn

Java: s.length()
来源：http://fk.lnxyls.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://yu.hahajie.cn

Ruby: s.length
来源：http://bv.asd995.cn

C#:   s.Length
来源：http://qm.lnxyls.cn

[A23] 大小写转换
来源：http://nl.asd995.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://np.chemitech.net.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kz.huanxung.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xd.yuntaijiaju.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hw.gzmigu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ui.shxzskj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wu.szxytkj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yk.jctech888.com.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://im.yuexingan06.cn

[A24] 去除首尾空白
来源：http://ht.jctech888.com.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://yl.jctech888.com.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sh.yuexingan06.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lz.521024.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qv.newstarts.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rj.lnxyls.cn

Go:   strings.TrimSpace(s)
来源：http://zl.9csxet.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bl.jctech888.com.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tt.jctech888.com.cn

[A25] 字符串比较
来源：http://ga.huixinmuqiang.cn

Py:   s1 == s2; s1 != s2
来源：http://lu.szsharing.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://oq.9csxet.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pz.wgjwhj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xe.szxytkj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xo.wgjwhj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ji.yuntaijiaju.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://bi.nicolike.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yx.nicolike.cn

[A26] 类型转换总览
来源：http://yw.newstarts.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wl.muxihuayi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cb.haigaiapp.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gq.huixinmuqiang.cn

TS:   Number() String() Boolean() x as number
来源：http://hw.shtwfgs.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://aj.asd995.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ag.asd995.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://cl.jianghongdianzi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uu.szxytkj.cn

================================================================================
来源：http://bj.hnjuh.cn

B. 流程控制
来源：http://zg.huanxung.cn

================================================================================
来源：http://jm.gzmigu.cn

[B01] 条件判断 if / else
来源：http://ui.9csxet.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://yq.nszjky.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ii.huixiangedu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zz.yuexingan06.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jo.colortex.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ag.hahajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yh.nicolike.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sf.huixiangedu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://an.muxihuayi.cn

[B02] 多分支 else if / elif
来源：http://fz.bjjhwx.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nd.wgjwhj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vq.shtwfgs.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zo.bjjhwx.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://im.gzmigu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gr.huixiangedu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cr.szxytkj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wi.newstarts.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ji.shxzukj.cn

[B03] switch / match / case
来源：http://ky.huanxung.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ld.asd995.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wu.hahajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kq.gzmigu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kc.huanxung.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ci.hnjuh.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ha.asd995.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rz.shxzskj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lv.bjjhwx.cn

[B04] for 计数循环
来源：http://fw.szsharing.cn

Py:   for i in range(10): print(i)
来源：http://at.hnjuh.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cv.gzmigu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yt.hnjuh.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ym.bjjhwx.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://io.asd995.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cr.szsharing.cn

Ruby: 10.times { |i| puts i }
来源：http://be.nszjky.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nf.huixiangedu.cn

[B05] 遍历数组 / 列表
来源：http://mn.nszjky.cn

Py:   for item in arr: print(item)
来源：http://hy.nicolike.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rm.colortex.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hr.9csxet.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bf.nszjky.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://js.huixiangedu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sa.shtwfgs.cn

Ruby: arr.each { |item| puts item }
来源：http://kt.panjiajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ks.hahajie.cn

[B06] 遍历字典 / 对象
来源：http://sx.asd995.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://oo.shtwfgs.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qe.shxzskj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pg.shxzskj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://di.lnxyls.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cx.bjjhwx.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yb.huixiangedu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gv.bookmarksfly.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lp.shtwfgs.cn

[B07] while 循环
来源：http://bq.newstarts.cn

Py:   while i < 10: i += 1
来源：http://sa.asd995.cn

PHP:  while ($i < 10) { $i++; }
来源：http://cv.szxytkj.cn

JS:   while (i < 10) { i++; }
来源：http://cu.huanxung.cn

TS:   while (i < 10) { i++; }
来源：http://gu.asd995.cn

Java: while (i < 10) { i++; }
来源：http://sv.shxzukj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ln.wgjwhj.cn

Ruby: while i < 10; i += 1; end
来源：http://xx.521024.cn

C#:   while (i < 10) { i++; }
来源：http://im.haigaiapp.cn

[B08] do-while（至少执行一次）
来源：http://ir.colortex.cn

Py:   # 无 do-while：用 while True + break
来源：http://vk.huixiangedu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://kp.huanxung.cn

JS:   do { i++; } while (i < 10);
来源：http://gu.asd995.cn

TS:   do { i++; } while (i < 10);
来源：http://ew.shxzukj.cn

Java: do { i++; } while (i < 10);
来源：http://cl.haigaiapp.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fa.hnjuh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ou.shxzskj.cn

C#:   do { i++; } while (i < 10);
来源：http://jy.bjjhwx.cn

[B09] break 与 continue
来源：http://os.lnxyls.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ma.nszjky.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xy.shtwfgs.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qb.szsharing.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ao.szxytkj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yr.panjiajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tv.521024.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ly.shtwfgs.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://na.gzmigu.cn

[B10] 遍历同时拿索引
来源：http://ah.9csxet.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ik.panjiajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sg.nszjky.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bo.gzmigu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vn.9csxet.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sc.huanxung.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zf.huixiangedu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vb.huanxung.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ee.huixiangedu.cn

[B11] 生成数字序列 / 区间
来源：http://gw.newstarts.cn

Py:   list(range(0, 10, 2))
来源：http://ry.huixiangedu.cn

PHP:  range(0, 10, 2);
来源：http://sw.jianghongdianzi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gb.panjiajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kl.yuexingan06.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nq.jctech888.com.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zr.huixinmuqiang.cn

Ruby: (0...10).step(2).to_a
来源：http://ik.521024.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kq.hnjuh.cn

[B12] 跳出多层循环
来源：http://ll.9csxet.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ve.521024.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://io.szxytkj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ad.colortex.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vz.shxzskj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mg.yuexingan06.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cm.bookmarksfly.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dw.yuexingan06.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://iy.nszjky.cn

[B13] 判断是否为数字
来源：http://zm.yuexingan06.cn

Py:   isinstance(x, (int, float))
来源：http://cb.bookmarksfly.cn

PHP:  is_numeric($x)
来源：http://zq.szxytkj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wl.lnxyls.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ku.yuntaijiaju.cn

Java: x instanceof Number
来源：http://zt.shtwfgs.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ia.gzmigu.cn

Ruby: x.is_a?(Numeric)
来源：http://aq.asd995.cn

C#:   x is int or double or decimal
来源：http://fi.yuexingan06.cn

[B14] 判断值是否在集合内
来源：http://xz.shtwfgs.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xe.jianghongdianzi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kf.nicolike.cn

JS:   [1, 2, 3].includes(x)
来源：http://nw.bookmarksfly.cn

TS:   [1, 2, 3].includes(x)
来源：http://ln.haigaiapp.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://no.jctech888.com.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ny.yuexingan06.cn

Ruby: [1, 2, 3].include?(x)
来源：http://iq.wgjwhj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pc.panjiajie.cn

[B15] 布尔运算与取反
来源：http://vu.bjjhwx.cn

Py:   a and b or not c
来源：http://kz.shxzskj.cn

PHP:  $a && $b || !$c
来源：http://gn.haigaiapp.cn

JS:   a && b || !c
来源：http://zq.jianghongdianzi.cn

TS:   a && b || !c
来源：http://hd.wgjwhj.cn

Java: a && b || !c
来源：http://bs.bjjhwx.cn

Go:   a && b || !c
来源：http://my.asd995.cn

Ruby: a && b || !c
来源：http://dm.hahajie.cn

C#:   a && b || !c
来源：http://zp.huanxung.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vt.huixinmuqiang.cn

Py:   if not data: return
来源：http://co.nszjky.cn

PHP:  if (!$data) { return; }
来源：http://hi.chemitech.net.cn

JS:   if (!data) return;
来源：http://oz.huanxung.cn

TS:   if (!data) return;
来源：http://ms.huixinmuqiang.cn

Java: if (data == null) return;
来源：http://ey.yuntaijiaju.cn

Go:   if data == nil { return }
来源：http://kh.shxzukj.cn

Ruby: return if data.nil?
来源：http://yd.haigaiapp.cn

C#:   if (data == null) return;
来源：http://ru.521024.cn

================================================================================
来源：http://dj.gzmigu.cn

C. 函数与作用域
来源：http://lw.nszjky.cn

================================================================================
来源：http://jy.yuexingan06.cn

[C01] 定义函数
来源：http://nk.huixinmuqiang.cn

Py:   def add(a, b): return a + b
来源：http://fr.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://af.shxzskj.cn

JS:   function add(a, b) { return a + b; }
来源：http://ux.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://st.shxzskj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://cz.521024.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jt.lnxyls.cn

Ruby: def add(a, b); a + b; end
来源：http://jv.szsharing.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ut.muxihuayi.cn

[C02] 默认参数
来源：http://zz.jctech888.com.cn

Py:   def greet(name="World"): return name
来源：http://wk.asd995.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ua.asd995.cn

JS:   function greet(name = "World") { return name; }
来源：http://hx.asd995.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vg.muxihuayi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://pr.chemitech.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yu.521024.cn

Ruby: def greet(name = "World") = name
来源：http://uz.lnxyls.cn

C#:   string Greet(string name = "World") => name;
来源：http://dd.hnjuh.cn

[C03] 可变参数
来源：http://eu.bookmarksfly.cn

Py:   def total(*args): return sum(args)
来源：http://iv.huixiangedu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://us.szxytkj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vh.colortex.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vi.yuexingan06.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://es.szxytkj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ha.huanxung.cn

Ruby: def total(*nums); nums.sum; end
来源：http://od.haigaiapp.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ro.gzmigu.cn

[C04] 命名参数 / 关键字参数
来源：http://jg.huixiangedu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sf.hnjuh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yu.newstarts.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kr.bookmarksfly.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ih.szsharing.cn

Java: // 无：用 Builder 模式或 record
来源：http://zh.szsharing.cn

Go:   // 无：用配置结构体参数
来源：http://jv.chemitech.net.cn

Ruby: f(a: 1, b: 2)
来源：http://ca.hnjuh.cn

C#:   f(a: 1, b: 2)
来源：http://jp.wgjwhj.cn

[C05] 返回多个值
来源：http://xp.asd995.cn

Py:   return a, b
来源：http://ww.9csxet.cn

PHP:  return [$a, $b];
来源：http://jr.huixinmuqiang.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ct.muxihuayi.cn

TS:   return { a, b };
来源：http://ln.hahajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ho.nszjky.cn

Go:   return a, b
来源：http://cl.nicolike.cn

Ruby: return a, b
来源：http://yg.chemitech.net.cn

C#:   return (a, b);              // ValueTuple
来源：http://am.wgjwhj.cn

[C06] 匿名函数 / lambda
来源：http://ri.szxytkj.cn

Py:   square = lambda x: x * x
来源：http://aa.9csxet.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ef.huanxung.cn

JS:   const square = x => x * x;
来源：http://ej.9csxet.cn

TS:   const square = (x: number): number => x * x;
来源：http://yf.lnxyls.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zb.hahajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://uk.szxytkj.cn

Ruby: square = ->(x) { x * x }
来源：http://gt.asd995.cn

C#:   Func<int, int> square = x => x * x;
来源：http://en.nicolike.cn

[C07] 把函数作为参数传入
来源：http://gj.jctech888.com.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tk.hahajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://dv.wgjwhj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dy.jianghongdianzi.cn

TS:   arr.map(String)
来源：http://wj.wgjwhj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lc.hnjuh.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://eo.hnjuh.cn

Ruby: arr.map(&:upcase)
来源：http://mb.colortex.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ez.huanxung.cn

[C08] 闭包
来源：http://jh.chemitech.net.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wp.huanxung.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://er.muxihuayi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ho.huixinmuqiang.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jr.szxytkj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zi.muxihuayi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nl.newstarts.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://js.chemitech.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uk.jctech888.com.cn

[C09] 递归
来源：http://kw.colortex.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cy.huixinmuqiang.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://an.shxzukj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oa.jctech888.com.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://so.shtwfgs.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kd.shtwfgs.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jb.huanxung.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://oo.newstarts.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cc.muxihuayi.cn

[C10] 变量作用域
来源：http://xe.shxzskj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lx.huanxung.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zn.nicolike.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ia.jctech888.com.cn

TS:   同 JS
来源：http://ht.colortex.cn

Java: 方法内为块级作用域
来源：http://hr.yuntaijiaju.cn

Go:   花括号块级作用域
来源：http://ug.bookmarksfly.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://or.asd995.cn

C#:   块级作用域
来源：http://lv.shxzskj.cn

[C11] 模块导入与导出
来源：http://rp.bookmarksfly.cn

Py:   from module import func
来源：http://ut.yuexingan06.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://rp.521024.cn


<!-- 参考信息 -->