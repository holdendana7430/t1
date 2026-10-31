代发 wailian999

[A22] 获取字符串长度
来源：http://li.huixinmuqiang.cn

Py:   len(s)
来源：http://ru.huanxung.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://uw.muxihuayi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xw.521024.cn

TS:   s.length
来源：http://sp.huixiangedu.cn

Java: s.length()
来源：http://co.hahajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://op.wgjwhj.cn

Ruby: s.length
来源：http://kb.hahajie.cn

C#:   s.Length
来源：http://by.chemitech.net.cn

[A23] 大小写转换
来源：http://az.panjiajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://st.huanxung.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ll.panjiajie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mt.huixiangedu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xy.9csxet.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://yk.nszjky.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ap.wgjwhj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qb.huixinmuqiang.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://kb.huanxung.cn

[A24] 去除首尾空白
来源：http://cd.huixiangedu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sk.gzmigu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xb.lnxyls.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sy.9csxet.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ci.lnxyls.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rm.panjiajie.cn

Go:   strings.TrimSpace(s)
来源：http://uj.huixiangedu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ek.huixiangedu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vm.shxzskj.cn

[A25] 字符串比较
来源：http://di.shtwfgs.cn

Py:   s1 == s2; s1 != s2
来源：http://df.shxzukj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://eq.shxzukj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fk.521024.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ea.nicolike.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tg.nszjky.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kc.chemitech.net.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://gu.huixiangedu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dd.szxytkj.cn

[A26] 类型转换总览
来源：http://ji.hnjuh.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://td.gzmigu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sr.haigaiapp.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fm.jianghongdianzi.cn

TS:   Number() String() Boolean() x as number
来源：http://aq.9csxet.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hf.shxzskj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sj.jctech888.com.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://qh.szxytkj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uj.nszjky.cn

================================================================================
来源：http://xg.wgjwhj.cn

B. 流程控制
来源：http://ub.haigaiapp.cn

================================================================================
来源：http://dc.nicolike.cn

[B01] 条件判断 if / else
来源：http://sw.nicolike.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ch.hnjuh.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fh.colortex.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sc.shxzukj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dy.haigaiapp.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vz.gzmigu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fm.nicolike.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sq.asd995.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ql.haigaiapp.cn

[B02] 多分支 else if / elif
来源：http://bp.asd995.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ef.nicolike.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xk.shtwfgs.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pz.jctech888.com.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://le.nszjky.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cm.szsharing.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ds.szsharing.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ll.panjiajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tu.jctech888.com.cn

[B03] switch / match / case
来源：http://ih.521024.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://iz.muxihuayi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gq.huixiangedu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qo.colortex.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mv.asd995.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rn.panjiajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mg.yuntaijiaju.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://oy.haigaiapp.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gs.yuexingan06.cn

[B04] for 计数循环
来源：http://se.yuntaijiaju.cn

Py:   for i in range(10): print(i)
来源：http://jo.shxzukj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://oo.muxihuayi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sc.yuexingan06.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://le.panjiajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wc.9csxet.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ik.shxzukj.cn

Ruby: 10.times { |i| puts i }
来源：http://xj.huixinmuqiang.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ua.nszjky.cn

[B05] 遍历数组 / 列表
来源：http://cd.521024.cn

Py:   for item in arr: print(item)
来源：http://ul.asd995.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cm.szsharing.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ju.bjjhwx.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://uy.huixiangedu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gl.newstarts.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hw.haigaiapp.cn

Ruby: arr.each { |item| puts item }
来源：http://wo.shxzskj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ff.muxihuayi.cn

[B06] 遍历字典 / 对象
来源：http://xz.huixiangedu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://cf.huixiangedu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mb.nicolike.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ja.huixinmuqiang.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bd.nicolike.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ix.nicolike.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rl.jctech888.com.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://py.szxytkj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gg.wgjwhj.cn

[B07] while 循环
来源：http://xw.muxihuayi.cn

Py:   while i < 10: i += 1
来源：http://qa.haigaiapp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zm.hahajie.cn

JS:   while (i < 10) { i++; }
来源：http://ax.wgjwhj.cn

TS:   while (i < 10) { i++; }
来源：http://tj.huixiangedu.cn

Java: while (i < 10) { i++; }
来源：http://ns.jctech888.com.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xe.hahajie.cn

Ruby: while i < 10; i += 1; end
来源：http://tp.bookmarksfly.cn

C#:   while (i < 10) { i++; }
来源：http://qh.521024.cn

[B08] do-while（至少执行一次）
来源：http://nt.bjjhwx.cn

Py:   # 无 do-while：用 while True + break
来源：http://yg.asd995.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://do.nszjky.cn

JS:   do { i++; } while (i < 10);
来源：http://gf.huixinmuqiang.cn

