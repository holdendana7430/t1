代发 wailian999

JS:   [a, b] = [b, a];
来源：http://ab.chemitech.net.cn

TS:   [a, b] = [b, a];
来源：http://aj.szsharing.cn

Java: int t = a; a = b; b = t;
来源：http://va.haigaiapp.cn

Go:   a, b = b, a
来源：http://dt.bookmarksfly.cn

Ruby: a, b = b, a
来源：http://ct.chemitech.net.cn

C#:   (a, b) = (b, a);
来源：http://bn.wgjwhj.cn

[A20] 读取标准输入
来源：http://hm.colortex.cn

Py:   name = input("请输入：")
来源：http://mz.jianghongdianzi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://db.huanxung.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://es.wgjwhj.cn

TS:   // Node.js：readline 模块
来源：http://kw.9csxet.cn

Java: new Scanner(System.in).nextLine()
来源：http://hw.asd995.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gz.hahajie.cn

Ruby: gets.chomp
来源：http://wh.yuexingan06.cn

C#:   Console.ReadLine();
来源：http://ye.jctech888.com.cn

[A21] 保留指定小数位输出
来源：http://vx.nszjky.cn

Py:   f"{3.14159:.2f}"
来源：http://xn.szxytkj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://li.huixinmuqiang.cn

JS:   (3.14159).toFixed(2)
来源：http://em.wgjwhj.cn

TS:   (3.14159).toFixed(2)
来源：http://ta.yuntaijiaju.cn

Java: String.format("%.2f", 3.14159)
来源：http://pw.9csxet.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sq.9csxet.cn

Ruby: format("%.2f", 3.14159)
来源：http://wz.521024.cn

C#:   3.14159.ToString("F2")
来源：http://ug.hahajie.cn

[A22] 获取字符串长度
来源：http://wn.chemitech.net.cn

Py:   len(s)
来源：http://yo.huixinmuqiang.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wl.huanxung.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zp.521024.cn

TS:   s.length
来源：http://li.bookmarksfly.cn

Java: s.length()
来源：http://fn.shxzskj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bq.huanxung.cn

Ruby: s.length
来源：http://dg.bjjhwx.cn

C#:   s.Length
来源：http://uu.yuexingan06.cn

[A23] 大小写转换
来源：http://uy.jianghongdianzi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://hy.bjjhwx.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qv.colortex.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kk.huixinmuqiang.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.9csxet.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ny.huixiangedu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gw.jianghongdianzi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hx.newstarts.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://tv.szxytkj.cn

[A24] 去除首尾空白
来源：http://xh.huixinmuqiang.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nn.szsharing.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pj.nszjky.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uh.9csxet.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fq.shxzukj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ir.521024.cn

Go:   strings.TrimSpace(s)
来源：http://im.yuexingan06.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ko.gzmigu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://in.panjiajie.cn

[A25] 字符串比较
来源：http://lx.huanxung.cn

Py:   s1 == s2; s1 != s2
来源：http://fp.wgjwhj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mw.hnjuh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://et.bookmarksfly.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bv.colortex.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ee.haigaiapp.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kd.bjjhwx.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://gi.nszjky.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sw.szxytkj.cn

[A26] 类型转换总览
来源：http://sf.huixinmuqiang.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tf.panjiajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gx.jianghongdianzi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jx.yuexingan06.cn

TS:   Number() String() Boolean() x as number
来源：http://mo.chemitech.net.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dr.huixiangedu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://iw.panjiajie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ox.jctech888.com.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ao.newstarts.cn

================================================================================
来源：http://vy.gzmigu.cn

B. 流程控制
来源：http://dw.521024.cn

================================================================================
来源：http://hc.haigaiapp.cn

[B01] 条件判断 if / else
来源：http://kq.shxzukj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://sd.wgjwhj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vi.shxzukj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wh.nszjky.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zk.jctech888.com.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://af.shxzskj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yn.lnxyls.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sq.muxihuayi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.asd995.cn

[B02] 多分支 else if / elif
来源：http://xu.huixinmuqiang.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wl.huixinmuqiang.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sb.huanxung.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ey.szxytkj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wf.panjiajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ot.nicolike.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nt.bookmarksfly.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rc.521024.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uq.huixinmuqiang.cn

[B03] switch / match / case
来源：http://ep.szsharing.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bl.asd995.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://za.szxytkj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mq.huixiangedu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xs.shxzukj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dx.yuntaijiaju.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nj.bjjhwx.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lv.haigaiapp.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tc.yuntaijiaju.cn

[B04] for 计数循环
来源：http://wl.gzmigu.cn

Py:   for i in range(10): print(i)
来源：http://wf.bjjhwx.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wt.panjiajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ww.gzmigu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rs.jctech888.com.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://up.yuexingan06.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ym.shtwfgs.cn

