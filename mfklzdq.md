代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://hc.colortex.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://va.hnjuh.cn

Ruby: format("%.2f", 3.14159)
来源：http://rn.shtwfgs.cn

C#:   3.14159.ToString("F2")
来源：http://zz.haigaiapp.cn

[A22] 获取字符串长度
来源：http://je.huanxung.cn

Py:   len(s)
来源：http://jf.521024.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ih.shxzukj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://sp.newstarts.cn

TS:   s.length
来源：http://rd.jctech888.com.cn

Java: s.length()
来源：http://kz.muxihuayi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ly.huanxung.cn

Ruby: s.length
来源：http://dg.bjjhwx.cn

C#:   s.Length
来源：http://gu.yuntaijiaju.cn

[A23] 大小写转换
来源：http://dg.lnxyls.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://gy.gzmigu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ym.shxzskj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://sn.jctech888.com.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://sg.wgjwhj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qw.szsharing.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ua.yuexingan06.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rc.wgjwhj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://oz.9csxet.cn

[A24] 去除首尾空白
来源：http://ig.chemitech.net.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tb.bjjhwx.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://eo.9csxet.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vv.huanxung.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ao.shtwfgs.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dt.yuntaijiaju.cn

Go:   strings.TrimSpace(s)
来源：http://fw.nszjky.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ie.gzmigu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ep.shxzukj.cn

[A25] 字符串比较
来源：http://wv.bjjhwx.cn

Py:   s1 == s2; s1 != s2
来源：http://xm.huixinmuqiang.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ph.521024.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wa.huixiangedu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lh.bookmarksfly.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qm.szsharing.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dy.shtwfgs.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://se.newstarts.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vz.9csxet.cn

[A26] 类型转换总览
来源：http://jf.521024.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ct.wgjwhj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://su.shxzukj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fo.huixinmuqiang.cn

TS:   Number() String() Boolean() x as number
来源：http://jt.yuexingan06.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ay.szsharing.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kx.jctech888.com.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rw.lnxyls.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mx.yuexingan06.cn

================================================================================
来源：http://sr.szxytkj.cn

B. 流程控制
来源：http://bw.huixiangedu.cn

================================================================================
来源：http://bs.gzmigu.cn

[B01] 条件判断 if / else
来源：http://od.huixiangedu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ht.nicolike.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fj.nicolike.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rw.bjjhwx.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://me.hnjuh.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://pk.newstarts.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jr.haigaiapp.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vm.yuntaijiaju.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rq.lnxyls.cn

[B02] 多分支 else if / elif
来源：http://hd.shxzskj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dw.muxihuayi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sb.huanxung.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iw.521024.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ss.szsharing.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uy.bjjhwx.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hf.szxytkj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ru.szsharing.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://us.bookmarksfly.cn

[B03] switch / match / case
来源：http://ms.lnxyls.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pw.hnjuh.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nb.nicolike.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ld.colortex.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uf.muxihuayi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://me.hnjuh.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kt.521024.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gi.szxytkj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zw.hnjuh.cn

[B04] for 计数循环
来源：http://ky.huixiangedu.cn

Py:   for i in range(10): print(i)
来源：http://cd.newstarts.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jp.bjjhwx.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lo.hahajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zx.hahajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ns.newstarts.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ja.521024.cn

Ruby: 10.times { |i| puts i }
来源：http://hh.huixiangedu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gv.huixiangedu.cn

[B05] 遍历数组 / 列表
来源：http://fe.muxihuayi.cn

Py:   for item in arr: print(item)
来源：http://xb.bookmarksfly.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lu.hnjuh.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://pz.szsharing.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qf.panjiajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://mk.hahajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pz.haigaiapp.cn

Ruby: arr.each { |item| puts item }
来源：http://yc.haigaiapp.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xb.nszjky.cn

[B06] 遍历字典 / 对象
来源：http://lt.colortex.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ie.wgjwhj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://al.shtwfgs.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dg.huanxung.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cl.shtwfgs.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fa.wgjwhj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ob.colortex.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ka.hahajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sr.jctech888.com.cn

[B07] while 循环
来源：http://qw.bookmarksfly.cn

Py:   while i < 10: i += 1
来源：http://zi.chemitech.net.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vn.lnxyls.cn

JS:   while (i < 10) { i++; }
来源：http://et.bjjhwx.cn

TS:   while (i < 10) { i++; }
来源：http://di.asd995.cn

Java: while (i < 10) { i++; }
来源：http://zi.yuntaijiaju.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://si.asd995.cn

Ruby: while i < 10; i += 1; end
来源：http://tw.yuntaijiaju.cn

C#:   while (i < 10) { i++; }
来源：http://uh.asd995.cn

