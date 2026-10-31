代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lw.wgjwhj.cn

Ruby: gets.chomp
来源：http://ba.9csxet.cn

C#:   Console.ReadLine();
来源：http://bp.hahajie.cn

[A21] 保留指定小数位输出
来源：http://tv.huixinmuqiang.cn

Py:   f"{3.14159:.2f}"
来源：http://fc.lnxyls.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ba.szxytkj.cn

JS:   (3.14159).toFixed(2)
来源：http://hu.nicolike.cn

TS:   (3.14159).toFixed(2)
来源：http://bl.huanxung.cn

Java: String.format("%.2f", 3.14159)
来源：http://hu.521024.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qn.shtwfgs.cn

Ruby: format("%.2f", 3.14159)
来源：http://lb.lnxyls.cn

C#:   3.14159.ToString("F2")
来源：http://fy.nicolike.cn

[A22] 获取字符串长度
来源：http://ru.9csxet.cn

Py:   len(s)
来源：http://vk.newstarts.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ce.jianghongdianzi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ik.haigaiapp.cn

TS:   s.length
来源：http://mf.colortex.cn

Java: s.length()
来源：http://zj.huixiangedu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hv.hahajie.cn

Ruby: s.length
来源：http://nn.asd995.cn

C#:   s.Length
来源：http://xm.wgjwhj.cn

[A23] 大小写转换
来源：http://ki.newstarts.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://yn.asd995.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yi.shtwfgs.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://au.huixiangedu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hy.bookmarksfly.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cj.panjiajie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mu.nicolike.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://oi.colortex.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://aw.wgjwhj.cn

[A24] 去除首尾空白
来源：http://ex.shxzskj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xz.shxzukj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://eq.hnjuh.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gs.shtwfgs.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lg.bookmarksfly.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://sb.muxihuayi.cn

Go:   strings.TrimSpace(s)
来源：http://sz.wgjwhj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://iv.huixiangedu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yu.szxytkj.cn

[A25] 字符串比较
来源：http://oe.szxytkj.cn

Py:   s1 == s2; s1 != s2
来源：http://hn.bjjhwx.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ex.huixinmuqiang.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lf.colortex.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ru.muxihuayi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://na.huanxung.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ky.shxzskj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rc.bjjhwx.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sj.jctech888.com.cn

[A26] 类型转换总览
来源：http://fy.shtwfgs.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dp.haigaiapp.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ag.asd995.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kc.shxzskj.cn

TS:   Number() String() Boolean() x as number
来源：http://jb.colortex.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ev.yuntaijiaju.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rz.szsharing.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://fm.nicolike.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rl.bookmarksfly.cn

================================================================================
来源：http://dm.lnxyls.cn

B. 流程控制
来源：http://bt.nszjky.cn

================================================================================
来源：http://ec.panjiajie.cn

[B01] 条件判断 if / else
来源：http://rb.shtwfgs.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://sj.jctech888.com.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://et.gzmigu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vu.hnjuh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vf.shtwfgs.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ei.wgjwhj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yf.yuntaijiaju.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jq.lnxyls.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ug.9csxet.cn

[B02] 多分支 else if / elif
来源：http://zv.hahajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://of.szsharing.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sp.shxzukj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fi.shxzskj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pl.521024.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zt.lnxyls.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vn.jianghongdianzi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pb.huixiangedu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cc.yuntaijiaju.cn

[B03] switch / match / case
来源：http://jn.lnxyls.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gv.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://me.shxzskj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sa.szxytkj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ox.hahajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dt.yuexingan06.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jl.huanxung.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bt.yuexingan06.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zp.shxzukj.cn

[B04] for 计数循环
来源：http://no.asd995.cn

Py:   for i in range(10): print(i)
来源：http://at.bookmarksfly.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lo.asd995.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bj.9csxet.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qb.asd995.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cq.szxytkj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://du.newstarts.cn

Ruby: 10.times { |i| puts i }
来源：http://qo.asd995.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ei.muxihuayi.cn

[B05] 遍历数组 / 列表
来源：http://xq.lnxyls.cn

Py:   for item in arr: print(item)
来源：http://sn.hahajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jv.lnxyls.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ut.panjiajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://av.shxzskj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://cq.huixiangedu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wq.huixinmuqiang.cn

Ruby: arr.each { |item| puts item }
来源：http://tv.shxzskj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fv.shxzskj.cn

[B06] 遍历字典 / 对象
来源：http://aj.szxytkj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pn.521024.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dz.nszjky.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xe.szxytkj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://aq.szsharing.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ch.huixiangedu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rp.nicolike.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nx.wgjwhj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://td.bjjhwx.cn

[B07] while 循环
来源：http://wz.gzmigu.cn

