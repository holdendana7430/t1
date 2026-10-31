代发 wailian999

JS:   [a, b] = [b, a];
来源：http://fo.nszjky.cn

TS:   [a, b] = [b, a];
来源：http://yv.nszjky.cn

Java: int t = a; a = b; b = t;
来源：http://zr.521024.cn

Go:   a, b = b, a
来源：http://df.huanxung.cn

Ruby: a, b = b, a
来源：http://aa.huixinmuqiang.cn

C#:   (a, b) = (b, a);
来源：http://pp.shxzukj.cn

[A20] 读取标准输入
来源：http://vp.gzmigu.cn

Py:   name = input("请输入：")
来源：http://mi.shtwfgs.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://zl.szxytkj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bb.yuntaijiaju.cn

TS:   // Node.js：readline 模块
来源：http://rb.yuexingan06.cn

Java: new Scanner(System.in).nextLine()
来源：http://wd.nicolike.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hx.shtwfgs.cn

Ruby: gets.chomp
来源：http://rn.yuntaijiaju.cn

C#:   Console.ReadLine();
来源：http://rz.yuexingan06.cn

[A21] 保留指定小数位输出
来源：http://lk.9csxet.cn

Py:   f"{3.14159:.2f}"
来源：http://pz.panjiajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xp.muxihuayi.cn

JS:   (3.14159).toFixed(2)
来源：http://yl.shxzskj.cn

TS:   (3.14159).toFixed(2)
来源：http://aa.szxytkj.cn

Java: String.format("%.2f", 3.14159)
来源：http://kp.wgjwhj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ob.lnxyls.cn

Ruby: format("%.2f", 3.14159)
来源：http://ak.szxytkj.cn

C#:   3.14159.ToString("F2")
来源：http://hs.bjjhwx.cn

[A22] 获取字符串长度
来源：http://nn.nicolike.cn

Py:   len(s)
来源：http://eb.nicolike.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://lg.bookmarksfly.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ih.bjjhwx.cn

TS:   s.length
来源：http://ha.nicolike.cn

Java: s.length()
来源：http://qu.shtwfgs.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ey.colortex.cn

Ruby: s.length
来源：http://ni.nszjky.cn

C#:   s.Length
来源：http://ix.bookmarksfly.cn

[A23] 大小写转换
来源：http://vk.colortex.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://mp.panjiajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://on.yuntaijiaju.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hk.huixinmuqiang.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lb.gzmigu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ct.newstarts.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vx.szsharing.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bf.hahajie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zi.chemitech.net.cn

[A24] 去除首尾空白
来源：http://xx.szsharing.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://to.shxzukj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fh.shxzukj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qq.huixinmuqiang.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ya.hahajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ea.huanxung.cn

Go:   strings.TrimSpace(s)
来源：http://pz.521024.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fq.shtwfgs.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kd.jianghongdianzi.cn

[A25] 字符串比较
来源：http://ll.jctech888.com.cn

Py:   s1 == s2; s1 != s2
来源：http://ys.nszjky.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://az.panjiajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wg.wgjwhj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xl.bookmarksfly.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tm.haigaiapp.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nt.nszjky.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://dn.asd995.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dr.hnjuh.cn

[A26] 类型转换总览
来源：http://gu.wgjwhj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kb.asd995.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kr.9csxet.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pu.9csxet.cn

TS:   Number() String() Boolean() x as number
来源：http://dk.huixinmuqiang.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bj.nszjky.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://no.newstarts.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://oe.yuntaijiaju.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ty.jctech888.com.cn

================================================================================
来源：http://hn.gzmigu.cn

B. 流程控制
来源：http://kw.szsharing.cn

================================================================================
来源：http://lf.szsharing.cn

[B01] 条件判断 if / else
来源：http://ot.nicolike.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://be.jianghongdianzi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tq.jianghongdianzi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mw.huixiangedu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gm.muxihuayi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vh.asd995.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wd.lnxyls.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pa.huixiangedu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://er.jianghongdianzi.cn

[B02] 多分支 else if / elif
来源：http://my.lnxyls.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fg.yuntaijiaju.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bs.newstarts.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ue.hnjuh.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uf.jianghongdianzi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hk.gzmigu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tc.muxihuayi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ry.newstarts.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://th.chemitech.net.cn

[B03] switch / match / case
来源：http://ad.hahajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jr.muxihuayi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hj.shxzukj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ds.bookmarksfly.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kg.shtwfgs.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kb.shxzskj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tx.huixiangedu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lc.muxihuayi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wz.gzmigu.cn

[B04] for 计数循环
来源：http://de.huanxung.cn

Py:   for i in range(10): print(i)
来源：http://ta.shxzukj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://um.shxzukj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gn.shxzukj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://el.9csxet.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://by.huixinmuqiang.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mt.jianghongdianzi.cn

