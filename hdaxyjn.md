代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://gq.shxzskj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cv.521024.cn

TS:   // Node.js：readline 模块
来源：http://de.muxihuayi.cn

Java: new Scanner(System.in).nextLine()
来源：http://iy.9csxet.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vz.nszjky.cn

Ruby: gets.chomp
来源：http://nx.yuexingan06.cn

C#:   Console.ReadLine();
来源：http://ga.szxytkj.cn

[A21] 保留指定小数位输出
来源：http://ns.huanxung.cn

Py:   f"{3.14159:.2f}"
来源：http://nx.muxihuayi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wo.shxzukj.cn

JS:   (3.14159).toFixed(2)
来源：http://ht.hnjuh.cn

TS:   (3.14159).toFixed(2)
来源：http://vp.chemitech.net.cn

Java: String.format("%.2f", 3.14159)
来源：http://aq.lnxyls.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://is.nicolike.cn

Ruby: format("%.2f", 3.14159)
来源：http://xi.bookmarksfly.cn

C#:   3.14159.ToString("F2")
来源：http://eg.shtwfgs.cn

[A22] 获取字符串长度
来源：http://cp.huixinmuqiang.cn

Py:   len(s)
来源：http://yv.szsharing.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ar.huixinmuqiang.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://py.bookmarksfly.cn

TS:   s.length
来源：http://ou.yuexingan06.cn

Java: s.length()
来源：http://sa.hahajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://uu.muxihuayi.cn

Ruby: s.length
来源：http://vf.szsharing.cn

C#:   s.Length
来源：http://wq.yuntaijiaju.cn

[A23] 大小写转换
来源：http://ms.wgjwhj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://sl.521024.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yu.shxzskj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pk.huixiangedu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ac.newstarts.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dw.521024.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jg.bookmarksfly.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pu.muxihuayi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qm.chemitech.net.cn

[A24] 去除首尾空白
来源：http://sd.huixiangedu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zn.yuexingan06.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://od.muxihuayi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oy.hahajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://la.haigaiapp.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://my.bjjhwx.cn

Go:   strings.TrimSpace(s)
来源：http://tl.szsharing.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wa.newstarts.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gp.jianghongdianzi.cn

[A25] 字符串比较
来源：http://yq.huixinmuqiang.cn

Py:   s1 == s2; s1 != s2
来源：http://fy.szsharing.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://lw.huanxung.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bb.jctech888.com.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gk.bookmarksfly.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ft.bjjhwx.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ax.huixiangedu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://gt.yuexingan06.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yq.muxihuayi.cn

[A26] 类型转换总览
来源：http://ri.szxytkj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sd.lnxyls.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://du.szsharing.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://os.panjiajie.cn

TS:   Number() String() Boolean() x as number
来源：http://gt.muxihuayi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lv.huixinmuqiang.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cv.shtwfgs.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://aj.huixiangedu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://et.chemitech.net.cn

================================================================================
来源：http://zj.wgjwhj.cn

B. 流程控制
来源：http://wj.panjiajie.cn

================================================================================
来源：http://nr.shxzukj.cn

[B01] 条件判断 if / else
来源：http://at.shxzskj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://oc.yuntaijiaju.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://id.panjiajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qf.szxytkj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://uv.shxzukj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://iy.asd995.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mq.521024.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qv.shtwfgs.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kd.hahajie.cn

[B02] 多分支 else if / elif
来源：http://fn.nszjky.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bs.gzmigu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zp.521024.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dg.hahajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bb.lnxyls.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ix.huixiangedu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qz.huixiangedu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dc.yuexingan06.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sl.hahajie.cn

[B03] switch / match / case
来源：http://ml.hnjuh.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lh.9csxet.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://da.szsharing.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nq.hahajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://my.nszjky.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tf.huixinmuqiang.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ka.colortex.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://st.panjiajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dq.shxzukj.cn

[B04] for 计数循环
来源：http://dd.huixiangedu.cn

Py:   for i in range(10): print(i)
来源：http://nx.yuexingan06.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zc.hahajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tx.bjjhwx.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://je.shxzukj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ph.newstarts.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kp.hahajie.cn

Ruby: 10.times { |i| puts i }
来源：http://hz.wgjwhj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fr.szsharing.cn

[B05] 遍历数组 / 列表
来源：http://zv.hnjuh.cn

Py:   for item in arr: print(item)
来源：http://rr.colortex.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cd.huanxung.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://pp.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ro.colortex.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hf.yuntaijiaju.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xr.lnxyls.cn

Ruby: arr.each { |item| puts item }
来源：http://gi.shxzukj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pp.yuntaijiaju.cn