Ruby: 10.times { |i| puts i }
来源：http://fm.wgjwhj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nc.shxzskj.cn

[B05] 遍历数组 / 列表
来源：http://ta.521024.cn

Py:   for item in arr: print(item)
来源：http://sj.haigaiapp.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ax.nszjky.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wb.muxihuayi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ct.newstarts.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://bi.bookmarksfly.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://uw.szsharing.cn

Ruby: arr.each { |item| puts item }
来源：http://bn.shtwfgs.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fs.bookmarksfly.cn

[B06] 遍历字典 / 对象
来源：http://px.bjjhwx.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://de.hahajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ad.bjjhwx.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tk.gzmigu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://we.wgjwhj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cu.nszjky.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hr.asd995.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zz.nszjky.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xd.yuntaijiaju.cn

[B07] while 循环
来源：http://xn.muxihuayi.cn

Py:   while i < 10: i += 1
来源：http://om.jianghongdianzi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://oq.huixiangedu.cn

JS:   while (i < 10) { i++; }
来源：http://oo.nicolike.cn

TS:   while (i < 10) { i++; }
来源：http://jk.shxzskj.cn

Java: while (i < 10) { i++; }
来源：http://ef.bookmarksfly.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tz.wgjwhj.cn

Ruby: while i < 10; i += 1; end
来源：http://ky.asd995.cn

C#:   while (i < 10) { i++; }
来源：http://zu.bookmarksfly.cn

[B08] do-while（至少执行一次）
来源：http://ud.szsharing.cn

Py:   # 无 do-while：用 while True + break
来源：http://nl.muxihuayi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cd.huixiangedu.cn

JS:   do { i++; } while (i < 10);
来源：http://qi.nicolike.cn

TS:   do { i++; } while (i < 10);
来源：http://ff.nszjky.cn

Java: do { i++; } while (i < 10);
来源：http://hv.bookmarksfly.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bo.huixinmuqiang.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rn.shxzskj.cn

C#:   do { i++; } while (i < 10);
来源：http://fl.bookmarksfly.cn

[B09] break 与 continue
来源：http://hz.jctech888.com.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bv.9csxet.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://eh.szsharing.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gu.bookmarksfly.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rn.nicolike.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xu.szxytkj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fi.chemitech.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ql.hahajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pd.szxytkj.cn

[B10] 遍历同时拿索引
来源：http://hb.lnxyls.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bg.shtwfgs.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ea.asd995.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pl.hnjuh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ky.huixinmuqiang.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sa.521024.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gu.shtwfgs.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jk.wgjwhj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://es.shxzskj.cn

[B11] 生成数字序列 / 区间
来源：http://si.gzmigu.cn

Py:   list(range(0, 10, 2))
来源：http://ez.asd995.cn

PHP:  range(0, 10, 2);
来源：http://ed.yuexingan06.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qx.colortex.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uo.haigaiapp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sx.huixiangedu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gf.jctech888.com.cn

Ruby: (0...10).step(2).to_a
来源：http://df.jianghongdianzi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mr.wgjwhj.cn

[B12] 跳出多层循环
来源：http://ag.panjiajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://se.hahajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://dt.shxzskj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jl.szsharing.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bm.gzmigu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gu.hnjuh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ds.bookmarksfly.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zr.nicolike.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rs.newstarts.cn

[B13] 判断是否为数字
来源：http://vx.shtwfgs.cn

Py:   isinstance(x, (int, float))
来源：http://ud.jianghongdianzi.cn

PHP:  is_numeric($x)
来源：http://oi.haigaiapp.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pt.nszjky.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iw.szxytkj.cn

Java: x instanceof Number
来源：http://qr.nszjky.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://df.shxzskj.cn

Ruby: x.is_a?(Numeric)
来源：http://iz.newstarts.cn

C#:   x is int or double or decimal
来源：http://jl.yuexingan06.cn

[B14] 判断值是否在集合内
来源：http://jn.chemitech.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gq.9csxet.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://na.9csxet.cn

JS:   [1, 2, 3].includes(x)
来源：http://jy.bjjhwx.cn

TS:   [1, 2, 3].includes(x)
来源：http://uv.newstarts.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ds.haigaiapp.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nj.yuexingan06.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zi.bookmarksfly.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pf.muxihuayi.cn

[B15] 布尔运算与取反
来源：http://vs.nicolike.cn

Py:   a and b or not c
来源：http://ne.hahajie.cn

PHP:  $a && $b || !$c
来源：http://om.shxzukj.cn

JS:   a && b || !c
来源：http://st.szxytkj.cn

TS:   a && b || !c
来源：http://py.shxzukj.cn

Java: a && b || !c
来源：http://bu.szsharing.cn

Go:   a && b || !c
来源：http://yl.hnjuh.cn

Ruby: a && b || !c
来源：http://cd.hnjuh.cn

