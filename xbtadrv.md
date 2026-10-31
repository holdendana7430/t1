代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pj.huixiangedu.cn

Ruby: gets.chomp
来源：http://bk.hnjuh.cn

C#:   Console.ReadLine();
来源：http://wf.wgjwhj.cn

[A21] 保留指定小数位输出
来源：http://bt.lnxyls.cn

Py:   f"{3.14159:.2f}"
来源：http://jw.nicolike.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qi.shtwfgs.cn

JS:   (3.14159).toFixed(2)
来源：http://qm.jianghongdianzi.cn

TS:   (3.14159).toFixed(2)
来源：http://vt.shxzskj.cn

Java: String.format("%.2f", 3.14159)
来源：http://rc.jianghongdianzi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ie.huixinmuqiang.cn

Ruby: format("%.2f", 3.14159)
来源：http://uv.haigaiapp.cn

C#:   3.14159.ToString("F2")
来源：http://yj.bookmarksfly.cn

[A22] 获取字符串长度
来源：http://et.nicolike.cn

Py:   len(s)
来源：http://vx.huixiangedu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ux.jctech888.com.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bp.colortex.cn

TS:   s.length
来源：http://ks.nicolike.cn

Java: s.length()
来源：http://df.521024.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://uf.521024.cn

Ruby: s.length
来源：http://nf.bookmarksfly.cn

C#:   s.Length
来源：http://nv.yuntaijiaju.cn

[A23] 大小写转换
来源：http://wh.shxzukj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://kd.muxihuayi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ba.panjiajie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xq.bookmarksfly.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://uf.newstarts.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mr.huanxung.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dj.shxzskj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zu.shtwfgs.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qb.yuexingan06.cn

[A24] 去除首尾空白
来源：http://fs.muxihuayi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://eu.huanxung.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hr.nszjky.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cm.shtwfgs.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wp.shxzskj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cm.yuntaijiaju.cn

Go:   strings.TrimSpace(s)
来源：http://gm.huixiangedu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qb.colortex.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vv.hnjuh.cn

[A25] 字符串比较
来源：http://vx.haigaiapp.cn

Py:   s1 == s2; s1 != s2
来源：http://ya.haigaiapp.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ag.bookmarksfly.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gi.chemitech.net.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://oj.bookmarksfly.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mk.yuntaijiaju.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ba.chemitech.net.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://al.huixinmuqiang.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cj.bookmarksfly.cn

[A26] 类型转换总览
来源：http://lx.hnjuh.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ag.yuntaijiaju.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gf.muxihuayi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ab.gzmigu.cn

TS:   Number() String() Boolean() x as number
来源：http://ve.9csxet.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rc.nicolike.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ue.yuntaijiaju.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://kg.colortex.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fc.chemitech.net.cn

================================================================================
来源：http://gg.colortex.cn

B. 流程控制
来源：http://sc.nicolike.cn

================================================================================
来源：http://au.wgjwhj.cn

[B01] 条件判断 if / else
来源：http://zx.nicolike.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://nn.lnxyls.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://iz.hahajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://oa.nicolike.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jh.9csxet.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://sv.haigaiapp.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ae.newstarts.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tf.huixinmuqiang.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://st.bookmarksfly.cn

[B02] 多分支 else if / elif
来源：http://sj.jctech888.com.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bp.shxzukj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lp.yuexingan06.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ep.nszjky.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wa.haigaiapp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pi.panjiajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rk.muxihuayi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bu.wgjwhj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ny.muxihuayi.cn

[B03] switch / match / case
来源：http://lo.nicolike.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fu.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zg.9csxet.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tr.shtwfgs.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bo.hnjuh.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://yu.9csxet.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://us.yuntaijiaju.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rz.colortex.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lp.yuexingan06.cn

[B04] for 计数循环
来源：http://hq.nicolike.cn

Py:   for i in range(10): print(i)
来源：http://qy.nicolike.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xt.newstarts.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gu.9csxet.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sg.wgjwhj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bu.shxzukj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fh.wgjwhj.cn

Ruby: 10.times { |i| puts i }
来源：http://bd.bjjhwx.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sh.huixiangedu.cn

[B05] 遍历数组 / 列表
来源：http://ok.jianghongdianzi.cn

Py:   for item in arr: print(item)
来源：http://yp.colortex.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tx.lnxyls.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fm.muxihuayi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://dp.szxytkj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://bl.panjiajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wu.haigaiapp.cn

Ruby: arr.each { |item| puts item }
来源：http://fm.lnxyls.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://il.shxzukj.cn

[B06] 遍历字典 / 对象
来源：http://pl.yuexingan06.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ou.muxihuayi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://db.asd995.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vg.wgjwhj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sc.huanxung.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ht.jctech888.com.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://oy.shtwfgs.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://su.bjjhwx.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zk.nicolike.cn