Py:   while i < 10: i += 1
来源：http://kg.asd995.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qo.shxzukj.cn

JS:   while (i < 10) { i++; }
来源：http://jq.colortex.cn

TS:   while (i < 10) { i++; }
来源：http://mf.yuexingan06.cn

Java: while (i < 10) { i++; }
来源：http://il.nicolike.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://np.nicolike.cn

Ruby: while i < 10; i += 1; end
来源：http://lw.szxytkj.cn

C#:   while (i < 10) { i++; }
来源：http://ze.muxihuayi.cn

[B08] do-while（至少执行一次）
来源：http://xy.9csxet.cn

Py:   # 无 do-while：用 while True + break
来源：http://ph.521024.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ip.bjjhwx.cn

JS:   do { i++; } while (i < 10);
来源：http://yw.lnxyls.cn

TS:   do { i++; } while (i < 10);
来源：http://ut.haigaiapp.cn

Java: do { i++; } while (i < 10);
来源：http://tg.shxzukj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://rl.wgjwhj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://li.yuntaijiaju.cn

C#:   do { i++; } while (i < 10);
来源：http://vg.newstarts.cn

[B09] break 与 continue
来源：http://ge.huixiangedu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bg.huanxung.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dn.newstarts.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mg.bjjhwx.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://is.bookmarksfly.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://am.panjiajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://im.huixinmuqiang.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dh.gzmigu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sn.huanxung.cn

[B10] 遍历同时拿索引
来源：http://zr.panjiajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gl.yuexingan06.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kc.hahajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ac.yuexingan06.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mu.bjjhwx.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xd.wgjwhj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sd.yuexingan06.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://af.szxytkj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qi.huixiangedu.cn

[B11] 生成数字序列 / 区间
来源：http://gr.yuexingan06.cn

Py:   list(range(0, 10, 2))
来源：http://mo.gzmigu.cn

PHP:  range(0, 10, 2);
来源：http://dt.newstarts.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pn.bjjhwx.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://po.szxytkj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vd.shxzukj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ng.shxzukj.cn

Ruby: (0...10).step(2).to_a
来源：http://nl.9csxet.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wu.hahajie.cn

[B12] 跳出多层循环
来源：http://dc.muxihuayi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://aj.haigaiapp.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ok.huanxung.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://oj.hahajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hr.panjiajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://aa.hahajie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jv.nszjky.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tn.szxytkj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://od.muxihuayi.cn

[B13] 判断是否为数字
来源：http://dy.9csxet.cn

Py:   isinstance(x, (int, float))
来源：http://ai.chemitech.net.cn

PHP:  is_numeric($x)
来源：http://ca.bookmarksfly.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.gzmigu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lv.jianghongdianzi.cn

Java: x instanceof Number
来源：http://bs.yuntaijiaju.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://au.colortex.cn

Ruby: x.is_a?(Numeric)
来源：http://hl.bjjhwx.cn

C#:   x is int or double or decimal
来源：http://eh.yuexingan06.cn

[B14] 判断值是否在集合内
来源：http://ms.haigaiapp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vo.panjiajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mz.jianghongdianzi.cn

JS:   [1, 2, 3].includes(x)
来源：http://ds.yuntaijiaju.cn

TS:   [1, 2, 3].includes(x)
来源：http://ig.panjiajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://nx.haigaiapp.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://no.jctech888.com.cn

Ruby: [1, 2, 3].include?(x)
来源：http://hc.huixinmuqiang.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rt.yuntaijiaju.cn

[B15] 布尔运算与取反
来源：http://gq.bjjhwx.cn

Py:   a and b or not c
来源：http://vx.haigaiapp.cn

PHP:  $a && $b || !$c
来源：http://uf.shtwfgs.cn

JS:   a && b || !c
来源：http://lp.huanxung.cn

TS:   a && b || !c
来源：http://ml.bjjhwx.cn

Java: a && b || !c
来源：http://im.panjiajie.cn

Go:   a && b || !c
来源：http://yj.hnjuh.cn

Ruby: a && b || !c
来源：http://is.hahajie.cn

C#:   a && b || !c
来源：http://uk.chemitech.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fy.huixiangedu.cn

Py:   if not data: return
来源：http://lh.asd995.cn

PHP:  if (!$data) { return; }
来源：http://vj.nicolike.cn

JS:   if (!data) return;
来源：http://dr.szxytkj.cn

TS:   if (!data) return;
来源：http://si.lnxyls.cn

Java: if (data == null) return;
来源：http://pc.wgjwhj.cn

Go:   if data == nil { return }
来源：http://ow.huanxung.cn

Ruby: return if data.nil?
来源：http://du.bookmarksfly.cn

C#:   if (data == null) return;
来源：http://ut.szxytkj.cn

