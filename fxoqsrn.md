代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://ku.jianghongdianzi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wa.9csxet.cn

TS:   // Node.js：readline 模块
来源：http://ux.hahajie.cn

Java: new Scanner(System.in).nextLine()
来源：http://hf.gzmigu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://un.hahajie.cn

Ruby: gets.chomp
来源：http://ju.jianghongdianzi.cn

C#:   Console.ReadLine();
来源：http://ef.jctech888.com.cn

[A21] 保留指定小数位输出
来源：http://pd.huixiangedu.cn

Py:   f"{3.14159:.2f}"
来源：http://ou.nszjky.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jd.nicolike.cn

JS:   (3.14159).toFixed(2)
来源：http://hv.yuexingan06.cn

TS:   (3.14159).toFixed(2)
来源：http://tm.yuntaijiaju.cn

Java: String.format("%.2f", 3.14159)
来源：http://zh.szxytkj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sz.huixiangedu.cn

Ruby: format("%.2f", 3.14159)
来源：http://za.szxytkj.cn

C#:   3.14159.ToString("F2")
来源：http://nt.jctech888.com.cn

[A22] 获取字符串长度
来源：http://je.szxytkj.cn

Py:   len(s)
来源：http://bv.521024.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wo.huixinmuqiang.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://li.gzmigu.cn

TS:   s.length
来源：http://hr.shtwfgs.cn

Java: s.length()
来源：http://gc.gzmigu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qn.huixiangedu.cn

Ruby: s.length
来源：http://ik.shxzukj.cn

C#:   s.Length
来源：http://lb.yuexingan06.cn

[A23] 大小写转换
来源：http://hr.panjiajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://nj.newstarts.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ay.haigaiapp.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fz.jianghongdianzi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rs.bookmarksfly.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mi.nszjky.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bm.jctech888.com.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://am.shxzukj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://xa.huanxung.cn

[A24] 去除首尾空白
来源：http://df.szxytkj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://da.jctech888.com.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wq.muxihuayi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uv.bjjhwx.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://og.yuntaijiaju.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tt.nszjky.cn

Go:   strings.TrimSpace(s)
来源：http://qg.gzmigu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://yz.9csxet.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://he.shxzskj.cn

[A25] 字符串比较
来源：http://jv.521024.cn

Py:   s1 == s2; s1 != s2
来源：http://im.panjiajie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://be.bookmarksfly.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wh.wgjwhj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qw.521024.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zu.nicolike.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ma.szxytkj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://oj.muxihuayi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://er.shtwfgs.cn

[A26] 类型转换总览
来源：http://dy.colortex.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sx.gzmigu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ys.nicolike.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://se.shtwfgs.cn

TS:   Number() String() Boolean() x as number
来源：http://bu.huixiangedu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bp.yuexingan06.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lf.huanxung.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://jc.hnjuh.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lc.muxihuayi.cn

================================================================================
来源：http://gi.hahajie.cn

B. 流程控制
来源：http://pj.hnjuh.cn

================================================================================
来源：http://ty.szsharing.cn

[B01] 条件判断 if / else
来源：http://kh.huixinmuqiang.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://lv.shxzukj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kk.jctech888.com.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xk.wgjwhj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yr.wgjwhj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qj.hnjuh.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gk.jctech888.com.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ig.yuexingan06.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ej.colortex.cn

[B02] 多分支 else if / elif
来源：http://ow.wgjwhj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pq.szxytkj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xe.szxytkj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hq.shxzskj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xi.521024.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uu.huixinmuqiang.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kj.yuexingan06.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://id.yuntaijiaju.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://up.521024.cn

[B03] switch / match / case
来源：http://ht.gzmigu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ru.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qy.newstarts.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://iu.bjjhwx.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ym.panjiajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rk.hnjuh.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://iu.colortex.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gp.haigaiapp.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vj.haigaiapp.cn

[B04] for 计数循环
来源：http://vh.newstarts.cn

Py:   for i in range(10): print(i)
来源：http://ed.nicolike.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gz.shxzskj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://du.newstarts.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ev.nszjky.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dd.nszjky.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ni.shxzskj.cn

Ruby: 10.times { |i| puts i }
来源：http://qa.huixiangedu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://of.newstarts.cn

[B05] 遍历数组 / 列表
来源：http://wy.9csxet.cn

Py:   for item in arr: print(item)
来源：http://zp.shtwfgs.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kn.asd995.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ux.jianghongdianzi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://cm.asd995.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://tx.nicolike.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wg.huanxung.cn

Ruby: arr.each { |item| puts item }
来源：http://zx.panjiajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bz.panjiajie.cn

