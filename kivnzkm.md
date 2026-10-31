代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://td.hnjuh.cn

Ruby: gets.chomp
来源：http://ro.bookmarksfly.cn

C#:   Console.ReadLine();
来源：http://qk.lnxyls.cn

[A21] 保留指定小数位输出
来源：http://ng.hnjuh.cn

Py:   f"{3.14159:.2f}"
来源：http://pt.shxzskj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://og.huanxung.cn

JS:   (3.14159).toFixed(2)
来源：http://ml.shtwfgs.cn

TS:   (3.14159).toFixed(2)
来源：http://yu.huixiangedu.cn

Java: String.format("%.2f", 3.14159)
来源：http://tg.szsharing.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://dh.yuexingan06.cn

Ruby: format("%.2f", 3.14159)
来源：http://xk.shtwfgs.cn

C#:   3.14159.ToString("F2")
来源：http://bz.huanxung.cn

[A22] 获取字符串长度
来源：http://vm.hahajie.cn

Py:   len(s)
来源：http://zz.newstarts.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ff.newstarts.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://dv.jctech888.com.cn

TS:   s.length
来源：http://au.gzmigu.cn

Java: s.length()
来源：http://mz.asd995.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kf.muxihuayi.cn

Ruby: s.length
来源：http://pq.nszjky.cn

C#:   s.Length
来源：http://rl.shxzskj.cn

[A23] 大小写转换
来源：http://ai.huixinmuqiang.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://fq.newstarts.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mr.jianghongdianzi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vj.bjjhwx.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cd.newstarts.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://re.haigaiapp.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://th.huanxung.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ie.bookmarksfly.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://os.haigaiapp.cn

[A24] 去除首尾空白
来源：http://tu.newstarts.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wy.bookmarksfly.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://uj.nszjky.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ya.haigaiapp.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ur.yuexingan06.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xo.521024.cn

Go:   strings.TrimSpace(s)
来源：http://pn.nszjky.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lm.hahajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vv.huixiangedu.cn

[A25] 字符串比较
来源：http://kv.szxytkj.cn

Py:   s1 == s2; s1 != s2
来源：http://jm.9csxet.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ls.bjjhwx.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://st.bookmarksfly.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gb.hnjuh.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jq.jctech888.com.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lz.nszjky.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://jb.shxzskj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gm.muxihuayi.cn

[A26] 类型转换总览
来源：http://zd.asd995.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vk.jctech888.com.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ua.hnjuh.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zr.newstarts.cn

TS:   Number() String() Boolean() x as number
来源：http://oc.521024.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vf.wgjwhj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ev.nszjky.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://uy.hnjuh.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cv.gzmigu.cn

================================================================================
来源：http://xc.9csxet.cn

B. 流程控制
来源：http://wr.wgjwhj.cn

================================================================================
来源：http://hz.yuexingan06.cn

[B01] 条件判断 if / else
来源：http://mg.szxytkj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://pf.bookmarksfly.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xx.nicolike.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nv.nszjky.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sc.huixiangedu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://zo.nicolike.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://av.yuntaijiaju.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://oe.chemitech.net.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tk.szxytkj.cn

[B02] 多分支 else if / elif
来源：http://jc.huixiangedu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tb.huanxung.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://uc.newstarts.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ew.colortex.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ok.bookmarksfly.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xg.521024.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xl.huixiangedu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ye.hnjuh.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wm.chemitech.net.cn

[B03] switch / match / case
来源：http://yp.huixiangedu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jk.yuexingan06.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://iu.szsharing.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nk.jctech888.com.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://id.shxzskj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ih.szxytkj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vj.shxzukj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ma.panjiajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xq.lnxyls.cn

[B04] for 计数循环
来源：http://uh.jianghongdianzi.cn

Py:   for i in range(10): print(i)
来源：http://ps.szxytkj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sr.gzmigu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kv.asd995.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ch.yuexingan06.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mi.gzmigu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rk.huixinmuqiang.cn

Ruby: 10.times { |i| puts i }
来源：http://gv.hahajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vp.wgjwhj.cn

[B05] 遍历数组 / 列表
来源：http://tk.bookmarksfly.cn

Py:   for item in arr: print(item)
来源：http://ci.wgjwhj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://po.jctech888.com.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://lx.hnjuh.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://go.shtwfgs.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hi.hahajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bg.lnxyls.cn

Ruby: arr.each { |item| puts item }
来源：http://ly.asd995.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wt.jctech888.com.cn

[B06] 遍历字典 / 对象
来源：http://bo.9csxet.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ca.szxytkj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://eh.huixinmuqiang.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ps.yuntaijiaju.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xy.newstarts.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xe.bookmarksfly.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pi.szxytkj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rj.bjjhwx.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yw.gzmigu.cn

