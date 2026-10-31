代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://pa.szsharing.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wb.colortex.cn

JS:   (3.14159).toFixed(2)
来源：http://ri.nicolike.cn

TS:   (3.14159).toFixed(2)
来源：http://mh.521024.cn

Java: String.format("%.2f", 3.14159)
来源：http://hr.yuexingan06.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vg.huixiangedu.cn

Ruby: format("%.2f", 3.14159)
来源：http://dr.huanxung.cn

C#:   3.14159.ToString("F2")
来源：http://dg.szsharing.cn

[A22] 获取字符串长度
来源：http://lb.muxihuayi.cn

Py:   len(s)
来源：http://ha.lnxyls.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xz.bjjhwx.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://li.wgjwhj.cn

TS:   s.length
来源：http://ly.bookmarksfly.cn

Java: s.length()
来源：http://ti.shxzukj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ty.gzmigu.cn

Ruby: s.length
来源：http://kl.newstarts.cn

C#:   s.Length
来源：http://js.shxzukj.cn

[A23] 大小写转换
来源：http://ir.yuntaijiaju.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ak.szxytkj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cv.newstarts.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fy.shxzskj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gi.shtwfgs.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://sr.jianghongdianzi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nk.colortex.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://io.muxihuayi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://de.bookmarksfly.cn

[A24] 去除首尾空白
来源：http://lz.bjjhwx.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://oo.shxzukj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rg.521024.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uk.huanxung.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cc.colortex.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ty.yuexingan06.cn

Go:   strings.TrimSpace(s)
来源：http://kq.huixiangedu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vo.nszjky.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://np.szsharing.cn

[A25] 字符串比较
来源：http://fe.lnxyls.cn

Py:   s1 == s2; s1 != s2
来源：http://nt.asd995.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fr.newstarts.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://sr.jianghongdianzi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://te.nicolike.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vy.lnxyls.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ji.hahajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://st.huixiangedu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://my.shxzskj.cn

[A26] 类型转换总览
来源：http://vg.yuexingan06.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ko.wgjwhj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ql.hahajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ii.newstarts.cn

TS:   Number() String() Boolean() x as number
来源：http://rz.haigaiapp.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dp.szxytkj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qv.huanxung.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://fw.shtwfgs.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://sr.huixinmuqiang.cn

================================================================================
来源：http://tb.shxzukj.cn

B. 流程控制
来源：http://yp.muxihuayi.cn

================================================================================
来源：http://fn.gzmigu.cn

[B01] 条件判断 if / else
来源：http://lj.hahajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xv.chemitech.net.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hb.jctech888.com.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://av.huanxung.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jj.huixiangedu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ci.huixiangedu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rc.panjiajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gm.yuntaijiaju.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qd.nszjky.cn

[B02] 多分支 else if / elif
来源：http://zg.jctech888.com.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xt.gzmigu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://js.asd995.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://da.nszjky.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qg.panjiajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yj.shxzukj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gb.wgjwhj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wq.huixinmuqiang.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tn.muxihuayi.cn

[B03] switch / match / case
来源：http://nu.haigaiapp.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bd.521024.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fd.szxytkj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yd.panjiajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zw.yuntaijiaju.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ab.gzmigu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pq.muxihuayi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jb.panjiajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mi.haigaiapp.cn

[B04] for 计数循环
来源：http://og.asd995.cn

Py:   for i in range(10): print(i)
来源：http://fc.asd995.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mv.wgjwhj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eu.wgjwhj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fv.wgjwhj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ar.jctech888.com.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qo.yuexingan06.cn

Ruby: 10.times { |i| puts i }
来源：http://mm.hahajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bq.szxytkj.cn

[B05] 遍历数组 / 列表
来源：http://px.shtwfgs.cn

Py:   for item in arr: print(item)
来源：http://ke.shxzskj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nh.gzmigu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zu.nszjky.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://kf.wgjwhj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gl.wgjwhj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fx.chemitech.net.cn

Ruby: arr.each { |item| puts item }
来源：http://nm.jctech888.com.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ek.bjjhwx.cn

[B06] 遍历字典 / 对象
来源：http://ek.panjiajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://cr.hahajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xt.hahajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pp.muxihuayi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cs.newstarts.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://es.hnjuh.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vf.hnjuh.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://va.jianghongdianzi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zw.asd995.cn

[B07] while 循环
来源：http://fq.yuexingan06.cn

Py:   while i < 10: i += 1
来源：http://vb.521024.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ub.hahajie.cn

JS:   while (i < 10) { i++; }
来源：http://bq.521024.cn

TS:   while (i < 10) { i++; }
来源：http://vt.jianghongdianzi.cn