TS:   do { i++; } while (i < 10);
来源：http://eq.shxzukj.cn

Java: do { i++; } while (i < 10);
来源：http://wj.chemitech.net.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sr.muxihuayi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jq.huixiangedu.cn

C#:   do { i++; } while (i < 10);
来源：http://ge.wgjwhj.cn

[B09] break 与 continue
来源：http://tx.bjjhwx.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ch.jianghongdianzi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pn.shxzskj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sw.huanxung.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ay.yuexingan06.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gt.asd995.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://aw.bookmarksfly.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fx.bookmarksfly.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vl.chemitech.net.cn

[B10] 遍历同时拿索引
来源：http://gf.colortex.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ab.huixinmuqiang.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wl.jctech888.com.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zc.yuntaijiaju.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dp.jianghongdianzi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qz.jctech888.com.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rj.wgjwhj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uc.shtwfgs.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://af.haigaiapp.cn

[B11] 生成数字序列 / 区间
来源：http://zg.huanxung.cn

Py:   list(range(0, 10, 2))
来源：http://gv.huixiangedu.cn

PHP:  range(0, 10, 2);
来源：http://ka.huixinmuqiang.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ex.szxytkj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yf.bookmarksfly.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cm.szsharing.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ur.haigaiapp.cn

Ruby: (0...10).step(2).to_a
来源：http://cd.haigaiapp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kq.nszjky.cn

[B12] 跳出多层循环
来源：http://it.521024.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://sf.muxihuayi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://id.huixiangedu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kl.muxihuayi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zh.bjjhwx.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yj.9csxet.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yt.bjjhwx.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wa.shxzukj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gw.muxihuayi.cn

[B13] 判断是否为数字
来源：http://lt.wgjwhj.cn

Py:   isinstance(x, (int, float))
来源：http://if.9csxet.cn

PHP:  is_numeric($x)
来源：http://mt.hnjuh.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rs.lnxyls.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fz.shtwfgs.cn

Java: x instanceof Number
来源：http://nh.huanxung.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sc.bjjhwx.cn

Ruby: x.is_a?(Numeric)
来源：http://ue.huixinmuqiang.cn

C#:   x is int or double or decimal
来源：http://ql.huixiangedu.cn

[B14] 判断值是否在集合内
来源：http://pl.521024.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rz.hahajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wu.shxzskj.cn

JS:   [1, 2, 3].includes(x)
来源：http://hu.jianghongdianzi.cn

TS:   [1, 2, 3].includes(x)
来源：http://ca.521024.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ya.szxytkj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pb.hahajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://bi.yuntaijiaju.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qv.shxzukj.cn

[B15] 布尔运算与取反
来源：http://tb.521024.cn

Py:   a and b or not c
来源：http://xs.shxzskj.cn

PHP:  $a && $b || !$c
来源：http://ix.hahajie.cn

JS:   a && b || !c
来源：http://jf.huixiangedu.cn

TS:   a && b || !c
来源：http://eu.shxzukj.cn

Java: a && b || !c
来源：http://ot.muxihuayi.cn

Go:   a && b || !c
来源：http://tp.gzmigu.cn

Ruby: a && b || !c
来源：http://qy.shtwfgs.cn

C#:   a && b || !c
来源：http://la.yuntaijiaju.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ju.huixinmuqiang.cn

Py:   if not data: return
来源：http://ck.bookmarksfly.cn

PHP:  if (!$data) { return; }
来源：http://tz.bjjhwx.cn

JS:   if (!data) return;
来源：http://my.521024.cn

TS:   if (!data) return;
来源：http://wv.bookmarksfly.cn

Java: if (data == null) return;
来源：http://gf.yuexingan06.cn

Go:   if data == nil { return }
来源：http://mi.shtwfgs.cn

Ruby: return if data.nil?
来源：http://pg.szsharing.cn

C#:   if (data == null) return;
来源：http://gv.9csxet.cn

================================================================================
来源：http://ua.shxzskj.cn

C. 函数与作用域
来源：http://xd.huanxung.cn

================================================================================
来源：http://zh.yuntaijiaju.cn

[C01] 定义函数
来源：http://ng.szxytkj.cn

Py:   def add(a, b): return a + b
来源：http://fn.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nt.shxzskj.cn

JS:   function add(a, b) { return a + b; }
来源：http://uc.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cx.521024.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://cu.nszjky.cn

Go:   func add(a, b int) int { return a + b }
来源：http://kj.bjjhwx.cn

Ruby: def add(a, b); a + b; end
来源：http://cq.huixiangedu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wy.jianghongdianzi.cn

[C02] 默认参数
来源：http://hs.huanxung.cn

Py:   def greet(name="World"): return name
来源：http://zh.shtwfgs.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ii.muxihuayi.cn

