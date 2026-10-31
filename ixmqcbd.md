代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://re.chemitech.net.cn

Ruby: gets.chomp
来源：http://qw.shxzukj.cn

C#:   Console.ReadLine();
来源：http://le.muxihuayi.cn

[A21] 保留指定小数位输出
来源：http://pr.huixiangedu.cn

Py:   f"{3.14159:.2f}"
来源：http://qa.newstarts.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hy.shxzukj.cn

JS:   (3.14159).toFixed(2)
来源：http://oz.newstarts.cn

TS:   (3.14159).toFixed(2)
来源：http://vc.521024.cn

Java: String.format("%.2f", 3.14159)
来源：http://gg.yuexingan06.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hu.shxzukj.cn

Ruby: format("%.2f", 3.14159)
来源：http://yg.nszjky.cn

C#:   3.14159.ToString("F2")
来源：http://pb.bjjhwx.cn

[A22] 获取字符串长度
来源：http://hi.shxzskj.cn

Py:   len(s)
来源：http://xt.newstarts.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xc.asd995.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kl.hahajie.cn

TS:   s.length
来源：http://rh.hnjuh.cn

Java: s.length()
来源：http://di.chemitech.net.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wk.huanxung.cn

Ruby: s.length
来源：http://nw.nszjky.cn

C#:   s.Length
来源：http://kb.9csxet.cn

[A23] 大小写转换
来源：http://hb.szxytkj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://xe.hahajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ea.szxytkj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mt.shtwfgs.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zg.panjiajie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xh.jianghongdianzi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bm.jctech888.com.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wl.yuntaijiaju.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://gc.muxihuayi.cn

[A24] 去除首尾空白
来源：http://xy.szsharing.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ru.jctech888.com.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://py.gzmigu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ir.szxytkj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gd.nszjky.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ce.haigaiapp.cn

Go:   strings.TrimSpace(s)
来源：http://ln.chemitech.net.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://at.yuntaijiaju.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gs.nicolike.cn

[A25] 字符串比较
来源：http://ju.nicolike.cn

Py:   s1 == s2; s1 != s2
来源：http://fx.yuntaijiaju.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ju.newstarts.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xz.bookmarksfly.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kz.huixiangedu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xf.shxzskj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xv.hahajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://oo.szxytkj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hn.huixinmuqiang.cn

[A26] 类型转换总览
来源：http://im.yuexingan06.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ak.shxzskj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://my.shtwfgs.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hh.hnjuh.cn

TS:   Number() String() Boolean() x as number
来源：http://ta.bjjhwx.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pt.szsharing.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://es.asd995.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://wy.jianghongdianzi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ls.newstarts.cn

================================================================================
来源：http://sx.colortex.cn

B. 流程控制
来源：http://to.haigaiapp.cn

================================================================================
来源：http://hc.9csxet.cn

[B01] 条件判断 if / else
来源：http://kk.huixiangedu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vb.huixiangedu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tr.newstarts.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://im.bjjhwx.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fr.jianghongdianzi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ro.shxzskj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://iy.asd995.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rp.lnxyls.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gg.newstarts.cn

[B02] 多分支 else if / elif
来源：http://ew.bjjhwx.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jo.newstarts.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mq.wgjwhj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bg.haigaiapp.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mc.hnjuh.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bn.jctech888.com.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nr.wgjwhj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vz.bookmarksfly.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ty.haigaiapp.cn

[B03] switch / match / case
来源：http://of.lnxyls.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xd.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ts.lnxyls.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://aq.huixinmuqiang.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qz.hahajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vm.shxzskj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://py.shtwfgs.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gm.lnxyls.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://oc.wgjwhj.cn

[B04] for 计数循环
来源：http://om.huixiangedu.cn

Py:   for i in range(10): print(i)
来源：http://sr.huanxung.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zc.nszjky.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hj.nicolike.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fu.colortex.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wh.panjiajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jj.newstarts.cn

Ruby: 10.times { |i| puts i }
来源：http://un.bookmarksfly.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xq.lnxyls.cn

[B05] 遍历数组 / 列表
来源：http://yx.colortex.cn

Py:   for item in arr: print(item)
来源：http://os.9csxet.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://eo.hahajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dm.chemitech.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://aq.chemitech.net.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yz.yuexingan06.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zh.521024.cn

Ruby: arr.each { |item| puts item }
来源：http://fb.asd995.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ec.lnxyls.cn

[B06] 遍历字典 / 对象
来源：http://yi.jianghongdianzi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mn.szsharing.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pe.hnjuh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vv.jctech888.com.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ar.huixiangedu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ba.shtwfgs.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kn.bjjhwx.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qe.nszjky.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tu.muxihuayi.cn

[B07] while 循环
来源：http://fp.jctech888.com.cn

