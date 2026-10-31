代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://pr.chemitech.net.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cc.haigaiapp.cn

TS:   // Node.js：readline 模块
来源：http://yp.jctech888.com.cn

Java: new Scanner(System.in).nextLine()
来源：http://hi.huixiangedu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xc.szxytkj.cn

Ruby: gets.chomp
来源：http://tb.muxihuayi.cn

C#:   Console.ReadLine();
来源：http://xh.nicolike.cn

[A21] 保留指定小数位输出
来源：http://bs.wgjwhj.cn

Py:   f"{3.14159:.2f}"
来源：http://mv.bjjhwx.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jz.huixiangedu.cn

JS:   (3.14159).toFixed(2)
来源：http://dz.haigaiapp.cn

TS:   (3.14159).toFixed(2)
来源：http://gf.chemitech.net.cn

Java: String.format("%.2f", 3.14159)
来源：http://ol.hnjuh.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ip.asd995.cn

Ruby: format("%.2f", 3.14159)
来源：http://jp.hnjuh.cn

C#:   3.14159.ToString("F2")
来源：http://ck.wgjwhj.cn

[A22] 获取字符串长度
来源：http://wp.newstarts.cn

Py:   len(s)
来源：http://nj.9csxet.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ir.chemitech.net.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://yh.colortex.cn

TS:   s.length
来源：http://ur.panjiajie.cn

Java: s.length()
来源：http://jr.hnjuh.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hw.newstarts.cn

Ruby: s.length
来源：http://ft.yuexingan06.cn

C#:   s.Length
来源：http://nh.yuexingan06.cn

[A23] 大小写转换
来源：http://lg.nicolike.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://if.huixiangedu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://es.jctech888.com.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://id.nszjky.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hj.shtwfgs.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zs.haigaiapp.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://oq.panjiajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vx.hnjuh.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qk.wgjwhj.cn

[A24] 去除首尾空白
来源：http://le.newstarts.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sw.jianghongdianzi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vd.hnjuh.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ws.nszjky.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ys.newstarts.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nm.asd995.cn

Go:   strings.TrimSpace(s)
来源：http://rx.jianghongdianzi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hf.muxihuayi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wf.hahajie.cn

[A25] 字符串比较
来源：http://cw.hahajie.cn

Py:   s1 == s2; s1 != s2
来源：http://kr.jianghongdianzi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gy.shxzskj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ta.chemitech.net.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://eq.asd995.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mu.asd995.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wy.haigaiapp.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://gm.muxihuayi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jl.newstarts.cn

[A26] 类型转换总览
来源：http://sk.nicolike.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mi.panjiajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kb.shtwfgs.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nd.haigaiapp.cn

TS:   Number() String() Boolean() x as number
来源：http://ww.newstarts.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ze.szxytkj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ad.yuntaijiaju.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://kb.shxzskj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ig.lnxyls.cn

================================================================================
来源：http://lo.nszjky.cn

B. 流程控制
来源：http://sv.muxihuayi.cn

================================================================================
来源：http://ol.colortex.cn

[B01] 条件判断 if / else
来源：http://jc.lnxyls.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://iu.muxihuayi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qe.shxzskj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rr.nszjky.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ma.shxzskj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://sj.9csxet.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://il.szxytkj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tg.szsharing.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ns.haigaiapp.cn

[B02] 多分支 else if / elif
来源：http://xs.szxytkj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kp.bookmarksfly.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xl.szsharing.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xt.huanxung.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sj.jctech888.com.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dv.szxytkj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://sz.jctech888.com.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://sp.panjiajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cc.muxihuayi.cn

[B03] switch / match / case
来源：http://jx.hahajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ph.nszjky.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ye.lnxyls.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nj.jctech888.com.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mv.9csxet.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bv.chemitech.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vk.jianghongdianzi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jc.huanxung.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sy.colortex.cn

[B04] for 计数循环
来源：http://hu.shxzskj.cn

Py:   for i in range(10): print(i)
来源：http://it.asd995.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ru.panjiajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qk.huixiangedu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dp.colortex.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://sj.gzmigu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ig.lnxyls.cn

Ruby: 10.times { |i| puts i }
来源：http://lo.colortex.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xn.shtwfgs.cn

[B05] 遍历数组 / 列表
来源：http://kw.bjjhwx.cn

Py:   for item in arr: print(item)
来源：http://jj.szsharing.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kr.gzmigu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://lu.newstarts.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://vl.bookmarksfly.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pl.yuexingan06.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hw.huixiangedu.cn

Ruby: arr.each { |item| puts item }
来源：http://id.shxzskj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://iq.jianghongdianzi.cn