[B07] while 循环
来源：http://mr.szxytkj.cn

Py:   while i < 10: i += 1
来源：http://vg.shxzukj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lt.yuntaijiaju.cn

JS:   while (i < 10) { i++; }
来源：http://qc.jctech888.com.cn

TS:   while (i < 10) { i++; }
来源：http://ee.shxzskj.cn

Java: while (i < 10) { i++; }
来源：http://mp.jctech888.com.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kx.haigaiapp.cn

Ruby: while i < 10; i += 1; end
来源：http://qw.szsharing.cn

C#:   while (i < 10) { i++; }
来源：http://es.wgjwhj.cn

[B08] do-while（至少执行一次）
来源：http://fk.huanxung.cn

Py:   # 无 do-while：用 while True + break
来源：http://wd.jianghongdianzi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ow.colortex.cn

JS:   do { i++; } while (i < 10);
来源：http://ma.hahajie.cn

TS:   do { i++; } while (i < 10);
来源：http://xv.wgjwhj.cn

Java: do { i++; } while (i < 10);
来源：http://br.shtwfgs.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://zm.bookmarksfly.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xw.bookmarksfly.cn

C#:   do { i++; } while (i < 10);
来源：http://cz.gzmigu.cn

[B09] break 与 continue
来源：http://cp.nszjky.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bx.huanxung.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jp.hnjuh.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yg.9csxet.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xw.huixiangedu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wm.huanxung.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sa.shtwfgs.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tb.9csxet.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://au.huixinmuqiang.cn

[B10] 遍历同时拿索引
来源：http://av.asd995.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dc.nicolike.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ht.bookmarksfly.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ob.yuexingan06.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qe.szxytkj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pg.hahajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qo.shtwfgs.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xo.9csxet.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://od.shtwfgs.cn

[B11] 生成数字序列 / 区间
来源：http://uo.9csxet.cn

Py:   list(range(0, 10, 2))
来源：http://fx.huanxung.cn

PHP:  range(0, 10, 2);
来源：http://mq.panjiajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fn.jctech888.com.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sv.bjjhwx.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qn.colortex.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wt.newstarts.cn

Ruby: (0...10).step(2).to_a
来源：http://fe.haigaiapp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rn.hnjuh.cn

[B12] 跳出多层循环
来源：http://zi.szxytkj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://en.shxzskj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ru.shtwfgs.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qu.gzmigu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tf.nicolike.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lt.jctech888.com.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://oz.szxytkj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dr.shtwfgs.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ya.yuntaijiaju.cn

[B13] 判断是否为数字
来源：http://jt.colortex.cn

Py:   isinstance(x, (int, float))
来源：http://rz.9csxet.cn

PHP:  is_numeric($x)
来源：http://ia.nszjky.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fq.panjiajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zp.huixinmuqiang.cn

Java: x instanceof Number
来源：http://wf.haigaiapp.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wk.panjiajie.cn

Ruby: x.is_a?(Numeric)
来源：http://we.colortex.cn

C#:   x is int or double or decimal
来源：http://yp.szxytkj.cn

[B14] 判断值是否在集合内
来源：http://ax.newstarts.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wx.huixiangedu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pc.9csxet.cn

JS:   [1, 2, 3].includes(x)
来源：http://gd.jianghongdianzi.cn

TS:   [1, 2, 3].includes(x)
来源：http://da.panjiajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://yd.jctech888.com.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://aj.hnjuh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ys.bjjhwx.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uu.wgjwhj.cn

[B15] 布尔运算与取反
来源：http://nf.jctech888.com.cn

Py:   a and b or not c
来源：http://mk.hahajie.cn

PHP:  $a && $b || !$c
来源：http://pd.haigaiapp.cn

JS:   a && b || !c
来源：http://yp.shtwfgs.cn

TS:   a && b || !c
来源：http://qf.szxytkj.cn

Java: a && b || !c
来源：http://zm.9csxet.cn

Go:   a && b || !c
来源：http://cg.jctech888.com.cn

Ruby: a && b || !c
来源：http://oa.asd995.cn

C#:   a && b || !c
来源：http://up.jianghongdianzi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://me.newstarts.cn

Py:   if not data: return
来源：http://ow.hahajie.cn

PHP:  if (!$data) { return; }
来源：http://az.wgjwhj.cn

JS:   if (!data) return;
来源：http://dt.yuexingan06.cn

TS:   if (!data) return;
来源：http://ch.shtwfgs.cn

Java: if (data == null) return;
来源：http://ls.huixiangedu.cn

Go:   if data == nil { return }
来源：http://zs.wgjwhj.cn

Ruby: return if data.nil?
来源：http://fw.nszjky.cn

