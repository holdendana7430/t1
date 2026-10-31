代发 wailian999

Ruby: a, b = b, a
来源：http://zy.hahajie.cn

C#:   (a, b) = (b, a);
来源：http://ef.panjiajie.cn

[A20] 读取标准输入
来源：http://ok.gzmigu.cn

Py:   name = input("请输入：")
来源：http://ne.wgjwhj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://na.huixiangedu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qk.lnxyls.cn

TS:   // Node.js：readline 模块
来源：http://ud.huixinmuqiang.cn

Java: new Scanner(System.in).nextLine()
来源：http://wb.nicolike.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://sb.bookmarksfly.cn

Ruby: gets.chomp
来源：http://ng.shtwfgs.cn

C#:   Console.ReadLine();
来源：http://pm.colortex.cn

[A21] 保留指定小数位输出
来源：http://sd.shtwfgs.cn

Py:   f"{3.14159:.2f}"
来源：http://la.wgjwhj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ul.jctech888.com.cn

JS:   (3.14159).toFixed(2)
来源：http://ca.gzmigu.cn

TS:   (3.14159).toFixed(2)
来源：http://nb.asd995.cn

Java: String.format("%.2f", 3.14159)
来源：http://rq.gzmigu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qg.newstarts.cn

Ruby: format("%.2f", 3.14159)
来源：http://am.shtwfgs.cn

C#:   3.14159.ToString("F2")
来源：http://bc.shxzukj.cn

[A22] 获取字符串长度
来源：http://oj.9csxet.cn

Py:   len(s)
来源：http://me.jctech888.com.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xc.asd995.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ka.hahajie.cn

TS:   s.length
来源：http://vt.9csxet.cn

Java: s.length()
来源：http://cm.szsharing.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ys.huixinmuqiang.cn

Ruby: s.length
来源：http://gv.panjiajie.cn

C#:   s.Length
来源：http://fs.bookmarksfly.cn

[A23] 大小写转换
来源：http://wq.huixinmuqiang.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://sc.jctech888.com.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://tz.haigaiapp.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fa.nszjky.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nm.szsharing.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://sg.colortex.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ax.newstarts.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://eg.panjiajie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://yw.wgjwhj.cn

[A24] 去除首尾空白
来源：http://it.szxytkj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xa.yuexingan06.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gi.huanxung.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eh.haigaiapp.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vv.9csxet.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ft.chemitech.net.cn

Go:   strings.TrimSpace(s)
来源：http://aa.szsharing.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rq.jctech888.com.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kg.chemitech.net.cn

[A25] 字符串比较
来源：http://sj.gzmigu.cn

Py:   s1 == s2; s1 != s2
来源：http://fg.haigaiapp.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ms.panjiajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zv.shxzukj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pi.szsharing.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gj.lnxyls.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qf.newstarts.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://cp.bookmarksfly.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://by.521024.cn

[A26] 类型转换总览
来源：http://lc.colortex.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hv.panjiajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bf.jianghongdianzi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zn.yuexingan06.cn

TS:   Number() String() Boolean() x as number
来源：http://as.521024.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nw.chemitech.net.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gc.9csxet.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://yi.hnjuh.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nd.hahajie.cn

================================================================================
来源：http://pu.521024.cn

B. 流程控制
来源：http://mr.lnxyls.cn

================================================================================
来源：http://bt.jctech888.com.cn

[B01] 条件判断 if / else
来源：http://gr.lnxyls.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://id.szxytkj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://of.shxzukj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://se.jctech888.com.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://be.huixinmuqiang.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://zt.chemitech.net.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ha.szsharing.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://be.nicolike.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fh.nicolike.cn

[B02] 多分支 else if / elif
来源：http://dm.bjjhwx.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gn.chemitech.net.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ma.nszjky.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uc.521024.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rv.jctech888.com.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ip.huixiangedu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://oo.asd995.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://js.shxzskj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ru.panjiajie.cn

[B03] switch / match / case
来源：http://ol.panjiajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cv.haigaiapp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qy.lnxyls.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yw.jianghongdianzi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hp.shtwfgs.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pf.jctech888.com.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ys.muxihuayi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://er.hnjuh.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qs.szxytkj.cn

[B04] for 计数循环
来源：http://ur.chemitech.net.cn

Py:   for i in range(10): print(i)
来源：http://yu.jctech888.com.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tu.521024.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wl.hahajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://un.shxzskj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uo.shxzskj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.szxytkj.cn

Ruby: 10.times { |i| puts i }
来源：http://ip.wgjwhj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bc.haigaiapp.cn

[B05] 遍历数组 / 列表
来源：http://za.huixiangedu.cn