[B06] 遍历字典 / 对象
来源：http://bz.shxzukj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ac.huixiangedu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fq.hnjuh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ta.bookmarksfly.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mn.bjjhwx.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://em.huanxung.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pu.szxytkj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xz.nicolike.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jb.nicolike.cn

[B07] while 循环
来源：http://qk.haigaiapp.cn

Py:   while i < 10: i += 1
来源：http://xy.9csxet.cn

PHP:  while ($i < 10) { $i++; }
来源：http://pu.shxzukj.cn

JS:   while (i < 10) { i++; }
来源：http://ym.bjjhwx.cn

TS:   while (i < 10) { i++; }
来源：http://hk.nszjky.cn

Java: while (i < 10) { i++; }
来源：http://rm.nicolike.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ta.huixiangedu.cn

Ruby: while i < 10; i += 1; end
来源：http://fn.haigaiapp.cn

C#:   while (i < 10) { i++; }
来源：http://gh.shxzukj.cn

[B08] do-while（至少执行一次）
来源：http://lf.colortex.cn

Py:   # 无 do-while：用 while True + break
来源：http://li.huixinmuqiang.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://tz.hahajie.cn

JS:   do { i++; } while (i < 10);
来源：http://jt.yuexingan06.cn

TS:   do { i++; } while (i < 10);
来源：http://tn.521024.cn

Java: do { i++; } while (i < 10);
来源：http://ph.nszjky.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://af.haigaiapp.cn

Ruby: begin; i += 1; end while i < 10
来源：http://iw.9csxet.cn

C#:   do { i++; } while (i < 10);
来源：http://zb.haigaiapp.cn

[B09] break 与 continue
来源：http://dq.huixinmuqiang.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kg.huixiangedu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gf.haigaiapp.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aq.hahajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pr.bookmarksfly.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zn.shtwfgs.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zr.hahajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vz.bjjhwx.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tf.chemitech.net.cn

[B10] 遍历同时拿索引
来源：http://nw.newstarts.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://uk.muxihuayi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zv.hnjuh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fb.gzmigu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nv.szsharing.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ls.colortex.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dr.lnxyls.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yi.jianghongdianzi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gx.asd995.cn

[B11] 生成数字序列 / 区间
来源：http://iv.panjiajie.cn

Py:   list(range(0, 10, 2))
来源：http://zi.shxzukj.cn

PHP:  range(0, 10, 2);
来源：http://zm.bookmarksfly.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gq.521024.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://er.haigaiapp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tk.shtwfgs.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ep.lnxyls.cn

Ruby: (0...10).step(2).to_a
来源：http://hx.gzmigu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hl.asd995.cn

[B12] 跳出多层循环
来源：http://jj.nszjky.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://uc.wgjwhj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://if.panjiajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zv.huanxung.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kj.huixiangedu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vf.szxytkj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://en.colortex.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nq.gzmigu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dh.9csxet.cn

[B13] 判断是否为数字
来源：http://ms.nszjky.cn

Py:   isinstance(x, (int, float))
来源：http://gg.newstarts.cn

PHP:  is_numeric($x)
来源：http://fm.gzmigu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cl.szxytkj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ac.lnxyls.cn

Java: x instanceof Number
来源：http://rk.lnxyls.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ok.9csxet.cn

Ruby: x.is_a?(Numeric)
来源：http://tf.panjiajie.cn

C#:   x is int or double or decimal
来源：http://yt.panjiajie.cn

[B14] 判断值是否在集合内
来源：http://vd.shxzukj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vh.panjiajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fq.huixiangedu.cn

JS:   [1, 2, 3].includes(x)
来源：http://yl.shxzskj.cn

TS:   [1, 2, 3].includes(x)
来源：http://qu.chemitech.net.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://zu.muxihuayi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rw.chemitech.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zx.haigaiapp.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sp.huanxung.cn

[B15] 布尔运算与取反
来源：http://ep.haigaiapp.cn

Py:   a and b or not c
来源：http://yz.lnxyls.cn

PHP:  $a && $b || !$c
来源：http://hy.huanxung.cn

JS:   a && b || !c
来源：http://cl.bjjhwx.cn

TS:   a && b || !c
来源：http://sd.yuntaijiaju.cn

Java: a && b || !c
来源：http://xy.szxytkj.cn

Go:   a && b || !c
来源：http://kg.huixiangedu.cn

Ruby: a && b || !c
来源：http://ji.chemitech.net.cn

C#:   a && b || !c
来源：http://ll.jianghongdianzi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vx.hnjuh.cn

Py:   if not data: return
来源：http://fc.jianghongdianzi.cn

PHP:  if (!$data) { return; }
来源：http://sw.shxzskj.cn

JS:   if (!data) return;
来源：http://vu.bookmarksfly.cn