Py:   while i < 10: i += 1
来源：http://cg.asd995.cn

PHP:  while ($i < 10) { $i++; }
来源：http://tq.nszjky.cn

JS:   while (i < 10) { i++; }
来源：http://ka.yuntaijiaju.cn

TS:   while (i < 10) { i++; }
来源：http://sz.nicolike.cn

Java: while (i < 10) { i++; }
来源：http://sy.hnjuh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xf.9csxet.cn

Ruby: while i < 10; i += 1; end
来源：http://yg.szsharing.cn

C#:   while (i < 10) { i++; }
来源：http://pi.panjiajie.cn

[B08] do-while（至少执行一次）
来源：http://rw.yuexingan06.cn

Py:   # 无 do-while：用 while True + break
来源：http://yr.huanxung.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://dc.9csxet.cn

JS:   do { i++; } while (i < 10);
来源：http://tn.shxzukj.cn

TS:   do { i++; } while (i < 10);
来源：http://ek.shxzukj.cn

Java: do { i++; } while (i < 10);
来源：http://zg.muxihuayi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://yu.huixinmuqiang.cn

Ruby: begin; i += 1; end while i < 10
来源：http://my.panjiajie.cn

C#:   do { i++; } while (i < 10);
来源：http://vw.yuexingan06.cn

[B09] break 与 continue
来源：http://vh.bookmarksfly.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kk.muxihuayi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dl.wgjwhj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wx.szsharing.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eu.hnjuh.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yw.chemitech.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wv.hahajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://uh.lnxyls.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://py.521024.cn

[B10] 遍历同时拿索引
来源：http://ph.newstarts.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cn.bookmarksfly.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hu.muxihuayi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vn.szxytkj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://an.shxzskj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fi.muxihuayi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qh.szxytkj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xt.jctech888.com.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wx.colortex.cn

[B11] 生成数字序列 / 区间
来源：http://uh.jianghongdianzi.cn

Py:   list(range(0, 10, 2))
来源：http://sq.jctech888.com.cn

PHP:  range(0, 10, 2);
来源：http://yh.szsharing.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lu.chemitech.net.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sh.huixiangedu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rx.jianghongdianzi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://us.haigaiapp.cn

Ruby: (0...10).step(2).to_a
来源：http://pq.haigaiapp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rh.nicolike.cn

[B12] 跳出多层循环
来源：http://qo.521024.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://dk.yuexingan06.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://uc.nszjky.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tz.asd995.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pw.muxihuayi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ib.lnxyls.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dr.bjjhwx.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://aw.shxzukj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ir.nicolike.cn

[B13] 判断是否为数字
来源：http://gf.huanxung.cn

Py:   isinstance(x, (int, float))
来源：http://bl.shxzukj.cn

PHP:  is_numeric($x)
来源：http://ax.hnjuh.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fh.haigaiapp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xo.asd995.cn

Java: x instanceof Number
来源：http://xm.jctech888.com.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uv.haigaiapp.cn

Ruby: x.is_a?(Numeric)
来源：http://vm.nszjky.cn

C#:   x is int or double or decimal
来源：http://jw.newstarts.cn

[B14] 判断值是否在集合内
来源：http://vl.wgjwhj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hf.nicolike.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kb.yuntaijiaju.cn

JS:   [1, 2, 3].includes(x)
来源：http://zt.shtwfgs.cn

TS:   [1, 2, 3].includes(x)
来源：http://zo.yuexingan06.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://je.521024.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bk.asd995.cn

Ruby: [1, 2, 3].include?(x)
来源：http://tp.huixinmuqiang.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://og.gzmigu.cn

[B15] 布尔运算与取反
来源：http://ta.huixinmuqiang.cn

Py:   a and b or not c
来源：http://cd.521024.cn

PHP:  $a && $b || !$c
来源：http://pp.jianghongdianzi.cn

JS:   a && b || !c
来源：http://fv.newstarts.cn

TS:   a && b || !c
来源：http://yj.hnjuh.cn

Java: a && b || !c
来源：http://la.haigaiapp.cn

Go:   a && b || !c
来源：http://ou.bookmarksfly.cn

Ruby: a && b || !c
来源：http://ic.huixiangedu.cn

C#:   a && b || !c
来源：http://xd.chemitech.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://un.jianghongdianzi.cn

Py:   if not data: return
来源：http://xx.shxzukj.cn

PHP:  if (!$data) { return; }
来源：http://jv.lnxyls.cn

JS:   if (!data) return;
来源：http://ap.haigaiapp.cn

TS:   if (!data) return;
来源：http://yw.521024.cn

Java: if (data == null) return;
来源：http://rf.panjiajie.cn

Go:   if data == nil { return }
来源：http://og.panjiajie.cn