Py:   for item in arr: print(item)
来源：http://ae.shxzskj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zk.shxzskj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wb.nicolike.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://lh.shxzukj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vy.huixinmuqiang.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fd.panjiajie.cn

Ruby: arr.each { |item| puts item }
来源：http://vq.yuntaijiaju.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ns.szsharing.cn

[B06] 遍历字典 / 对象
来源：http://gu.asd995.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://wp.yuntaijiaju.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sl.nszjky.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nc.haigaiapp.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zd.bjjhwx.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://oa.shxzukj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pg.szsharing.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ah.bjjhwx.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wj.nszjky.cn

[B07] while 循环
来源：http://ho.nszjky.cn

Py:   while i < 10: i += 1
来源：http://bq.nicolike.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xz.yuntaijiaju.cn

JS:   while (i < 10) { i++; }
来源：http://by.shtwfgs.cn

TS:   while (i < 10) { i++; }
来源：http://ar.521024.cn

Java: while (i < 10) { i++; }
来源：http://ww.jianghongdianzi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dd.muxihuayi.cn

Ruby: while i < 10; i += 1; end
来源：http://zu.jctech888.com.cn

C#:   while (i < 10) { i++; }
来源：http://kp.huixiangedu.cn

[B08] do-while（至少执行一次）
来源：http://ro.yuexingan06.cn

Py:   # 无 do-while：用 while True + break
来源：http://xw.shxzskj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ry.szsharing.cn

JS:   do { i++; } while (i < 10);
来源：http://ou.haigaiapp.cn

TS:   do { i++; } while (i < 10);
来源：http://ge.panjiajie.cn

Java: do { i++; } while (i < 10);
来源：http://mm.lnxyls.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wn.hnjuh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ko.jctech888.com.cn

C#:   do { i++; } while (i < 10);
来源：http://ig.colortex.cn

[B09] break 与 continue
来源：http://yf.huixinmuqiang.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mt.huixinmuqiang.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fc.shtwfgs.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rh.szxytkj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hb.huixiangedu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ff.panjiajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://uz.shxzukj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lm.9csxet.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qa.huixiangedu.cn

[B10] 遍历同时拿索引
来源：http://ba.yuntaijiaju.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rw.bjjhwx.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wh.yuexingan06.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ml.jctech888.com.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qw.gzmigu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qs.jianghongdianzi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uh.yuexingan06.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mc.shtwfgs.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hu.hahajie.cn

[B11] 生成数字序列 / 区间
来源：http://pk.hahajie.cn

Py:   list(range(0, 10, 2))
来源：http://st.jianghongdianzi.cn

PHP:  range(0, 10, 2);
来源：http://uz.shxzukj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ih.yuexingan06.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cb.muxihuayi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rv.gzmigu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ct.jctech888.com.cn

Ruby: (0...10).step(2).to_a
来源：http://vb.asd995.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ed.newstarts.cn

[B12] 跳出多层循环
来源：http://qv.yuexingan06.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fq.huixiangedu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://xb.newstarts.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ev.bjjhwx.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dq.huixinmuqiang.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://md.bookmarksfly.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ew.wgjwhj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zg.yuexingan06.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://si.521024.cn

[B13] 判断是否为数字
来源：http://xj.hahajie.cn

Py:   isinstance(x, (int, float))
来源：http://ym.yuntaijiaju.cn

PHP:  is_numeric($x)
来源：http://ug.panjiajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qn.colortex.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kh.bookmarksfly.cn

Java: x instanceof Number
来源：http://jc.nszjky.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fx.lnxyls.cn

Ruby: x.is_a?(Numeric)
来源：http://rj.nszjky.cn

C#:   x is int or double or decimal
来源：http://kn.bjjhwx.cn

[B14] 判断值是否在集合内
来源：http://wr.newstarts.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fy.lnxyls.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vq.muxihuayi.cn

JS:   [1, 2, 3].includes(x)
来源：http://zm.bjjhwx.cn

TS:   [1, 2, 3].includes(x)
来源：http://ko.shtwfgs.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://sf.jianghongdianzi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yn.shxzskj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mq.colortex.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hc.colortex.cn

[B15] 布尔运算与取反
来源：http://uv.colortex.cn

Py:   a and b or not c
来源：http://lr.jctech888.com.cn

PHP:  $a && $b || !$c
来源：http://sy.asd995.cn

JS:   a && b || !c
来源：http://hi.nicolike.cn

TS:   a && b || !c
来源：http://ny.huixiangedu.cn

Java: a && b || !c
来源：http://xw.muxihuayi.cn

Go:   a && b || !c
来源：http://oc.yuntaijiaju.cn

Ruby: a && b || !c
来源：http://zw.521024.cn

C#:   a && b || !c
来源：http://jn.chemitech.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hy.bookmarksfly.cn

Py:   if not data: return
来源：http://mf.gzmigu.cn