TS:   if (!data) return;
来源：http://ek.gzmigu.cn

Java: if (data == null) return;
来源：http://vn.huixiangedu.cn

Go:   if data == nil { return }
来源：http://oe.muxihuayi.cn

Ruby: return if data.nil?
来源：http://km.colortex.cn

C#:   if (data == null) return;
来源：http://je.huixiangedu.cn

================================================================================
来源：http://rn.yuntaijiaju.cn

C. 函数与作用域
来源：http://cb.gzmigu.cn

================================================================================
来源：http://ch.szxytkj.cn

[C01] 定义函数
来源：http://cg.bookmarksfly.cn

Py:   def add(a, b): return a + b
来源：http://ad.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eg.521024.cn

JS:   function add(a, b) { return a + b; }
来源：http://sn.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fh.szxytkj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://sd.panjiajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zs.huixinmuqiang.cn

Ruby: def add(a, b); a + b; end
来源：http://ef.yuntaijiaju.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ir.asd995.cn

[C02] 默认参数
来源：http://dh.haigaiapp.cn

Py:   def greet(name="World"): return name
来源：http://oa.bjjhwx.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://am.shxzukj.cn

JS:   function greet(name = "World") { return name; }
来源：http://nf.asd995.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yt.panjiajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cf.gzmigu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zl.chemitech.net.cn

Ruby: def greet(name = "World") = name
来源：http://uc.9csxet.cn

C#:   string Greet(string name = "World") => name;
来源：http://in.newstarts.cn

[C03] 可变参数
来源：http://lz.szsharing.cn

Py:   def total(*args): return sum(args)
来源：http://wb.jianghongdianzi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wm.yuntaijiaju.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ol.shtwfgs.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jn.yuexingan06.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vb.szsharing.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wr.gzmigu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vv.lnxyls.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://uw.yuexingan06.cn

[C04] 命名参数 / 关键字参数
来源：http://vz.bjjhwx.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yt.nszjky.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://da.nicolike.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rb.asd995.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pi.521024.cn

Java: // 无：用 Builder 模式或 record
来源：http://qo.yuntaijiaju.cn

Go:   // 无：用配置结构体参数
来源：http://ag.hahajie.cn

Ruby: f(a: 1, b: 2)
来源：http://sf.wgjwhj.cn

C#:   f(a: 1, b: 2)
来源：http://bv.panjiajie.cn

[C05] 返回多个值
来源：http://be.asd995.cn

Py:   return a, b
来源：http://av.panjiajie.cn

PHP:  return [$a, $b];
来源：http://nc.yuexingan06.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yu.9csxet.cn

TS:   return { a, b };
来源：http://sv.szxytkj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kw.hnjuh.cn

Go:   return a, b
来源：http://ww.hahajie.cn

Ruby: return a, b
来源：http://sc.szsharing.cn

C#:   return (a, b);              // ValueTuple
来源：http://dy.huixinmuqiang.cn

[C06] 匿名函数 / lambda
来源：http://th.huixinmuqiang.cn

Py:   square = lambda x: x * x
来源：http://ad.jctech888.com.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ro.shxzskj.cn

JS:   const square = x => x * x;
来源：http://hq.shtwfgs.cn

TS:   const square = (x: number): number => x * x;
来源：http://we.nicolike.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ot.hahajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://vo.newstarts.cn

Ruby: square = ->(x) { x * x }
来源：http://lc.521024.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hy.wgjwhj.cn

[C07] 把函数作为参数传入
来源：http://ne.hahajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jm.panjiajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ta.gzmigu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vd.szsharing.cn

TS:   arr.map(String)
来源：http://nd.yuexingan06.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ob.hahajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ao.hnjuh.cn

Ruby: arr.map(&:upcase)
来源：http://vv.jctech888.com.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ab.jctech888.com.cn

[C08] 闭包
来源：http://hu.chemitech.net.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://za.hahajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xa.bookmarksfly.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vb.hnjuh.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fk.nszjky.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jc.chemitech.net.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://si.lnxyls.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ee.hahajie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wt.lnxyls.cn

[C09] 递归
来源：http://do.bjjhwx.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cl.huanxung.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yj.jctech888.com.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xq.hahajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cr.panjiajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rj.hahajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ia.huanxung.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pv.jctech888.com.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pk.wgjwhj.cn

[C10] 变量作用域
来源：http://cg.shxzskj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gs.bookmarksfly.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://iv.asd995.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bu.chemitech.net.cn

TS:   同 JS
来源：http://pm.nicolike.cn

Java: 方法内为块级作用域
来源：http://fx.shtwfgs.cn

Go:   花括号块级作用域
来源：http://ld.wgjwhj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xy.panjiajie.cn


<!-- 参考信息 -->