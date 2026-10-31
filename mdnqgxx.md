代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://cp.yuexingan06.cn

Ruby: gets.chomp
来源：http://xf.yuexingan06.cn

C#:   Console.ReadLine();
来源：http://ub.shtwfgs.cn

[A21] 保留指定小数位输出
来源：http://gv.yuntaijiaju.cn

Py:   f"{3.14159:.2f}"
来源：http://dv.huixinmuqiang.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rt.wgjwhj.cn

JS:   (3.14159).toFixed(2)
来源：http://ps.szsharing.cn

TS:   (3.14159).toFixed(2)
来源：http://tw.jctech888.com.cn

Java: String.format("%.2f", 3.14159)
来源：http://qf.huixiangedu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://bm.szxytkj.cn

Ruby: format("%.2f", 3.14159)
来源：http://vq.asd995.cn

C#:   3.14159.ToString("F2")
来源：http://jh.shxzukj.cn

[A22] 获取字符串长度
来源：http://ut.nicolike.cn

Py:   len(s)
来源：http://dx.chemitech.net.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hf.huixiangedu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rk.colortex.cn

TS:   s.length
来源：http://tm.lnxyls.cn

Java: s.length()
来源：http://lm.521024.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://eh.yuexingan06.cn

Ruby: s.length
来源：http://db.bookmarksfly.cn

C#:   s.Length
来源：http://no.shtwfgs.cn

[A23] 大小写转换
来源：http://iz.newstarts.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://qi.bjjhwx.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://th.shxzskj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tx.szsharing.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nf.lnxyls.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cn.newstarts.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tr.jctech888.com.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vi.9csxet.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://vs.colortex.cn

[A24] 去除首尾空白
来源：http://lu.muxihuayi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jb.szxytkj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tq.9csxet.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jn.jctech888.com.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kr.yuexingan06.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ev.huixinmuqiang.cn

Go:   strings.TrimSpace(s)
来源：http://mo.newstarts.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://sb.szsharing.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://eu.jianghongdianzi.cn

[A25] 字符串比较
来源：http://ot.haigaiapp.cn

Py:   s1 == s2; s1 != s2
来源：http://bl.shxzukj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ka.newstarts.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ry.huixiangedu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yq.szxytkj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pn.nicolike.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gs.chemitech.net.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://mj.haigaiapp.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://op.shxzukj.cn

[A26] 类型转换总览
来源：http://cz.szxytkj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ug.hahajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hh.lnxyls.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://oq.bjjhwx.cn

TS:   Number() String() Boolean() x as number
来源：http://sm.hahajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://da.lnxyls.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xl.bookmarksfly.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rk.jianghongdianzi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://du.521024.cn

================================================================================
来源：http://vs.huixinmuqiang.cn

B. 流程控制
来源：http://mh.nszjky.cn

================================================================================
来源：http://hz.panjiajie.cn

[B01] 条件判断 if / else
来源：http://dj.shtwfgs.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://qc.shxzukj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wq.lnxyls.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tg.jctech888.com.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://db.bjjhwx.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bv.bjjhwx.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dq.shxzskj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qo.muxihuayi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nj.panjiajie.cn

[B02] 多分支 else if / elif
来源：http://yy.gzmigu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jf.shxzskj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://eq.huixinmuqiang.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ng.szxytkj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ya.nszjky.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hi.muxihuayi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://iq.hnjuh.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ry.huanxung.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://au.bjjhwx.cn

[B03] switch / match / case
来源：http://ob.nicolike.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mp.hahajie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lz.nicolike.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rg.nicolike.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://af.colortex.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lr.nicolike.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kg.lnxyls.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ac.bjjhwx.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qg.chemitech.net.cn

[B04] for 计数循环
来源：http://po.muxihuayi.cn

Py:   for i in range(10): print(i)
来源：http://zp.hnjuh.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pq.lnxyls.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kg.shxzukj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://od.wgjwhj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yt.wgjwhj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lg.9csxet.cn

Ruby: 10.times { |i| puts i }
来源：http://lc.jctech888.com.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cc.shxzukj.cn

[B05] 遍历数组 / 列表
来源：http://jk.hnjuh.cn

Py:   for item in arr: print(item)
来源：http://gr.huixinmuqiang.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rh.colortex.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://xp.bookmarksfly.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ke.shtwfgs.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zq.chemitech.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://an.shxzskj.cn

Ruby: arr.each { |item| puts item }
来源：http://oo.bookmarksfly.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vi.szxytkj.cn

[B06] 遍历字典 / 对象
来源：http://qu.yuexingan06.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sr.shxzskj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cr.yuntaijiaju.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uc.huixinmuqiang.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://or.wgjwhj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yn.huixiangedu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bg.gzmigu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yt.shxzukj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xu.colortex.cn