JS:   function greet(name = "World") { return name; }
来源：http://fg.nicolike.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://nk.huixinmuqiang.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://el.chemitech.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://eo.hahajie.cn

Ruby: def greet(name = "World") = name
来源：http://mq.shxzukj.cn

C#:   string Greet(string name = "World") => name;
来源：http://ut.asd995.cn

[C03] 可变参数
来源：http://ws.asd995.cn

Py:   def total(*args): return sum(args)
来源：http://qu.yuntaijiaju.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cs.newstarts.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ge.jctech888.com.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rz.hnjuh.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://we.huixiangedu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yq.haigaiapp.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ap.lnxyls.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://py.panjiajie.cn

[C04] 命名参数 / 关键字参数
来源：http://ny.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mq.bookmarksfly.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fq.shtwfgs.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pb.colortex.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mt.muxihuayi.cn

Java: // 无：用 Builder 模式或 record
来源：http://pq.haigaiapp.cn

Go:   // 无：用配置结构体参数
来源：http://ly.nszjky.cn

Ruby: f(a: 1, b: 2)
来源：http://tc.jctech888.com.cn

C#:   f(a: 1, b: 2)
来源：http://es.haigaiapp.cn

[C05] 返回多个值
来源：http://xr.huanxung.cn

Py:   return a, b
来源：http://tq.bjjhwx.cn

PHP:  return [$a, $b];
来源：http://ns.huixinmuqiang.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://iz.hahajie.cn

TS:   return { a, b };
来源：http://bx.lnxyls.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yk.bookmarksfly.cn

Go:   return a, b
来源：http://rc.nszjky.cn

Ruby: return a, b
来源：http://qb.huixiangedu.cn

C#:   return (a, b);              // ValueTuple
来源：http://py.lnxyls.cn

[C06] 匿名函数 / lambda
来源：http://ko.newstarts.cn

Py:   square = lambda x: x * x
来源：http://ek.lnxyls.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ul.huixinmuqiang.cn

JS:   const square = x => x * x;
来源：http://ip.hahajie.cn

TS:   const square = (x: number): number => x * x;
来源：http://zw.9csxet.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bt.shxzukj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ej.huixinmuqiang.cn

Ruby: square = ->(x) { x * x }
来源：http://gx.wgjwhj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://as.szxytkj.cn

[C07] 把函数作为参数传入
来源：http://uz.asd995.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mu.9csxet.cn

PHP:  array_map("strtoupper", $arr);
来源：http://yj.chemitech.net.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qh.panjiajie.cn

TS:   arr.map(String)
来源：http://gu.yuexingan06.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cv.9csxet.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uk.hnjuh.cn

Ruby: arr.map(&:upcase)
来源：http://ny.521024.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ut.huixiangedu.cn

[C08] 闭包
来源：http://fc.bjjhwx.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uz.jctech888.com.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.nszjky.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ri.colortex.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jy.nicolike.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ch.szsharing.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nk.asd995.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dt.shtwfgs.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://da.chemitech.net.cn

[C09] 递归
来源：http://pd.huanxung.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pg.huixinmuqiang.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://eh.bookmarksfly.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qn.chemitech.net.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ac.huanxung.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xd.huixiangedu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://he.shtwfgs.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xr.huixiangedu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://km.szsharing.cn

[C10] 变量作用域
来源：http://ft.haigaiapp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fn.jctech888.com.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hl.wgjwhj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mu.hnjuh.cn

TS:   同 JS
来源：http://tj.wgjwhj.cn

Java: 方法内为块级作用域
来源：http://ck.szsharing.cn

Go:   花括号块级作用域
来源：http://qv.bjjhwx.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yc.yuntaijiaju.cn

C#:   块级作用域
来源：http://hu.gzmigu.cn

[C11] 模块导入与导出
来源：http://se.hnjuh.cn

Py:   from module import func
来源：http://qg.hahajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xj.9csxet.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://by.yuntaijiaju.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vg.gzmigu.cn

Java: import java.util.List;
来源：http://wa.lnxyls.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vu.chemitech.net.cn

Ruby: require "json"; require_relative "./util"
来源：http://gc.panjiajie.cn

C#:   using System.Text;
来源：http://ok.gzmigu.cn

[C12] 立即执行函数 IIFE
来源：http://hw.bookmarksfly.cn

Py:   (lambda: print("run"))()
来源：http://wl.wgjwhj.cn

PHP:  (function () { echo "run"; })();
来源：http://kc.yuexingan06.cn

JS:   (() => { console.log("run"); })();
来源：http://kh.huanxung.cn

TS:   (() => { console.log("run"); })();
来源：http://sz.nicolike.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dh.bjjhwx.cn


<!-- 参考信息 -->