Java: while (i < 10) { i++; }
来源：http://nt.yuntaijiaju.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ja.wgjwhj.cn

Ruby: while i < 10; i += 1; end
来源：http://eo.huanxung.cn

C#:   while (i < 10) { i++; }
来源：http://tj.bjjhwx.cn

[B08] do-while（至少执行一次）
来源：http://ti.huixinmuqiang.cn

Py:   # 无 do-while：用 while True + break
来源：http://gg.9csxet.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://dp.szxytkj.cn

JS:   do { i++; } while (i < 10);
来源：http://yx.wgjwhj.cn

TS:   do { i++; } while (i < 10);
来源：http://pp.bookmarksfly.cn

Java: do { i++; } while (i < 10);
来源：http://ww.huixinmuqiang.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bm.wgjwhj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://gd.jctech888.com.cn

C#:   do { i++; } while (i < 10);
来源：http://uv.nszjky.cn

[B09] break 与 continue
来源：http://uk.9csxet.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vb.jianghongdianzi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://de.lnxyls.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://os.newstarts.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vi.hnjuh.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lp.521024.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sh.yuntaijiaju.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zo.jctech888.com.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tw.huixinmuqiang.cn

[B10] 遍历同时拿索引
来源：http://ie.yuexingan06.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sw.yuntaijiaju.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dy.shtwfgs.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ir.jianghongdianzi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cb.shxzukj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://he.huixinmuqiang.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qc.muxihuayi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qp.gzmigu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jr.521024.cn

[B11] 生成数字序列 / 区间
来源：http://jc.jianghongdianzi.cn

Py:   list(range(0, 10, 2))
来源：http://pv.hahajie.cn

PHP:  range(0, 10, 2);
来源：http://uz.yuexingan06.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kd.chemitech.net.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wv.chemitech.net.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sm.shxzukj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fm.shtwfgs.cn

Ruby: (0...10).step(2).to_a
来源：http://jy.colortex.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yj.szxytkj.cn

[B12] 跳出多层循环
来源：http://ua.huanxung.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://kq.bjjhwx.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ul.haigaiapp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://am.hahajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hm.bookmarksfly.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bk.colortex.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dp.bjjhwx.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fu.shxzskj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wm.521024.cn

[B13] 判断是否为数字
来源：http://om.shtwfgs.cn

Py:   isinstance(x, (int, float))
来源：http://fg.newstarts.cn

PHP:  is_numeric($x)
来源：http://tw.huixinmuqiang.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yu.szxytkj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jh.shxzukj.cn

Java: x instanceof Number
来源：http://ky.9csxet.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pe.newstarts.cn

Ruby: x.is_a?(Numeric)
来源：http://du.colortex.cn

C#:   x is int or double or decimal
来源：http://ac.shxzskj.cn

[B14] 判断值是否在集合内
来源：http://rc.hahajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gu.yuntaijiaju.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ge.szsharing.cn

JS:   [1, 2, 3].includes(x)
来源：http://ws.nszjky.cn

TS:   [1, 2, 3].includes(x)
来源：http://ao.shtwfgs.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ll.yuntaijiaju.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vo.huanxung.cn

Ruby: [1, 2, 3].include?(x)
来源：http://wf.wgjwhj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qo.asd995.cn

[B15] 布尔运算与取反
来源：http://zh.yuexingan06.cn

Py:   a and b or not c
来源：http://oq.chemitech.net.cn

PHP:  $a && $b || !$c
来源：http://ou.newstarts.cn

JS:   a && b || !c
来源：http://jm.nszjky.cn

TS:   a && b || !c
来源：http://cz.wgjwhj.cn

Java: a && b || !c
来源：http://gt.hahajie.cn

Go:   a && b || !c
来源：http://fm.jctech888.com.cn

Ruby: a && b || !c
来源：http://de.lnxyls.cn

C#:   a && b || !c
来源：http://ih.muxihuayi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bg.nicolike.cn

Py:   if not data: return
来源：http://mj.shxzukj.cn

PHP:  if (!$data) { return; }
来源：http://kn.nszjky.cn

JS:   if (!data) return;
来源：http://ys.shxzukj.cn

TS:   if (!data) return;
来源：http://yr.huanxung.cn

Java: if (data == null) return;
来源：http://wf.gzmigu.cn

Go:   if data == nil { return }
来源：http://zv.shtwfgs.cn

Ruby: return if data.nil?
来源：http://nn.bjjhwx.cn

C#:   if (data == null) return;
来源：http://ho.shxzukj.cn

================================================================================
来源：http://dx.521024.cn

C. 函数与作用域
来源：http://ru.gzmigu.cn

================================================================================
来源：http://rx.huixiangedu.cn

