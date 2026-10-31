代发 wailian999

Ruby: a, b = b, a
来源：http://ck.521024.cn

C#:   (a, b) = (b, a);
来源：http://th.bjjhwx.cn

[A20] 读取标准输入
来源：http://uv.panjiajie.cn

Py:   name = input("请输入：")
来源：http://ab.nszjky.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://st.yuntaijiaju.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://py.9csxet.cn

TS:   // Node.js：readline 模块
来源：http://er.bookmarksfly.cn

Java: new Scanner(System.in).nextLine()
来源：http://tr.huanxung.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zr.9csxet.cn

Ruby: gets.chomp
来源：http://nk.9csxet.cn

C#:   Console.ReadLine();
来源：http://ig.asd995.cn

[A21] 保留指定小数位输出
来源：http://xm.chemitech.net.cn

Py:   f"{3.14159:.2f}"
来源：http://hc.huixinmuqiang.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xl.huixinmuqiang.cn

JS:   (3.14159).toFixed(2)
来源：http://ww.nicolike.cn

TS:   (3.14159).toFixed(2)
来源：http://zx.szsharing.cn

Java: String.format("%.2f", 3.14159)
来源：http://cy.shxzukj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pm.nicolike.cn

Ruby: format("%.2f", 3.14159)
来源：http://sd.shxzukj.cn

C#:   3.14159.ToString("F2")
来源：http://sr.szxytkj.cn

[A22] 获取字符串长度
来源：http://rx.521024.cn

Py:   len(s)
来源：http://dt.hnjuh.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://uu.521024.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://yv.haigaiapp.cn

TS:   s.length
来源：http://nz.jctech888.com.cn

Java: s.length()
来源：http://wi.yuexingan06.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bm.huanxung.cn

Ruby: s.length
来源：http://ev.bjjhwx.cn

C#:   s.Length
来源：http://sf.shxzukj.cn

[A23] 大小写转换
来源：http://ql.muxihuayi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ou.shxzskj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ir.yuntaijiaju.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://lt.wgjwhj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lz.jianghongdianzi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://br.muxihuayi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cr.shxzskj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ga.gzmigu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://dh.yuexingan06.cn

[A24] 去除首尾空白
来源：http://pt.huixinmuqiang.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sv.szsharing.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gu.huanxung.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tr.gzmigu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gd.bjjhwx.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rm.bjjhwx.cn

Go:   strings.TrimSpace(s)
来源：http://oc.colortex.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ij.huixiangedu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sk.szsharing.cn

[A25] 字符串比较
来源：http://oh.jctech888.com.cn

Py:   s1 == s2; s1 != s2
来源：http://vs.haigaiapp.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vf.shxzskj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wm.panjiajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ou.lnxyls.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://uf.huixinmuqiang.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kw.szsharing.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ah.colortex.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wa.shxzukj.cn

[A26] 类型转换总览
来源：http://gs.gzmigu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tg.lnxyls.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fl.shxzskj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://do.colortex.cn

TS:   Number() String() Boolean() x as number
来源：http://qt.jianghongdianzi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://sf.521024.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nb.shtwfgs.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://bl.bjjhwx.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yi.chemitech.net.cn

================================================================================
来源：http://gp.nicolike.cn

B. 流程控制
来源：http://eq.yuexingan06.cn

================================================================================
来源：http://ps.lnxyls.cn

[B01] 条件判断 if / else
来源：http://cr.muxihuayi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://qi.jctech888.com.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://oo.szxytkj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ts.jianghongdianzi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bg.shtwfgs.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://zg.szsharing.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gf.huanxung.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jl.lnxyls.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://iq.muxihuayi.cn

[B02] 多分支 else if / elif
来源：http://do.newstarts.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kw.szxytkj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://su.yuexingan06.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aa.panjiajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cb.bookmarksfly.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ev.newstarts.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xp.colortex.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://op.9csxet.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yn.huixiangedu.cn

[B03] switch / match / case
来源：http://eq.bookmarksfly.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ap.shxzukj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wm.szsharing.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mx.panjiajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oy.huanxung.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xm.9csxet.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ju.shxzukj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ty.hahajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rt.asd995.cn

[B04] for 计数循环
来源：http://ay.huixinmuqiang.cn

Py:   for i in range(10): print(i)
来源：http://ge.9csxet.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cq.lnxyls.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yd.asd995.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ca.nszjky.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nd.bookmarksfly.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pv.muxihuayi.cn

Ruby: 10.times { |i| puts i }
来源：http://ag.yuntaijiaju.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jo.szsharing.cn

[B05] 遍历数组 / 列表
来源：http://kq.bookmarksfly.cn