C#:   a && b || !c
来源：http://zd.szsharing.cn

[B16] 卫语句：不满足条件提前返回
来源：http://mk.bjjhwx.cn

Py:   if not data: return
来源：http://qv.shxzukj.cn

PHP:  if (!$data) { return; }
来源：http://er.gzmigu.cn

JS:   if (!data) return;
来源：http://ye.521024.cn

TS:   if (!data) return;
来源：http://rq.lnxyls.cn

Java: if (data == null) return;
来源：http://ad.shxzskj.cn

Go:   if data == nil { return }
来源：http://bt.yuntaijiaju.cn

Ruby: return if data.nil?
来源：http://jj.nszjky.cn

C#:   if (data == null) return;
来源：http://sw.jctech888.com.cn

================================================================================
来源：http://dq.colortex.cn

C. 函数与作用域
来源：http://wz.huixiangedu.cn

================================================================================
来源：http://hv.szxytkj.cn

[C01] 定义函数
来源：http://gr.lnxyls.cn

Py:   def add(a, b): return a + b
来源：http://wd.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vu.yuntaijiaju.cn

JS:   function add(a, b) { return a + b; }
来源：http://jg.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://db.jctech888.com.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://eq.panjiajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ty.huixinmuqiang.cn

Ruby: def add(a, b); a + b; end
来源：http://se.nicolike.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vl.lnxyls.cn

[C02] 默认参数
来源：http://db.huanxung.cn

Py:   def greet(name="World"): return name
来源：http://gg.jianghongdianzi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yg.newstarts.cn

JS:   function greet(name = "World") { return name; }
来源：http://vq.colortex.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://oi.panjiajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ij.yuexingan06.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gl.jianghongdianzi.cn

Ruby: def greet(name = "World") = name
来源：http://ab.gzmigu.cn

C#:   string Greet(string name = "World") => name;
来源：http://jg.hahajie.cn

[C03] 可变参数
来源：http://rz.shxzskj.cn

Py:   def total(*args): return sum(args)
来源：http://xk.yuntaijiaju.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ah.yuntaijiaju.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://op.yuexingan06.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ol.muxihuayi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://km.chemitech.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tv.yuntaijiaju.cn

Ruby: def total(*nums); nums.sum; end
来源：http://up.szxytkj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nj.9csxet.cn

[C04] 命名参数 / 关键字参数
来源：http://co.gzmigu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ig.huixiangedu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://up.newstarts.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bm.asd995.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fp.yuexingan06.cn

Java: // 无：用 Builder 模式或 record
来源：http://ib.nszjky.cn

Go:   // 无：用配置结构体参数
来源：http://me.newstarts.cn

Ruby: f(a: 1, b: 2)
来源：http://am.muxihuayi.cn

C#:   f(a: 1, b: 2)
来源：http://cz.szxytkj.cn

[C05] 返回多个值
来源：http://xg.shxzskj.cn

Py:   return a, b
来源：http://za.lnxyls.cn

PHP:  return [$a, $b];
来源：http://ck.9csxet.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qp.jctech888.com.cn

TS:   return { a, b };
来源：http://qv.nicolike.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qb.huixiangedu.cn

Go:   return a, b
来源：http://zp.hnjuh.cn

Ruby: return a, b
来源：http://so.gzmigu.cn

C#:   return (a, b);              // ValueTuple
来源：http://hx.huixiangedu.cn

[C06] 匿名函数 / lambda
来源：http://ub.shxzskj.cn

Py:   square = lambda x: x * x
来源：http://cy.huixiangedu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://co.jctech888.com.cn

JS:   const square = x => x * x;
来源：http://oj.jctech888.com.cn

TS:   const square = (x: number): number => x * x;
来源：http://hi.yuexingan06.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fp.wgjwhj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ik.hahajie.cn

Ruby: square = ->(x) { x * x }
来源：http://cj.chemitech.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://uk.huixinmuqiang.cn

[C07] 把函数作为参数传入
来源：http://tn.yuexingan06.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ls.hahajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wp.newstarts.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zc.shxzskj.cn

TS:   arr.map(String)
来源：http://ri.colortex.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mb.bjjhwx.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://oj.bjjhwx.cn

Ruby: arr.map(&:upcase)
来源：http://yd.521024.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://tp.gzmigu.cn

[C08] 闭包
来源：http://ge.shxzukj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ec.bjjhwx.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://re.panjiajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sw.521024.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://on.shxzukj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xq.shtwfgs.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://da.wgjwhj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jv.jctech888.com.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://et.szsharing.cn

[C09] 递归
来源：http://fg.huanxung.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://oh.jctech888.com.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://on.wgjwhj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qk.haigaiapp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://se.shxzskj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://is.chemitech.net.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zk.jctech888.com.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://oq.panjiajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yz.chemitech.net.cn


<!-- 参考信息 -->