Ruby: 10.times { |i| puts i }
来源：http://gb.panjiajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://oz.shxzskj.cn

[B05] 遍历数组 / 列表
来源：http://dv.szxytkj.cn

Py:   for item in arr: print(item)
来源：http://jm.yuntaijiaju.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ov.szxytkj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://me.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://dw.yuntaijiaju.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://od.jctech888.com.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bp.521024.cn

Ruby: arr.each { |item| puts item }
来源：http://yj.jctech888.com.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ir.shtwfgs.cn

[B06] 遍历字典 / 对象
来源：http://zd.jianghongdianzi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ra.nicolike.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ea.nicolike.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://px.chemitech.net.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ha.huanxung.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://an.huixinmuqiang.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sr.newstarts.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://if.asd995.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qt.bjjhwx.cn

[B07] while 循环
来源：http://rk.huixiangedu.cn

Py:   while i < 10: i += 1
来源：http://st.yuntaijiaju.cn

PHP:  while ($i < 10) { $i++; }
来源：http://cv.hnjuh.cn

JS:   while (i < 10) { i++; }
来源：http://kl.shtwfgs.cn

TS:   while (i < 10) { i++; }
来源：http://pv.haigaiapp.cn

Java: while (i < 10) { i++; }
来源：http://du.jianghongdianzi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bv.yuntaijiaju.cn

Ruby: while i < 10; i += 1; end
来源：http://my.gzmigu.cn

C#:   while (i < 10) { i++; }
来源：http://na.panjiajie.cn

[B08] do-while（至少执行一次）
来源：http://tt.panjiajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://br.muxihuayi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://bi.huixinmuqiang.cn

JS:   do { i++; } while (i < 10);
来源：http://vf.bookmarksfly.cn

TS:   do { i++; } while (i < 10);
来源：http://ow.521024.cn

Java: do { i++; } while (i < 10);
来源：http://ro.lnxyls.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://iw.yuntaijiaju.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rv.szxytkj.cn

C#:   do { i++; } while (i < 10);
来源：http://ci.haigaiapp.cn

[B09] break 与 continue
来源：http://lf.szxytkj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pl.chemitech.net.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://td.9csxet.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ip.wgjwhj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yl.huixiangedu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yr.huixiangedu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://co.hnjuh.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rd.bjjhwx.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://id.panjiajie.cn

[B10] 遍历同时拿索引
来源：http://av.wgjwhj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pi.yuntaijiaju.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bp.shxzukj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://th.szsharing.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fc.lnxyls.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ya.asd995.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gf.jianghongdianzi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kv.9csxet.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cb.hnjuh.cn

[B11] 生成数字序列 / 区间
来源：http://kl.szxytkj.cn

Py:   list(range(0, 10, 2))
来源：http://du.chemitech.net.cn

PHP:  range(0, 10, 2);
来源：http://in.chemitech.net.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kb.lnxyls.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rw.colortex.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vq.haigaiapp.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qe.yuexingan06.cn

Ruby: (0...10).step(2).to_a
来源：http://ma.bookmarksfly.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gc.huixinmuqiang.cn

[B12] 跳出多层循环
来源：http://ul.521024.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://oa.shxzskj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://sh.jianghongdianzi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://td.newstarts.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dg.nicolike.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wr.newstarts.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ev.panjiajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wc.szsharing.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pe.gzmigu.cn

[B13] 判断是否为数字
来源：http://eu.shtwfgs.cn

Py:   isinstance(x, (int, float))
来源：http://fu.521024.cn

PHP:  is_numeric($x)
来源：http://sk.szsharing.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ld.hnjuh.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://em.jianghongdianzi.cn

Java: x instanceof Number
来源：http://cq.jianghongdianzi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bv.nszjky.cn

Ruby: x.is_a?(Numeric)
来源：http://fn.shtwfgs.cn

C#:   x is int or double or decimal
来源：http://cg.gzmigu.cn

[B14] 判断值是否在集合内
来源：http://mr.9csxet.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qj.521024.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bo.yuntaijiaju.cn

JS:   [1, 2, 3].includes(x)
来源：http://qm.huanxung.cn

TS:   [1, 2, 3].includes(x)
来源：http://wx.newstarts.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://nw.jianghongdianzi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://un.9csxet.cn

Ruby: [1, 2, 3].include?(x)
来源：http://sm.shtwfgs.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dp.hahajie.cn

[B15] 布尔运算与取反
来源：http://nm.panjiajie.cn

Py:   a and b or not c
来源：http://rm.bookmarksfly.cn

PHP:  $a && $b || !$c
来源：http://nq.panjiajie.cn

JS:   a && b || !c
来源：http://lc.shtwfgs.cn

TS:   a && b || !c
来源：http://si.colortex.cn

Java: a && b || !c
来源：http://so.wgjwhj.cn

Go:   a && b || !c
来源：http://ge.panjiajie.cn