Py:   for item in arr: print(item)
来源：http://yl.shxzskj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lg.hahajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ef.9csxet.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://nu.jctech888.com.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://aa.colortex.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pa.colortex.cn

Ruby: arr.each { |item| puts item }
来源：http://qe.hahajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zg.hnjuh.cn

[B06] 遍历字典 / 对象
来源：http://qy.nszjky.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xh.shxzskj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vz.jctech888.com.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ny.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xk.shxzskj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hh.hahajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cw.huanxung.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://at.jctech888.com.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sb.jianghongdianzi.cn

[B07] while 循环
来源：http://gi.9csxet.cn

Py:   while i < 10: i += 1
来源：http://ui.huixiangedu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vs.huixiangedu.cn

JS:   while (i < 10) { i++; }
来源：http://cg.nszjky.cn

TS:   while (i < 10) { i++; }
来源：http://kz.asd995.cn

Java: while (i < 10) { i++; }
来源：http://rx.muxihuayi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zy.bjjhwx.cn

Ruby: while i < 10; i += 1; end
来源：http://hy.panjiajie.cn

C#:   while (i < 10) { i++; }
来源：http://by.szsharing.cn

[B08] do-while（至少执行一次）
来源：http://pp.huixinmuqiang.cn

Py:   # 无 do-while：用 while True + break
来源：http://yt.shtwfgs.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xs.bjjhwx.cn

JS:   do { i++; } while (i < 10);
来源：http://hg.huanxung.cn

TS:   do { i++; } while (i < 10);
来源：http://cn.huixiangedu.cn

Java: do { i++; } while (i < 10);
来源：http://tx.jianghongdianzi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://dd.yuntaijiaju.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jm.shtwfgs.cn

C#:   do { i++; } while (i < 10);
来源：http://qf.asd995.cn

[B09] break 与 continue
来源：http://ab.nicolike.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nl.bjjhwx.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zj.huanxung.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://df.huixiangedu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sd.muxihuayi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vq.bjjhwx.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hw.newstarts.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pe.yuexingan06.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vf.9csxet.cn

[B10] 遍历同时拿索引
来源：http://yq.huanxung.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xx.newstarts.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mc.521024.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ss.szsharing.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ro.colortex.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hk.jianghongdianzi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://im.bookmarksfly.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lh.hahajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wh.shxzskj.cn

[B11] 生成数字序列 / 区间
来源：http://va.colortex.cn

Py:   list(range(0, 10, 2))
来源：http://aa.yuexingan06.cn

PHP:  range(0, 10, 2);
来源：http://np.9csxet.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yf.panjiajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fe.nszjky.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wr.jctech888.com.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pc.asd995.cn

Ruby: (0...10).step(2).to_a
来源：http://bh.jctech888.com.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hv.chemitech.net.cn

[B12] 跳出多层循环
来源：http://jd.szxytkj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://sm.hnjuh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://oi.asd995.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dc.bookmarksfly.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nx.521024.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lc.yuexingan06.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://il.asd995.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gw.nicolike.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fj.muxihuayi.cn

[B13] 判断是否为数字
来源：http://mo.colortex.cn

Py:   isinstance(x, (int, float))
来源：http://iq.shxzukj.cn

PHP:  is_numeric($x)
来源：http://tf.jctech888.com.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ra.521024.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ia.szsharing.cn

Java: x instanceof Number
来源：http://bd.bjjhwx.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wc.haigaiapp.cn

Ruby: x.is_a?(Numeric)
来源：http://cq.muxihuayi.cn

C#:   x is int or double or decimal
来源：http://mh.gzmigu.cn

[B14] 判断值是否在集合内
来源：http://dq.szsharing.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://la.wgjwhj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tk.bookmarksfly.cn

JS:   [1, 2, 3].includes(x)
来源：http://pt.newstarts.cn

TS:   [1, 2, 3].includes(x)
来源：http://nk.nszjky.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://pa.chemitech.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://up.hahajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ky.bjjhwx.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kr.lnxyls.cn

[B15] 布尔运算与取反
来源：http://od.nicolike.cn

Py:   a and b or not c
来源：http://tu.newstarts.cn

PHP:  $a && $b || !$c
来源：http://gw.nszjky.cn

JS:   a && b || !c
来源：http://hl.jctech888.com.cn

TS:   a && b || !c
来源：http://od.nicolike.cn

Java: a && b || !c
来源：http://qd.colortex.cn

Go:   a && b || !c
来源：http://gp.yuntaijiaju.cn

Ruby: a && b || !c
来源：http://tl.shxzskj.cn

C#:   a && b || !c
来源：http://cn.hahajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://pe.szxytkj.cn

Py:   if not data: return
来源：http://bs.gzmigu.cn

PHP:  if (!$data) { return; }
来源：http://cy.shtwfgs.cn

