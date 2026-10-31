代发 wailian999

[A22] 获取字符串长度
来源：http://wd.szxytkj.cn

Py:   len(s)
来源：http://wg.huanxung.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vz.panjiajie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lh.haigaiapp.cn

TS:   s.length
来源：http://et.jctech888.com.cn

Java: s.length()
来源：http://uy.hahajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fb.huixiangedu.cn

Ruby: s.length
来源：http://xr.yuexingan06.cn

C#:   s.Length
来源：http://yh.yuntaijiaju.cn

[A23] 大小写转换
来源：http://yk.shxzukj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://cb.jianghongdianzi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ym.huixiangedu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jy.muxihuayi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cw.asd995.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zj.nicolike.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rr.haigaiapp.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yy.huixiangedu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qi.huixinmuqiang.cn

[A24] 去除首尾空白
来源：http://ns.jctech888.com.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tz.bookmarksfly.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dm.chemitech.net.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qn.huanxung.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nc.bookmarksfly.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nn.huixiangedu.cn

Go:   strings.TrimSpace(s)
来源：http://ya.9csxet.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hf.lnxyls.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kc.hnjuh.cn

[A25] 字符串比较
来源：http://pw.wgjwhj.cn

Py:   s1 == s2; s1 != s2
来源：http://hy.wgjwhj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://aq.huixiangedu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ik.huixiangedu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bg.yuexingan06.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ps.shxzukj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://as.hnjuh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://fq.haigaiapp.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sr.jctech888.com.cn

[A26] 类型转换总览
来源：http://hl.wgjwhj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gv.yuntaijiaju.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xc.huixiangedu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rm.bjjhwx.cn

TS:   Number() String() Boolean() x as number
来源：http://ko.huixiangedu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wd.hnjuh.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vc.shtwfgs.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://pm.huanxung.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ea.9csxet.cn

================================================================================
来源：http://xs.asd995.cn

B. 流程控制
来源：http://rv.shxzskj.cn

================================================================================
来源：http://it.bookmarksfly.cn

[B01] 条件判断 if / else
来源：http://qd.asd995.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://aq.szsharing.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wm.newstarts.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://em.shtwfgs.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dg.bjjhwx.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://gv.shtwfgs.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rf.shxzskj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vg.huanxung.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mg.asd995.cn

[B02] 多分支 else if / elif
来源：http://gu.szsharing.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xb.shtwfgs.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bx.shxzskj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ws.huixiangedu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kx.521024.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oz.asd995.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://en.shtwfgs.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://me.asd995.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hl.shxzukj.cn

[B03] switch / match / case
来源：http://xl.huixiangedu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://os.jianghongdianzi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qz.yuntaijiaju.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ov.shxzukj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ja.jianghongdianzi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bg.nicolike.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ea.chemitech.net.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://aw.chemitech.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sr.szxytkj.cn

[B04] for 计数循环
来源：http://dw.bookmarksfly.cn

Py:   for i in range(10): print(i)
来源：http://uz.huixiangedu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yq.yuexingan06.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kp.shxzskj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gm.nicolike.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jn.yuntaijiaju.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://to.muxihuayi.cn

Ruby: 10.times { |i| puts i }
来源：http://ul.huixinmuqiang.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ok.shxzskj.cn

[B05] 遍历数组 / 列表
来源：http://jw.huanxung.cn

Py:   for item in arr: print(item)
来源：http://jv.nicolike.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://el.yuntaijiaju.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://at.huixinmuqiang.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://al.jianghongdianzi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ue.yuexingan06.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ao.gzmigu.cn

Ruby: arr.each { |item| puts item }
来源：http://jr.szxytkj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cj.bookmarksfly.cn

[B06] 遍历字典 / 对象
来源：http://am.chemitech.net.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ht.9csxet.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mz.huixiangedu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ec.9csxet.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ka.lnxyls.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cj.newstarts.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ji.huanxung.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://is.chemitech.net.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://li.wgjwhj.cn

[B07] while 循环
来源：http://zt.bjjhwx.cn

Py:   while i < 10: i += 1
来源：http://lw.gzmigu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zf.haigaiapp.cn

JS:   while (i < 10) { i++; }
来源：http://ff.huanxung.cn

TS:   while (i < 10) { i++; }
来源：http://fx.521024.cn

Java: while (i < 10) { i++; }
来源：http://im.huanxung.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ei.colortex.cn

Ruby: while i < 10; i += 1; end
来源：http://tu.jianghongdianzi.cn

C#:   while (i < 10) { i++; }
来源：http://sz.yuexingan06.cn

[B08] do-while（至少执行一次）
来源：http://jx.huixinmuqiang.cn

Py:   # 无 do-while：用 while True + break
来源：http://cf.shtwfgs.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vo.yuexingan06.cn