[B06] 遍历字典 / 对象
来源：http://gf.nicolike.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qp.shxzukj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hc.gzmigu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://si.jianghongdianzi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://by.yuntaijiaju.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cl.shxzukj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bx.huixinmuqiang.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ym.muxihuayi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://di.asd995.cn

[B07] while 循环
来源：http://ad.wgjwhj.cn

Py:   while i < 10: i += 1
来源：http://jv.huanxung.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lb.jctech888.com.cn

JS:   while (i < 10) { i++; }
来源：http://uv.wgjwhj.cn

TS:   while (i < 10) { i++; }
来源：http://xg.nszjky.cn

Java: while (i < 10) { i++; }
来源：http://zr.gzmigu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nx.bookmarksfly.cn

Ruby: while i < 10; i += 1; end
来源：http://fo.bjjhwx.cn

C#:   while (i < 10) { i++; }
来源：http://mc.panjiajie.cn

[B08] do-while（至少执行一次）
来源：http://md.panjiajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://xo.newstarts.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://lx.9csxet.cn

JS:   do { i++; } while (i < 10);
来源：http://iu.haigaiapp.cn

TS:   do { i++; } while (i < 10);
来源：http://zm.hahajie.cn

Java: do { i++; } while (i < 10);
来源：http://zh.hahajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://et.huixinmuqiang.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ua.hnjuh.cn

C#:   do { i++; } while (i < 10);
来源：http://ha.newstarts.cn

[B09] break 与 continue
来源：http://wl.lnxyls.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vu.szxytkj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wc.szsharing.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ed.shxzskj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ek.huixinmuqiang.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xs.huixinmuqiang.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://us.asd995.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gz.szxytkj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vv.szxytkj.cn

[B10] 遍历同时拿索引
来源：http://bm.haigaiapp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kl.9csxet.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jy.hahajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kf.9csxet.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uf.newstarts.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gp.muxihuayi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sr.lnxyls.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gm.jctech888.com.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://aa.yuexingan06.cn

[B11] 生成数字序列 / 区间
来源：http://mn.colortex.cn

Py:   list(range(0, 10, 2))
来源：http://ps.shtwfgs.cn

PHP:  range(0, 10, 2);
来源：http://be.shxzukj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zg.nszjky.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nl.haigaiapp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gk.szxytkj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pv.chemitech.net.cn

Ruby: (0...10).step(2).to_a
来源：http://hs.gzmigu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uf.huixinmuqiang.cn

[B12] 跳出多层循环
来源：http://wy.panjiajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://cx.lnxyls.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ro.yuexingan06.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sq.521024.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fy.szxytkj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gl.hahajie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://li.huanxung.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kr.9csxet.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wy.hahajie.cn

[B13] 判断是否为数字
来源：http://is.shxzukj.cn

Py:   isinstance(x, (int, float))
来源：http://ly.szsharing.cn

PHP:  is_numeric($x)
来源：http://nv.szsharing.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://he.panjiajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://as.haigaiapp.cn

Java: x instanceof Number
来源：http://xg.bookmarksfly.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cl.9csxet.cn

Ruby: x.is_a?(Numeric)
来源：http://hy.haigaiapp.cn

C#:   x is int or double or decimal
来源：http://ur.9csxet.cn

[B14] 判断值是否在集合内
来源：http://ak.bookmarksfly.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lg.wgjwhj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sf.newstarts.cn

JS:   [1, 2, 3].includes(x)
来源：http://ma.shxzukj.cn

TS:   [1, 2, 3].includes(x)
来源：http://nt.9csxet.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ff.hnjuh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://db.chemitech.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://bw.gzmigu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zj.huanxung.cn

[B15] 布尔运算与取反
来源：http://gs.colortex.cn

Py:   a and b or not c
来源：http://pb.panjiajie.cn

PHP:  $a && $b || !$c
来源：http://ss.shxzskj.cn

JS:   a && b || !c
来源：http://et.yuexingan06.cn

TS:   a && b || !c
来源：http://we.bjjhwx.cn

Java: a && b || !c
来源：http://zm.bjjhwx.cn

Go:   a && b || !c
来源：http://kb.asd995.cn

Ruby: a && b || !c
来源：http://kh.521024.cn

C#:   a && b || !c
来源：http://vj.huixinmuqiang.cn

[B16] 卫语句：不满足条件提前返回
来源：http://my.nicolike.cn

Py:   if not data: return
来源：http://zq.nicolike.cn

PHP:  if (!$data) { return; }
来源：http://aa.shxzukj.cn

JS:   if (!data) return;
来源：http://vx.nszjky.cn

TS:   if (!data) return;
来源：http://zg.hahajie.cn

Java: if (data == null) return;
来源：http://jf.newstarts.cn