[C01] 定义函数
来源：http://av.hnjuh.cn

Py:   def add(a, b): return a + b
来源：http://yl.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uf.haigaiapp.cn

JS:   function add(a, b) { return a + b; }
来源：http://pm.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://de.nszjky.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zh.hnjuh.cn

Go:   func add(a, b int) int { return a + b }
来源：http://fx.yuexingan06.cn

Ruby: def add(a, b); a + b; end
来源：http://ds.colortex.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://oh.panjiajie.cn

[C02] 默认参数
来源：http://jz.huixiangedu.cn

Py:   def greet(name="World"): return name
来源：http://oq.nicolike.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bh.wgjwhj.cn

JS:   function greet(name = "World") { return name; }
来源：http://av.nicolike.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://li.szsharing.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ad.nicolike.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ax.lnxyls.cn

Ruby: def greet(name = "World") = name
来源：http://rw.shtwfgs.cn

C#:   string Greet(string name = "World") => name;
来源：http://st.nszjky.cn

[C03] 可变参数
来源：http://li.muxihuayi.cn

Py:   def total(*args): return sum(args)
来源：http://oz.shxzskj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ee.huixiangedu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cy.newstarts.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zx.bjjhwx.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ix.colortex.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://oy.jianghongdianzi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yh.muxihuayi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ix.lnxyls.cn

[C04] 命名参数 / 关键字参数
来源：http://es.huanxung.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ja.shxzukj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bf.shxzukj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qv.jianghongdianzi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vy.nicolike.cn

Java: // 无：用 Builder 模式或 record
来源：http://og.gzmigu.cn

Go:   // 无：用配置结构体参数
来源：http://ef.haigaiapp.cn

Ruby: f(a: 1, b: 2)
来源：http://lp.jianghongdianzi.cn

C#:   f(a: 1, b: 2)
来源：http://tn.huixiangedu.cn

[C05] 返回多个值
来源：http://sc.nszjky.cn

Py:   return a, b
来源：http://zg.lnxyls.cn

PHP:  return [$a, $b];
来源：http://hu.newstarts.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pw.bookmarksfly.cn

TS:   return { a, b };
来源：http://ra.jctech888.com.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ly.shtwfgs.cn

Go:   return a, b
来源：http://pu.bjjhwx.cn

Ruby: return a, b
来源：http://du.szsharing.cn

C#:   return (a, b);              // ValueTuple
来源：http://az.lnxyls.cn

[C06] 匿名函数 / lambda
来源：http://hm.bjjhwx.cn

Py:   square = lambda x: x * x
来源：http://hm.lnxyls.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://va.gzmigu.cn

JS:   const square = x => x * x;
来源：http://rf.newstarts.cn

TS:   const square = (x: number): number => x * x;
来源：http://yk.nszjky.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vy.wgjwhj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://in.yuexingan06.cn

Ruby: square = ->(x) { x * x }
来源：http://ys.nicolike.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ss.521024.cn

[C07] 把函数作为参数传入
来源：http://fs.nszjky.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cw.jctech888.com.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xl.wgjwhj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nk.wgjwhj.cn

TS:   arr.map(String)
来源：http://nz.gzmigu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zd.hnjuh.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ot.gzmigu.cn

Ruby: arr.map(&:upcase)
来源：http://to.szsharing.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pr.521024.cn

[C08] 闭包
来源：http://cm.9csxet.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://np.huanxung.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://eq.huixinmuqiang.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bc.huixinmuqiang.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ux.jianghongdianzi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://st.huixinmuqiang.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mf.szxytkj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://oj.shtwfgs.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://al.wgjwhj.cn

[C09] 递归
来源：http://mf.wgjwhj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zc.wgjwhj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ph.colortex.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://th.nicolike.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ea.asd995.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yc.huixinmuqiang.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gb.jctech888.com.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zp.jctech888.com.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lw.colortex.cn

[C10] 变量作用域
来源：http://sn.jianghongdianzi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gu.yuexingan06.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://im.szsharing.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cj.panjiajie.cn

TS:   同 JS
来源：http://gi.huixiangedu.cn

Java: 方法内为块级作用域
来源：http://ow.huanxung.cn

Go:   花括号块级作用域
来源：http://hv.bjjhwx.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ce.hahajie.cn

C#:   块级作用域
来源：http://xy.bjjhwx.cn

[C11] 模块导入与导出
来源：http://ob.hnjuh.cn

Py:   from module import func
来源：http://ee.jianghongdianzi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://sy.hnjuh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://io.newstarts.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wx.nicolike.cn

Java: import java.util.List;
来源：http://bl.asd995.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qi.shxzskj.cn


<!-- 参考信息 -->