JS:   do { i++; } while (i < 10);
来源：http://wp.newstarts.cn

TS:   do { i++; } while (i < 10);
来源：http://kr.chemitech.net.cn

Java: do { i++; } while (i < 10);
来源：http://mh.shxzskj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sb.nszjky.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rf.colortex.cn

C#:   do { i++; } while (i < 10);
来源：http://ys.haigaiapp.cn

[B09] break 与 continue
来源：http://ny.lnxyls.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ya.jianghongdianzi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pp.bjjhwx.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rk.shtwfgs.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eu.huanxung.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fx.521024.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rp.szxytkj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yw.panjiajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jv.asd995.cn

[B10] 遍历同时拿索引
来源：http://lm.asd995.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ub.asd995.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wg.jianghongdianzi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jn.shxzskj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pg.muxihuayi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://io.yuexingan06.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hi.521024.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zq.shtwfgs.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xl.asd995.cn

[B11] 生成数字序列 / 区间
来源：http://np.shxzukj.cn

Py:   list(range(0, 10, 2))
来源：http://ec.haigaiapp.cn

PHP:  range(0, 10, 2);
来源：http://sz.huixinmuqiang.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://su.asd995.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hs.521024.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bu.521024.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://up.chemitech.net.cn

Ruby: (0...10).step(2).to_a
来源：http://sj.hnjuh.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ed.wgjwhj.cn

[B12] 跳出多层循环
来源：http://cn.yuexingan06.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://el.muxihuayi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://bi.gzmigu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uo.jianghongdianzi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wg.jianghongdianzi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vj.jctech888.com.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://le.huixinmuqiang.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vb.colortex.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wq.shtwfgs.cn

[B13] 判断是否为数字
来源：http://sf.panjiajie.cn

Py:   isinstance(x, (int, float))
来源：http://mf.gzmigu.cn

PHP:  is_numeric($x)
来源：http://iu.wgjwhj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cu.shxzskj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fm.newstarts.cn

Java: x instanceof Number
来源：http://xb.9csxet.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ly.yuntaijiaju.cn

Ruby: x.is_a?(Numeric)
来源：http://li.jianghongdianzi.cn

C#:   x is int or double or decimal
来源：http://nr.521024.cn

[B14] 判断值是否在集合内
来源：http://bi.chemitech.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ox.szxytkj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qu.bookmarksfly.cn

JS:   [1, 2, 3].includes(x)
来源：http://hz.yuexingan06.cn

TS:   [1, 2, 3].includes(x)
来源：http://zs.jctech888.com.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://pw.szsharing.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hc.haigaiapp.cn

Ruby: [1, 2, 3].include?(x)
来源：http://eu.jianghongdianzi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://te.jianghongdianzi.cn

[B15] 布尔运算与取反
来源：http://rr.huixiangedu.cn

Py:   a and b or not c
来源：http://fr.hahajie.cn

PHP:  $a && $b || !$c
来源：http://ah.jianghongdianzi.cn

JS:   a && b || !c
来源：http://oi.asd995.cn

TS:   a && b || !c
来源：http://wk.shxzskj.cn

Java: a && b || !c
来源：http://dc.shxzukj.cn

Go:   a && b || !c
来源：http://ud.szsharing.cn

Ruby: a && b || !c
来源：http://wq.huixinmuqiang.cn

C#:   a && b || !c
来源：http://lc.nicolike.cn

[B16] 卫语句：不满足条件提前返回
来源：http://rz.521024.cn

Py:   if not data: return
来源：http://yn.shtwfgs.cn

PHP:  if (!$data) { return; }
来源：http://lg.hahajie.cn

JS:   if (!data) return;
来源：http://ux.yuexingan06.cn

TS:   if (!data) return;
来源：http://sh.yuexingan06.cn

Java: if (data == null) return;
来源：http://hk.asd995.cn

Go:   if data == nil { return }
来源：http://yl.nicolike.cn

Ruby: return if data.nil?
来源：http://fq.chemitech.net.cn

C#:   if (data == null) return;
来源：http://ay.yuexingan06.cn

================================================================================
来源：http://vj.colortex.cn

C. 函数与作用域
来源：http://aa.nicolike.cn

================================================================================
来源：http://oh.bjjhwx.cn

[C01] 定义函数
来源：http://go.haigaiapp.cn

Py:   def add(a, b): return a + b
来源：http://an.muxihuayi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ni.shtwfgs.cn

JS:   function add(a, b) { return a + b; }
来源：http://ci.huixinmuqiang.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vo.shtwfgs.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bp.newstarts.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xc.lnxyls.cn

Ruby: def add(a, b); a + b; end
来源：http://gs.bookmarksfly.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xp.huixinmuqiang.cn

[C02] 默认参数
来源：http://ad.muxihuayi.cn

