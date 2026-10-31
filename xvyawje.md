代发 wailian999

C#:   (int)'A'; (char)65
来源：http://fe.gzmigu.cn

[A19] 交换两个变量
来源：http://vr.szsharing.cn

Py:   a, b = b, a
来源：http://pb.muxihuayi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://yk.colortex.cn

JS:   [a, b] = [b, a];
来源：http://dz.huixinmuqiang.cn

TS:   [a, b] = [b, a];
来源：http://gm.nszjky.cn

Java: int t = a; a = b; b = t;
来源：http://vf.szxytkj.cn

Go:   a, b = b, a
来源：http://ew.shxzukj.cn

Ruby: a, b = b, a
来源：http://ic.huanxung.cn

C#:   (a, b) = (b, a);
来源：http://im.nicolike.cn

[A20] 读取标准输入
来源：http://lu.nicolike.cn

Py:   name = input("请输入：")
来源：http://wk.huixinmuqiang.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://qx.huanxung.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gd.521024.cn

TS:   // Node.js：readline 模块
来源：http://ct.shtwfgs.cn

Java: new Scanner(System.in).nextLine()
来源：http://rn.yuexingan06.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://se.yuntaijiaju.cn

Ruby: gets.chomp
来源：http://ca.bjjhwx.cn

C#:   Console.ReadLine();
来源：http://yp.shtwfgs.cn

[A21] 保留指定小数位输出
来源：http://lz.bjjhwx.cn

Py:   f"{3.14159:.2f}"
来源：http://fb.shxzskj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hw.szxytkj.cn

JS:   (3.14159).toFixed(2)
来源：http://mc.nszjky.cn

TS:   (3.14159).toFixed(2)
来源：http://tf.newstarts.cn

Java: String.format("%.2f", 3.14159)
来源：http://dv.bookmarksfly.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sj.hnjuh.cn

Ruby: format("%.2f", 3.14159)
来源：http://fr.huixinmuqiang.cn

C#:   3.14159.ToString("F2")
来源：http://th.haigaiapp.cn

[A22] 获取字符串长度
来源：http://zh.nicolike.cn

Py:   len(s)
来源：http://lz.bookmarksfly.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://oy.jianghongdianzi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ig.szsharing.cn

TS:   s.length
来源：http://mm.huixiangedu.cn

Java: s.length()
来源：http://xq.shxzskj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vf.jctech888.com.cn

Ruby: s.length
来源：http://we.huixinmuqiang.cn

C#:   s.Length
来源：http://jv.hahajie.cn

[A23] 大小写转换
来源：http://vn.lnxyls.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://qw.nszjky.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://nm.newstarts.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hy.shxzskj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jx.newstarts.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://uj.muxihuayi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pl.nicolike.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rz.shtwfgs.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://hx.shtwfgs.cn

[A24] 去除首尾空白
来源：http://eh.hnjuh.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xo.bookmarksfly.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://aq.haigaiapp.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tc.huanxung.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sr.hnjuh.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jp.jctech888.com.cn

Go:   strings.TrimSpace(s)
来源：http://rq.jctech888.com.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://uq.shtwfgs.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zh.szsharing.cn

[A25] 字符串比较
来源：http://wh.shtwfgs.cn

Py:   s1 == s2; s1 != s2
来源：http://yr.521024.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ow.huixinmuqiang.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kg.chemitech.net.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wv.lnxyls.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ss.lnxyls.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pg.lnxyls.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ft.bookmarksfly.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mx.jianghongdianzi.cn

[A26] 类型转换总览
来源：http://zt.shxzukj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fz.nicolike.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ul.9csxet.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xc.lnxyls.cn

TS:   Number() String() Boolean() x as number
来源：http://ow.newstarts.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xh.muxihuayi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ha.shtwfgs.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://bn.nszjky.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ho.newstarts.cn

================================================================================
来源：http://cn.shxzskj.cn

B. 流程控制
来源：http://eq.yuntaijiaju.cn

================================================================================
来源：http://cs.szxytkj.cn

[B01] 条件判断 if / else
来源：http://bi.bjjhwx.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hh.muxihuayi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://av.muxihuayi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cr.szxytkj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://op.gzmigu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://yl.szxytkj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dy.jianghongdianzi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hn.chemitech.net.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hj.huanxung.cn

[B02] 多分支 else if / elif
来源：http://bq.nicolike.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sa.muxihuayi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mr.hnjuh.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bx.huanxung.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qd.bookmarksfly.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gp.szsharing.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rb.shtwfgs.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://aq.asd995.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yq.nicolike.cn

[B03] switch / match / case
来源：http://ui.jianghongdianzi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rd.gzmigu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tu.nicolike.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rw.asd995.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gv.haigaiapp.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ax.nicolike.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kg.huixiangedu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nh.huixiangedu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zy.shtwfgs.cn

[B04] for 计数循环
来源：http://gw.lnxyls.cn