[B07] while 循环
来源：http://wr.wgjwhj.cn

Py:   while i < 10: i += 1
来源：http://bp.yuexingan06.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bc.wgjwhj.cn

JS:   while (i < 10) { i++; }
来源：http://pl.chemitech.net.cn

TS:   while (i < 10) { i++; }
来源：http://yk.huanxung.cn

Java: while (i < 10) { i++; }
来源：http://ek.hnjuh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fm.bookmarksfly.cn

Ruby: while i < 10; i += 1; end
来源：http://qa.521024.cn

C#:   while (i < 10) { i++; }
来源：http://jn.haigaiapp.cn

[B08] do-while（至少执行一次）
来源：http://sj.shxzukj.cn

Py:   # 无 do-while：用 while True + break
来源：http://gg.szsharing.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mq.colortex.cn

JS:   do { i++; } while (i < 10);
来源：http://wu.huixinmuqiang.cn

TS:   do { i++; } while (i < 10);
来源：http://ms.bookmarksfly.cn

Java: do { i++; } while (i < 10);
来源：http://ub.nszjky.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://pj.hahajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jy.521024.cn

C#:   do { i++; } while (i < 10);
来源：http://qp.shtwfgs.cn

[B09] break 与 continue
来源：http://nx.nszjky.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vd.huanxung.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ob.bjjhwx.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sy.bjjhwx.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kz.jctech888.com.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uw.jctech888.com.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cn.chemitech.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ss.jctech888.com.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ys.huanxung.cn

[B10] 遍历同时拿索引
来源：http://gc.lnxyls.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kr.gzmigu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cm.jianghongdianzi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cj.gzmigu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://be.shxzskj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kq.panjiajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://we.asd995.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pr.9csxet.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vd.newstarts.cn

[B11] 生成数字序列 / 区间
来源：http://ls.wgjwhj.cn

Py:   list(range(0, 10, 2))
来源：http://jj.huixinmuqiang.cn

PHP:  range(0, 10, 2);
来源：http://ih.asd995.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cf.newstarts.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qc.jctech888.com.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rc.newstarts.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pd.jctech888.com.cn

Ruby: (0...10).step(2).to_a
来源：http://gr.lnxyls.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wk.yuexingan06.cn

[B12] 跳出多层循环
来源：http://rq.asd995.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://cc.szxytkj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://sf.haigaiapp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ch.nicolike.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hr.yuexingan06.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://al.shxzukj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fi.chemitech.net.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tf.newstarts.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ta.szsharing.cn

[B13] 判断是否为数字
来源：http://iw.colortex.cn

Py:   isinstance(x, (int, float))
来源：http://gh.hnjuh.cn

PHP:  is_numeric($x)
来源：http://sk.shxzukj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sm.gzmigu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://je.hahajie.cn

Java: x instanceof Number
来源：http://yu.yuexingan06.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kg.gzmigu.cn

Ruby: x.is_a?(Numeric)
来源：http://jj.chemitech.net.cn

C#:   x is int or double or decimal
来源：http://dq.muxihuayi.cn

[B14] 判断值是否在集合内
来源：http://td.lnxyls.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ey.wgjwhj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xc.panjiajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://cc.yuexingan06.cn

TS:   [1, 2, 3].includes(x)
来源：http://bm.asd995.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xk.huixinmuqiang.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nd.jctech888.com.cn

Ruby: [1, 2, 3].include?(x)
来源：http://wv.nicolike.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vs.szxytkj.cn

[B15] 布尔运算与取反
来源：http://il.lnxyls.cn

Py:   a and b or not c
来源：http://tt.lnxyls.cn

PHP:  $a && $b || !$c
来源：http://zt.huixiangedu.cn

JS:   a && b || !c
来源：http://pk.panjiajie.cn

TS:   a && b || !c
来源：http://ey.asd995.cn

Java: a && b || !c
来源：http://zl.yuntaijiaju.cn

Go:   a && b || !c
来源：http://gw.huanxung.cn

Ruby: a && b || !c
来源：http://np.haigaiapp.cn

C#:   a && b || !c
来源：http://km.jianghongdianzi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://og.newstarts.cn

Py:   if not data: return
来源：http://ou.huixiangedu.cn

PHP:  if (!$data) { return; }
来源：http://xj.bookmarksfly.cn

JS:   if (!data) return;
来源：http://ft.yuexingan06.cn

TS:   if (!data) return;
来源：http://aj.gzmigu.cn

Java: if (data == null) return;
来源：http://uj.521024.cn

Go:   if data == nil { return }
来源：http://tm.nszjky.cn

Ruby: return if data.nil?
来源：http://pp.nszjky.cn

C#:   if (data == null) return;
来源：http://ez.muxihuayi.cn