Go:   if data == nil { return }
来源：http://dd.9csxet.cn

Ruby: return if data.nil?
来源：http://kz.jctech888.com.cn

C#:   if (data == null) return;
来源：http://ks.colortex.cn

================================================================================
来源：http://hg.jctech888.com.cn

C. 函数与作用域
来源：http://tp.wgjwhj.cn

================================================================================
来源：http://xt.chemitech.net.cn

[C01] 定义函数
来源：http://pr.huixiangedu.cn

Py:   def add(a, b): return a + b
来源：http://ze.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rx.szsharing.cn

JS:   function add(a, b) { return a + b; }
来源：http://ch.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bx.lnxyls.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mr.nicolike.cn

Go:   func add(a, b int) int { return a + b }
来源：http://sg.chemitech.net.cn

Ruby: def add(a, b); a + b; end
来源：http://ji.hnjuh.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xp.asd995.cn

[C02] 默认参数
来源：http://yp.bjjhwx.cn

Py:   def greet(name="World"): return name
来源：http://mn.hnjuh.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qy.haigaiapp.cn

JS:   function greet(name = "World") { return name; }
来源：http://ja.521024.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qs.jianghongdianzi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://tb.jctech888.com.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mz.bjjhwx.cn

Ruby: def greet(name = "World") = name
来源：http://hz.shxzukj.cn

C#:   string Greet(string name = "World") => name;
来源：http://ju.chemitech.net.cn

[C03] 可变参数
来源：http://sz.szsharing.cn

Py:   def total(*args): return sum(args)
来源：http://hx.huixinmuqiang.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zg.muxihuayi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ev.yuexingan06.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pb.yuntaijiaju.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mi.newstarts.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://oz.gzmigu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fk.szxytkj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ub.newstarts.cn

[C04] 命名参数 / 关键字参数
来源：http://eq.yuexingan06.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sk.panjiajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rh.huixinmuqiang.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vs.lnxyls.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mp.panjiajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://gf.hahajie.cn

Go:   // 无：用配置结构体参数
来源：http://ae.lnxyls.cn

Ruby: f(a: 1, b: 2)
来源：http://ru.bookmarksfly.cn

C#:   f(a: 1, b: 2)
来源：http://od.bjjhwx.cn

[C05] 返回多个值
来源：http://mr.wgjwhj.cn

Py:   return a, b
来源：http://ee.bookmarksfly.cn

PHP:  return [$a, $b];
来源：http://mx.chemitech.net.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://se.jianghongdianzi.cn

TS:   return { a, b };
来源：http://sx.muxihuayi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vi.gzmigu.cn

Go:   return a, b
来源：http://yy.newstarts.cn

Ruby: return a, b
来源：http://qi.hnjuh.cn

C#:   return (a, b);              // ValueTuple
来源：http://rh.colortex.cn

[C06] 匿名函数 / lambda
来源：http://an.9csxet.cn

Py:   square = lambda x: x * x
来源：http://uc.newstarts.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://sj.shxzukj.cn

JS:   const square = x => x * x;
来源：http://ag.colortex.cn

TS:   const square = (x: number): number => x * x;
来源：http://vl.szsharing.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://av.gzmigu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://li.colortex.cn

Ruby: square = ->(x) { x * x }
来源：http://kx.lnxyls.cn

C#:   Func<int, int> square = x => x * x;
来源：http://pg.lnxyls.cn

[C07] 把函数作为参数传入
来源：http://ls.huixiangedu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://le.yuntaijiaju.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hi.szxytkj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wp.newstarts.cn

TS:   arr.map(String)
来源：http://xh.huixiangedu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pj.huixiangedu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dw.szxytkj.cn

Ruby: arr.map(&:upcase)
来源：http://hj.haigaiapp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ue.colortex.cn

[C08] 闭包
来源：http://ow.newstarts.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bn.szsharing.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jq.hnjuh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fj.yuexingan06.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tr.nicolike.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tz.521024.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sy.colortex.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gb.colortex.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bb.shtwfgs.cn

[C09] 递归
来源：http://bv.9csxet.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://oz.bjjhwx.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bf.nicolike.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uq.szsharing.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://le.huixiangedu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ba.muxihuayi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ki.yuntaijiaju.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jh.yuexingan06.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://he.shxzukj.cn

[C10] 变量作用域
来源：http://rf.shxzskj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ee.asd995.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://uh.gzmigu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ff.9csxet.cn

TS:   同 JS
来源：http://pe.szxytkj.cn

Java: 方法内为块级作用域
来源：http://nw.shtwfgs.cn

Go:   花括号块级作用域
来源：http://mc.wgjwhj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ka.yuexingan06.cn


<!-- 参考信息 -->