[B08] do-while（至少执行一次）
来源：http://zk.jianghongdianzi.cn

Py:   # 无 do-while：用 while True + break
来源：http://mh.chemitech.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://tk.huixiangedu.cn

JS:   do { i++; } while (i < 10);
来源：http://vh.jianghongdianzi.cn

TS:   do { i++; } while (i < 10);
来源：http://xg.colortex.cn

Java: do { i++; } while (i < 10);
来源：http://tq.huanxung.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vo.muxihuayi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://yb.szxytkj.cn

C#:   do { i++; } while (i < 10);
来源：http://wk.lnxyls.cn

[B09] break 与 continue
来源：http://mu.yuexingan06.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wk.szsharing.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uc.shxzukj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://we.szsharing.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bt.chemitech.net.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dl.nszjky.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tb.nicolike.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dn.bjjhwx.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ff.asd995.cn

[B10] 遍历同时拿索引
来源：http://jd.szxytkj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://uz.9csxet.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zs.bjjhwx.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qv.hnjuh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wj.gzmigu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ar.hnjuh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ch.haigaiapp.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xd.chemitech.net.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wx.hnjuh.cn

[B11] 生成数字序列 / 区间
来源：http://mv.chemitech.net.cn

Py:   list(range(0, 10, 2))
来源：http://ln.haigaiapp.cn

PHP:  range(0, 10, 2);
来源：http://cj.lnxyls.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ld.huixinmuqiang.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ok.muxihuayi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ps.huixiangedu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hp.bookmarksfly.cn

Ruby: (0...10).step(2).to_a
来源：http://my.panjiajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vk.szsharing.cn

[B12] 跳出多层循环
来源：http://qm.521024.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://gs.bjjhwx.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://qs.bookmarksfly.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xb.asd995.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://og.newstarts.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mv.newstarts.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zr.szxytkj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gw.nicolike.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wp.nszjky.cn

[B13] 判断是否为数字
来源：http://gv.gzmigu.cn

Py:   isinstance(x, (int, float))
来源：http://ba.huanxung.cn

PHP:  is_numeric($x)
来源：http://rn.szsharing.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wc.nszjky.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ix.szsharing.cn

Java: x instanceof Number
来源：http://gk.wgjwhj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ct.521024.cn

Ruby: x.is_a?(Numeric)
来源：http://uf.jctech888.com.cn

C#:   x is int or double or decimal
来源：http://oa.jianghongdianzi.cn

[B14] 判断值是否在集合内
来源：http://yi.shxzskj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ta.szsharing.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dc.asd995.cn

JS:   [1, 2, 3].includes(x)
来源：http://gw.521024.cn

TS:   [1, 2, 3].includes(x)
来源：http://lw.nicolike.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://is.nicolike.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vf.huanxung.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ce.lnxyls.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kv.wgjwhj.cn

[B15] 布尔运算与取反
来源：http://sg.wgjwhj.cn

Py:   a and b or not c
来源：http://kk.nszjky.cn

PHP:  $a && $b || !$c
来源：http://od.huixinmuqiang.cn

JS:   a && b || !c
来源：http://kn.521024.cn

TS:   a && b || !c
来源：http://mr.wgjwhj.cn

Java: a && b || !c
来源：http://ok.newstarts.cn

Go:   a && b || !c
来源：http://ny.shxzskj.cn

Ruby: a && b || !c
来源：http://zh.nszjky.cn

C#:   a && b || !c
来源：http://fu.wgjwhj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fu.shtwfgs.cn

Py:   if not data: return
来源：http://jf.huanxung.cn

PHP:  if (!$data) { return; }
来源：http://ig.9csxet.cn

JS:   if (!data) return;
来源：http://dv.huanxung.cn

TS:   if (!data) return;
来源：http://ng.hnjuh.cn

Java: if (data == null) return;
来源：http://sz.shxzukj.cn

Go:   if data == nil { return }
来源：http://ko.9csxet.cn

Ruby: return if data.nil?
来源：http://gn.shxzukj.cn

C#:   if (data == null) return;
来源：http://ig.shxzukj.cn

================================================================================
来源：http://ns.shtwfgs.cn

C. 函数与作用域
来源：http://bo.nicolike.cn

================================================================================
来源：http://yw.hnjuh.cn

[C01] 定义函数
来源：http://kg.chemitech.net.cn

Py:   def add(a, b): return a + b
来源：http://om.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wj.huixinmuqiang.cn

JS:   function add(a, b) { return a + b; }
来源：http://cq.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pv.colortex.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://jy.shtwfgs.cn

Go:   func add(a, b int) int { return a + b }
来源：http://lr.shxzskj.cn