[B07] while 循环
来源：http://jt.bjjhwx.cn

Py:   while i < 10: i += 1
来源：http://eg.haigaiapp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gi.bookmarksfly.cn

JS:   while (i < 10) { i++; }
来源：http://nk.newstarts.cn

TS:   while (i < 10) { i++; }
来源：http://lc.lnxyls.cn

Java: while (i < 10) { i++; }
来源：http://xo.shxzukj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ln.wgjwhj.cn

Ruby: while i < 10; i += 1; end
来源：http://zs.chemitech.net.cn

C#:   while (i < 10) { i++; }
来源：http://ju.nszjky.cn

[B08] do-while（至少执行一次）
来源：http://wh.bookmarksfly.cn

Py:   # 无 do-while：用 while True + break
来源：http://fn.chemitech.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://tu.colortex.cn

JS:   do { i++; } while (i < 10);
来源：http://fn.shtwfgs.cn

TS:   do { i++; } while (i < 10);
来源：http://cj.nicolike.cn

Java: do { i++; } while (i < 10);
来源：http://wv.shxzukj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://kx.bjjhwx.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hu.nicolike.cn

C#:   do { i++; } while (i < 10);
来源：http://rw.yuntaijiaju.cn

[B09] break 与 continue
来源：http://dq.nicolike.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://os.wgjwhj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uq.huanxung.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wa.huixiangedu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pa.hahajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gm.huixinmuqiang.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ys.huixiangedu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ka.huixinmuqiang.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ce.panjiajie.cn

[B10] 遍历同时拿索引
来源：http://wu.hahajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xi.yuexingan06.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qy.shtwfgs.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://im.szxytkj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qe.colortex.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://du.huixinmuqiang.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zd.nszjky.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jo.jctech888.com.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ts.shtwfgs.cn

[B11] 生成数字序列 / 区间
来源：http://st.newstarts.cn

Py:   list(range(0, 10, 2))
来源：http://dh.chemitech.net.cn

PHP:  range(0, 10, 2);
来源：http://su.jianghongdianzi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dd.521024.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bu.nicolike.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cg.jctech888.com.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jx.huanxung.cn

Ruby: (0...10).step(2).to_a
来源：http://nz.newstarts.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ec.muxihuayi.cn

[B12] 跳出多层循环
来源：http://hf.shtwfgs.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://sr.nicolike.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://xo.szxytkj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kg.szxytkj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cq.nicolike.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://je.521024.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ed.yuntaijiaju.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mr.muxihuayi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lv.gzmigu.cn

[B13] 判断是否为数字
来源：http://xw.asd995.cn

Py:   isinstance(x, (int, float))
来源：http://pj.szxytkj.cn

PHP:  is_numeric($x)
来源：http://jz.wgjwhj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dz.hahajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://in.nszjky.cn

Java: x instanceof Number
来源：http://zp.yuntaijiaju.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ve.shxzukj.cn

Ruby: x.is_a?(Numeric)
来源：http://wz.hahajie.cn

C#:   x is int or double or decimal
来源：http://lj.nszjky.cn

[B14] 判断值是否在集合内
来源：http://ua.yuexingan06.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ay.jctech888.com.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gl.asd995.cn

JS:   [1, 2, 3].includes(x)
来源：http://dy.asd995.cn

TS:   [1, 2, 3].includes(x)
来源：http://lw.muxihuayi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ji.gzmigu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://me.huanxung.cn

Ruby: [1, 2, 3].include?(x)
来源：http://yb.521024.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yj.chemitech.net.cn

[B15] 布尔运算与取反
来源：http://lw.huixiangedu.cn

Py:   a and b or not c
来源：http://sn.asd995.cn

PHP:  $a && $b || !$c
来源：http://mz.wgjwhj.cn

JS:   a && b || !c
来源：http://pu.521024.cn

TS:   a && b || !c
来源：http://fb.szsharing.cn

Java: a && b || !c
来源：http://to.haigaiapp.cn

Go:   a && b || !c
来源：http://ed.nszjky.cn

Ruby: a && b || !c
来源：http://ma.chemitech.net.cn

C#:   a && b || !c
来源：http://gp.lnxyls.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gm.jianghongdianzi.cn

Py:   if not data: return
来源：http://mi.jctech888.com.cn

PHP:  if (!$data) { return; }
来源：http://fr.panjiajie.cn

JS:   if (!data) return;
来源：http://qw.yuntaijiaju.cn

TS:   if (!data) return;
来源：http://rl.jianghongdianzi.cn

Java: if (data == null) return;
来源：http://yc.lnxyls.cn

Go:   if data == nil { return }
来源：http://km.yuexingan06.cn

Ruby: return if data.nil?
来源：http://tu.yuntaijiaju.cn