================================================================================
来源：http://do.jianghongdianzi.cn

C. 函数与作用域
来源：http://kt.nszjky.cn

================================================================================
来源：http://rq.chemitech.net.cn

[C01] 定义函数
来源：http://uh.colortex.cn

Py:   def add(a, b): return a + b
来源：http://kg.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cz.9csxet.cn

JS:   function add(a, b) { return a + b; }
来源：http://im.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pm.colortex.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://pu.jianghongdianzi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://fo.huixiangedu.cn

Ruby: def add(a, b); a + b; end
来源：http://tn.lnxyls.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tb.muxihuayi.cn

[C02] 默认参数
来源：http://dj.huanxung.cn

Py:   def greet(name="World"): return name
来源：http://ye.colortex.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://mg.muxihuayi.cn

JS:   function greet(name = "World") { return name; }
来源：http://jh.wgjwhj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lq.jianghongdianzi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jt.asd995.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rt.shtwfgs.cn

Ruby: def greet(name = "World") = name
来源：http://ro.wgjwhj.cn

C#:   string Greet(string name = "World") => name;
来源：http://pl.huanxung.cn

[C03] 可变参数
来源：http://lb.shtwfgs.cn

Py:   def total(*args): return sum(args)
来源：http://lv.shxzukj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ch.hnjuh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ua.wgjwhj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xk.yuntaijiaju.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jw.szsharing.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fz.huixinmuqiang.cn

Ruby: def total(*nums); nums.sum; end
来源：http://bq.panjiajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://am.huixinmuqiang.cn

[C04] 命名参数 / 关键字参数
来源：http://ey.szsharing.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pr.hahajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ak.shtwfgs.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ge.shxzskj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zv.colortex.cn

Java: // 无：用 Builder 模式或 record
来源：http://lv.jctech888.com.cn

Go:   // 无：用配置结构体参数
来源：http://jf.muxihuayi.cn

Ruby: f(a: 1, b: 2)
来源：http://rj.521024.cn

C#:   f(a: 1, b: 2)
来源：http://wh.lnxyls.cn

[C05] 返回多个值
来源：http://si.huixinmuqiang.cn

Py:   return a, b
来源：http://ob.szsharing.cn

PHP:  return [$a, $b];
来源：http://dz.shtwfgs.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ls.nicolike.cn

TS:   return { a, b };
来源：http://dt.haigaiapp.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xh.bjjhwx.cn

Go:   return a, b
来源：http://ko.jianghongdianzi.cn

Ruby: return a, b
来源：http://te.szsharing.cn

C#:   return (a, b);              // ValueTuple
来源：http://nk.shtwfgs.cn

[C06] 匿名函数 / lambda
来源：http://ey.nicolike.cn

Py:   square = lambda x: x * x
来源：http://ar.jianghongdianzi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://va.bookmarksfly.cn

JS:   const square = x => x * x;
来源：http://zs.hnjuh.cn

TS:   const square = (x: number): number => x * x;
来源：http://fu.gzmigu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ke.wgjwhj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qy.hnjuh.cn

Ruby: square = ->(x) { x * x }
来源：http://jv.newstarts.cn

C#:   Func<int, int> square = x => x * x;
来源：http://mi.yuexingan06.cn

[C07] 把函数作为参数传入
来源：http://cr.nicolike.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qt.jctech888.com.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kn.yuntaijiaju.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ul.bjjhwx.cn

TS:   arr.map(String)
来源：http://kz.521024.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://to.nszjky.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gc.wgjwhj.cn

Ruby: arr.map(&:upcase)
来源：http://yz.panjiajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://lz.lnxyls.cn

[C08] 闭包
来源：http://au.bjjhwx.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ud.yuexingan06.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yz.szsharing.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fi.panjiajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jn.shxzukj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xf.9csxet.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ks.muxihuayi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://km.jianghongdianzi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gg.nicolike.cn

[C09] 递归
来源：http://qe.9csxet.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rp.muxihuayi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://se.9csxet.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fy.yuntaijiaju.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bw.haigaiapp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://eu.gzmigu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ub.chemitech.net.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://va.gzmigu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://my.huixiangedu.cn

[C10] 变量作用域
来源：http://bb.huanxung.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fp.521024.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://an.colortex.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://oz.colortex.cn

TS:   同 JS
来源：http://if.521024.cn

Java: 方法内为块级作用域
来源：http://yq.lnxyls.cn

Go:   花括号块级作用域
来源：http://an.huixinmuqiang.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ua.huixiangedu.cn

C#:   块级作用域
来源：http://of.lnxyls.cn

[C11] 模块导入与导出
来源：http://xl.jctech888.com.cn

Py:   from module import func
来源：http://ye.muxihuayi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tm.chemitech.net.cn


<!-- 参考信息 -->