Py:   for i in range(10): print(i)
来源：http://fh.chemitech.net.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nb.muxihuayi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uy.haigaiapp.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yx.lnxyls.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tr.bjjhwx.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kq.bjjhwx.cn

Ruby: 10.times { |i| puts i }
来源：http://wk.9csxet.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://oh.hahajie.cn

[B05] 遍历数组 / 列表
来源：http://sl.lnxyls.cn

Py:   for item in arr: print(item)
来源：http://fg.asd995.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://el.szxytkj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://go.521024.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qe.haigaiapp.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lt.bookmarksfly.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pt.yuexingan06.cn

Ruby: arr.each { |item| puts item }
来源：http://dg.huanxung.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xj.gzmigu.cn

[B06] 遍历字典 / 对象
来源：http://le.huixinmuqiang.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ae.jianghongdianzi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qu.muxihuayi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gx.jctech888.com.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sa.hnjuh.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wt.hnjuh.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mm.shxzukj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zq.szxytkj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://eo.szxytkj.cn

[B07] while 循环
来源：http://ks.asd995.cn

Py:   while i < 10: i += 1
来源：http://lp.lnxyls.cn

PHP:  while ($i < 10) { $i++; }
来源：http://nk.jctech888.com.cn

JS:   while (i < 10) { i++; }
来源：http://nw.lnxyls.cn

TS:   while (i < 10) { i++; }
来源：http://ty.panjiajie.cn

Java: while (i < 10) { i++; }
来源：http://mb.lnxyls.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ev.shxzskj.cn

Ruby: while i < 10; i += 1; end
来源：http://zz.shtwfgs.cn

C#:   while (i < 10) { i++; }
来源：http://cl.521024.cn

[B08] do-while（至少执行一次）
来源：http://eg.nszjky.cn

Py:   # 无 do-while：用 while True + break
来源：http://vz.huixinmuqiang.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://lm.huixiangedu.cn

JS:   do { i++; } while (i < 10);
来源：http://tq.hahajie.cn

TS:   do { i++; } while (i < 10);
来源：http://vt.521024.cn

Java: do { i++; } while (i < 10);
来源：http://xh.shxzukj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ji.shxzukj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mq.gzmigu.cn

C#:   do { i++; } while (i < 10);
来源：http://fo.shxzskj.cn

[B09] break 与 continue
来源：http://hq.nicolike.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.szxytkj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vk.huanxung.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dy.huixinmuqiang.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lp.huixiangedu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sb.yuexingan06.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://om.9csxet.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ak.bjjhwx.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mu.shxzskj.cn

[B10] 遍历同时拿索引
来源：http://yj.szxytkj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tc.szsharing.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kk.asd995.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dv.huixinmuqiang.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://un.jctech888.com.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cy.huixiangedu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://as.yuexingan06.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ay.yuexingan06.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zf.asd995.cn

[B11] 生成数字序列 / 区间
来源：http://we.shxzskj.cn

Py:   list(range(0, 10, 2))
来源：http://xf.wgjwhj.cn

PHP:  range(0, 10, 2);
来源：http://ek.bjjhwx.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gp.nicolike.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://su.jctech888.com.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jc.haigaiapp.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ui.yuntaijiaju.cn

Ruby: (0...10).step(2).to_a
来源：http://mg.haigaiapp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pt.nszjky.cn

[B12] 跳出多层循环
来源：http://wi.szxytkj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fs.wgjwhj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ay.asd995.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://et.huanxung.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://uf.521024.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ua.newstarts.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://eh.jctech888.com.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kv.haigaiapp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wt.szsharing.cn

[B13] 判断是否为数字
来源：http://ym.szsharing.cn

Py:   isinstance(x, (int, float))
来源：http://rs.hnjuh.cn

PHP:  is_numeric($x)
来源：http://to.lnxyls.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pb.hnjuh.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pq.asd995.cn

Java: x instanceof Number
来源：http://zh.nicolike.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://to.lnxyls.cn

Ruby: x.is_a?(Numeric)
来源：http://cl.gzmigu.cn

C#:   x is int or double or decimal
来源：http://uc.shxzukj.cn

[B14] 判断值是否在集合内
来源：http://hp.gzmigu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zg.jctech888.com.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pz.hahajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://cd.lnxyls.cn

TS:   [1, 2, 3].includes(x)
来源：http://cx.chemitech.net.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://wa.huanxung.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mf.lnxyls.cn

Ruby: [1, 2, 3].include?(x)
来源：http://lt.bookmarksfly.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nx.shxzskj.cn

[B15] 布尔运算与取反
来源：http://aw.nicolike.cn

Py:   a and b or not c
来源：http://rj.shxzskj.cn

PHP:  $a && $b || !$c
来源：http://rp.huanxung.cn

JS:   a && b || !c
来源：http://wk.521024.cn

TS:   a && b || !c
来源：http://jk.huanxung.cn