[B06] 遍历字典 / 对象
来源：http://ez.huixiangedu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pf.panjiajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tb.hnjuh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ap.gzmigu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zk.asd995.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lb.jianghongdianzi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nd.szsharing.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ju.gzmigu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cu.hnjuh.cn

[B07] while 循环
来源：http://uv.haigaiapp.cn

Py:   while i < 10: i += 1
来源：http://mt.szsharing.cn

PHP:  while ($i < 10) { $i++; }
来源：http://oq.shtwfgs.cn

JS:   while (i < 10) { i++; }
来源：http://su.jctech888.com.cn

TS:   while (i < 10) { i++; }
来源：http://va.szsharing.cn

Java: while (i < 10) { i++; }
来源：http://qi.huixiangedu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tk.shtwfgs.cn

Ruby: while i < 10; i += 1; end
来源：http://bj.gzmigu.cn

C#:   while (i < 10) { i++; }
来源：http://uh.nicolike.cn

[B08] do-while（至少执行一次）
来源：http://uy.shtwfgs.cn

Py:   # 无 do-while：用 while True + break
来源：http://mj.panjiajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://nc.521024.cn

JS:   do { i++; } while (i < 10);
来源：http://gn.panjiajie.cn

TS:   do { i++; } while (i < 10);
来源：http://xw.huanxung.cn

Java: do { i++; } while (i < 10);
来源：http://qp.bjjhwx.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xa.bookmarksfly.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fn.9csxet.cn

C#:   do { i++; } while (i < 10);
来源：http://bf.bookmarksfly.cn

[B09] break 与 continue
来源：http://qj.shxzukj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ok.gzmigu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jv.shtwfgs.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iz.asd995.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sx.shtwfgs.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ew.haigaiapp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fy.shxzukj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vi.lnxyls.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cn.muxihuayi.cn

[B10] 遍历同时拿索引
来源：http://wm.gzmigu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://li.nicolike.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sx.huanxung.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://of.jctech888.com.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gc.yuexingan06.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://un.521024.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://co.bookmarksfly.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ob.hahajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xo.shtwfgs.cn

[B11] 生成数字序列 / 区间
来源：http://gq.colortex.cn

Py:   list(range(0, 10, 2))
来源：http://mp.chemitech.net.cn

PHP:  range(0, 10, 2);
来源：http://dl.bjjhwx.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://um.shtwfgs.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cj.haigaiapp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bf.hahajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jz.muxihuayi.cn

Ruby: (0...10).step(2).to_a
来源：http://yd.gzmigu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fc.nszjky.cn

[B12] 跳出多层循环
来源：http://qr.huixiangedu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://lo.wgjwhj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://go.lnxyls.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://am.chemitech.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sn.muxihuayi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://uw.colortex.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://aq.gzmigu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gm.shxzukj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ru.colortex.cn

[B13] 判断是否为数字
来源：http://vf.gzmigu.cn

Py:   isinstance(x, (int, float))
来源：http://qa.lnxyls.cn

PHP:  is_numeric($x)
来源：http://xw.haigaiapp.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ub.huanxung.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hi.shxzskj.cn

Java: x instanceof Number
来源：http://sp.colortex.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mr.wgjwhj.cn

Ruby: x.is_a?(Numeric)
来源：http://ru.huixiangedu.cn

C#:   x is int or double or decimal
来源：http://vr.huixiangedu.cn

[B14] 判断值是否在集合内
来源：http://es.bjjhwx.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dc.colortex.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mz.szsharing.cn

JS:   [1, 2, 3].includes(x)
来源：http://xx.nszjky.cn

TS:   [1, 2, 3].includes(x)
来源：http://tg.521024.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://lo.chemitech.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://om.szxytkj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://iz.shxzskj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cj.jctech888.com.cn

[B15] 布尔运算与取反
来源：http://um.nicolike.cn

Py:   a and b or not c
来源：http://ue.yuexingan06.cn

PHP:  $a && $b || !$c
来源：http://ak.newstarts.cn

JS:   a && b || !c
来源：http://xy.asd995.cn

TS:   a && b || !c
来源：http://yc.newstarts.cn

Java: a && b || !c
来源：http://jq.nszjky.cn

Go:   a && b || !c
来源：http://jt.hahajie.cn

Ruby: a && b || !c
来源：http://ll.nszjky.cn

C#:   a && b || !c
来源：http://fk.muxihuayi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ae.hnjuh.cn

Py:   if not data: return
来源：http://xv.lnxyls.cn

PHP:  if (!$data) { return; }
来源：http://cb.jianghongdianzi.cn

JS:   if (!data) return;
来源：http://hn.nicolike.cn

TS:   if (!data) return;
来源：http://qh.521024.cn

Java: if (data == null) return;
来源：http://xd.shxzukj.cn