PHP:  if (!$data) { return; }
来源：http://vt.wgjwhj.cn

JS:   if (!data) return;
来源：http://lo.gzmigu.cn

TS:   if (!data) return;
来源：http://up.asd995.cn

Java: if (data == null) return;
来源：http://zj.hahajie.cn

Go:   if data == nil { return }
来源：http://vw.asd995.cn

Ruby: return if data.nil?
来源：http://pw.huixinmuqiang.cn

C#:   if (data == null) return;
来源：http://cv.panjiajie.cn

================================================================================
来源：http://nc.hnjuh.cn

C. 函数与作用域
来源：http://fv.yuexingan06.cn

================================================================================
来源：http://wm.yuexingan06.cn

[C01] 定义函数
来源：http://yy.huixinmuqiang.cn

Py:   def add(a, b): return a + b
来源：http://js.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rw.bookmarksfly.cn

JS:   function add(a, b) { return a + b; }
来源：http://wk.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hb.muxihuayi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lv.panjiajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xb.yuexingan06.cn

Ruby: def add(a, b); a + b; end
来源：http://yo.hahajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qf.lnxyls.cn

[C02] 默认参数
来源：http://yb.yuexingan06.cn

Py:   def greet(name="World"): return name
来源：http://rw.haigaiapp.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://rz.chemitech.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://pp.yuntaijiaju.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yo.shtwfgs.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://me.bookmarksfly.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://iz.nszjky.cn

Ruby: def greet(name = "World") = name
来源：http://fb.gzmigu.cn

C#:   string Greet(string name = "World") => name;
来源：http://gk.shxzskj.cn

[C03] 可变参数
来源：http://gw.jianghongdianzi.cn

Py:   def total(*args): return sum(args)
来源：http://lc.hahajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bt.newstarts.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fb.huixinmuqiang.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fg.yuntaijiaju.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qt.colortex.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fy.521024.cn

Ruby: def total(*nums); nums.sum; end
来源：http://se.nszjky.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kz.gzmigu.cn

[C04] 命名参数 / 关键字参数
来源：http://rl.gzmigu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://co.shxzskj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tz.asd995.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yd.jianghongdianzi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://li.shtwfgs.cn

Java: // 无：用 Builder 模式或 record
来源：http://qs.yuntaijiaju.cn

Go:   // 无：用配置结构体参数
来源：http://vc.panjiajie.cn

Ruby: f(a: 1, b: 2)
来源：http://jg.yuexingan06.cn

C#:   f(a: 1, b: 2)
来源：http://eu.huixiangedu.cn

[C05] 返回多个值
来源：http://qu.huanxung.cn

Py:   return a, b
来源：http://gx.huixinmuqiang.cn

PHP:  return [$a, $b];
来源：http://xe.9csxet.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jo.szxytkj.cn

TS:   return { a, b };
来源：http://uw.nszjky.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yw.bookmarksfly.cn

Go:   return a, b
来源：http://dw.bjjhwx.cn

Ruby: return a, b
来源：http://io.colortex.cn

C#:   return (a, b);              // ValueTuple
来源：http://jb.nicolike.cn

[C06] 匿名函数 / lambda
来源：http://dv.huixinmuqiang.cn

Py:   square = lambda x: x * x
来源：http://bq.gzmigu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://cx.gzmigu.cn

JS:   const square = x => x * x;
来源：http://wj.szxytkj.cn

TS:   const square = (x: number): number => x * x;
来源：http://vs.huixinmuqiang.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://su.nszjky.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fg.panjiajie.cn

Ruby: square = ->(x) { x * x }
来源：http://bl.gzmigu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://nk.521024.cn

[C07] 把函数作为参数传入
来源：http://fb.lnxyls.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vb.nicolike.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kw.colortex.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://af.bookmarksfly.cn

TS:   arr.map(String)
来源：http://ac.shxzukj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://by.shxzukj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://al.huanxung.cn

Ruby: arr.map(&:upcase)
来源：http://oq.newstarts.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fx.huixiangedu.cn

[C08] 闭包
来源：http://ju.yuntaijiaju.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://sh.hahajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qa.hnjuh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qr.gzmigu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://om.haigaiapp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nz.huixiangedu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bq.shxzskj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dn.nszjky.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bu.yuntaijiaju.cn

[C09] 递归
来源：http://lb.shxzskj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qq.szxytkj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://on.huixiangedu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sn.yuntaijiaju.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ww.asd995.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fj.hahajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hp.huixiangedu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://iy.huanxung.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gd.huanxung.cn

[C10] 变量作用域
来源：http://sf.yuntaijiaju.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nl.szxytkj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://sg.hahajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kc.9csxet.cn


<!-- 参考信息 -->