C#:   if (data == null) return;
来源：http://vc.bookmarksfly.cn

================================================================================
来源：http://ym.bjjhwx.cn

C. 函数与作用域
来源：http://fa.szsharing.cn

================================================================================
来源：http://de.nicolike.cn

[C01] 定义函数
来源：http://wl.shtwfgs.cn

Py:   def add(a, b): return a + b
来源：http://vt.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vz.huixiangedu.cn

JS:   function add(a, b) { return a + b; }
来源：http://dy.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fq.jianghongdianzi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hw.jianghongdianzi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ad.huixiangedu.cn

Ruby: def add(a, b); a + b; end
来源：http://ah.shxzukj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jv.szxytkj.cn

[C02] 默认参数
来源：http://sd.yuexingan06.cn

Py:   def greet(name="World"): return name
来源：http://rl.9csxet.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dk.colortex.cn

JS:   function greet(name = "World") { return name; }
来源：http://uf.szxytkj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://sc.nszjky.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zn.panjiajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fx.9csxet.cn

Ruby: def greet(name = "World") = name
来源：http://ac.gzmigu.cn

C#:   string Greet(string name = "World") => name;
来源：http://fw.jctech888.com.cn

[C03] 可变参数
来源：http://mc.huanxung.cn

Py:   def total(*args): return sum(args)
来源：http://ce.bookmarksfly.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ne.yuntaijiaju.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mh.szsharing.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xu.muxihuayi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://an.521024.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sv.yuntaijiaju.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qx.nicolike.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ir.shxzskj.cn

[C04] 命名参数 / 关键字参数
来源：http://ej.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ue.muxihuayi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://or.szsharing.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zh.newstarts.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xb.huixinmuqiang.cn

Java: // 无：用 Builder 模式或 record
来源：http://la.shtwfgs.cn

Go:   // 无：用配置结构体参数
来源：http://ja.jianghongdianzi.cn

Ruby: f(a: 1, b: 2)
来源：http://ye.jctech888.com.cn

C#:   f(a: 1, b: 2)
来源：http://it.yuntaijiaju.cn

[C05] 返回多个值
来源：http://ps.wgjwhj.cn

Py:   return a, b
来源：http://cs.9csxet.cn

PHP:  return [$a, $b];
来源：http://ij.muxihuayi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ty.nszjky.cn

TS:   return { a, b };
来源：http://fv.gzmigu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fs.wgjwhj.cn

Go:   return a, b
来源：http://sp.bjjhwx.cn

Ruby: return a, b
来源：http://pw.jctech888.com.cn

C#:   return (a, b);              // ValueTuple
来源：http://rt.wgjwhj.cn

[C06] 匿名函数 / lambda
来源：http://nb.yuntaijiaju.cn

Py:   square = lambda x: x * x
来源：http://vs.gzmigu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://cs.jctech888.com.cn

JS:   const square = x => x * x;
来源：http://fc.szsharing.cn

TS:   const square = (x: number): number => x * x;
来源：http://ql.521024.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gw.haigaiapp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zn.panjiajie.cn

Ruby: square = ->(x) { x * x }
来源：http://lh.jctech888.com.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ph.hahajie.cn

[C07] 把函数作为参数传入
来源：http://fm.hnjuh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xy.521024.cn

PHP:  array_map("strtoupper", $arr);
来源：http://pw.huixinmuqiang.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hw.muxihuayi.cn

TS:   arr.map(String)
来源：http://vh.huanxung.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ju.bookmarksfly.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nr.jianghongdianzi.cn

Ruby: arr.map(&:upcase)
来源：http://ay.521024.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qz.huanxung.cn

[C08] 闭包
来源：http://ng.nicolike.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ms.nszjky.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gz.asd995.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fv.asd995.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://al.shxzukj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lz.bookmarksfly.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://uo.nicolike.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://al.chemitech.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zn.haigaiapp.cn

[C09] 递归
来源：http://qy.huixinmuqiang.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lo.asd995.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fm.shxzskj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qm.yuntaijiaju.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gh.lnxyls.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lp.hnjuh.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cb.jianghongdianzi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://to.colortex.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uj.yuexingan06.cn

[C10] 变量作用域
来源：http://zq.wgjwhj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://aq.yuntaijiaju.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qx.szsharing.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://au.szsharing.cn

TS:   同 JS
来源：http://ua.colortex.cn

Java: 方法内为块级作用域
来源：http://kk.jianghongdianzi.cn

Go:   花括号块级作用域
来源：http://ru.chemitech.net.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xo.colortex.cn

C#:   块级作用域
来源：http://po.newstarts.cn

[C11] 模块导入与导出
来源：http://qb.bjjhwx.cn

Py:   from module import func
来源：http://cj.nszjky.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://nd.panjiajie.cn


<!-- 参考信息 -->