Java: a && b || !c
来源：http://zk.szsharing.cn

Go:   a && b || !c
来源：http://yb.9csxet.cn

Ruby: a && b || !c
来源：http://af.hahajie.cn

C#:   a && b || !c
来源：http://pk.gzmigu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ri.jianghongdianzi.cn

Py:   if not data: return
来源：http://xy.bjjhwx.cn

PHP:  if (!$data) { return; }
来源：http://uc.521024.cn

JS:   if (!data) return;
来源：http://lf.521024.cn

TS:   if (!data) return;
来源：http://vd.wgjwhj.cn

Java: if (data == null) return;
来源：http://om.jctech888.com.cn

Go:   if data == nil { return }
来源：http://ca.9csxet.cn

Ruby: return if data.nil?
来源：http://yy.jianghongdianzi.cn

C#:   if (data == null) return;
来源：http://bg.newstarts.cn

================================================================================
来源：http://bz.huixinmuqiang.cn

C. 函数与作用域
来源：http://ur.huixiangedu.cn

================================================================================
来源：http://vl.szsharing.cn

[C01] 定义函数
来源：http://dl.bookmarksfly.cn

Py:   def add(a, b): return a + b
来源：http://dq.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dz.haigaiapp.cn

JS:   function add(a, b) { return a + b; }
来源：http://lg.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zi.asd995.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://nd.shtwfgs.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rc.huixiangedu.cn

Ruby: def add(a, b); a + b; end
来源：http://nv.nicolike.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ro.huixinmuqiang.cn

[C02] 默认参数
来源：http://zn.huixinmuqiang.cn

Py:   def greet(name="World"): return name
来源：http://ao.lnxyls.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://nn.chemitech.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://iu.bjjhwx.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://un.9csxet.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cv.huixinmuqiang.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tl.hahajie.cn

Ruby: def greet(name = "World") = name
来源：http://qd.bjjhwx.cn

C#:   string Greet(string name = "World") => name;
来源：http://ad.gzmigu.cn

[C03] 可变参数
来源：http://ky.colortex.cn

Py:   def total(*args): return sum(args)
来源：http://pn.521024.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qz.yuexingan06.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pe.521024.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://th.lnxyls.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://uu.hnjuh.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xd.bjjhwx.cn

Ruby: def total(*nums); nums.sum; end
来源：http://se.newstarts.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pf.hahajie.cn

[C04] 命名参数 / 关键字参数
来源：http://uw.yuexingan06.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bm.huanxung.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xb.chemitech.net.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mk.newstarts.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ff.521024.cn

Java: // 无：用 Builder 模式或 record
来源：http://mk.yuntaijiaju.cn

Go:   // 无：用配置结构体参数
来源：http://om.jianghongdianzi.cn

Ruby: f(a: 1, b: 2)
来源：http://ps.bookmarksfly.cn

C#:   f(a: 1, b: 2)
来源：http://pb.szxytkj.cn

[C05] 返回多个值
来源：http://kk.hahajie.cn

Py:   return a, b
来源：http://ca.yuexingan06.cn

PHP:  return [$a, $b];
来源：http://jy.szxytkj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://im.nicolike.cn

TS:   return { a, b };
来源：http://hs.9csxet.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ov.shtwfgs.cn

Go:   return a, b
来源：http://zi.yuntaijiaju.cn

Ruby: return a, b
来源：http://eu.muxihuayi.cn

C#:   return (a, b);              // ValueTuple
来源：http://sc.jctech888.com.cn

[C06] 匿名函数 / lambda
来源：http://tx.bookmarksfly.cn

Py:   square = lambda x: x * x
来源：http://yn.szsharing.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://jn.huanxung.cn

JS:   const square = x => x * x;
来源：http://cz.szxytkj.cn

TS:   const square = (x: number): number => x * x;
来源：http://su.panjiajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://oj.shxzukj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://lc.szxytkj.cn

Ruby: square = ->(x) { x * x }
来源：http://dk.hnjuh.cn

C#:   Func<int, int> square = x => x * x;
来源：http://vb.hnjuh.cn

[C07] 把函数作为参数传入
来源：http://ob.asd995.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sf.521024.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bi.jianghongdianzi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ev.shtwfgs.cn

TS:   arr.map(String)
来源：http://pb.shxzukj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bv.shxzskj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mt.bookmarksfly.cn

Ruby: arr.map(&:upcase)
来源：http://yt.gzmigu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://tc.bookmarksfly.cn

[C08] 闭包
来源：http://wk.bookmarksfly.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://sd.huanxung.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://li.yuexingan06.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://li.szsharing.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bk.bjjhwx.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gc.shtwfgs.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ba.shtwfgs.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lx.newstarts.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ic.lnxyls.cn

[C09] 递归
来源：http://md.huixinmuqiang.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yp.haigaiapp.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zv.panjiajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oi.shtwfgs.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jg.huixinmuqiang.cn


<!-- 参考信息 -->