================================================================================
来源：http://gc.gzmigu.cn

C. 函数与作用域
来源：http://nx.lnxyls.cn

================================================================================
来源：http://lm.huixiangedu.cn

[C01] 定义函数
来源：http://zr.panjiajie.cn

Py:   def add(a, b): return a + b
来源：http://eu.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rn.huanxung.cn

JS:   function add(a, b) { return a + b; }
来源：http://rg.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vf.jianghongdianzi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zu.9csxet.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hu.hahajie.cn

Ruby: def add(a, b); a + b; end
来源：http://gd.jianghongdianzi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ny.muxihuayi.cn

[C02] 默认参数
来源：http://ls.chemitech.net.cn

Py:   def greet(name="World"): return name
来源：http://eb.shtwfgs.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vi.muxihuayi.cn

JS:   function greet(name = "World") { return name; }
来源：http://ue.jctech888.com.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fy.jianghongdianzi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://pi.asd995.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://px.shxzukj.cn

Ruby: def greet(name = "World") = name
来源：http://kw.nicolike.cn

C#:   string Greet(string name = "World") => name;
来源：http://au.shtwfgs.cn

[C03] 可变参数
来源：http://cf.muxihuayi.cn

Py:   def total(*args): return sum(args)
来源：http://aa.huanxung.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://iz.chemitech.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rg.yuntaijiaju.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qz.haigaiapp.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://za.szxytkj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ib.haigaiapp.cn

Ruby: def total(*nums); nums.sum; end
来源：http://kd.muxihuayi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xe.yuexingan06.cn

[C04] 命名参数 / 关键字参数
来源：http://up.521024.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qk.bookmarksfly.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hu.wgjwhj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://it.huixinmuqiang.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bg.bookmarksfly.cn

Java: // 无：用 Builder 模式或 record
来源：http://du.huixinmuqiang.cn

Go:   // 无：用配置结构体参数
来源：http://lf.gzmigu.cn

Ruby: f(a: 1, b: 2)
来源：http://rz.521024.cn

C#:   f(a: 1, b: 2)
来源：http://wu.hahajie.cn

[C05] 返回多个值
来源：http://nv.lnxyls.cn

Py:   return a, b
来源：http://wi.bjjhwx.cn

PHP:  return [$a, $b];
来源：http://zm.shxzskj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fl.9csxet.cn

TS:   return { a, b };
来源：http://iz.521024.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ce.huixiangedu.cn

Go:   return a, b
来源：http://dw.colortex.cn

Ruby: return a, b
来源：http://tf.colortex.cn

C#:   return (a, b);              // ValueTuple
来源：http://gu.shtwfgs.cn

[C06] 匿名函数 / lambda
来源：http://se.nszjky.cn

Py:   square = lambda x: x * x
来源：http://sk.shtwfgs.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bt.muxihuayi.cn

JS:   const square = x => x * x;
来源：http://ua.shxzskj.cn

TS:   const square = (x: number): number => x * x;
来源：http://td.panjiajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lh.nicolike.cn

Go:   sq := func(x int) int { return x * x }
来源：http://vt.hahajie.cn

Ruby: square = ->(x) { x * x }
来源：http://jk.hnjuh.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ux.jctech888.com.cn

[C07] 把函数作为参数传入
来源：http://hx.shxzukj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://eb.9csxet.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kg.shtwfgs.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sl.huixinmuqiang.cn

TS:   arr.map(String)
来源：http://xl.huanxung.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lf.colortex.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zv.wgjwhj.cn

Ruby: arr.map(&:upcase)
来源：http://fp.521024.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://tf.gzmigu.cn

[C08] 闭包
来源：http://oa.chemitech.net.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yi.hahajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jy.szxytkj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://us.huixiangedu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qr.lnxyls.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bu.hahajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lv.9csxet.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://za.yuntaijiaju.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ec.newstarts.cn

[C09] 递归
来源：http://yw.szsharing.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nx.hnjuh.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zi.9csxet.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vr.bjjhwx.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sn.gzmigu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vj.szxytkj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zz.nicolike.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vi.lnxyls.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gm.szsharing.cn

[C10] 变量作用域
来源：http://ir.bookmarksfly.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kw.jianghongdianzi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jv.asd995.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fj.yuntaijiaju.cn

TS:   同 JS
来源：http://ox.shxzukj.cn

Java: 方法内为块级作用域
来源：http://gb.huanxung.cn

Go:   花括号块级作用域
来源：http://jh.huanxung.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ir.chemitech.net.cn

C#:   块级作用域
来源：http://vx.colortex.cn

[C11] 模块导入与导出
来源：http://bg.bookmarksfly.cn

Py:   from module import func
来源：http://bl.bjjhwx.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vx.shtwfgs.cn


<!-- 参考信息 -->