Go:   if data == nil { return }
来源：http://lz.huixiangedu.cn

Ruby: return if data.nil?
来源：http://jp.bookmarksfly.cn

C#:   if (data == null) return;
来源：http://ki.haigaiapp.cn

================================================================================
来源：http://ye.jianghongdianzi.cn

C. 函数与作用域
来源：http://es.panjiajie.cn

================================================================================
来源：http://wm.huixiangedu.cn

[C01] 定义函数
来源：http://rj.nszjky.cn

Py:   def add(a, b): return a + b
来源：http://th.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ip.huixinmuqiang.cn

JS:   function add(a, b) { return a + b; }
来源：http://cw.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://on.huixiangedu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://pb.bjjhwx.cn

Go:   func add(a, b int) int { return a + b }
来源：http://uf.9csxet.cn

Ruby: def add(a, b); a + b; end
来源：http://vc.nicolike.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mf.newstarts.cn

[C02] 默认参数
来源：http://gr.colortex.cn

Py:   def greet(name="World"): return name
来源：http://sq.muxihuayi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hb.panjiajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://ou.szsharing.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ai.jianghongdianzi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qj.muxihuayi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kn.hahajie.cn

Ruby: def greet(name = "World") = name
来源：http://yh.lnxyls.cn

C#:   string Greet(string name = "World") => name;
来源：http://jq.jianghongdianzi.cn

[C03] 可变参数
来源：http://lb.muxihuayi.cn

Py:   def total(*args): return sum(args)
来源：http://av.gzmigu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fs.yuexingan06.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dv.shxzukj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sw.bjjhwx.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vc.9csxet.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pb.bookmarksfly.cn

Ruby: def total(*nums); nums.sum; end
来源：http://df.chemitech.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gg.haigaiapp.cn

[C04] 命名参数 / 关键字参数
来源：http://sc.wgjwhj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ni.haigaiapp.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tx.nszjky.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xv.521024.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ix.gzmigu.cn

Java: // 无：用 Builder 模式或 record
来源：http://lp.yuntaijiaju.cn

Go:   // 无：用配置结构体参数
来源：http://ne.hnjuh.cn

Ruby: f(a: 1, b: 2)
来源：http://em.chemitech.net.cn

C#:   f(a: 1, b: 2)
来源：http://bw.szsharing.cn

[C05] 返回多个值
来源：http://sa.szxytkj.cn

Py:   return a, b
来源：http://rr.bookmarksfly.cn

PHP:  return [$a, $b];
来源：http://gs.yuexingan06.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://cj.gzmigu.cn

TS:   return { a, b };
来源：http://lm.yuexingan06.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qd.wgjwhj.cn

Go:   return a, b
来源：http://la.jctech888.com.cn

Ruby: return a, b
来源：http://ze.nszjky.cn

C#:   return (a, b);              // ValueTuple
来源：http://jb.chemitech.net.cn

[C06] 匿名函数 / lambda
来源：http://tf.bookmarksfly.cn

Py:   square = lambda x: x * x
来源：http://kt.huanxung.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xd.shtwfgs.cn

JS:   const square = x => x * x;
来源：http://nh.nszjky.cn

TS:   const square = (x: number): number => x * x;
来源：http://ed.521024.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dr.newstarts.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rx.shtwfgs.cn

Ruby: square = ->(x) { x * x }
来源：http://by.haigaiapp.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hp.huixinmuqiang.cn

[C07] 把函数作为参数传入
来源：http://ju.haigaiapp.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://av.9csxet.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ig.jctech888.com.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tz.huixiangedu.cn

TS:   arr.map(String)
来源：http://ic.nicolike.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ik.yuexingan06.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://do.shxzukj.cn

Ruby: arr.map(&:upcase)
来源：http://pz.muxihuayi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://bb.shtwfgs.cn

[C08] 闭包
来源：http://ix.huixinmuqiang.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dv.haigaiapp.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rx.jctech888.com.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cu.chemitech.net.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wz.szxytkj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lw.asd995.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nq.szsharing.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vz.szsharing.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://sq.nicolike.cn

[C09] 递归
来源：http://eo.nicolike.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://me.bookmarksfly.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uk.szsharing.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xk.jianghongdianzi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ak.shxzskj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://oc.gzmigu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ua.jianghongdianzi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nr.bookmarksfly.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dx.lnxyls.cn

[C10] 变量作用域
来源：http://ik.gzmigu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nr.wgjwhj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zi.wgjwhj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xs.shtwfgs.cn

TS:   同 JS
来源：http://zq.haigaiapp.cn

Java: 方法内为块级作用域
来源：http://pm.bjjhwx.cn

Go:   花括号块级作用域
来源：http://zc.nicolike.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dh.shxzskj.cn


<!-- 参考信息 -->