Py:   def greet(name="World"): return name
来源：http://my.jctech888.com.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.hahajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://vy.yuntaijiaju.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lz.nicolike.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ds.jctech888.com.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rg.gzmigu.cn

Ruby: def greet(name = "World") = name
来源：http://ea.bookmarksfly.cn

C#:   string Greet(string name = "World") => name;
来源：http://fz.huanxung.cn

[C03] 可变参数
来源：http://lx.bjjhwx.cn

Py:   def total(*args): return sum(args)
来源：http://vb.huixinmuqiang.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wq.asd995.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qj.yuntaijiaju.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fy.colortex.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hd.nszjky.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ra.haigaiapp.cn

Ruby: def total(*nums); nums.sum; end
来源：http://st.shxzskj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ma.lnxyls.cn

[C04] 命名参数 / 关键字参数
来源：http://ln.colortex.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ma.szsharing.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rx.gzmigu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bp.bookmarksfly.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://eh.521024.cn

Java: // 无：用 Builder 模式或 record
来源：http://oz.shxzukj.cn

Go:   // 无：用配置结构体参数
来源：http://jw.shtwfgs.cn

Ruby: f(a: 1, b: 2)
来源：http://pe.panjiajie.cn

C#:   f(a: 1, b: 2)
来源：http://dg.9csxet.cn

[C05] 返回多个值
来源：http://fy.szsharing.cn

Py:   return a, b
来源：http://ge.shxzukj.cn

PHP:  return [$a, $b];
来源：http://tp.yuexingan06.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qq.wgjwhj.cn

TS:   return { a, b };
来源：http://qa.bjjhwx.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fx.jianghongdianzi.cn

Go:   return a, b
来源：http://yx.chemitech.net.cn

Ruby: return a, b
来源：http://zn.muxihuayi.cn

C#:   return (a, b);              // ValueTuple
来源：http://mu.asd995.cn

[C06] 匿名函数 / lambda
来源：http://xy.muxihuayi.cn

Py:   square = lambda x: x * x
来源：http://kt.shxzskj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://de.huixinmuqiang.cn

JS:   const square = x => x * x;
来源：http://xv.lnxyls.cn

TS:   const square = (x: number): number => x * x;
来源：http://jm.wgjwhj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nu.wgjwhj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://je.panjiajie.cn

Ruby: square = ->(x) { x * x }
来源：http://ya.asd995.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qb.huixinmuqiang.cn

[C07] 把函数作为参数传入
来源：http://nu.hahajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wx.nszjky.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ak.hahajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rz.gzmigu.cn

TS:   arr.map(String)
来源：http://dz.newstarts.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fk.huixiangedu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://us.shxzskj.cn

Ruby: arr.map(&:upcase)
来源：http://vm.hahajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://nl.shxzskj.cn

[C08] 闭包
来源：http://tg.yuntaijiaju.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cm.shxzukj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cm.szxytkj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qb.yuntaijiaju.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://df.huanxung.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pv.hahajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://va.szxytkj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mw.jianghongdianzi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://if.shxzskj.cn

[C09] 递归
来源：http://fl.hnjuh.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gd.shtwfgs.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sj.yuexingan06.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pt.hahajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iw.shxzskj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ic.panjiajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ys.jctech888.com.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fp.bjjhwx.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kd.hahajie.cn

[C10] 变量作用域
来源：http://uf.jctech888.com.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rp.haigaiapp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mr.yuexingan06.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://on.huixinmuqiang.cn

TS:   同 JS
来源：http://vm.shxzukj.cn

Java: 方法内为块级作用域
来源：http://oq.shxzukj.cn

Go:   花括号块级作用域
来源：http://vw.haigaiapp.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ag.muxihuayi.cn

C#:   块级作用域
来源：http://rf.yuexingan06.cn

[C11] 模块导入与导出
来源：http://tf.jianghongdianzi.cn

Py:   from module import func
来源：http://ju.huixinmuqiang.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zp.hahajie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://xd.yuntaijiaju.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tl.hnjuh.cn

Java: import java.util.List;
来源：http://bh.yuexingan06.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://su.yuntaijiaju.cn

Ruby: require "json"; require_relative "./util"
来源：http://qy.shxzukj.cn

C#:   using System.Text;
来源：http://bk.newstarts.cn

[C12] 立即执行函数 IIFE
来源：http://em.hnjuh.cn

Py:   (lambda: print("run"))()
来源：http://ay.szxytkj.cn

PHP:  (function () { echo "run"; })();
来源：http://wb.newstarts.cn

JS:   (() => { console.log("run"); })();
来源：http://wi.jianghongdianzi.cn

TS:   (() => { console.log("run"); })();
来源：http://fp.muxihuayi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xx.szxytkj.cn


<!-- 参考信息 -->