C#:   if (data == null) return;
来源：http://ng.szsharing.cn

================================================================================
来源：http://qg.asd995.cn

C. 函数与作用域
来源：http://wl.gzmigu.cn

================================================================================
来源：http://oa.jctech888.com.cn

[C01] 定义函数
来源：http://vj.nicolike.cn

Py:   def add(a, b): return a + b
来源：http://xx.muxihuayi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ix.szsharing.cn

JS:   function add(a, b) { return a + b; }
来源：http://bq.huixinmuqiang.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bu.szxytkj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://es.nicolike.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qw.nszjky.cn

Ruby: def add(a, b); a + b; end
来源：http://nz.9csxet.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zf.521024.cn

[C02] 默认参数
来源：http://vf.chemitech.net.cn

Py:   def greet(name="World"): return name
来源：http://gj.newstarts.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ee.huixiangedu.cn

JS:   function greet(name = "World") { return name; }
来源：http://je.gzmigu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qi.shtwfgs.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://mf.9csxet.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sf.shxzskj.cn

Ruby: def greet(name = "World") = name
来源：http://co.hnjuh.cn

C#:   string Greet(string name = "World") => name;
来源：http://og.muxihuayi.cn

[C03] 可变参数
来源：http://zg.hnjuh.cn

Py:   def total(*args): return sum(args)
来源：http://wp.bjjhwx.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ad.nicolike.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xg.yuexingan06.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vq.yuexingan06.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rn.9csxet.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rr.muxihuayi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ry.jctech888.com.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://op.shxzskj.cn

[C04] 命名参数 / 关键字参数
来源：http://nj.wgjwhj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uh.shtwfgs.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nr.yuexingan06.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bz.shtwfgs.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xx.newstarts.cn

Java: // 无：用 Builder 模式或 record
来源：http://ec.lnxyls.cn

Go:   // 无：用配置结构体参数
来源：http://sz.bjjhwx.cn

Ruby: f(a: 1, b: 2)
来源：http://iu.9csxet.cn

C#:   f(a: 1, b: 2)
来源：http://xx.gzmigu.cn

[C05] 返回多个值
来源：http://qb.hahajie.cn

Py:   return a, b
来源：http://xl.shxzskj.cn

PHP:  return [$a, $b];
来源：http://dq.nszjky.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qs.huixiangedu.cn

TS:   return { a, b };
来源：http://ug.521024.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ba.panjiajie.cn

Go:   return a, b
来源：http://li.haigaiapp.cn

Ruby: return a, b
来源：http://cx.chemitech.net.cn

C#:   return (a, b);              // ValueTuple
来源：http://us.nszjky.cn

[C06] 匿名函数 / lambda
来源：http://ki.hnjuh.cn

Py:   square = lambda x: x * x
来源：http://pl.huixinmuqiang.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pv.shxzukj.cn

JS:   const square = x => x * x;
来源：http://ry.nszjky.cn

TS:   const square = (x: number): number => x * x;
来源：http://xc.shxzskj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fq.newstarts.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fn.shtwfgs.cn

Ruby: square = ->(x) { x * x }
来源：http://uj.lnxyls.cn

C#:   Func<int, int> square = x => x * x;
来源：http://kb.nicolike.cn

[C07] 把函数作为参数传入
来源：http://sc.yuexingan06.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ux.yuexingan06.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ln.asd995.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rx.shxzukj.cn

TS:   arr.map(String)
来源：http://zl.huanxung.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ol.gzmigu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sn.haigaiapp.cn

Ruby: arr.map(&:upcase)
来源：http://vq.huixiangedu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://uc.chemitech.net.cn

[C08] 闭包
来源：http://hc.nicolike.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rp.bookmarksfly.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xm.asd995.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ve.nszjky.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rn.chemitech.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sv.wgjwhj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mk.lnxyls.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dd.huixiangedu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://oo.jianghongdianzi.cn

[C09] 递归
来源：http://am.nszjky.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dg.szsharing.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rj.lnxyls.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rj.nszjky.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pc.asd995.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yp.hahajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mp.yuntaijiaju.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ww.bookmarksfly.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://aa.521024.cn

[C10] 变量作用域
来源：http://wp.haigaiapp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qm.jianghongdianzi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ud.szxytkj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kr.521024.cn

TS:   同 JS
来源：http://np.jctech888.com.cn

Java: 方法内为块级作用域
来源：http://ta.shxzukj.cn

Go:   花括号块级作用域
来源：http://pq.nicolike.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fw.szsharing.cn

C#:   块级作用域
来源：http://sl.colortex.cn

[C11] 模块导入与导出
来源：http://oc.jctech888.com.cn

Py:   from module import func
来源：http://tm.muxihuayi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://og.panjiajie.cn


<!-- 参考信息 -->