Ruby: a && b || !c
来源：http://fg.huanxung.cn

C#:   a && b || !c
来源：http://pe.haigaiapp.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xk.yuntaijiaju.cn

Py:   if not data: return
来源：http://lz.jianghongdianzi.cn

PHP:  if (!$data) { return; }
来源：http://vh.chemitech.net.cn

JS:   if (!data) return;
来源：http://yd.shtwfgs.cn

TS:   if (!data) return;
来源：http://if.nszjky.cn

Java: if (data == null) return;
来源：http://pe.muxihuayi.cn

Go:   if data == nil { return }
来源：http://cz.yuntaijiaju.cn

Ruby: return if data.nil?
来源：http://mp.9csxet.cn

C#:   if (data == null) return;
来源：http://zc.yuexingan06.cn

================================================================================
来源：http://fz.shtwfgs.cn

C. 函数与作用域
来源：http://gw.bookmarksfly.cn

================================================================================
来源：http://pv.haigaiapp.cn

[C01] 定义函数
来源：http://ig.bjjhwx.cn

Py:   def add(a, b): return a + b
来源：http://ox.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cf.asd995.cn

JS:   function add(a, b) { return a + b; }
来源：http://gu.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zb.9csxet.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gh.nicolike.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hk.yuntaijiaju.cn

Ruby: def add(a, b); a + b; end
来源：http://qx.panjiajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mq.lnxyls.cn

[C02] 默认参数
来源：http://kd.bjjhwx.cn

Py:   def greet(name="World"): return name
来源：http://ss.bjjhwx.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://jj.huixinmuqiang.cn

JS:   function greet(name = "World") { return name; }
来源：http://xd.huanxung.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://tj.colortex.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://mi.yuntaijiaju.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ej.yuexingan06.cn

Ruby: def greet(name = "World") = name
来源：http://mh.yuexingan06.cn

C#:   string Greet(string name = "World") => name;
来源：http://io.jianghongdianzi.cn

[C03] 可变参数
来源：http://gi.bjjhwx.cn

Py:   def total(*args): return sum(args)
来源：http://jf.panjiajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xo.jctech888.com.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cs.nicolike.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ae.yuntaijiaju.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://uv.panjiajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gr.colortex.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yn.nszjky.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://om.szsharing.cn

[C04] 命名参数 / 关键字参数
来源：http://wl.colortex.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://br.muxihuayi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zy.9csxet.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://aq.bookmarksfly.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xr.asd995.cn

Java: // 无：用 Builder 模式或 record
来源：http://yn.shxzskj.cn

Go:   // 无：用配置结构体参数
来源：http://hi.szxytkj.cn

Ruby: f(a: 1, b: 2)
来源：http://pm.haigaiapp.cn

C#:   f(a: 1, b: 2)
来源：http://my.nszjky.cn

[C05] 返回多个值
来源：http://qf.panjiajie.cn

Py:   return a, b
来源：http://nn.newstarts.cn

PHP:  return [$a, $b];
来源：http://zk.newstarts.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ph.jctech888.com.cn

TS:   return { a, b };
来源：http://hy.jctech888.com.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jw.szxytkj.cn

Go:   return a, b
来源：http://gt.muxihuayi.cn

Ruby: return a, b
来源：http://yd.muxihuayi.cn

C#:   return (a, b);              // ValueTuple
来源：http://mn.shtwfgs.cn

[C06] 匿名函数 / lambda
来源：http://zl.521024.cn

Py:   square = lambda x: x * x
来源：http://yz.hnjuh.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://uv.yuexingan06.cn

JS:   const square = x => x * x;
来源：http://oo.szsharing.cn

TS:   const square = (x: number): number => x * x;
来源：http://ka.hahajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://da.huixinmuqiang.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fe.colortex.cn

Ruby: square = ->(x) { x * x }
来源：http://so.panjiajie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qw.gzmigu.cn

[C07] 把函数作为参数传入
来源：http://ad.muxihuayi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wh.lnxyls.cn

PHP:  array_map("strtoupper", $arr);
来源：http://eb.szsharing.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://th.newstarts.cn

TS:   arr.map(String)
来源：http://te.szsharing.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vj.huanxung.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ji.haigaiapp.cn

Ruby: arr.map(&:upcase)
来源：http://nv.521024.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pv.jctech888.com.cn

[C08] 闭包
来源：http://ex.panjiajie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hw.newstarts.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://md.huixiangedu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pd.nicolike.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yi.yuexingan06.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lu.jctech888.com.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wq.521024.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yd.wgjwhj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kd.huixinmuqiang.cn

[C09] 递归
来源：http://or.szxytkj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nk.muxihuayi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qv.shtwfgs.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vc.bookmarksfly.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://so.yuntaijiaju.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rj.shxzskj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qm.gzmigu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xq.huanxung.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hk.hnjuh.cn


<!-- 参考信息 -->