Ruby: return if data.nil?
来源：http://ps.hnjuh.cn

C#:   if (data == null) return;
来源：http://av.szsharing.cn

================================================================================
来源：http://tp.shxzskj.cn

C. 函数与作用域
来源：http://vr.asd995.cn

================================================================================
来源：http://am.521024.cn

[C01] 定义函数
来源：http://bf.haigaiapp.cn

Py:   def add(a, b): return a + b
来源：http://mr.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dw.newstarts.cn

JS:   function add(a, b) { return a + b; }
来源：http://oj.szxytkj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kf.szsharing.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://oq.haigaiapp.cn

Go:   func add(a, b int) int { return a + b }
来源：http://un.huixiangedu.cn

Ruby: def add(a, b); a + b; end
来源：http://qq.chemitech.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yk.gzmigu.cn

[C02] 默认参数
来源：http://vi.nicolike.cn

Py:   def greet(name="World"): return name
来源：http://ru.asd995.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lk.jctech888.com.cn

JS:   function greet(name = "World") { return name; }
来源：http://gd.521024.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ck.newstarts.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://mw.shtwfgs.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://je.bookmarksfly.cn

Ruby: def greet(name = "World") = name
来源：http://cc.chemitech.net.cn

C#:   string Greet(string name = "World") => name;
来源：http://zw.hnjuh.cn

[C03] 可变参数
来源：http://vn.huixiangedu.cn

Py:   def total(*args): return sum(args)
来源：http://vm.newstarts.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://os.huanxung.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nz.newstarts.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ti.panjiajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sb.huixiangedu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://db.lnxyls.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tg.hahajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://su.lnxyls.cn

[C04] 命名参数 / 关键字参数
来源：http://jb.asd995.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kd.gzmigu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lc.asd995.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cy.shxzukj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ws.panjiajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://gs.haigaiapp.cn

Go:   // 无：用配置结构体参数
来源：http://vw.huixinmuqiang.cn

Ruby: f(a: 1, b: 2)
来源：http://zc.asd995.cn

C#:   f(a: 1, b: 2)
来源：http://ky.shxzskj.cn

[C05] 返回多个值
来源：http://iy.szxytkj.cn

Py:   return a, b
来源：http://fk.huanxung.cn

PHP:  return [$a, $b];
来源：http://ax.shxzukj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://tw.yuntaijiaju.cn

TS:   return { a, b };
来源：http://sp.haigaiapp.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qy.colortex.cn

Go:   return a, b
来源：http://jm.wgjwhj.cn

Ruby: return a, b
来源：http://ri.muxihuayi.cn

C#:   return (a, b);              // ValueTuple
来源：http://gr.shtwfgs.cn

[C06] 匿名函数 / lambda
来源：http://cl.yuntaijiaju.cn

Py:   square = lambda x: x * x
来源：http://ps.szsharing.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://cv.huixiangedu.cn

JS:   const square = x => x * x;
来源：http://uz.jctech888.com.cn

TS:   const square = (x: number): number => x * x;
来源：http://hd.huanxung.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nf.521024.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dc.shtwfgs.cn

Ruby: square = ->(x) { x * x }
来源：http://fw.huixiangedu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://rz.huanxung.cn

[C07] 把函数作为参数传入
来源：http://yu.hahajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://as.huanxung.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ab.haigaiapp.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sr.muxihuayi.cn

TS:   arr.map(String)
来源：http://yn.yuexingan06.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://iv.bookmarksfly.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hi.chemitech.net.cn

Ruby: arr.map(&:upcase)
来源：http://bi.gzmigu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pj.shtwfgs.cn

[C08] 闭包
来源：http://xa.nicolike.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kz.huixiangedu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mg.wgjwhj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ns.521024.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://je.nicolike.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ul.nicolike.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wx.asd995.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yg.huanxung.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ee.panjiajie.cn

[C09] 递归
来源：http://wy.521024.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rh.szxytkj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://py.lnxyls.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hl.szsharing.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ma.yuexingan06.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://oh.hnjuh.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cm.muxihuayi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lh.lnxyls.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wo.bjjhwx.cn

[C10] 变量作用域
来源：http://di.panjiajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qw.colortex.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://br.lnxyls.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://of.szxytkj.cn

TS:   同 JS
来源：http://zu.huanxung.cn

Java: 方法内为块级作用域
来源：http://yt.muxihuayi.cn

Go:   花括号块级作用域
来源：http://bx.chemitech.net.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cb.hahajie.cn

C#:   块级作用域
来源：http://sy.szxytkj.cn

[C11] 模块导入与导出
来源：http://mo.szsharing.cn

Py:   from module import func
来源：http://is.bjjhwx.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kr.521024.cn


<!-- 参考信息 -->