JS:   if (!data) return;
来源：http://uz.muxihuayi.cn

TS:   if (!data) return;
来源：http://pn.shtwfgs.cn

Java: if (data == null) return;
来源：http://il.jianghongdianzi.cn

Go:   if data == nil { return }
来源：http://ah.hahajie.cn

Ruby: return if data.nil?
来源：http://dk.nszjky.cn

C#:   if (data == null) return;
来源：http://pj.colortex.cn

================================================================================
来源：http://he.shxzskj.cn

C. 函数与作用域
来源：http://rb.jianghongdianzi.cn

================================================================================
来源：http://ik.huixiangedu.cn

[C01] 定义函数
来源：http://yo.nicolike.cn

Py:   def add(a, b): return a + b
来源：http://cf.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rn.wgjwhj.cn

JS:   function add(a, b) { return a + b; }
来源：http://hq.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://eo.lnxyls.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wl.9csxet.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ue.nicolike.cn

Ruby: def add(a, b); a + b; end
来源：http://ml.asd995.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pu.huixiangedu.cn

[C02] 默认参数
来源：http://uu.newstarts.cn

Py:   def greet(name="World"): return name
来源：http://vy.9csxet.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://le.haigaiapp.cn

JS:   function greet(name = "World") { return name; }
来源：http://ot.yuntaijiaju.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://mt.bjjhwx.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://tc.yuexingan06.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ko.szsharing.cn

Ruby: def greet(name = "World") = name
来源：http://eq.shxzukj.cn

C#:   string Greet(string name = "World") => name;
来源：http://ib.9csxet.cn

[C03] 可变参数
来源：http://lp.panjiajie.cn

Py:   def total(*args): return sum(args)
来源：http://cj.huanxung.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sm.jctech888.com.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ov.lnxyls.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tq.szsharing.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cw.newstarts.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sg.bjjhwx.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tw.gzmigu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://uy.chemitech.net.cn

[C04] 命名参数 / 关键字参数
来源：http://yw.shxzukj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ey.hnjuh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://si.bookmarksfly.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://od.szxytkj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gw.lnxyls.cn

Java: // 无：用 Builder 模式或 record
来源：http://kv.huanxung.cn

Go:   // 无：用配置结构体参数
来源：http://dl.szsharing.cn

Ruby: f(a: 1, b: 2)
来源：http://if.huixiangedu.cn

C#:   f(a: 1, b: 2)
来源：http://ho.shtwfgs.cn

[C05] 返回多个值
来源：http://la.bookmarksfly.cn

Py:   return a, b
来源：http://wz.wgjwhj.cn

PHP:  return [$a, $b];
来源：http://gd.jctech888.com.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vj.shxzukj.cn

TS:   return { a, b };
来源：http://va.colortex.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tp.bookmarksfly.cn

Go:   return a, b
来源：http://ce.huixinmuqiang.cn

Ruby: return a, b
来源：http://ty.shtwfgs.cn

C#:   return (a, b);              // ValueTuple
来源：http://ou.bookmarksfly.cn

[C06] 匿名函数 / lambda
来源：http://ih.colortex.cn

Py:   square = lambda x: x * x
来源：http://pj.asd995.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xo.haigaiapp.cn

JS:   const square = x => x * x;
来源：http://bu.9csxet.cn

TS:   const square = (x: number): number => x * x;
来源：http://xq.huixinmuqiang.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pv.hahajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://sf.yuntaijiaju.cn

Ruby: square = ->(x) { x * x }
来源：http://yn.yuexingan06.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wl.nszjky.cn

[C07] 把函数作为参数传入
来源：http://ik.haigaiapp.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qt.yuexingan06.cn

PHP:  array_map("strtoupper", $arr);
来源：http://sw.bookmarksfly.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cw.gzmigu.cn

TS:   arr.map(String)
来源：http://tv.muxihuayi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tq.521024.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rn.shtwfgs.cn

Ruby: arr.map(&:upcase)
来源：http://cj.521024.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://iu.huixiangedu.cn

[C08] 闭包
来源：http://vm.yuntaijiaju.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kp.bjjhwx.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uz.colortex.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ai.hnjuh.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sz.huanxung.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pe.szxytkj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pg.hahajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hi.shxzukj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ig.panjiajie.cn

[C09] 递归
来源：http://aw.hnjuh.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yk.szxytkj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jv.wgjwhj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rr.yuexingan06.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jj.wgjwhj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dx.bjjhwx.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://by.shxzukj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uq.huanxung.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lm.hahajie.cn

[C10] 变量作用域
来源：http://yy.gzmigu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qs.huanxung.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zf.huixinmuqiang.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://iy.yuexingan06.cn


<!-- 参考信息 -->