Ruby: def add(a, b); a + b; end
来源：http://fu.panjiajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ec.shxzukj.cn

[C02] 默认参数
来源：http://sp.asd995.cn

Py:   def greet(name="World"): return name
来源：http://ky.newstarts.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://nn.bjjhwx.cn

JS:   function greet(name = "World") { return name; }
来源：http://yg.521024.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gv.gzmigu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://uv.nicolike.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bf.asd995.cn

Ruby: def greet(name = "World") = name
来源：http://ea.shxzskj.cn

C#:   string Greet(string name = "World") => name;
来源：http://tn.haigaiapp.cn

[C03] 可变参数
来源：http://jv.9csxet.cn

Py:   def total(*args): return sum(args)
来源：http://tr.9csxet.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mj.colortex.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rf.asd995.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hd.muxihuayi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://br.wgjwhj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rw.asd995.cn

Ruby: def total(*nums); nums.sum; end
来源：http://og.shxzukj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://re.asd995.cn

[C04] 命名参数 / 关键字参数
来源：http://xw.shtwfgs.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nz.chemitech.net.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rr.bjjhwx.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hm.szxytkj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mq.huanxung.cn

Java: // 无：用 Builder 模式或 record
来源：http://se.panjiajie.cn

Go:   // 无：用配置结构体参数
来源：http://lx.gzmigu.cn

Ruby: f(a: 1, b: 2)
来源：http://es.shxzukj.cn

C#:   f(a: 1, b: 2)
来源：http://hh.panjiajie.cn

[C05] 返回多个值
来源：http://tj.gzmigu.cn

Py:   return a, b
来源：http://zy.yuexingan06.cn

PHP:  return [$a, $b];
来源：http://yg.colortex.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yf.lnxyls.cn

TS:   return { a, b };
来源：http://nq.yuexingan06.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ba.asd995.cn

Go:   return a, b
来源：http://qp.panjiajie.cn

Ruby: return a, b
来源：http://ij.521024.cn

C#:   return (a, b);              // ValueTuple
来源：http://kj.panjiajie.cn

[C06] 匿名函数 / lambda
来源：http://lq.bookmarksfly.cn

Py:   square = lambda x: x * x
来源：http://tk.521024.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://it.bookmarksfly.cn

JS:   const square = x => x * x;
来源：http://jk.yuexingan06.cn

TS:   const square = (x: number): number => x * x;
来源：http://ci.521024.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://os.bookmarksfly.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wd.huixinmuqiang.cn

Ruby: square = ->(x) { x * x }
来源：http://vs.521024.cn

C#:   Func<int, int> square = x => x * x;
来源：http://kv.gzmigu.cn

[C07] 把函数作为参数传入
来源：http://ne.shtwfgs.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ql.gzmigu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bo.yuexingan06.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rg.gzmigu.cn

TS:   arr.map(String)
来源：http://ax.asd995.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gi.colortex.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rl.asd995.cn

Ruby: arr.map(&:upcase)
来源：http://me.huanxung.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ja.szxytkj.cn

[C08] 闭包
来源：http://lm.szsharing.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ty.bjjhwx.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ml.szsharing.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pp.newstarts.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wg.yuntaijiaju.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tu.muxihuayi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://co.colortex.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://by.szxytkj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://sg.wgjwhj.cn

[C09] 递归
来源：http://jn.muxihuayi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ox.szsharing.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hm.huixiangedu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kt.panjiajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nl.panjiajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cp.gzmigu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://em.shtwfgs.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://az.shxzukj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rd.wgjwhj.cn

[C10] 变量作用域
来源：http://sx.bjjhwx.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fu.haigaiapp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ae.muxihuayi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mm.asd995.cn

TS:   同 JS
来源：http://hf.huixinmuqiang.cn

Java: 方法内为块级作用域
来源：http://rb.shtwfgs.cn

Go:   花括号块级作用域
来源：http://bq.shtwfgs.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vr.wgjwhj.cn

C#:   块级作用域
来源：http://ar.chemitech.net.cn

[C11] 模块导入与导出
来源：http://on.shtwfgs.cn

Py:   from module import func
来源：http://do.9csxet.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://uc.muxihuayi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://eh.panjiajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rq.yuntaijiaju.cn

Java: import java.util.List;
来源：http://ek.huixiangedu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gq.asd995.cn

Ruby: require "json"; require_relative "./util"
来源：http://na.szxytkj.cn

C#:   using System.Text;
来源：http://nl.panjiajie.cn

[C12] 立即执行函数 IIFE
来源：http://xv.nszjky.cn

Py:   (lambda: print("run"))()
来源：http://xy.hahajie.cn


<!-- 参考信息 -->